WHAT IS THIS?
=============

Linux Kernel source code for the devices: 
* bq curie 2 
* bq curie 2 3G 
* bq curie 2 Quad Core 
* bq curie 2 Quad Core 3G

BUILD INSTRUCTIONS?
===================

Specific sources are separated by branches and each version is tagged with it's corresponding number. First, you should
clone the project:

	$ git clone git@github.com:bq/curie-2.git

After it, choose the version you would like to build:

	$ cd curie-2/
	$ git checkout 2.0.0_20140312-1248

Finally, build the kernel according the next defconfig files:

| device 										| defconfig								|
| --------------------------|-------------------------|
| bq curie 2 							  | curie2_defconfig				|
| bq curie 2 3G 						| curie2_3g_defconfig		  |
| bq curie 2 Quad Core 		  |	curie2_qc_defconfig		  |
| bq curie 2 Quad Core 3G	  |	curie2_qc_3g_defconfig	|

	$ cd kernel/
	$ make curie2_defconfig
	$ make kernel.img
