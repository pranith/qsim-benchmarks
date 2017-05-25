# qsim-benchmarks

To compile for qsim use parsecmgmt in parsec-3.0 folder. Example:

	$ cd parsec-3.0
	$ source env.sh
	$ parsecmgmt -a build -p blackscholes -c gcc-hooks
	
To cross compile for ARM64, do the following:

	$ export PARSECPLAT=aarch64
	$ export ARCH_PREFIX=aarch64-linux-gnu-
	$ parsecmgmt -a build -p blackscholes -c gcc-hooks
	
To create tar files, use the following command after building as above:
	
	$ parsecmgmt -a mktar -p blackscholes -c gcc-hooks
	
You will find a tar file in the tars folder of parsec-3.0 which you can use in
your simulation through qsim.
