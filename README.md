# Fully-Differential-6th-Order-Sallen-Key-Active-Low-Pass-Filter
README
Design and Implementation of a Fully Differential 6th-Order Sallen-Key Active Low-Pass Filter

- Overview
  This project presents the design and simulation of a fully differential 6th-order Sallen-Key active low-pass filter tailored for wideband wireless communication systems. The design emphasizes high linearity,      low power consumption, and robust common-mode noise rejection, making it suitable for integration in analog baseband signal processing.

- Team Members
    Mostafa Mohamed Mostafa 

    Adham Khaled Abdel Aziz 

    Mahmoud Ahmed AbdAl-Wahab 

-Supervisor: 
  Eng. Yousef Ali


- Objectives
    Implement a 6th-order Butterworth filter using three cascaded 2nd-order Sallen-Key stages.

    Achieve a closed-loop gain of 1 V/V with a 20 MHz bandwidth.

    Ensure high Common-Mode Rejection Ratio (CMRR > 60 dB) and group delay < 30 ns.

    Design for integration in a TSMC 65nm CMOS process with a 1.2 V supply.


- Design Phases
    Phase I – Folded OTA Design: Creation and simulation of a folded operational transconductance amplifier.

    Phase II – 2nd-Order Stage Design: Design of individual second-order Sallen-Key stages using equal R methodology.
  
    Phase III – Cascaded Architecture: Integration of three identical 2nd-order stages to form the complete 6th-order low-pass filter.

    Common-Mode Feedback (CMFB): Initial testing with an ideal CMFB block, to be replaced with a real implementation in future work.


- Simulation Results
    AC Analysis: Verified gain flatness within <1 dB ripple, attenuation >55 dBc at 10× the cutoff frequency.

    Transient Analysis: Demonstrated stable response to input step signals with minimal overshoot and acceptable settling times.

    Group Delay: Maintained flat delay across the passband, supporting wideband signal fidelity.


📈 Specifications Summary
Parameter         	Target Value
Technology        	  180nm
Supply Voltage        1.2 V
Closed-Loop Gain	    1 V/V
Bandwidth	            20 MHz
CMRR	               >60 dB
Group Delay	         <30 ns
Dynamic Range	        50 dB
Load Capacitance     	40 fF
Gain Ripple         	<1 dB

- Next Steps
    CMFB Integration: Replace the ideal CMFB with a real implementation.

    Extended Simulation: Include PVT corners, noise analysis, and Monte Carlo simulations.

    Optimization: Fine-tune component values and improve layout considerations for fabrication-readiness.

- References
    Hu, Q. et al. A 100–170MHz Fully-Differential Sallen-Key 6th-Order Low-Pass Filter...

    Karki, J. Active Low-Pass Filter Design, Texas Instruments.

    Sedra, A. & Smith, K. Microelectronic Circuits, 7th Edition.

    Razavi, B. Design of Analog CMOS Integrated Circuits.

    Franco, S. Design with Operational Amplifiers and Analog Integrated Circuits, 4th Edition.
