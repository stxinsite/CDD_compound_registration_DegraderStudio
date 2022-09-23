# CDD_compound_registration_DegraderStudio

Restricted use tool for Degraderstudio to register new compounds to CDD and return SiTX numbers. 


To Use:

Build: singularity build --fakeroot CDD_API_compound_reg_dynamite.sif CDD_API_compound_reg_dynamite.def


Run:

singularity run -H ${PWD} /projects2/common/CDD_API_compound_reg_degraderstudio/main/CDD_API_compound_reg_dynamite.sif file_path file_name projects hypothesis creators


Test run example:

cd /bgfs01/insite02/songlu.li/

singularity run -H ${PWD} /projects2/common/CDD_API_compound_reg_degraderstudio/main/CDD_API_compound_reg_dynamite.sif design_set_001.sdf TEST test_hypothesis 'Songlu Li'