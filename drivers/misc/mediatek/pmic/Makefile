subdir-ccflags-$(CONFIG_MTK_PMIC_CHIP_MT6335)+= -I$(srctree)/drivers/misc/mediatek/pmic/include/mt6335
subdir-ccflags-$(CONFIG_MTK_PMIC_CHIP_MT6353)+= -I$(srctree)/drivers/misc/mediatek/pmic/include/mt6353

obj-$(CONFIG_MTK_EXTBUCK) += extbuck/
obj-$(CONFIG_MTK_PMIC_COMMON) += common/
obj-$(CONFIG_MTK_PMIC_CHIP_MT6313) += mt6313/
obj-$(CONFIG_MTK_PMIC_CHIP_MT6335) += mt6335/
obj-$(CONFIG_MTK_PMIC_CHIP_MT6336) += mt6336/
obj-$(CONFIG_MTK_PMIC_CHIP_MT6337) += mt6337/
obj-$(CONFIG_MTK_PMIC_CHIP_MT6353) += mt6353/

obj-$(CONFIG_MTK_AUXADC_INTF)   += mtk_auxadc_intf.o

obj-$(CONFIG_MFD_RT5081_PMU)	+= rt5081/
obj-y += mtk_battery_adc_intf.o

ifneq (,$(findstring evb,$(CONFIG_ARCH_MTK_PROJECT)))
	subdir-ccflags-y += -DMTK_EVB_PLATFORM
$(warning MTK_EVB_PLATFORM)
else
$(warning NOT_MTK_EVB_PLATFORM)
endif
