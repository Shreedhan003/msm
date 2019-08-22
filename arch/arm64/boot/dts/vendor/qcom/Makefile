# SPDX-License-Identifier: GPL-2.0

ifeq ($(CONFIG_MACH_XIAOMI_SDM660),y)
ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
dtbo-$(CONFIG_MACH_XIAOMI_LAVENDER) += sdm660-mtp-lavender-overlay.dtbo
sdm660-mtp-lavender-overlay.dtbo-base := sdm660-mtp-lavender.dtb
else
dtb-$(CONFIG_MACH_XIAOMI_LAVENDER) := sdm660-mtp-lavender.dtb
dtb-$(CONFIG_MACH_XIAOMI_TULIP) := sdm636-mtp-tulip.dtb
dtb-$(CONFIG_MACH_XIAOMI_WAYNE) := sdm660-mtp-wayne.dtb sdm660-mtp-jasmine.dtb
dtb-$(CONFIG_MACH_XIAOMI_WHYRED) := sdm636-mtp-whyred.dtb
endif

ifeq ($(CONFIG_BUILD_ARM64_DT_OVERLAY),y)
dtbo-$(CONFIG_ARCH_SDM660) += \

else
dtb-$(CONFIG_ARCH_SDM660) += \
endif

always		:= $(dtb-y)
subdir-y	:= $(dts-dirs)
clean-files    := *.dtb *.dtbo
