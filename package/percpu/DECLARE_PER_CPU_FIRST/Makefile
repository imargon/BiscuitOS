################################################
#
# DECLARE_PER_CPU_FIRST
#
################################################
PK_DECLARE_PER_CPU_FIRST_NAME        := DECLARE_PER_CPU_FIRST
PK_DECLARE_PER_CPU_FIRST_VERSION     := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_VERSION)
PK_DECLARE_PER_CPU_FIRST_SITE        := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_URL)
PK_DECLARE_PER_CPU_FIRST_GITHUB      := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_GITHUB)
PK_DECLARE_PER_CPU_FIRST_SUBNAME     :=
PK_DECLARE_PER_CPU_FIRST_BUILDARCH   := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_BUILDARCH)
PK_DECLARE_PER_CPU_FIRST_DIR         := $(srctree)/package/percpu/DECLARE_PER_CPU_FIRST
PK_DECLARE_PER_CPU_FIRST_PATCH       := $(PK_DECLARE_PER_CPU_FIRST_DIR)/patch
PK_DECLARE_PER_CPU_FIRST_BSBIT       := DECLARE_PER_CPU_FIRST-$(PK_DECLARE_PER_CPU_FIRST_VERSION).bsbit
PK_DECLARE_PER_CPU_FIRST_OUT         :=
PK_DECLARE_PER_CPU_FIRST_SCRIPTS     := $(srctree)/scripts/package/package-module.sh
PK_DECLARE_PER_CPU_FIRST_TAR         := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_TAR)
PK_DECLARE_PER_CPU_FIRST_PACKAGE     :=
PK_DECLARE_PER_CPU_FIRST_CONFIG      := $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CONFIG)
SUB_TARGET                  += $(PK_DECLARE_PER_CPU_FIRST_DIR)/build

PK_DECLARE_PER_CPU_FIRST_sh = $(CONFIG_SHELL) $(PK_DECLARE_PER_CPU_FIRST_SCRIPTS) \
                 $1X \
                 $(PK_DECLARE_PER_CPU_FIRST_NAME)X \
                 $(PK_DECLARE_PER_CPU_FIRST_VERSION)X \
                 $(PK_DECLARE_PER_CPU_FIRST_SITE)X \
                 $(PK_DECLARE_PER_CPU_FIRST_GITHUB)X \
                 $(PK_DECLARE_PER_CPU_FIRST_PATCH)X \
                 $(CONFIG_LINUX_KERNEL_VERSION)X \
	         $(CONFIG_MAIN_PROJ_NAME)X \
                 $(PK_DECLARE_PER_CPU_FIRST_TAR)X \
                 $(CONFIG_LINUX_KERNEL_CROSS_COMPILE)X \
                 $(PK_DECLARE_PER_CPU_FIRST_SUBNAME)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CONFIG)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_LIBPATH)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CPPFLAGS)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_DPKCONFIG)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CFLAGS)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_LDFLAGS)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CXXFLAGS)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_ASFLAGS)X \
                 $(PK_DECLARE_PER_CPU_FIRST_BSBIT)X \
                 $(PK_DECLARE_PER_CPU_FIRST_BUILDARCH)X \
		 $(PK_DECLARE_PER_CPU_FIRST_CSRCFILE)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_SRCFILE)X \
                 $(CONFIG_PK_DECLARE_PER_CPU_FIRST_CSRCFILE)

$(PK_DECLARE_PER_CPU_FIRST_DIR)/build: FORCE
	$(Q)$(call PK_DECLARE_PER_CPU_FIRST_sh,$(srctree))
