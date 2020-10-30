# LicheePi_Zero
LicheePi_Zero Code
包括 Uboot和 BuildBoot两个工程
Uboot：
source /etc/profile
make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- LicheePi_Zero_Hetao_defconfig
make ARCH=arm menuconfig
time make ARCH=arm CROSS_COMPILE=arm-linux-gnueabihf- 2>&1 | tee build.log
dd if=u-boot-sunxi-with-spl.bin of=uboot.img bs=1024 seek=8
or./img.sh
