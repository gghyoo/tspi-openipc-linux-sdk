#
# SPDX-License-Identifier:	GPL-2.0+
#

obj-$(CONFIG_$(SPL_TPL_)CLK) += clk/
obj-$(CONFIG_$(SPL_TPL_)DM) += core/
obj-$(CONFIG_$(SPL_TPL_)DM_CRYPTO) += crypto/
obj-$(CONFIG_$(SPL_TPL_)DM_RNG) += rng/
obj-$(CONFIG_$(SPL_TPL_)DRIVERS_MISC_SUPPORT) += misc/ sysreset/ firmware/
obj-$(CONFIG_$(SPL_TPL_)I2C_SUPPORT) += i2c/
obj-$(CONFIG_$(SPL_TPL_)LED) += led/
obj-$(CONFIG_$(SPL_TPL_)INPUT) += input/
obj-$(CONFIG_$(SPL_TPL_)MMC_SUPPORT) += mmc/
obj-$(CONFIG_$(SPL_TPL_)NAND_SUPPORT) += mtd/nand/raw/
obj-$(CONFIG_$(SPL_TPL_)PHY) += phy/
obj-$(CONFIG_$(SPL_TPL_)PINCTRL) += pinctrl/
obj-$(CONFIG_$(SPL_TPL_)RAM) += ram/
obj-$(CONFIG_$(SPL_TPL_)SERIAL_SUPPORT) += serial/
obj-$(CONFIG_$(SPL_TPL_)SPI_FLASH_SUPPORT) += mtd/spi/
obj-$(CONFIG_$(SPL_TPL_)SPI_SUPPORT) += spi/
obj-$(CONFIG_$(SPL_TPL_)TIMER) += timer/
obj-$(CONFIG_$(SPL_TPL_)IRQ) += irq/

ifndef CONFIG_TPL_BUILD
ifdef CONFIG_SPL_BUILD
obj-$(CONFIG_SPL_ADC_SUPPORT) += adc/
obj-$(CONFIG_SPL_CPU_SUPPORT) += cpu/
obj-$(CONFIG_SPL_CRYPTO_SUPPORT) += crypto/
obj-$(CONFIG_SPL_GPIO_SUPPORT) += gpio/
obj-$(CONFIG_SPL_MPC8XXX_INIT_DDR_SUPPORT) += ddr/fsl/
obj-$(CONFIG_ARMADA_38X) += ddr/marvell/a38x/
obj-$(CONFIG_ARMADA_XP) += ddr/marvell/axp/
obj-$(CONFIG_ALTERA_SDRAM) += ddr/altera/
obj-$(CONFIG_SPL_POWER_SUPPORT) += power/
obj-$(CONFIG_SPL_DM_PMIC) += power/pmic/
obj-$(CONFIG_SPL_DM_REGULATOR) += power/regulator/
obj-$(CONFIG_SPL_DM_FUEL_GAUGE) += power/fuel_gauge/
obj-$(CONFIG_SPL_DM_FUEL_GAUGE) += power/charge/
obj-$(CONFIG_SPL_PWM_SUPPORT) += pwm/
obj-$(CONFIG_SPL_MTD_SUPPORT) += mtd/
obj-$(CONFIG_SPL_ONENAND_SUPPORT) += mtd/onenand/
obj-$(CONFIG_SPL_UBI) += mtd/ubispl/
obj-$(CONFIG_SPL_DMA_SUPPORT) += dma/
obj-$(CONFIG_SPL_ETH_SUPPORT) += net/
obj-$(CONFIG_SPL_ETH_SUPPORT) += net/phy/
obj-$(CONFIG_SPL_USBETH_SUPPORT) += net/phy/
obj-$(CONFIG_SPL_PCI_SUPPORT) += pci/
obj-$(CONFIG_SPL_PCH_SUPPORT) += pch/
obj-$(CONFIG_SPL_RTC_SUPPORT) += rtc/
obj-$(CONFIG_SPL_MUSB_NEW_SUPPORT) += usb/musb-new/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/udc/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/
obj-$(CONFIG_SPL_USB_GADGET) += usb/common/
obj-$(CONFIG_SPL_USB_GADGET) += usb/gadget/udc/
obj-$(CONFIG_SPL_DFU) += dfu/
obj-$(CONFIG_SPL_WATCHDOG_SUPPORT) += watchdog/
obj-$(CONFIG_SPL_USB_HOST_SUPPORT) += usb/host/
obj-$(CONFIG_OMAP_USB_PHY) += usb/phy/
obj-$(CONFIG_SPL_SATA_SUPPORT) += ata/ scsi/
obj-$(CONFIG_SPL_USB_HOST_SUPPORT) += block/
obj-$(CONFIG_SPL_MMC_SUPPORT) += block/
obj-$(CONFIG_SPL_MTD_SUPPORT) += block/
obj-$(CONFIG_SPL_FPGA_SUPPORT) += fpga/
obj-$(CONFIG_SPL_RKNAND_SUPPORT) += rknand/
obj-$(CONFIG_SPL_RKNAND_SUPPORT) += block/
endif
endif

ifdef CONFIG_TPL_BUILD

obj-$(CONFIG_TPL_MPC8XXX_INIT_DDR_SUPPORT) += ddr/fsl/

endif

ifeq ($(CONFIG_SPL_BUILD)$(CONFIG_TPL_BUILD),)

obj-y += adc/
obj-y += ata/
obj-$(CONFIG_DM_DEMO) += demo/
obj-$(CONFIG_BIOSEMU) += bios_emulator/
obj-y += block/
obj-$(CONFIG_BOOTCOUNT_LIMIT) += bootcount/
obj-$(CONFIG_CPU) += cpu/
obj-y += crypto/
obj-y += firmware/
obj-$(CONFIG_FPGA) += fpga/
obj-y += misc/
obj-$(CONFIG_MMC) += mmc/
obj-$(CONFIG_NVME) += nvme/
obj-$(CONFIG_RKNAND) += rknand/
obj-$(CONFIG_RKFLASH) += rkflash/
obj-y += pcmcia/
obj-$(CONFIG_DM_POWER_DELIVERY) += power/power_delivery/
obj-y += dfu/
obj-$(CONFIG_X86) += pch/
obj-y += phy/marvell/
obj-y += rtc/
obj-y += scsi/
obj-y += sound/
obj-y += spmi/
obj-y += sysreset/
obj-y += tpm/
obj-y += video/
obj-$(CONFIG_RP_POWER) += rongpin/
obj-y += watchdog/
obj-$(CONFIG_QE) += qe/
obj-$(CONFIG_U_QE) += qe/
obj-y += mailbox/
obj-y += memory/
obj-y += pwm/
obj-y += input/
# SOC specific infrastructure drivers.
obj-y += soc/
obj-$(CONFIG_REMOTEPROC) += remoteproc/
obj-y += thermal/
obj-y += ufs/

obj-$(CONFIG_MACH_PIC32) += ddr/microchip/
endif

obj-$(CONFIG_$(SPL_TPL_)DM_RESET) += reset/

