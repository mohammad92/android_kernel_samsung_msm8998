#
# Makefile for the sensors drivers.
#

# Each configuration option enables a list of files.

ccflags-y := $(KBUILD_FP_SENSOR_CFLAGS)

obj-$(CONFIG_SENSORS_FINGERPRINT)		+= fingerprint_sysfs.o
obj-$(CONFIG_SENSORS_VFS8XXX)			+= vfs8xxx.o
obj-$(CONFIG_SENSORS_VFS8XXX_EGIS)		+= vfs8xxx_egis.o
obj-$(CONFIG_SENSORS_ET5XX)			+= et5xx-spi.o et5xx-spi_data_transfer.o
