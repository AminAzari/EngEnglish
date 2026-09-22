# Part 5: Technical Vocabulary Reference Appendix

## Scientific and Technical English for Electrical Engineering
**Level:** Undergraduate (B2–C1)  
**Purpose:** Comprehensive vocabulary reference organized by EE topic

---

## How to Use This Appendix

Each topic section contains:
1. **Vocabulary List** — Key terms with definitions, example sentences, Persian equivalents, and related terms
2. **Fill-in-the-Blank Exercise** — Practice using terms in context
3. **Matching Exercise** — Connect terms to their definitions
4. **Sentence Construction Exercise** — Build technical sentences from given terms
5. **Technical Reading Passage** — Short passage with comprehension questions

---


## 1. Electrical Circuits

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Voltage** | The electric potential difference between two points, measured in volts (V). | The voltage across the resistor was measured to be 5 V. | ولتاژ | potential, EMF, potential difference |
| 2 | **Current** | The flow of electric charge through a conductor, measured in amperes (A). | The current flowing through the circuit is 2 A. | جریان | amperage, flow, charge flow |
| 3 | **Resistance** | The opposition to current flow in a circuit, measured in ohms (Ω). | The resistance of the copper wire increases with temperature. | مقاومت | resistor, resistivity, ohmic |
| 4 | **Impedance** | The total opposition to AC current flow, combining resistance and reactance, measured in ohms (Ω). | The impedance of this RLC circuit varies with frequency. | امپدانس | reactance, admittance, complex impedance |
| 5 | **Capacitance** | The ability of a component to store electric charge, measured in farads (F). | The capacitance of the parallel plate capacitor depends on the plate area. | خازن (ظرفیت خازنی) | capacitor, charge storage, dielectric |
| 6 | **Inductance** | The property of a conductor that opposes changes in current, measured in henrys (H). | The inductance of the coil creates a back-EMF when current changes rapidly. | القاگری (اندوکتانس) | inductor, coil, magnetic flux |
| 7 | **Transient** | A temporary response in a circuit before it reaches steady state. | The transient response of the RC circuit decays exponentially. | گذرا | transient response, decay, time constant |
| 8 | **Steady state** | The condition of a circuit after all transients have died out. | In steady state, the capacitor acts as an open circuit for DC. | حالت ماندگار (پایدار) | equilibrium, DC steady state |
| 9 | **Frequency response** | The measure of a circuit's output as a function of input signal frequency. | The frequency response of the filter shows a -3 dB cutoff at 1 kHz. | پاسخ فرکانسی | Bode plot, bandwidth, transfer function |
| 10 | **Kirchhoff's laws** | KVL: The sum of voltages around a loop equals zero. KCL: The sum of currents at a node equals zero. | Using Kirchhoff's voltage law, we can write the equation for each mesh. | قوانین کیرشهف | loop analysis, node analysis |
| 11 | **Ohm's law** | The relationship V = IR, stating voltage equals current times resistance. | According to Ohm's law, doubling the resistance halves the current for a fixed voltage. | قانون اهم | V=IR, linear resistance |
| 12 | **Series** | A circuit configuration where components are connected end-to-end, sharing the same current. | Three resistors connected in series have a total resistance equal to their sum. | سری | series connection, cascaded |
| 13 | **Parallel** | A circuit configuration where components share the same voltage across them. | Capacitors in parallel add up to give total capacitance. | موازی | parallel connection, shunt |
| 14 | **Node** | A point in a circuit where two or more elements are connected. | We applied KCL at each node to find the unknown currents. | گره | junction, connection point |
| 15 | **Mesh** | A loop in a circuit that does not contain any other loop within it. | Mesh analysis simplifies solving circuits with multiple loops. | مش (حلقه) | loop, mesh current method |


### Fill-in-the-Blank Exercise

Complete each sentence with the correct term from the vocabulary list.

1. The __________ of a capacitor is measured in farads.
2. According to __________, the sum of all voltages around a closed loop is zero.
3. In a __________ circuit, all components share the same current.
4. __________ is the total opposition to alternating current, including both resistance and reactance.
5. The __________ response occurs before the circuit reaches equilibrium.
6. A __________ is a point where two or more circuit elements meet.
7. __________ states that V = I × R for a linear resistor.
8. When the circuit has settled and no longer changes with time, it is said to be in __________.

**Answer Key:** 1. capacitance, 2. Kirchhoff's voltage law (KVL), 3. series, 4. Impedance, 5. transient, 6. node, 7. Ohm's law, 8. steady state

### Matching Exercise

Match each term (1–10) with its definition (A–J).

| Term | Definition |
|------|-----------|
| 1. Voltage | A. Opposition to current flow measured in ohms |
| 2. Current | B. A loop containing no other loops within it |
| 3. Resistance | C. The flow of electric charge through a conductor |
| 4. Inductance | D. Circuit configuration with same voltage across components |
| 5. Capacitance | E. Electric potential difference between two points |
| 6. Mesh | F. Temporary circuit behavior before reaching equilibrium |
| 7. Parallel | G. Property opposing changes in current |
| 8. Transient | H. Ability to store electric charge |
| 9. Steady state | I. Circuit output behavior as a function of frequency |
| 10. Frequency response | J. Condition after all transients have died out |

**Answer Key:** 1-E, 2-C, 3-A, 4-G, 5-H, 6-B, 7-D, 8-F, 9-J, 10-I

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **impedance, frequency, RLC circuit**
2. **Kirchhoff's current law, node, sum**
3. **transient, time constant, exponential**
4. **series, resistance, total**
5. **parallel, capacitance, equivalent**

*Example answer for 1:* "The impedance of an RLC circuit is a complex quantity that varies with the input frequency."

### Technical Reading Passage

**RC Circuit Transient Analysis**

When a DC voltage source is suddenly connected to a series RC circuit, the capacitor does not charge instantaneously. Instead, the voltage across the capacitor increases exponentially toward the source voltage. The time constant τ = RC determines how quickly this transient response occurs. After approximately 5τ, the circuit reaches steady state, and the capacitor voltage equals the source voltage. During the transient period, the current decreases exponentially from its initial maximum value of V/R toward zero. Understanding transient behavior is essential for designing timing circuits, filters, and signal conditioning systems. Engineers must consider both the transient and steady-state responses when analyzing circuit performance.

**Comprehension Questions:**
1. What happens to the capacitor voltage when a DC source is connected to an RC circuit?
2. What determines the speed of the transient response?
3. After how many time constants does the circuit approximately reach steady state?
4. What is the initial current value when the source is first connected?

---


## 2. Electronics

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Transistor** | A semiconductor device used to amplify or switch electronic signals. | The transistor operates in saturation mode when used as a switch. | ترانزیستور | BJT, FET, switch, amplifier |
| 2 | **Amplifier** | A circuit that increases the amplitude of a signal. | The audio amplifier provides a voltage gain of 40 dB. | تقویت‌کننده | gain, op-amp, buffer |
| 3 | **Gain** | The ratio of output to input signal amplitude in an amplifier. | The amplifier has a gain of 100, meaning the output is 100 times the input. | بهره (گین) | voltage gain, current gain, power gain |
| 4 | **Bandwidth** | The range of frequencies over which a circuit operates effectively. | The bandwidth of the amplifier extends from 20 Hz to 20 kHz. | پهنای باند | frequency range, -3 dB point |
| 5 | **Semiconductor** | A material with conductivity between a conductor and an insulator. | Silicon is the most commonly used semiconductor in IC fabrication. | نیمه‌رسانا (نیم‌رسانا) | silicon, germanium, doping |
| 6 | **Diode** | A two-terminal device that allows current flow in one direction only. | The diode conducts when forward-biased above 0.7 V for silicon. | دیود | rectifier, LED, Zener diode |
| 7 | **Bias** | The DC voltage or current applied to set the operating point of a device. | Proper bias ensures the transistor operates in the active region. | بایاس (پیش‌ولتاژ) | biasing, operating point, Q-point |
| 8 | **Integrated circuit (IC)** | A set of electronic circuits fabricated on a single semiconductor chip. | Modern integrated circuits contain billions of transistors on a single chip. | مدار مجتمع | chip, microchip, VLSI |
| 9 | **MOSFET** | Metal-Oxide-Semiconductor Field-Effect Transistor; a voltage-controlled device. | The MOSFET is widely used in digital logic circuits due to its low power consumption. | ماسفت | NMOS, PMOS, CMOS, FET |
| 10 | **Op-amp** | Operational amplifier; a high-gain differential amplifier used in analog circuits. | The op-amp is configured as an inverting amplifier with a gain of -10. | آپ-امپ (تقویت‌کننده عملیاتی) | inverting, non-inverting, differential |
| 11 | **ADC** | Analog-to-Digital Converter; converts continuous signals to discrete digital values. | The 12-bit ADC samples the input signal at 1 MHz. | مبدل آنالوگ به دیجیتال | resolution, sampling rate, quantization |
| 12 | **DAC** | Digital-to-Analog Converter; converts digital values to continuous analog signals. | The DAC reconstructs the audio signal from stored digital data. | مبدل دیجیتال به آنالوگ | reconstruction, output stage |
| 13 | **PCB** | Printed Circuit Board; a board used to mechanically support and electrically connect electronic components. | The PCB layout must minimize trace lengths for high-frequency signals. | برد مدار چاپی | layout, traces, copper layers |
| 14 | **SMD** | Surface-Mount Device; a component designed to be mounted directly on the PCB surface. | SMD components are smaller than through-hole parts and enable compact designs. | قطعه نصب سطحی | surface mount, reflow soldering |
| 15 | **Threshold voltage** | The minimum gate-source voltage needed to create a conducting channel in a MOSFET. | The threshold voltage of this NMOS transistor is approximately 0.7 V. | ولتاژ آستانه | Vth, turn-on voltage |


### Fill-in-the-Blank Exercise

1. A __________ is a semiconductor device that can amplify or switch signals.
2. The __________ of an amplifier is the ratio of output signal to input signal.
3. A __________ allows current to flow in only one direction.
4. The __________ converts analog signals into digital form for processing.
5. __________ is the range of frequencies over which a circuit operates effectively.
6. The __________ is the minimum gate voltage required to turn on a MOSFET.
7. An __________ contains millions of transistors fabricated on a single chip.
8. __________ components are mounted directly on the surface of the PCB.

**Answer Key:** 1. transistor, 2. gain, 3. diode, 4. ADC, 5. Bandwidth, 6. threshold voltage, 7. integrated circuit, 8. SMD

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Op-amp | A. A board used to support and connect electronic components |
| 2. MOSFET | B. Converts digital values to analog signals |
| 3. Bias | C. A voltage-controlled field-effect transistor |
| 4. Semiconductor | D. High-gain differential amplifier for analog circuits |
| 5. PCB | E. DC voltage applied to set the operating point |
| 6. DAC | F. Material with conductivity between conductor and insulator |
| 7. Gain | G. Component designed for surface mounting |
| 8. SMD | H. Ratio of output to input signal amplitude |
| 9. Bandwidth | I. Range of effective operating frequencies |
| 10. Transistor | J. Device used to amplify or switch electronic signals |

**Answer Key:** 1-D, 2-C, 3-E, 4-F, 5-A, 6-B, 7-H, 8-G, 9-I, 10-J

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **MOSFET, threshold voltage, conducting**
2. **ADC, resolution, sampling rate**
3. **op-amp, inverting, gain**
4. **PCB, traces, high-frequency**
5. **diode, forward-biased, current**

### Technical Reading Passage

**MOSFET Operation in Digital Circuits**

The MOSFET is the fundamental building block of modern digital electronics. It operates as a voltage-controlled switch. When the gate-source voltage exceeds the threshold voltage, the MOSFET turns on, allowing current to flow between the drain and source terminals. In CMOS technology, complementary pairs of NMOS and PMOS transistors are used together. This arrangement consumes very little static power because only one transistor in each pair conducts at any time. The small size of MOSFETs allows billions of transistors to be integrated on a single chip. Today's processors use transistors with gate lengths of just a few nanometers, enabling unprecedented computational power in compact integrated circuits.

**Comprehension Questions:**
1. What controls the on/off state of a MOSFET?
2. What does CMOS stand for, and why is it power-efficient?
3. Why can billions of transistors fit on a single chip?
4. What is the relationship between threshold voltage and MOSFET conduction?

---


## 3. Power Systems

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Power factor** | The ratio of real power to apparent power in an AC circuit. | A power factor of 0.85 means 85% of the apparent power is doing useful work. | ضریب توان | cos φ, real power, apparent power |
| 2 | **Transformer** | A device that transfers electrical energy between circuits through electromagnetic induction. | The step-up transformer increases the voltage from 11 kV to 132 kV for transmission. | ترانسفورماتور | step-up, step-down, turns ratio |
| 3 | **Grid** | The interconnected network for delivering electricity from producers to consumers. | The national grid operates at multiple voltage levels for efficient power delivery. | شبکه (برق) | power network, utility grid |
| 4 | **Load** | Any device or component that consumes electrical power. | The industrial load on this feeder is approximately 500 kW. | بار (الکتریکی) | demand, consumer, load profile |
| 5 | **Generation** | The process of producing electrical energy from various sources. | Electricity generation from natural gas accounts for 40% of the country's total output. | تولید (برق) | power plant, generator |
| 6 | **Transmission** | The bulk transfer of electrical power over long distances at high voltage. | High-voltage transmission lines reduce losses over long distances. | انتقال | HV lines, transmission tower |
| 7 | **Distribution** | The delivery of electricity from substations to end-users at lower voltages. | The distribution network operates at 11 kV and 400 V. | توزیع | feeder, distribution transformer |
| 8 | **Renewable energy** | Energy derived from naturally replenishing sources such as solar, wind, and hydro. | Renewable energy now contributes over 30% of global electricity generation. | انرژی تجدیدپذیر | solar, wind, hydro, biomass |
| 9 | **Inverter** | A device that converts DC power to AC power. | The solar inverter converts the DC output of the panels to grid-compatible AC. | اینورتر (مبدل DC به AC) | DC-AC converter, grid-tied inverter |
| 10 | **Converter** | A device that changes electrical energy from one form to another (AC-DC, DC-DC, etc.). | The buck converter steps down the 12 V supply to 3.3 V. | مبدل | rectifier, buck, boost |
| 11 | **Substation** | A facility where voltage is transformed and electricity is distributed. | The substation steps down the transmission voltage to distribution levels. | پست (برق) | switchyard, transformer station |
| 12 | **Fault** | An abnormal condition in a power system, such as a short circuit. | The protection relay cleared the fault within 100 milliseconds. | خطا (اتصالی) | short circuit, ground fault, fault current |
| 13 | **Protection** | Systems and devices designed to detect faults and isolate affected sections. | The protection system uses overcurrent relays to detect faults. | حفاظت | relay, circuit breaker, fuse |
| 14 | **Reactive power** | Power that oscillates between source and load without doing useful work, measured in VAR. | Capacitor banks are installed to compensate for reactive power demand. | توان راکتیو | VAR, compensation, power factor correction |
| 15 | **Harmonics** | Voltage or current components at frequencies that are multiples of the fundamental frequency. | Harmonics from nonlinear loads can cause overheating in transformers. | هارمونیک‌ها | THD, distortion, nonlinear loads |


### Fill-in-the-Blank Exercise

1. The __________ is the ratio of real power to apparent power in an AC system.
2. A __________ converts DC electricity from solar panels into AC for the grid.
3. __________ lines carry electricity at high voltages over long distances.
4. A __________ is an abnormal condition such as a short circuit in the power system.
5. __________ are frequency components that are integer multiples of the fundamental.
6. The __________ steps down voltage from transmission to distribution levels.
7. __________ power oscillates between source and load without performing useful work.
8. The __________ system detects faults and isolates the affected circuit section.

**Answer Key:** 1. power factor, 2. inverter, 3. Transmission, 4. fault, 5. Harmonics, 6. substation, 7. Reactive, 8. protection

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Transformer | A. Network for delivering electricity to consumers |
| 2. Grid | B. Device converting DC to AC |
| 3. Load | C. Energy from naturally replenishing sources |
| 4. Inverter | D. Device transferring energy through electromagnetic induction |
| 5. Renewable energy | E. Any device consuming electrical power |
| 6. Fault | F. Delivery of electricity to end-users |
| 7. Distribution | G. Abnormal condition like a short circuit |
| 8. Reactive power | H. Bulk transfer of power over long distances |
| 9. Transmission | I. Power oscillating without doing useful work |
| 10. Power factor | J. Ratio of real power to apparent power |

**Answer Key:** 1-D, 2-A, 3-E, 4-B, 5-C, 6-G, 7-F, 8-I, 9-H, 10-J

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **transformer, step-up, transmission voltage**
2. **power factor, capacitor bank, correction**
3. **harmonics, nonlinear loads, distortion**
4. **inverter, solar panels, grid-connected**
5. **fault, protection relay, circuit breaker**

### Technical Reading Passage

**Power Factor Correction in Industrial Systems**

Industrial facilities often have a low power factor due to inductive loads such as motors and transformers. A low power factor means that a significant portion of the apparent power is reactive power, which does not perform useful work but increases current flow in the system. This results in higher losses and may incur utility penalties. To improve the power factor, capacitor banks are installed to supply reactive power locally, reducing the reactive demand from the grid. Modern systems use automatic power factor correction controllers that switch capacitor steps based on real-time measurements. Maintaining a power factor above 0.95 is typically required by utility companies for industrial consumers.

**Comprehension Questions:**
1. Why do industrial facilities often have a low power factor?
2. What is the consequence of a low power factor on the electrical system?
3. How do capacitor banks improve the power factor?
4. What power factor value is typically required by utility companies?

---


## 4. Control Systems

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Feedback** | The return of a portion of the output signal to the input to regulate system behavior. | Negative feedback reduces the error between the desired and actual output. | فیدبک (بازخورد) | negative feedback, positive feedback |
| 2 | **Stability** | The property of a system to return to equilibrium after a disturbance. | The system is stable if all poles of the transfer function have negative real parts. | پایداری | BIBO stability, marginal stability |
| 3 | **Transfer function** | The ratio of the Laplace transform of the output to the input of a linear system. | The transfer function of this first-order system is G(s) = 1/(s+1). | تابع تبدیل | H(s), G(s), poles, zeros |
| 4 | **Controller** | A device or algorithm that generates control signals to regulate a system's output. | The PID controller adjusts the motor speed to match the setpoint. | کنترلر (کنترل‌کننده) | PID, compensator, regulator |
| 5 | **Response** | The output behavior of a system when subjected to an input signal. | The step response shows how quickly the system reaches the desired value. | پاسخ | step response, impulse response |
| 6 | **Overshoot** | The amount by which the system output exceeds the desired final value. | The maximum overshoot must be kept below 10% for this application. | فراجهش (اورشوت) | peak value, damping |
| 7 | **Settling time** | The time required for the system output to remain within a specified error band. | The settling time for the motor control system is less than 2 seconds. | زمان نشست | 2% criterion, 5% criterion |
| 8 | **PID** | Proportional-Integral-Derivative; a common three-term control algorithm. | The PID controller was tuned using the Ziegler-Nichols method. | پی‌آی‌دی | proportional, integral, derivative |
| 9 | **Plant** | The physical system or process being controlled. | The plant in this case is a DC motor driving a robotic arm. | پلنت (فرآیند) | process, system, actuator |
| 10 | **Open-loop** | A control system without feedback where output does not influence the input. | An open-loop system cannot correct for disturbances automatically. | حلقه‌باز | feedforward, no feedback |
| 11 | **Closed-loop** | A control system that uses feedback to compare output with the desired input. | The closed-loop system automatically adjusts for external disturbances. | حلقه‌بسته | feedback system, servo |
| 12 | **Bode plot** | A graphical representation of a system's frequency response (magnitude and phase). | The Bode plot shows a gain margin of 10 dB and a phase margin of 45°. | نمودار بود | gain margin, phase margin |
| 13 | **Root locus** | A graphical method showing how system poles move as a parameter varies. | The root locus plot reveals that increasing gain makes the system unstable. | مکان هندسی ریشه‌ها | pole placement, gain variation |
| 14 | **State space** | A mathematical model representing a system using state variables and matrix equations. | The state space representation uses matrices A, B, C, and D to describe the system. | فضای حالت | state vector, state equation |
| 15 | **Observer** | A system that estimates internal states of a plant from measured outputs. | A Luenberger observer was designed to estimate the unmeasured state variables. | رویتگر (مشاهده‌گر) | estimator, Luenberger observer, Kalman filter |


### Fill-in-the-Blank Exercise

1. __________ is the return of output information to the input to regulate performance.
2. A system is considered __________ if it returns to equilibrium after a disturbance.
3. The __________ is a three-term controller using proportional, integral, and derivative actions.
4. __________ is the amount by which the output exceeds the final desired value.
5. The __________ represents the physical system or process being controlled.
6. A __________ system uses feedback to compare actual output with desired input.
7. The __________ shows how poles move as gain varies.
8. An __________ estimates internal states that cannot be directly measured.

**Answer Key:** 1. Feedback, 2. stable, 3. PID controller, 4. Overshoot, 5. plant, 6. closed-loop, 7. root locus, 8. observer

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Transfer function | A. Time for output to stay within error band |
| 2. Settling time | B. Ratio of Laplace transforms of output to input |
| 3. Bode plot | C. Control system without feedback |
| 4. Open-loop | D. Graphical frequency response representation |
| 5. Feedback | E. Physical system being controlled |
| 6. Plant | F. Return of output to input for regulation |
| 7. State space | G. Amount output exceeds desired final value |
| 8. Overshoot | H. Mathematical model using state variables |
| 9. Stability | I. Device generating control signals |
| 10. Controller | J. Property of returning to equilibrium |

**Answer Key:** 1-B, 2-A, 3-D, 4-C, 5-F, 6-E, 7-H, 8-G, 9-J, 10-I

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **closed-loop, feedback, stability**
2. **PID, overshoot, settling time**
3. **transfer function, poles, stability**
4. **Bode plot, gain margin, phase margin**
5. **observer, state variables, estimation**

### Technical Reading Passage

**PID Control in Industrial Applications**

The PID controller is the most widely used control algorithm in industry. It combines three actions: proportional (P) responds to the current error, integral (I) eliminates steady-state error by accumulating past errors, and derivative (D) anticipates future errors based on the rate of change. Tuning a PID controller involves selecting appropriate gains for each term. If the proportional gain is too high, the system may exhibit excessive overshoot or become unstable. The integral term can cause windup problems if not properly limited. Modern industrial systems often use auto-tuning algorithms that automatically determine optimal PID parameters. The settling time and overshoot specifications guide the tuning process.

**Comprehension Questions:**
1. What are the three components of a PID controller?
2. Which component eliminates steady-state error?
3. What happens if the proportional gain is set too high?
4. What is "integral windup" and how is it addressed?

---


## 5. Telecommunications

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Modulation** | The process of varying a carrier signal to encode information. | Frequency modulation (FM) varies the carrier frequency to represent the message signal. | مدولاسیون | AM, FM, QAM, PSK |
| 2 | **Bandwidth** | The range of frequencies available for signal transmission. | The channel bandwidth of 20 MHz supports data rates up to 100 Mbps. | پهنای باند | spectral width, channel capacity |
| 3 | **Channel** | The medium or path through which a signal travels from transmitter to receiver. | The wireless channel introduces fading and multipath effects. | کانال | propagation path, link |
| 4 | **Noise** | Unwanted random signals that interfere with the desired signal. | Thermal noise limits the sensitivity of the receiver. | نویز | thermal noise, AWGN, interference |
| 5 | **Interference** | Unwanted signals from other sources that degrade communication quality. | Co-channel interference occurs when two transmitters use the same frequency. | تداخل | co-channel, adjacent channel |
| 6 | **Antenna** | A device that converts electrical signals to electromagnetic waves and vice versa. | The directional antenna focuses the transmitted energy toward the receiver. | آنتن | dipole, patch, array |
| 7 | **Propagation** | The travel of electromagnetic waves through a medium or free space. | Radio wave propagation is affected by reflection, diffraction, and scattering. | انتشار (امواج) | path loss, free-space, multipath |
| 8 | **Fading** | The variation in signal strength due to multipath propagation and movement. | Rayleigh fading models the signal variations in non-line-of-sight conditions. | فیدینگ (محوشدگی) | Rayleigh, Rician, fast fading, slow fading |
| 9 | **MIMO** | Multiple-Input Multiple-Output; a technique using multiple antennas at both transmitter and receiver. | MIMO technology increases channel capacity without additional bandwidth. | مایمو | spatial multiplexing, diversity |
| 10 | **Beamforming** | Technique of directing signal transmission toward a specific receiver using antenna arrays. | Beamforming in 5G allows focused energy delivery to individual users. | بیم‌فرمینگ (شکل‌دهی پرتو) | phased array, steering |
| 11 | **OFDM** | Orthogonal Frequency-Division Multiplexing; divides bandwidth into many narrow subcarriers. | OFDM is used in Wi-Fi and LTE because it is robust against multipath fading. | او‌اف‌دی‌ام | subcarrier, cyclic prefix, FFT |
| 12 | **5G** | The fifth generation of mobile network technology offering high speed and low latency. | 5G networks support ultra-reliable low-latency communication for autonomous vehicles. | نسل پنجم | NR, mmWave, massive MIMO |
| 13 | **Spectrum** | The range of electromagnetic frequencies used for communication. | Spectrum allocation is regulated by government agencies to prevent interference. | طیف (فرکانسی) | frequency band, allocation, licensing |
| 14 | **Multiplexing** | The technique of combining multiple signals for transmission over a shared medium. | Time-division multiplexing (TDM) allocates separate time slots to each user. | مالتی‌پلکسینگ | TDM, FDM, WDM, CDM |
| 15 | **Baseband** | The original frequency range of a signal before modulation. | The baseband signal is modulated onto a carrier for wireless transmission. | باند پایه | unmodulated, digital baseband |


### Fill-in-the-Blank Exercise

1. __________ is the process of encoding information onto a carrier signal.
2. The wireless __________ introduces fading and multipath effects on the signal.
3. __________ technology uses multiple antennas to increase capacity without extra bandwidth.
4. __________ directs transmitted energy toward a specific receiver using antenna arrays.
5. __________ divides the available bandwidth into many narrow orthogonal subcarriers.
6. Unwanted random signals that corrupt the desired signal are called __________.
7. __________ combines multiple signals for transmission over a single shared medium.
8. The __________ signal is the original unmodulated signal at its native frequency range.

**Answer Key:** 1. Modulation, 2. channel, 3. MIMO, 4. Beamforming, 5. OFDM, 6. noise, 7. Multiplexing, 8. baseband

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Antenna | A. Variation in signal strength due to multipath |
| 2. Fading | B. Device converting electrical signals to EM waves |
| 3. Propagation | C. Range of frequencies for signal transmission |
| 4. Bandwidth | D. Travel of electromagnetic waves through space |
| 5. 5G | E. Combining multiple signals on a shared medium |
| 6. Multiplexing | F. Fifth generation mobile network technology |
| 7. Interference | G. Frequency range regulated by government agencies |
| 8. Spectrum | H. Unwanted signals from other sources |
| 9. OFDM | I. Original frequency range before modulation |
| 10. Baseband | J. Technique dividing bandwidth into subcarriers |

**Answer Key:** 1-B, 2-A, 3-D, 4-C, 5-F, 6-E, 7-H, 8-G, 9-J, 10-I

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **OFDM, multipath fading, subcarriers**
2. **MIMO, antenna, spatial multiplexing**
3. **5G, low latency, beamforming**
4. **modulation, carrier, bandwidth**
5. **noise, SNR, receiver sensitivity**

### Technical Reading Passage

**5G and Massive MIMO Technology**

Fifth-generation (5G) wireless networks represent a major advancement in telecommunications. A key enabling technology is massive MIMO, which uses large antenna arrays with dozens or even hundreds of elements at the base station. By employing beamforming techniques, massive MIMO can direct narrow beams toward individual users, significantly increasing spectral efficiency and reducing interference. 5G also utilizes millimeter-wave frequencies above 24 GHz, providing enormous bandwidth for high data rates. However, millimeter-wave signals experience severe propagation losses and are easily blocked by obstacles. OFDM remains the fundamental waveform, with modifications for improved efficiency. These technologies together enable applications requiring ultra-low latency, such as autonomous driving and remote surgery.

**Comprehension Questions:**
1. What is massive MIMO and how many antenna elements does it use?
2. How does beamforming improve spectral efficiency?
3. What challenge do millimeter-wave frequencies face?
4. Name two applications requiring ultra-low latency.

---


## 6. Signal Processing

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Sampling** | The process of converting a continuous signal into a discrete sequence of values. | The sampling rate must be at least twice the maximum frequency to avoid aliasing. | نمونه‌برداری | sample rate, discretization |
| 2 | **Spectrum** | The representation of a signal in terms of its frequency components. | The spectrum of the audio signal shows dominant energy below 4 kHz. | طیف | frequency content, spectral analysis |
| 3 | **Filtering** | The process of selectively passing or blocking certain frequency components of a signal. | Low-pass filtering removes high-frequency noise from the sensor data. | فیلترینگ (پالایش) | low-pass, high-pass, band-pass |
| 4 | **Fourier transform** | A mathematical operation that decomposes a signal into its constituent frequencies. | The Fourier transform converts the time-domain signal into a frequency-domain representation. | تبدیل فوریه | DFT, DTFT, frequency analysis |
| 5 | **Frequency domain** | A representation of a signal as a function of frequency rather than time. | In the frequency domain, the filter characteristics are more easily visualized. | حوزه فرکانس | spectral representation |
| 6 | **Time domain** | A representation of a signal as a function of time. | The time domain waveform shows the amplitude variations over a 10 ms window. | حوزه زمان | temporal representation, waveform |
| 7 | **Convolution** | A mathematical operation expressing how the shape of one signal is modified by another. | The output of an LTI system is the convolution of the input with the impulse response. | کانولوشن (هم‌پیچش) | linear convolution, circular convolution |
| 8 | **Correlation** | A measure of similarity between two signals as a function of time lag. | Cross-correlation is used to detect the time delay between transmitted and received signals. | همبستگی | autocorrelation, cross-correlation |
| 9 | **FFT** | Fast Fourier Transform; an efficient algorithm for computing the discrete Fourier transform. | The FFT reduces the computation of a 1024-point DFT from O(N²) to O(N log N). | اف‌اف‌تی (تبدیل فوریه سریع) | DFT, radix-2, butterfly |
| 10 | **Window function** | A mathematical function applied to a signal segment to reduce spectral leakage. | The Hamming window is applied before computing the FFT to minimize side lobes. | تابع پنجره | Hamming, Hanning, rectangular |
| 11 | **Aliasing** | Distortion that occurs when a signal is sampled below the Nyquist rate. | Aliasing caused the 15 kHz tone to appear as a 1 kHz artifact in the sampled signal. | آلیاسینگ (نام مستعار فرکانسی) | folding, anti-aliasing filter |
| 12 | **Nyquist** | The theorem stating that sampling rate must be at least twice the signal's maximum frequency. | According to the Nyquist theorem, a 44.1 kHz sampling rate can capture frequencies up to 22.05 kHz. | نایکوئیست | Nyquist rate, Nyquist frequency |
| 13 | **Quantization** | The process of mapping continuous amplitude values to discrete levels. | 16-bit quantization provides 65,536 discrete amplitude levels. | کوانتیزاسیون (کمّی‌سازی) | quantization error, bit depth |
| 14 | **SNR** | Signal-to-Noise Ratio; the ratio of signal power to noise power, usually in dB. | An SNR of 60 dB indicates the signal is one million times stronger than the noise. | نسبت سیگنال به نویز | dB, noise floor, dynamic range |
| 15 | **Digital filter** | A computational system that processes discrete-time signals to achieve desired filtering. | The FIR digital filter has 64 taps and a linear phase response. | فیلتر دیجیتال | FIR, IIR, filter coefficients |


### Fill-in-the-Blank Exercise

1. __________ converts a continuous signal into discrete values at regular intervals.
2. The __________ theorem states that the sampling rate must be at least twice the highest frequency.
3. __________ occurs when a signal is sampled at a rate below the Nyquist rate.
4. The __________ efficiently computes the discrete Fourier transform in O(N log N) time.
5. __________ maps continuous amplitude values to a finite set of discrete levels.
6. The __________ of a signal shows its frequency components and their magnitudes.
7. A __________ is applied to a signal segment before FFT to reduce spectral leakage.
8. __________ is the ratio of desired signal power to background noise power.

**Answer Key:** 1. Sampling, 2. Nyquist, 3. Aliasing, 4. FFT, 5. Quantization, 6. spectrum, 7. window function, 8. SNR

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Fourier transform | A. Efficient algorithm for computing DFT |
| 2. FFT | B. Distortion from undersampling |
| 3. Aliasing | C. Decomposes signal into frequency components |
| 4. Convolution | D. Measure of similarity between two signals |
| 5. Correlation | E. Processing discrete signals to filter frequencies |
| 6. Digital filter | F. How one signal shape is modified by another |
| 7. Quantization | G. Signal representation as function of frequency |
| 8. Frequency domain | H. Mapping continuous values to discrete levels |
| 9. SNR | I. Function to reduce spectral leakage |
| 10. Window function | J. Ratio of signal power to noise power |

**Answer Key:** 1-C, 2-A, 3-B, 4-F, 5-D, 6-E, 7-H, 8-G, 9-J, 10-I

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **sampling, Nyquist, aliasing**
2. **FFT, spectrum, frequency domain**
3. **digital filter, FIR, linear phase**
4. **convolution, impulse response, LTI system**
5. **quantization, bit depth, resolution**

### Technical Reading Passage

**Digital Audio Processing Pipeline**

In digital audio systems, the analog signal from a microphone first passes through an anti-aliasing filter that limits the bandwidth to below half the sampling rate. The signal is then sampled at 44.1 kHz or 48 kHz, satisfying the Nyquist criterion for the audible range up to 20 kHz. Each sample undergoes quantization, typically at 16 or 24 bits, introducing a small quantization error. The digital samples can then be processed using digital filters for equalization, noise reduction, or effects. The FFT is commonly used to analyze the spectral content of audio frames. Finally, a DAC and reconstruction filter convert the processed digital signal back to analog for playback through speakers.

**Comprehension Questions:**
1. What is the purpose of the anti-aliasing filter?
2. Why is a 44.1 kHz sampling rate sufficient for audio?
3. What is quantization error and how is it minimized?
4. What role does the FFT play in the audio processing pipeline?

---


## 7. AI and Machine Learning in Engineering

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Neural network** | A computational model inspired by biological neurons, consisting of interconnected layers. | The neural network was trained to classify faults in power system equipment. | شبکه عصبی | neurons, layers, weights, activation |
| 2 | **Training** | The process of adjusting model parameters using data to minimize error. | Training the model on 10,000 labeled images took approximately 6 hours on a GPU. | آموزش | learning, optimization, epochs |
| 3 | **Inference** | Using a trained model to make predictions on new, unseen data. | The inference time of the model is less than 5 ms per image on the edge device. | استنتاج | prediction, deployment, runtime |
| 4 | **Dataset** | A collection of data samples used for training, validation, or testing a model. | The dataset contains 50,000 labeled samples of power quality disturbances. | مجموعه‌داده (دیتاست) | training set, test set, validation set |
| 5 | **Model** | A mathematical representation learned from data that can make predictions. | The regression model predicts energy consumption based on temperature and time of day. | مدل | architecture, parameters, weights |
| 6 | **Optimization** | The process of finding the best parameters that minimize the loss function. | Stochastic gradient descent is a common optimization algorithm for deep learning. | بهینه‌سازی | gradient descent, Adam, SGD |
| 7 | **Classification** | The task of assigning input data to one of several predefined categories. | The classification model identifies whether a signal pattern indicates a fault or normal operation. | طبقه‌بندی (دسته‌بندی) | classes, labels, softmax |
| 8 | **Prediction** | The output produced by a model when given new input data. | The model's prediction of tomorrow's solar power output has a 5% mean error. | پیش‌بینی | forecast, estimation, output |
| 9 | **Deep learning** | A subset of machine learning using neural networks with many layers. | Deep learning has achieved state-of-the-art results in image recognition and speech processing. | یادگیری عمیق | deep neural network, representation learning |
| 10 | **CNN** | Convolutional Neural Network; designed for processing grid-like data such as images. | The CNN extracts spatial features from satellite images to detect solar panel defects. | شبکه عصبی کانولوشنی | convolution layers, pooling, feature maps |
| 11 | **RNN** | Recurrent Neural Network; designed for sequential data with temporal dependencies. | The RNN processes time-series sensor data to predict equipment failure. | شبکه عصبی بازگشتی | LSTM, GRU, sequence modeling |
| 12 | **Overfitting** | When a model performs well on training data but poorly on unseen data. | Overfitting was reduced by adding dropout layers and using data augmentation. | بیش‌برازش | regularization, dropout, generalization |
| 13 | **Feature extraction** | The process of identifying and selecting relevant input variables from raw data. | Feature extraction from vibration signals reveals bearing fault characteristics. | استخراج ویژگی | feature engineering, dimensionality reduction |
| 14 | **Supervised** | A learning approach where the model is trained on labeled input-output pairs. | Supervised learning requires a labeled dataset to train the fault detection model. | نظارت‌شده (بانظارت) | labeled data, regression, classification |
| 15 | **Unsupervised** | A learning approach where the model finds patterns in data without labels. | Unsupervised clustering identified three distinct operating modes of the motor. | بدون‌نظارت | clustering, anomaly detection, PCA |


### Fill-in-the-Blank Exercise

1. A __________ is a computational model inspired by biological neurons.
2. __________ is the process of adjusting model parameters to minimize error.
3. __________ occurs when a model memorizes training data but fails on new data.
4. A __________ is a neural network designed to process grid-like data such as images.
5. __________ learning uses labeled input-output pairs for training.
6. __________ is using a trained model to make predictions on new data.
7. __________ identifies relevant variables from raw data for model input.
8. __________ is a learning approach that finds patterns without labeled data.

**Answer Key:** 1. neural network, 2. Training, 3. Overfitting, 4. CNN, 5. Supervised, 6. Inference, 7. Feature extraction, 8. Unsupervised

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Deep learning | A. Network for sequential data with temporal dependencies |
| 2. RNN | B. ML using neural networks with many layers |
| 3. Optimization | C. Collection of data samples for training/testing |
| 4. Dataset | D. Finding best parameters to minimize loss |
| 5. Classification | E. Model performs well on training but not new data |
| 6. Overfitting | F. Assigning input data to predefined categories |
| 7. CNN | G. Mathematical representation that makes predictions |
| 8. Model | H. Network for processing grid-like data |
| 9. Prediction | I. Output produced when model receives new input |
| 10. Inference | J. Using trained model on unseen data |

**Answer Key:** 1-B, 2-A, 3-D, 4-C, 5-F, 6-E, 7-H, 8-G, 9-I, 10-J

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **CNN, feature extraction, image classification**
2. **training, dataset, epochs, optimization**
3. **overfitting, regularization, generalization**
4. **RNN, time-series, prediction**
5. **unsupervised, clustering, anomaly detection**

### Technical Reading Passage

**Machine Learning for Predictive Maintenance**

Predictive maintenance uses machine learning models to forecast equipment failures before they occur. Sensors mounted on industrial motors, transformers, and turbines continuously collect vibration, temperature, and current data. Feature extraction algorithms identify patterns in these signals that correlate with degradation. A supervised classification model, trained on historical failure data, can distinguish between healthy and faulty operating conditions. Deep learning approaches such as CNNs and RNNs have shown superior performance in detecting subtle fault signatures. The trained model performs inference in real-time, alerting operators when the probability of failure exceeds a threshold. This approach significantly reduces unplanned downtime and maintenance costs.

**Comprehension Questions:**
1. What type of data do sensors collect for predictive maintenance?
2. What role does feature extraction play in the process?
3. Why are CNNs and RNNs particularly effective for fault detection?
4. What triggers an alert to operators in a predictive maintenance system?

---


## 8. Renewable Energy and Electric Vehicles

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Solar cell** | A device that converts sunlight directly into electricity through the photovoltaic effect. | The efficiency of modern silicon solar cells exceeds 22% under standard test conditions. | سلول خورشیدی | PV cell, photocell |
| 2 | **Photovoltaic (PV)** | Relating to the direct conversion of light into electricity using semiconductors. | The photovoltaic array on the rooftop generates 10 kW of peak power. | فتوولتائیک | solar, PV panel, PV system |
| 3 | **Wind turbine** | A machine that converts kinetic energy of wind into electrical energy. | The offshore wind turbine has a rated capacity of 12 MW. | توربین بادی | rotor, blade, nacelle, tower |
| 4 | **Battery** | An electrochemical device that stores and releases electrical energy. | The lithium-ion battery pack provides 75 kWh of energy storage for the EV. | باتری (باطری) | lithium-ion, lead-acid, cell, pack |
| 5 | **Energy storage** | Systems that capture energy for later use, balancing supply and demand. | Grid-scale energy storage helps integrate variable renewable generation. | ذخیره‌سازی انرژی | battery, pumped hydro, flywheel |
| 6 | **MPPT** | Maximum Power Point Tracking; an algorithm that optimizes power extraction from PV panels. | The MPPT controller adjusts the operating voltage to extract maximum power from the solar array. | ردیابی نقطه حداکثر توان | perturb and observe, incremental conductance |
| 7 | **Grid-tied** | A renewable energy system connected to the utility grid, allowing power exchange. | The grid-tied solar system exports excess energy to the utility during peak production. | متصل به شبکه | grid-connected, net metering |
| 8 | **Off-grid** | A power system that operates independently without connection to the utility grid. | The off-grid system uses batteries to store solar energy for nighttime use. | مستقل از شبکه | standalone, island mode |
| 9 | **EV (Electric Vehicle)** | A vehicle powered fully or partially by an electric motor and battery. | The EV accelerates from 0 to 100 km/h in 3.5 seconds using dual electric motors. | خودرو الکتریکی | BEV, PHEV, HEV |
| 10 | **Charging** | The process of replenishing energy in a battery from an external source. | Level 3 DC fast charging can replenish 80% of the battery in 30 minutes. | شارژ | fast charging, Level 2, Level 3 |
| 11 | **Range** | The maximum distance an electric vehicle can travel on a single full charge. | The EV has a range of 500 km on a full charge under highway driving conditions. | برد (مسافت) | range anxiety, EPA range |
| 12 | **Efficiency** | The ratio of useful output energy to total input energy, expressed as a percentage. | The overall efficiency of the solar-to-grid conversion chain is approximately 18%. | بازده (راندمان) | conversion efficiency, system efficiency |
| 13 | **Sustainability** | Meeting present energy needs without compromising future generations' resources. | Sustainability goals require a transition from fossil fuels to renewable energy sources. | پایداری (توسعه پایدار) | green energy, net-zero, decarbonization |
| 14 | **Carbon footprint** | The total greenhouse gas emissions caused by an activity, product, or system. | Electric vehicles have a lower lifetime carbon footprint compared to internal combustion vehicles. | ردپای کربن | CO₂ emissions, lifecycle assessment |
| 15 | **Smart grid** | An electricity network using digital communication to detect and react to changes in usage. | The smart grid enables demand response and real-time pricing for consumers. | شبکه هوشمند | AMI, demand response, IoT |


### Fill-in-the-Blank Exercise

1. A __________ converts sunlight directly into electricity using the photovoltaic effect.
2. __________ is an algorithm that optimizes the operating point of solar panels for maximum power.
3. A __________ system is connected to the utility grid and can export excess power.
4. The __________ of an EV refers to the maximum distance it can travel on a single charge.
5. __________ systems capture energy produced at one time for use at a later time.
6. The __________ uses digital communication technology to optimize electricity distribution.
7. __________ measures the total greenhouse gas emissions of a product or activity.
8. DC fast __________ can replenish most of an EV battery in under an hour.

**Answer Key:** 1. solar cell, 2. MPPT, 3. grid-tied, 4. range, 5. Energy storage, 6. smart grid, 7. Carbon footprint, 8. charging

### Matching Exercise

| Term | Definition |
|------|-----------|
| 1. Photovoltaic | A. Vehicle powered by electric motor and battery |
| 2. Wind turbine | B. Ratio of useful output to total input energy |
| 3. Battery | C. Operating independently of utility grid |
| 4. MPPT | D. Direct conversion of light into electricity |
| 5. Off-grid | E. Machine converting wind kinetic energy to electricity |
| 6. EV | F. Algorithm optimizing solar panel power extraction |
| 7. Efficiency | G. Electrochemical device storing electrical energy |
| 8. Smart grid | H. Meeting needs without compromising future resources |
| 9. Sustainability | I. Network using digital communication for optimization |
| 10. Carbon footprint | J. Total greenhouse gas emissions of a system |

**Answer Key:** 1-D, 2-E, 3-G, 4-F, 5-C, 6-A, 7-B, 8-I, 9-H, 10-J

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **solar cell, efficiency, photovoltaic**
2. **MPPT, maximum power, operating voltage**
3. **EV, range, battery capacity**
4. **smart grid, demand response, renewable integration**
5. **wind turbine, offshore, rated capacity**

### Technical Reading Passage

**Electric Vehicle Battery Technology**

The performance of electric vehicles depends heavily on battery technology. Modern EVs primarily use lithium-ion batteries due to their high energy density, long cycle life, and declining costs. A typical EV battery pack consists of thousands of individual cells arranged in modules. The Battery Management System (BMS) monitors cell voltages, temperatures, and state of charge to ensure safe operation and maximize battery lifespan. Fast charging technology allows drivers to replenish 80% capacity in approximately 30 minutes using DC fast chargers. However, frequent fast charging at high temperatures can accelerate battery degradation. Research into solid-state batteries promises even higher energy density and improved safety for next-generation electric vehicles.

**Comprehension Questions:**
1. Why are lithium-ion batteries preferred for modern EVs?
2. What is the role of the Battery Management System?
3. What is the trade-off associated with frequent fast charging?
4. What advantage do solid-state batteries promise over current technology?

---


## 9. Artificial Intelligence, LLMs & Machine Learning

### Vocabulary List

| # | Term | Definition | Example Sentence | Persian | Related Terms |
|---|------|-----------|-----------------|---------|---------------|
| 1 | **Artificial intelligence (AI)** | The field of computer science focused on creating systems capable of performing tasks that normally require human intelligence. | Artificial intelligence is being applied to optimize power grid operations and predict equipment failures. | هوش مصنوعی | machine learning, automation, intelligent systems |
| 2 | **Machine learning** | A subset of AI where algorithms learn patterns from data without being explicitly programmed. | Machine learning algorithms can detect anomalies in electrical signal patterns faster than traditional methods. | یادگیری ماشین | supervised learning, unsupervised learning, model |
| 3 | **Deep learning** | A branch of machine learning that uses neural networks with many hidden layers to learn complex representations. | Deep learning models have achieved remarkable accuracy in classifying power quality disturbances. | یادگیری عمیق | neural network, layers, representation learning |
| 4 | **Neural network** | A computational model consisting of interconnected nodes (neurons) organized in layers that process information. | The neural network architecture was designed with three hidden layers for motor fault classification. | شبکه عصبی | neurons, layers, weights, activation function |
| 5 | **Large language model (LLM)** | A type of AI model trained on vast amounts of text data, capable of understanding and generating human language. | Engineers are using large language models to automatically generate documentation from code comments. | مدل زبانی بزرگ | GPT, transformer, text generation |
| 6 | **Transformer (architecture)** | A neural network architecture based on self-attention mechanisms, highly effective for sequential data processing. | The transformer architecture has become the foundation of modern natural language processing systems. | ترنسفورمر (معماری) | attention, encoder-decoder, self-attention |
| 7 | **Attention mechanism** | A technique that allows a model to focus on relevant parts of the input when producing an output. | The attention mechanism enables the model to identify which sensor readings are most important for fault prediction. | مکانیزم توجه | self-attention, multi-head attention, weights |
| 8 | **Training data** | The labeled or unlabeled dataset used to teach a machine learning model to recognize patterns. | The training data for the fault detection system included 100,000 labeled voltage waveform samples. | داده آموزشی | labeled data, training set, data collection |
| 9 | **Inference** | The process of using a trained model to make predictions or decisions on new, unseen data. | The edge device performs inference in under 10 milliseconds, enabling real-time motor monitoring. | استنتاج | prediction, deployment, latency |
| 10 | **Fine-tuning** | The process of further training a pre-trained model on a specific dataset to adapt it to a particular task. | We fine-tuned the pre-trained model on our proprietary transformer fault dataset to improve accuracy. | تنظیم دقیق (فاین‌تیونینگ) | transfer learning, pre-training, adaptation |
| 11 | **Token** | The basic unit of text that a language model processes, which can be a word, subword, or character. | The LLM processes input text by breaking it into tokens, with each token representing approximately four characters. | توکن | tokenization, vocabulary, subword |
| 12 | **Context window** | The maximum number of tokens a language model can process in a single input-output interaction. | The model's context window of 128,000 tokens allows it to analyze entire technical manuals at once. | پنجره زمینه (متنی) | token limit, memory, input length |
| 13 | **Hallucination (AI)** | When an AI model generates plausible-sounding but factually incorrect or fabricated information. | Engineers must verify AI outputs carefully because hallucination can produce incorrect circuit specifications. | توهم (هوش مصنوعی) | confabulation, factual accuracy, grounding |
| 14 | **Prompt** | The input text or instruction given to a language model to elicit a desired response. | The engineer wrote a detailed prompt asking the LLM to explain the Fourier transform for signal analysis. | پرامپت (دستور ورودی) | input, query, instruction |
| 15 | **Prompt engineering** | The practice of designing and optimizing input prompts to obtain better results from language models. | Prompt engineering techniques helped the team get more accurate MATLAB code suggestions from the AI assistant. | مهندسی پرامپت | few-shot, chain-of-thought, system prompt |
| 16 | **Generative AI** | AI systems capable of creating new content such as text, images, code, or audio from learned patterns. | Generative AI tools are being used to draft technical reports and create circuit design suggestions. | هوش مصنوعی مولد | generation, creative AI, synthesis |
| 17 | **Natural language processing (NLP)** | The branch of AI focused on enabling computers to understand, interpret, and generate human language. | Natural language processing allows engineers to query technical databases using everyday language. | پردازش زبان طبیعی | text analysis, linguistics, computational linguistics |
| 18 | **Embedding** | A dense vector representation of data (words, sentences, or objects) in a continuous mathematical space. | Word embeddings capture semantic relationships, placing "voltage" and "potential" close together in vector space. | جاسازی (امبدینگ) | vector representation, semantic space, word2vec |
| 19 | **Retrieval-augmented generation (RAG)** | A technique that enhances LLM responses by retrieving relevant documents from an external knowledge base before generating. | The RAG system retrieves the latest power grid standards before generating compliance reports. | تولید تقویت‌شده با بازیابی | knowledge base, retrieval, grounding |
| 20 | **Parameter (model)** | A learnable value within a neural network (such as weights and biases) that is adjusted during training. | The large language model contains over 70 billion parameters, requiring significant computational resources for training. | پارامتر (مدل) | weights, biases, model size |
| 21 | **Supervised learning** | A machine learning approach where the model is trained on input-output pairs with known correct answers. | Supervised learning was used to train the classifier on labeled fault and no-fault power system data. | یادگیری بانظارت | labeled data, classification, regression |
| 22 | **Unsupervised learning** | A machine learning approach where the model discovers hidden patterns in data without labeled examples. | Unsupervised learning identified three distinct clusters of operating conditions in the wind turbine data. | یادگیری بدون‌نظارت | clustering, dimensionality reduction, anomaly detection |
| 23 | **Reinforcement learning** | A learning paradigm where an agent learns optimal actions through trial-and-error interaction with an environment. | Reinforcement learning optimized the energy management strategy of the microgrid by maximizing long-term reward. | یادگیری تقویتی | agent, reward, policy, environment |
| 24 | **Computer vision** | The field of AI that enables machines to interpret and understand visual information from images or video. | Computer vision algorithms inspect PCB assemblies to detect soldering defects automatically. | بینایی ماشین (کامپیوتر) | image recognition, object detection, segmentation |
| 25 | **Convolutional neural network (CNN)** | A deep learning architecture that uses convolution operations to extract spatial features from grid-like data. | The CNN achieved 98% accuracy in classifying power quality disturbance waveforms from oscilloscope images. | شبکه عصبی کانولوشنی | convolution, pooling, feature maps, filters |
| 26 | **Recurrent neural network (RNN)** | A neural network designed to process sequential data by maintaining a hidden state across time steps. | The RNN model processes time-series current measurements to predict remaining useful life of bearings. | شبکه عصبی بازگشتی | LSTM, GRU, sequence, hidden state |
| 27 | **Overfitting** | A condition where a model learns the training data too precisely, including noise, and fails to generalize to new data. | Overfitting was mitigated by applying dropout regularization and increasing the training dataset size. | بیش‌برازش | regularization, dropout, validation, generalization |
| 28 | **Dataset** | A structured collection of data samples organized for training, validating, or testing machine learning models. | The open-source dataset contains 200,000 labeled vibration signals from industrial motor bearings. | مجموعه‌داده (دیتاست) | training set, test set, validation set, data split |
| 29 | **Classification** | A supervised learning task that assigns input data points to one of several predefined discrete categories. | The classification model distinguishes between six types of power system faults with 95% accuracy. | طبقه‌بندی (دسته‌بندی) | classes, labels, softmax, decision boundary |
| 30 | **Regression** | A supervised learning task that predicts a continuous numerical output value from input features. | The regression model estimates transformer oil temperature based on load current and ambient conditions. | رگرسیون | linear regression, prediction, continuous output |


### Fill-in-the-Blank Exercise

Complete each sentence with the correct term from the vocabulary list.

1. A __________ is a neural network architecture that uses self-attention mechanisms and has become the foundation of modern NLP.
2. __________ refers to the process of adapting a pre-trained model to a specific task using a smaller, specialized dataset.
3. When an AI model generates plausible but factually incorrect information, this phenomenon is called __________.
4. The __________ determines how much text a language model can process in a single interaction.
5. __________ is the practice of designing effective input instructions to get better results from language models.
6. In __________, an agent learns to make decisions by receiving rewards or penalties from its environment.
7. A __________ is a dense vector representation that captures semantic meaning in a continuous mathematical space.
8. __________ enhances LLM outputs by first retrieving relevant information from an external knowledge base.
9. __________ is the basic unit of text processed by a language model, typically representing a word or subword.
10. The __________ approach requires labeled input-output pairs to train a predictive model.
11. __________ algorithms enable machines to interpret and understand visual information from images.
12. A model with 70 billion __________ requires enormous computational resources for training.
13. __________ is a subset of AI where algorithms learn patterns from data without explicit programming.
14. __________ AI systems can create new content such as text, images, or code from learned patterns.
15. __________ occurs when a model memorizes training data noise and performs poorly on new samples.

**Answer Key:** 1. transformer, 2. Fine-tuning, 3. hallucination, 4. context window, 5. Prompt engineering, 6. reinforcement learning, 7. embedding, 8. Retrieval-augmented generation (RAG), 9. Token, 10. supervised learning, 11. Computer vision, 12. parameters, 13. Machine learning, 14. Generative, 15. Overfitting

### Matching Exercise

Match each term (1–15) with its definition (A–O).

| Term | Definition |
|------|-----------|
| 1. Large language model (LLM) | A. The field enabling computers to understand and generate human language |
| 2. Attention mechanism | B. Creating new content such as text, images, or code from learned patterns |
| 3. Transformer | C. An AI model trained on vast text data to understand and generate language |
| 4. Prompt | D. Learning through trial-and-error interaction with an environment |
| 5. Hallucination | E. Neural network architecture based on self-attention mechanisms |
| 6. Generative AI | F. Technique allowing a model to focus on relevant parts of input |
| 7. NLP | G. The input text or instruction given to a language model |
| 8. Reinforcement learning | H. Model generates plausible but factually incorrect information |
| 9. RAG | I. Adapting a pre-trained model to a specific task |
| 10. Fine-tuning | J. Enhancing LLM responses by retrieving external documents first |
| 11. Embedding | K. A supervised task assigning data to predefined categories |
| 12. Context window | L. Maximum tokens a model can process in one interaction |
| 13. Classification | M. Dense vector representation in continuous mathematical space |
| 14. Regression | N. Deep learning architecture using convolution for spatial features |
| 15. CNN | O. Supervised task predicting a continuous numerical value |

**Answer Key:** 1-C, 2-F, 3-E, 4-G, 5-H, 6-B, 7-A, 8-D, 9-J, 10-I, 11-M, 12-L, 13-K, 14-O, 15-N

### Sentence Construction Exercise

Use the following terms to write technically correct sentences:

1. **large language model, prompt engineering, code generation**
2. **transformer, attention mechanism, sequential data**
3. **fine-tuning, pre-trained model, domain-specific dataset**
4. **RAG, knowledge base, hallucination**
5. **reinforcement learning, agent, reward, optimization**
6. **CNN, computer vision, defect detection**
7. **embedding, semantic similarity, vector space**
8. **supervised learning, classification, labeled data**
9. **overfitting, regularization, generalization**
10. **generative AI, NLP, technical documentation**

*Example answer for 1:* "By applying prompt engineering techniques, the engineer obtained accurate VHDL code generation from the large language model for the FPGA design project."

### Technical Reading Passage

**Using Machine Learning for Predictive Maintenance in Power Systems**

The reliability of electrical power systems depends on the continuous operation of critical assets such as transformers, circuit breakers, and transmission lines. Traditionally, maintenance has been either reactive (repairing after failure) or time-based (scheduled at fixed intervals). However, both approaches have significant drawbacks: reactive maintenance causes unexpected outages and costly emergency repairs, while time-based maintenance may perform unnecessary work or miss developing faults between scheduled inspections.

Machine learning offers a fundamentally better approach through predictive maintenance. By analyzing sensor data collected from power system equipment in real time, ML models can detect subtle patterns that indicate incipient failures long before catastrophic breakdown occurs. Modern transformers, for example, are equipped with sensors that continuously monitor dissolved gas concentrations in insulating oil, winding temperatures, partial discharge activity, and load current profiles. These measurements form a multivariate time-series dataset that captures the health state of the equipment.

Deep learning architectures are particularly suited to this task. Convolutional neural networks extract spatial features from vibration spectrograms and thermal images, while recurrent neural networks model temporal dependencies in sequential sensor readings. More recently, transformer-based architectures with attention mechanisms have demonstrated superior performance by capturing long-range dependencies across thousands of time steps without the vanishing gradient problem that limits traditional RNNs.

The development pipeline begins with collecting and labeling a training dataset that includes both normal operating conditions and various fault scenarios. Supervised learning algorithms train classification models to distinguish between healthy and degraded states. Unsupervised learning techniques complement this by detecting anomalies—unusual patterns that do not match any previously seen condition. Transfer learning and fine-tuning allow models pre-trained on large general datasets to be adapted to specific equipment types with limited local data.

Once trained, the model performs inference on streaming sensor data at the network edge, generating predictions with minimal latency. When the predicted probability of failure exceeds a configured threshold, the system alerts maintenance crews and recommends specific actions. Large language models are increasingly integrated into these systems to generate natural-language maintenance reports and answer operator queries about equipment condition using retrieval-augmented generation from technical manuals.

The adoption of ML-based predictive maintenance in power utilities has demonstrated measurable benefits: 30–50% reduction in unplanned outages, 25% decrease in overall maintenance costs, and extended equipment lifespan through condition-based intervention. As datasets grow and models improve through continuous learning, the accuracy and lead time of failure predictions will continue to advance, making AI an indispensable tool for modern power system operation.

**Comprehension Questions:**
1. What are the two traditional maintenance approaches, and what are their main drawbacks?
2. What types of sensor data are collected from power transformers for predictive maintenance?
3. Why are transformer-based architectures (attention models) advantageous over traditional RNNs for time-series analysis?
4. How do supervised and unsupervised learning complement each other in fault detection?
5. What is the role of transfer learning and fine-tuning in deploying models for specific equipment?
6. What does "inference at the network edge" mean, and why is low latency important?
7. How are large language models (LLMs) being integrated into predictive maintenance systems?
8. What measurable benefits has ML-based predictive maintenance demonstrated in power utilities?

---

## Quick Reference: Common Abbreviations in Electrical Engineering

| Abbreviation | Full Form | Persian |
|---|---|---|
| AC | Alternating Current | جریان متناوب |
| DC | Direct Current | جریان مستقیم |
| EMF | Electromotive Force | نیروی محرکه الکتریکی |
| IC | Integrated Circuit | مدار مجتمع |
| PCB | Printed Circuit Board | برد مدار چاپی |
| ADC | Analog-to-Digital Converter | مبدل آنالوگ به دیجیتال |
| DAC | Digital-to-Analog Converter | مبدل دیجیتال به آنالوگ |
| PID | Proportional-Integral-Derivative | تناسبی-انتگرالی-مشتقی |
| MIMO | Multiple-Input Multiple-Output | چند ورودی-چند خروجی |
| OFDM | Orthogonal Frequency-Division Multiplexing | مالتی‌پلکسینگ تقسیم فرکانس عمودی |
| FFT | Fast Fourier Transform | تبدیل فوریه سریع |
| SNR | Signal-to-Noise Ratio | نسبت سیگنال به نویز |
| CNN | Convolutional Neural Network | شبکه عصبی کانولوشنی |
| RNN | Recurrent Neural Network | شبکه عصبی بازگشتی |
| MPPT | Maximum Power Point Tracking | ردیابی نقطه حداکثر توان |
| EV | Electric Vehicle | خودرو الکتریکی |
| BMS | Battery Management System | سیستم مدیریت باتری |
| PV | Photovoltaic | فتوولتائیک |
| MOSFET | Metal-Oxide-Semiconductor FET | ترانزیستور اثر میدانی |
| KVL | Kirchhoff's Voltage Law | قانون ولتاژ کیرشهف |
| KCL | Kirchhoff's Current Law | قانون جریان کیرشهف |
| AI | Artificial Intelligence | هوش مصنوعی |
| LLM | Large Language Model | مدل زبانی بزرگ |
| NLP | Natural Language Processing | پردازش زبان طبیعی |
| RAG | Retrieval-Augmented Generation | تولید تقویت‌شده با بازیابی |
| ML | Machine Learning | یادگیری ماشین |
| RL | Reinforcement Learning | یادگیری تقویتی |

---

## Study Tips for Technical Vocabulary

1. **Active Use:** Don't just memorize definitions — use each term in a sentence related to your studies.
2. **Context Learning:** Read technical papers and identify vocabulary in context.
3. **Spaced Repetition:** Review vocabulary at increasing intervals (1 day, 3 days, 1 week, 2 weeks).
4. **Concept Mapping:** Draw connections between related terms within and across topics.
5. **Bilingual Practice:** Practice explaining concepts in both English and Persian.
6. **Technical Writing:** Write short paragraphs using 3-5 vocabulary terms from each section.
7. **Peer Discussion:** Discuss engineering concepts with classmates using the target vocabulary.

---

*End of Part 5: Technical Vocabulary Reference Appendix*
