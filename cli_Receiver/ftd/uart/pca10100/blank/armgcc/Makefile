PROJECT_NAME     := thread_cli_ftd_uart_pca10100
TARGETS          := nrf52833_xxaa
OUTPUT_DIRECTORY := _build

SDK_ROOT := ../../../../../../../..
PROJ_DIR := ../../..

$(OUTPUT_DIRECTORY)/nrf52833_xxaa.out: \
  LINKER_SCRIPT  := thread_cli_ftd_uart_gcc_nrf52.ld

# Source files common to all targets
SRC_FILES += \
  $(SDK_ROOT)/modules/nrfx/mdk/gcc_startup_nrf52833.S \
  $(SDK_ROOT)/components/boards/boards.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_backend_rtt.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_backend_serial.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_default_backends.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_frontend.c \
  $(SDK_ROOT)/components/libraries/log/src/nrf_log_str_formatter.c \
  $(SDK_ROOT)/components/libraries/button/app_button.c \
  $(SDK_ROOT)/components/libraries/util/app_error.c \
  $(SDK_ROOT)/components/libraries/util/app_error_handler_gcc.c \
  $(SDK_ROOT)/components/libraries/util/app_error_weak.c \
  $(SDK_ROOT)/components/libraries/scheduler/app_scheduler.c \
  $(SDK_ROOT)/components/libraries/timer/app_timer2.c \
  $(SDK_ROOT)/components/libraries/util/app_util_platform.c \
  $(SDK_ROOT)/components/libraries/assert/assert.c \
  $(SDK_ROOT)/components/libraries/timer/drv_rtc.c \
  $(SDK_ROOT)/components/libraries/mem_manager/mem_manager.c \
  $(SDK_ROOT)/components/libraries/util/nrf_assert.c \
  $(SDK_ROOT)/components/libraries/atomic_fifo/nrf_atfifo.c \
  $(SDK_ROOT)/components/libraries/atomic/nrf_atomic.c \
  $(SDK_ROOT)/components/libraries/balloc/nrf_balloc.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf.c \
  $(SDK_ROOT)/external/fprintf/nrf_fprintf_format.c \
  $(SDK_ROOT)/components/libraries/memobj/nrf_memobj.c \
  $(SDK_ROOT)/components/libraries/pwr_mgmt/nrf_pwr_mgmt.c \
  $(SDK_ROOT)/components/libraries/ringbuf/nrf_ringbuf.c \
  $(SDK_ROOT)/components/libraries/experimental_section_vars/nrf_section_iter.c \
  $(SDK_ROOT)/components/libraries/sortlist/nrf_sortlist.c \
  $(SDK_ROOT)/components/libraries/strerror/nrf_strerror.c \
  $(SDK_ROOT)/integration/nrfx/legacy/nrf_drv_clock.c \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd/nrf_nvic.c \
  $(SDK_ROOT)/modules/nrfx/hal/nrf_nvmc.c \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd/nrf_soc.c \
  $(SDK_ROOT)/modules/nrfx/soc/nrfx_atomic.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_clock.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_gpiote.c \
  $(SDK_ROOT)/modules/nrfx/drivers/src/nrfx_nvmc.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp.c \
  $(SDK_ROOT)/components/libraries/bsp/bsp_thread.c \
  $(PROJ_DIR)/../../main.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT_Syscalls_GCC.c \
  $(SDK_ROOT)/external/segger_rtt/SEGGER_RTT_printf.c \
  $(SDK_ROOT)/modules/nrfx/mdk/system_nrf52833.c \
  $(SDK_ROOT)/components/thread/utils/thread_utils.c \

# Include folders common to all targets
INC_FOLDERS += \
  $(SDK_ROOT)/external/openthread/mbedtls/mbedtls/platform \
  $(SDK_ROOT)/external/openthread/project/config \
  $(SDK_ROOT)/external/openthread/mbedtls \
  $(SDK_ROOT)/integration/nrfx \
  $(PROJ_DIR) \
  $(SDK_ROOT)/external/nrf_security/include \
  $(SDK_ROOT)/components/thread/utils \
  $(SDK_ROOT)/components/libraries/log/src \
  $(SDK_ROOT)/components/libraries/scheduler \
  ../config \
  $(SDK_ROOT)/components/libraries/experimental_section_vars \
  $(SDK_ROOT)/components/libraries/atomic_fifo \
  $(SDK_ROOT)/external/nRF-IEEE-802.15.4-radio-driver/src/fem \
  $(SDK_ROOT)/modules/nrfx/mdk \
  $(SDK_ROOT)/components/libraries/strerror \
  $(SDK_ROOT)/integration/nrfx/legacy \
  $(SDK_ROOT)/components/boards \
  $(SDK_ROOT)/components/drivers_nrf/nrf_soc_nosd \
  $(SDK_ROOT)/components/libraries/button \
  $(SDK_ROOT)/components/libraries/log \
  $(SDK_ROOT)/modules/nrfx/hal \
  $(SDK_ROOT)/components/libraries/mem_manager \
  $(SDK_ROOT)/components/libraries/bsp \
  $(SDK_ROOT)/external/openthread/project/nrf52833 \
  $(SDK_ROOT)/components/libraries/sortlist \
  $(SDK_ROOT)/modules/nrfx/drivers/include \
  $(SDK_ROOT)/components/libraries/ringbuf \
  $(SDK_ROOT)/external/fprintf \
  $(SDK_ROOT)/components/libraries/balloc \
  $(SDK_ROOT)/components/libraries/util \
  $(SDK_ROOT)/modules/nrfx \
  $(SDK_ROOT)/external/openthread/include \
  $(SDK_ROOT)/components \
  $(SDK_ROOT)/external/segger_rtt \
  $(SDK_ROOT)/components/libraries/memobj \
  $(SDK_ROOT)/external/nRF-IEEE-802.15.4-radio-driver/src/fem/three_pin_gpio \
  $(SDK_ROOT)/components/libraries/atomic \
  $(SDK_ROOT)/components/libraries/delay \
  $(SDK_ROOT)/components/toolchain/cmsis/include \
  $(SDK_ROOT)/external/nrf_security/mbedtls_plat_config \
  $(SDK_ROOT)/components/libraries/mutex \
  $(SDK_ROOT)/components/libraries/pwr_mgmt \
  $(SDK_ROOT)/components/libraries/timer \

# Libraries common to all targets
LIB_FILES += \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-cli-ftd.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-ftd.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-nrf52833-transport.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-platform-utils.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libmbedcrypto.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-nrf52833-sdk.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libnordicsemi-nrf52833-radio-driver.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-nrf52833-transport.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-platform-utils.a \
  $(SDK_ROOT)/external/openthread/lib/nrf52833/gcc/libopenthread-ftd.a \

# Optimization flags
OPT = -O3 -g3
# Uncomment the line below to enable link time optimization
#OPT += -flto

# C flags common to all targets
CFLAGS += $(OPT)
CFLAGS += -DAPP_TIMER_V2
CFLAGS += -DAPP_TIMER_V2_RTC1_ENABLED
CFLAGS += -DBOARD_PCA10100
CFLAGS += -DCONFIG_GPIO_AS_PINRESET
CFLAGS += -DENABLE_FEM
CFLAGS += -DFLOAT_ABI_HARD
CFLAGS += -DMBEDTLS_CONFIG_FILE=\"mbedtls-config.h\"
CFLAGS += -DMBEDTLS_USER_CONFIG_FILE=\"nrf52833-mbedtls-config.h\"
CFLAGS += -DNRF52833_XXAA
CFLAGS += -DOPENTHREAD_CONFIG_ENABLE_BUILTIN_MBEDTLS=1
CFLAGS += -DOPENTHREAD_CONFIG_FILE=\"openthread-config-wrap.h\"
CFLAGS += -DOPENTHREAD_FTD=1
CFLAGS += -DUART0_ENABLED=0
CFLAGS += -mcpu=cortex-m4
CFLAGS += -mthumb -mabi=aapcs
CFLAGS += -Wall -Werror
CFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# keep every function in a separate section, this allows linker to discard unused ones
CFLAGS += -ffunction-sections -fdata-sections -fno-strict-aliasing
CFLAGS += -fno-builtin -fshort-enums

# C++ flags common to all targets
CXXFLAGS += $(OPT)
# Assembler flags common to all targets
ASMFLAGS += -g3
ASMFLAGS += -mcpu=cortex-m4
ASMFLAGS += -mthumb -mabi=aapcs
ASMFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
ASMFLAGS += -DAPP_TIMER_V2
ASMFLAGS += -DAPP_TIMER_V2_RTC1_ENABLED
ASMFLAGS += -DBOARD_PCA10100
ASMFLAGS += -DCONFIG_GPIO_AS_PINRESET
ASMFLAGS += -DENABLE_FEM
ASMFLAGS += -DFLOAT_ABI_HARD
ASMFLAGS += -DNRF52833_XXAA
ASMFLAGS += -DOPENTHREAD_FTD=1
ASMFLAGS += -DUART0_ENABLED=0

# Linker flags
LDFLAGS += $(OPT)
LDFLAGS += -mthumb -mabi=aapcs -L$(SDK_ROOT)/modules/nrfx/mdk -T$(LINKER_SCRIPT)
LDFLAGS += -mcpu=cortex-m4
LDFLAGS += -mfloat-abi=hard -mfpu=fpv4-sp-d16
# let linker dump unused sections
LDFLAGS += -Wl,--gc-sections
# use newlib in nano version
LDFLAGS += --specs=nano.specs

nrf52833_xxaa: CFLAGS += -D__HEAP_SIZE=0
nrf52833_xxaa: CFLAGS += -D__STACK_SIZE=8192
nrf52833_xxaa: ASMFLAGS += -D__HEAP_SIZE=0
nrf52833_xxaa: ASMFLAGS += -D__STACK_SIZE=8192

# Add standard libraries at the very end of the linker input, after all objects
# that may need symbols provided by these libraries.
LIB_FILES += -lc -lnosys -lm -lstdc++


.PHONY: default help

# Default target - first one defined
default: nrf52833_xxaa

# Print all targets that can be built
help:
	@echo following targets are available:
	@echo		nrf52833_xxaa
	@echo		sdk_config - starting external tool for editing sdk_config.h
	@echo		flash      - flashing binary

TEMPLATE_PATH := $(SDK_ROOT)/components/toolchain/gcc


include $(TEMPLATE_PATH)/Makefile.common

$(foreach target, $(TARGETS), $(call define_target, $(target)))

.PHONY: flash erase

# Flash the program
flash: default
	@echo Flashing: $(OUTPUT_DIRECTORY)/nrf52833_xxaa.hex
	nrfjprog -f nrf52 --program $(OUTPUT_DIRECTORY)/nrf52833_xxaa.hex --sectorerase
	nrfjprog -f nrf52 --reset

erase:
	nrfjprog -f nrf52 --eraseall

SDK_CONFIG_FILE := ../config/sdk_config.h
CMSIS_CONFIG_TOOL := $(SDK_ROOT)/external_tools/cmsisconfig/CMSIS_Configuration_Wizard.jar
sdk_config:
	java -jar $(CMSIS_CONFIG_TOOL) $(SDK_CONFIG_FILE)
