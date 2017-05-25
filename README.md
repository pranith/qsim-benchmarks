# qsim-benchmarks

To compile use parsecmgmt in parsec-3.0 folder. Example:

	$ cd parsec-3.0
	$ source env.sh
	$ parsecmgmt -a build -p blackscholes
	
To cross compile for ARM64, do the following:

	$ export PARSECPLAT=aarch64
	$ export ARCH_PREFIX=aarch64-linux-gnu-
	$ parsecmgmt -a build -p blackscholes
