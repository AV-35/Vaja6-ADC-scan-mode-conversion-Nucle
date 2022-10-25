################################################################################
# Automatically-generated file. Do not edit!
# Toolchain: GNU Tools for STM32 (10.3-2021.10)
################################################################################

-include ../makefile.init

RM := rm -rf

# All of the sources participating in the build are defined here
-include sources.mk
-include Drivers/STM32L4xx_HAL_Driver/Src/subdir.mk
-include Core/Startup/subdir.mk
-include Core/Src/subdir.mk
-include objects.mk

ifneq ($(MAKECMDGOALS),clean)
ifneq ($(strip $(S_DEPS)),)
-include $(S_DEPS)
endif
ifneq ($(strip $(S_UPPER_DEPS)),)
-include $(S_UPPER_DEPS)
endif
ifneq ($(strip $(C_DEPS)),)
-include $(C_DEPS)
endif
endif

-include ../makefile.defs

OPTIONAL_TOOL_DEPS := \
$(wildcard ../makefile.defs) \
$(wildcard ../makefile.init) \
$(wildcard ../makefile.targets) \


BUILD_ARTIFACT_NAME := Vaja6-ADC-scan-mode-conversion-Nucle
BUILD_ARTIFACT_EXTENSION := elf
BUILD_ARTIFACT_PREFIX :=
BUILD_ARTIFACT := $(BUILD_ARTIFACT_PREFIX)$(BUILD_ARTIFACT_NAME)$(if $(BUILD_ARTIFACT_EXTENSION),.$(BUILD_ARTIFACT_EXTENSION),)

# Add inputs and outputs from these tool invocations to the build variables 
EXECUTABLES += \
Vaja6-ADC-scan-mode-conversion-Nucle.elf \

MAP_FILES += \
Vaja6-ADC-scan-mode-conversion-Nucle.map \

SIZE_OUTPUT += \
default.size.stdout \

OBJDUMP_LIST += \
Vaja6-ADC-scan-mode-conversion-Nucle.list \


# All Target
all: main-build

# Main-build Target
main-build: Vaja6-ADC-scan-mode-conversion-Nucle.elf secondary-outputs

# Tool invocations
Vaja6-ADC-scan-mode-conversion-Nucle.elf Vaja6-ADC-scan-mode-conversion-Nucle.map: $(OBJS) $(USER_OBJS) C:\Users\Vidmar\Documents\GitHub\Vaja6-ADC-scan-mode-conversion-Nucle\Vaja6-ADC\STM32L476RGTX_FLASH.ld makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-gcc -o "Vaja6-ADC-scan-mode-conversion-Nucle.elf" @"objects.list" $(USER_OBJS) $(LIBS) -mcpu=cortex-m4 -T"C:\Users\Vidmar\Documents\GitHub\Vaja6-ADC-scan-mode-conversion-Nucle\Vaja6-ADC\STM32L476RGTX_FLASH.ld" --specs=nosys.specs -Wl,-Map="Vaja6-ADC-scan-mode-conversion-Nucle.map" -Wl,--gc-sections -static --specs=nano.specs -mfpu=fpv4-sp-d16 -mfloat-abi=hard -mthumb -Wl,--start-group -lc -lm -Wl,--end-group
	@echo 'Finished building target: $@'
	@echo ' '

default.size.stdout: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-size  $(EXECUTABLES)
	@echo 'Finished building: $@'
	@echo ' '

Vaja6-ADC-scan-mode-conversion-Nucle.list: $(EXECUTABLES) makefile objects.list $(OPTIONAL_TOOL_DEPS)
	arm-none-eabi-objdump -h -S $(EXECUTABLES) > "Vaja6-ADC-scan-mode-conversion-Nucle.list"
	@echo 'Finished building: $@'
	@echo ' '

# Other Targets
clean:
	-$(RM) Vaja6-ADC-scan-mode-conversion-Nucle.elf Vaja6-ADC-scan-mode-conversion-Nucle.list Vaja6-ADC-scan-mode-conversion-Nucle.map default.size.stdout
	-@echo ' '

secondary-outputs: $(SIZE_OUTPUT) $(OBJDUMP_LIST)

fail-specified-linker-script-missing:
	@echo 'Error: Cannot find the specified linker script. Check the linker settings in the build configuration.'
	@exit 2

warn-no-linker-script-specified:
	@echo 'Warning: No linker script specified. Check the linker settings in the build configuration.'

.PHONY: all clean dependents main-build fail-specified-linker-script-missing warn-no-linker-script-specified

-include ../makefile.targets
