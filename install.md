NECESSARY software (tcsh, fortran compiler (ifort or gfortran), FFTW3, make, bc)
tar -xvf wien2k XX.tar
check_minimal_software_requirements.sh
gunzip *.gz
chmod +x ./expand_lapw
./expand_lapw
./siteconfig_lapw
./userconfig_lapw
export $SCRATCH=./
export $WIENROOT=[PATH_TO_WIEN2K]
