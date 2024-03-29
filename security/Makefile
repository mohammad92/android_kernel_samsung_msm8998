#
# Makefile for the kernel security code
#

obj-$(CONFIG_KEYS)			+= keys/
subdir-$(CONFIG_SECURITY_SELINUX)	+= selinux
subdir-$(CONFIG_SECURITY_SMACK)		+= smack
subdir-$(CONFIG_SECURITY_TOMOYO)        += tomoyo
subdir-$(CONFIG_SECURITY_APPARMOR)	+= apparmor
subdir-$(CONFIG_SECURITY_YAMA)		+= yama
subdir-$(CONFIG_ARCH_QCOM)	+= pfe
subdir-$(CONFIG_SECURITY_DSMS)		+= dsms

# always enable default capabilities
obj-y					+= commoncap.o
obj-$(CONFIG_MMU)			+= min_addr.o

# Object file lists
obj-$(CONFIG_SECURITY)			+= security.o
obj-$(CONFIG_SECURITYFS)		+= inode.o
obj-$(CONFIG_SECURITY_SELINUX)		+= selinux/
obj-$(CONFIG_SECURITY_SMACK)		+= smack/
obj-$(CONFIG_AUDIT)			+= lsm_audit.o
obj-$(CONFIG_SECURITY_TOMOYO)		+= tomoyo/
obj-$(CONFIG_SECURITY_APPARMOR)		+= apparmor/
obj-$(CONFIG_SECURITY_YAMA)		+= yama/
obj-$(CONFIG_ARCH_QCOM)				+= pfe/
obj-$(CONFIG_CGROUP_DEVICE)		+= device_cgroup.o
obj-$(CONFIG_SECURITY_DSMS)		+= dsms/

# Object integrity file lists
subdir-$(CONFIG_INTEGRITY)		+= integrity
obj-$(CONFIG_INTEGRITY)			+= integrity/

# TIMA uevent
obj-$(CONFIG_TIMA_UEVENT)     += tima_uevent/

# MST driver
obj-$(CONFIG_MST_LDO)	  += mstdrv/

# Knox SDP
obj-$(CONFIG_SDP) += sdp/
obj-$(CONFIG_SDP) += sdp/built-in.o

#TZ ICCC
obj-$(CONFIG_TZ_ICCC)     += tz_iccc/

#KNOX TEST
obj-$(CONFIG_KNOX_TEST)     += knox_test/
