A few notes about phase-shifting on stm32h723zgt6:

-TRIGGER does not work as the slave mode for TIM8, only RESET does.
-OC was changed to PWM mode, and OC_START was changed to PWM_START
-The register CCR2 resets every clock cycle so that TIM8 can "latch" onto a new phase shift
