#
# SPDX-License-Identifier:	GPL-2.0+
#

ifeq ($(CONFIG_EFI_APP),)
ifdef CONFIG_$(SPL_)X86_64
head-y := arch/x86/cpu/start64.o
else
head-y := arch/x86/cpu/start.o
endif
endif

head-$(CONFIG_$(SPL_)X86_16BIT_INIT) += arch/x86/cpu/start16.o
head-$(CONFIG_$(SPL_)X86_16BIT_INIT) += arch/x86/cpu/resetvec.o

libs-y += arch/x86/cpu/
libs-y += arch/x86/lib/
