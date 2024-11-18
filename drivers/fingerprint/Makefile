#
# Makefile for the sensors drivers.
#

# Each configuration option enables a list of files.

ccflags-$(CONFIG_SENSORS_FPRINT_SECURE) := -DENABLE_SENSORS_FPRINT_SECURE
ccflags-y += -Wformat

obj-$(CONFIG_SENSORS_FINGERPRINT)	+= fingerprint.o fingerprint_sysfs.o

fingerprint-$(CONFIG_SENSORS_FINGERPRINT)	+= fingerprint_common.o
fingerprint-$(CONFIG_SENSORS_FINGERPRINT_LSI)	+= fingerprint_common_lsi.o
fingerprint-$(CONFIG_SENSORS_FINGERPRINT_QCOM)	+= fingerprint_common_qcom.o
fingerprint-$(CONFIG_SENSORS_FINGERPRINT_MTK)	+= fingerprint_common_mtk.o

fingerprint-$(CONFIG_SENSORS_GW9558X)	+= gw9558x_common.o gw9558x_spidev.o
fingerprint-$(CONFIG_SENSORS_QBT2000)	+= qbt2000_common.o
obj-$(CONFIG_SENSORS_QBT2000)			+= qbt2000_spidev.o
