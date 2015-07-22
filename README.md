Files in project
-----
rop.h - gadget collection for various ROP versions

LoadCode.S - 1st stage Spider ARM code loader example

DownLoad.S - 1+1 stage loader example (experimental)

rop.S - 2nd stage ARM code loader example

index.html.template - a template for spider webkit exploit

How to build
-----
make index.html - build index.html with all regions 1st stage loader

make LoadCode.dat ASFLAGS="-DSPIDER_9" - build Spider 1st stage for version 1.7567 (fw9)

make rop.dat ASFLAGS="-DSPIDER_9 -DARM_CODE=arm.bin" - build for spider version 1.7567 (fw9) and include arm.bin as ARM payload
Available option
-----
ARM_CODE=arm.bin - include file content as ARM payload (for rop.S)

SPIDER_ARM_CODE_OFFSET=0x100 - set Spider ARM payload offset in file (for LoadCode.S)

Define value|Description|Status
----------|----------|----------
MSET_4X|use MSET fw 4.x JP/US/EU gadgets|OK
MSET_4X_DG|use MSET fw 4.x JP/US/EU downgraded gadgets|OK
MSET_6X|use MSET fw 6.x  JP/US/EU gadgets|OK
SPIDER_4X|use Spider 1.7495.JP/US/EU gadgets|OK
SPIDER_42_CN|use Spider 1.7538.CN FW4.2 gadgets|not working
SPIDER_45_CN|use Spider 1.7538.CN FW4.5 gadgets|not working
SPIDER_4X_TW|use Spider 1.7538.KR gadgets|not tested
SPIDER_4X_KR|use Spider 1.7538.TW gadgets|OK
SPIDER_5X|use Spider 1.7552.JP/US/EU gadgets|OK
SPIDER_5X_CN|use Spider 1.7552.CN gadgets|not tested
SPIDER_5X_TW|use Spider 1.7552.KR gadgets|not tested
SPIDER_5X_KR|use Spider 1.7552.TW gadgets|OK
SPIDER_9X|use Spider 1.7567.JP/US/EU gadgets|OK
SPIDER_9X_CN|use Spider 1.7567.CN gadgets|OK
SPIDER_9X_TW|use Spider 1.7567.KR gadgets|OK
SPIDER_9X_KR|use Spider 1.7567.TW gadgets|OK


