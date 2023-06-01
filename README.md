# PWM
* Switching frequency (f_sf) = (1/(2^R*(F_V+1))



* duty = ("duty")/([2^R]*[T_sf]*[F_V+1])

PWM model takes an input clock signal, duty cycle, and final value for counting.
It uses registers and logic to generate a PWM waveform with the specified duty cycle and frequency.
The Timer_PWM module handles the counting and timing aspects to produce the desired PWM signal.
