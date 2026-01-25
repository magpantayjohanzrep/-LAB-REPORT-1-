# EXPERIMENT 1 

# SETTING UP AN OSCILLOSCOPE 🧰 

# Objective 📌
- The goal of this experiment is to understand how a cathode ray oscilloscope (CRO) works. It involves learning how to properly configure the oscilloscope, produce a steady waveform display, and measure important characteristics of an AC signal,such as its peak-to-peak voltage and its period or frequency,using the scope’s calibration (CAL) output.


# Materials ⚙️
- Dual-channel 20 MHz oscilloscope
- Oscilloscope probe/lead
- Oscilloscope CAL (calibration) output

# Initial Setup 📌

- Adjust the intensity, focus, and display mode.

- Set the vertical controls, including AC coupling, volts per division, and vertical position.

- Set the horizontal controls such as the time per division and horizontal position.

- Configure the trigger system to AUTO, selecting the correct trigger source and slope.

# Powering Up 📌

- Switch on the oscilloscope and let it warm up.

- Fine-tune the brightness and focus to obtain a clear trace.

- Testing the Oscilloscope 📌

-  Connect Channel 1 to the CAL output.

- Check that a steady square-wave signal is visible on the display.

# Measuring Peak-to-Peak Voltage 📌

- Adjust the vertical scale so the waveform occupies most of the screen.

- Count how many vertical divisions span the waveform’s height.

- Multiply this number by the volts/div setting to get the peak-to-peak voltage.

- Record the measured Vpp value.

# Measuring Period and Frequency 📌

- Set the timebase so that one whole cycle is clearly shown.

- Count the horizontal divisions for one complete cycle.

- Multiply this by the time/div setting to determine the period.

- Compute the frequency by taking the inverse of the period.

# Results 🧪
A clear and stable square-wave from the CAL output was displayed. The peak-to-peak voltage was determined using the vertical divisions and volts/div settings. The period of the signal was obtained from the horizontal divisions and the timebase value, and the frequency was derived from the measured period.

# EXPERIMENT 2: An Introduction to the Telecoms-Trainer 101 🧰 

# Objective 📌
- This experiment provides a practical introduction to the Emona Telecoms-Trainer 101. The primary goal is to bridge the gap between theoretical block diagrams found in textbooks and physical hardware implementation.

# Materials ⚙️​

- Emona Telecoms-Trainer 101 (plus power-pack)
- Dual Channel 20MHz Oscilloscope
- two Emona Telecoms-Trainer 101 oscilloscope leads
- assorted Emona Telecoms - Trainer 101 patch leads
- For 2.1 only - one set of headphones (stereo)

# Part 2.1 Master Signals, Speech, and Buffer Modules 📌

# Circuit Diagram (Master Signals Module) ⚡

![Master Signals Module](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/91e1b71ede11ec6d4807ea3f68fabb7074b9b05b/docs/images/Screenshot%202026-01-25%20160721.png)

# Simulation 🧑‍🔧

![Master Signals](https://github.com/user-attachments/assets/ed1509e9-f817-46da-af13-21854475f405)
![Master Signals](https://github.com/user-attachments/assets/f99786af-8583-420e-a902-1600006f1005)

# Circuit Diagram (The Speech Module)

![Speech Module](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/a4e8689854dfe9545c7f2b2e5a7ba14e361ad451/docs/images/Screenshot%202026-01-25%20161538.png)

# Simulation 🧑‍🔧

![Image](https://github.com/user-attachments/assets/1c01ed0f-8caa-4005-8e85-6a458edd0ca0)

# Speech Module with Voice Input

https://github.com/user-attachments/assets/256c4d18-d75f-432f-a864-f71a33d00cf1

# Circuit Diagram (Buffer Module)

![Buffer Module](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/89860f7b829c9219838e7da167fcc418f42dd985/docs/images/Screenshot%202026-01-25%20161851.png)

# Output Waveform when being varied

# FULLY ANTI-Clockwise until there is a waveform
![Image](https://github.com/user-attachments/assets/444a3116-6d1c-4fc5-99fb-cc8ab2969286)

# FULLY Clockwise
![Image](https://github.com/user-attachments/assets/bdd3bad1-a697-4974-a11f-739c7ca15511)

# FULLY ANTI-Clockwise
![Image](https://github.com/user-attachments/assets/3a9df7fb-1bdd-4b49-9c3c-f69f6db18e46)

# Part 2.2: The Adder and Phase Shifter Modules 📌

# 4.1 The Adder Module
Used to combine multiple signals together.
* **Control G**: Varies the gain for Input A.
* **Control g**: Varies the gain for Input B.

![Image](https://github.com/user-attachments/assets/a8a89643-1b15-430c-a668-4046a72210e1)

https://github.com/user-attachments/assets/814bf475-49ec-4525-aa0f-7c52c3288c13

# 4.2 The Phase Shifter Module
Allows a signal to be shifted by a variable amount.
* **Phase Adjust**: Varies the shift amount.
* **Phase Change**: Toggles between $0^\circ$ and $180^\circ$ base positions.
* **Capability**: Can make the signal either lead or lag the input.

![Image](https://github.com/user-attachments/assets/705fcb6c-d8aa-4edd-a7fb-2870b4691aa7)

# PHASE SHIFTED
![Image](https://github.com/user-attachments/assets/0aefe038-a927-4bf0-bd31-e8ac7caeab2b)

---

# Part 2.3: The Voltage Controlled Oscillator (VCO) 📌

The VCO differs from Master Signals because its frequency is variable rather than fixed.
![Image](https://github.com/user-attachments/assets/1f4539b3-5794-4fb3-83ac-b932e7cbf39d)

![Image](https://github.com/user-attachments/assets/9255f7e6-4b63-4c5d-b90c-f9ad020352d9)

![Image](https://github.com/user-attachments/assets/e7b9c7ce-dd2a-4306-9b3e-dadd916889e6)

# 5.1 Frequency Ranges
| Range Setting | Min Frequency | Max Frequency |
| :--- | :--- | :--- |
| **LO** | [User Data] | [User Data] |
| **HI** | [User Data] | [User Data] |

# 5.2 Electronic Control
- When a Variable DCV module is connected to the VCO input, the oscillator’s frequency can be adjusted electronically:
- Increasing the DC voltage (rotating clockwise) raises the output frequency.
 -Lowering the DC voltage (rotating counter-clockwise) decreases or brings back the frequency.

# 6. Lab Questions
- Gain vs. Attenuation – Gain means the output signal becomes larger than the input, while attenuation means the output is reduced in size.
- Clipping Description – When the gain is set too high, the waveform becomes flattened or cut off at the top and bottom, indicating it has reached the supply limits.
- VCO Frequency Behavior – Rotating the DCV control clockwise causes the VCO’s output frequency to increase.


# EXPERIMENT 3: Using the Telecoms-Trainer 101 to model equations 🧰 

# Objectives 📌

- Understand mathematical modelling in telecommunications
  Recognize that communication system outputs can be expressed using equations and learn how these can be represented physically through electronic blocks.
  
- Gain familiarity with the Emona Telecoms-Trainer 101 functional modules
  Identify and use modules such as the Adder and Phase Shifter to construct simple mathematical relationships between signals.

- Implement and observe equations using real electronic signals
  
  Use the Trainer to realize equations such as:
  Output = Signal A + Signal B
  Output = Signal A + Signal B (with phase shift)
  Measure and compare theoretical and actual results.

- Analyze the effect of phase shifts on signal addition


# Material and Components Used ⚙️
- Emona Telecoms-Trainer 101 (plus power pack)
- Dual Channel 20MHz Oscilloscope
- two Emona Telecoms-Trainer 101 oscilloscope leads
- assorted Emona Telecoms-Trainer 101 patch leads


# Circuit Diagram (Figure 2) ⚡

![FIGURE 2](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/d4ca395e4cf3c554b7d8f29c1c5447ca00d16bde/docs/images/Screenshot%202026-01-21%20190551.png)

# Simulation and Wiring (Figure 2) 🧑‍🔧

![Simulation](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/6d76f86d5ad14a35605cd53cdbe5ce3b489189cd/docs/simulation_files/617358095_897551446298750_1158340221468789675_n.jpg)
![Wiring](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/ad17bb398c23420d14f65d6ba15d1f05d7514f4c/docs/images/616399135_1400971971738258_8887335393957020740_n.jpg)

# Results and Discussion for Figure 2🖋📒

- Question 1:
  Is the Adder module's measured output voltage exactly 8vp-p as theoretically predicted?

Answer: 

No, the Adder module’s measured output voltage is not exactly 8 Vp-p as predicted in theory. While the theoretical value assumes ideal conditions, the actual output is affected by factors such as module tolerances, internal losses, signal attenuation, and slight mismatches in the input amplitudes. These real-world imperfections cause the measured Vp-p to deviate from the calculated 8 Vp-p.

- Question 2:
  What are the two reasons for this?

Answer: 
- Measurement error, since oscilloscope readings are not perfectly precise.
- The module gains are not exactly 1, meaning the system does not behave ideally, causing small deviations from the theoretical output.

# Summarization

For the setup shown in Figure 2, the Master Signals module provided a 2 kHz sinewave with an amplitude of approximately 4 Vp-p, which served as the input for both channels of the Adder module. After the gains of the Adder’s inputs were adjusted to be nearly equal, the combined output was observed using the oscilloscope. Theoretically, adding two identical 4 Vp-p sinewaves should produce an output of 8 Vp-p, since the Adder module implements the equation Output = Signal A + Signal B.

However, the measured output was slightly different from the ideal 8 Vp-p value. This deviation is expected due to several practical factors. Oscilloscopes have limited measurement accuracy, which introduces small reading errors. Additionally, the gain controls of the Adder module cannot be set to exactly –1, resulting in slight mismatches in amplitude between the two input paths. Minor loading effects caused by the interconnected modules and probe connections can also reduce the signal amplitude.

Despite these small discrepancies, the resulting output waveform maintained the expected shape and frequency, demonstrating that the Adder module effectively performed the signal addition. The slight difference between theoretical and measured values reflects normal experimental limitations rather than incorrect modeling.

# Circuit Diagram (Figure 4) ⚡

![FIGURE 2](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/4d9737c5d8728fec64e0d1604a4a265a6cede6ef/docs/images/Screenshot%202026-01-21%20193945.png)

# Simulation and Wiring (Figure 4) 🧑‍🔧

![Simulation](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/e8475a9a4bd14f6cd67087b2277fabccb3a487a5/docs/images/615809531_2249552668871539_1734276010107472055_n.jpg)
![Wiring](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/9aa1d8be270f083e8141da0f72c77cbdffa66774/docs/images/614106418_1621581075862328_7500417655006312943_n.jpg)

# Results and Discussion for Figure 4🖋📒

 Question 3: What are two reasons for the output not being 0V as theoretically predicted?

  Answer:

  - The phase difference between the Adder’s two inputs is not exactly 180°, so the signals do not cancel perfectly.
  - The gains of the two input paths are not exactly the same, resulting in an imperfect subtraction and a non-zero output.

Question 4: What can be said about the phase shift between the signals on the Adder module's two inputs now?

Answer:

- The phase shift is now much closer to 180°, but it is still not perfectly 180°, so the signals do not fully cancel.

Question 5: What can be said about the gain of the Adder module's two inputs now?

Answer: 

The gains are now much closer to being equal, but they are still not exactly the same, which prevents perfect cancellation.

# Summarization

In the Figure 4 setup, the original 2 kHz sinewave from the Master Signals module was applied to one input of the Adder module, while the same signal was routed through the Phase Shifter module before reaching the second input. The Phase Shifter was set to provide a 180° phase shift, which means the two signals entering the Adder module had the same frequency and amplitude but were opposite in phase. Under ideal conditions, adding two perfectly equal signals that are 180° out of phase should result in complete cancellation, producing an output of 0 Vp-p.

When the output of the Adder module was measured on the oscilloscope, the resulting signal was not exactly zero, although it was significantly reduced compared to the input signals. This small remaining voltage can be explained by practical factors in the setup. The Phase Shifter does not produce a perfect 180° shift, so a slight phase error remains between the two signals. In addition, the gain settings of the Adder module may not match exactly, even when the controls are carefully adjusted. Small inaccuracies in the oscilloscope reading and minor loading effects from the leads can further contribute to a non-zero output.

Despite these limitations, the observed output still demonstrated a strong reduction in amplitude, confirming that the system effectively modeled the equation Output = Signal A + Signal B (with phase shift). The large decrease in amplitude shows that the two signals nearly cancel each other, highlighting how phase differences directly affect the result of signal addition. The small remaining output is consistent with normal experimental imperfections rather than incorrect behavior of the system.

# EXPERIMENT 4: Amplitude Modulation (AM) ∿

# Objectives 📌

- To construct the mathematical form of an AM signal using the available hardware modules.
- To examine how the message (baseband) signal interacts with the carrier signal.
- To study how different message inputs—such as a sinewave and speech—affect the modulation process.
- To compute and evaluate the modulation index ($m$) and observe what happens when the system becomes over-modulated.

# Material and Components Used ⚙️
- Emona Telecoms-Trainer 101 (plus power pack)
- Dual Channel 20MHz Oscilloscope
- two Emona Telecoms-Trainer 101 oscilloscope leads
- assorted Emona Telecoms-Trainer 101 patch leads

# Figure 1

![Diagram](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/72126976296dd6824e13e8a0a38e7bf212ab2eeb/docs/images/Screenshot%202026-01-25%20162851.png)

- Figure 1 illustrates the basic components involved in amplitude modulation. At the top, the message signal is shown as a low-frequency sine wave, representing information such as speech or music. Below it is the unmodulated carrier, a much higher-frequency sine wave that will be used to transmit the message. Since the carrier alone contains no information, its amplitude remains constant. At the bottom is the resulting AM signal, which is produced by varying the amplitude of the high-frequency carrier according to the instantaneous value of the message signal. When the message signal is high, the amplitude of the carrier increases; when the message signal is low, the carrier amplitude decreases. This variation creates an outer shape—called an envelope—that resembles the message signal.

# Figure 2

![Diagram](https://github.com/magpantayjohanzrep/-LAB-REPORT-1-/blob/72126976296dd6824e13e8a0a38e7bf212ab2eeb/docs/images/Screenshot%202026-01-25%20162916.png)

- Figure 2 presents the same AM signal but highlights its envelopes. The upper envelope traces the peaks of the modulated carrier and follows the exact shape of the message signal. The lower envelope traces the troughs of the AM wave and is the inverted version of the message. These two envelopes visually demonstrate how the message is embedded within the AM signal. Even though the modulated waveform itself oscillates rapidly, its overall outline still matches the message signal. This clearly shows that the amplitude of the carrier is being controlled by the message, which is the fundamental principle of amplitude modulation.

# Procedure 🔧

- Part A: Generating an AM signal using a simple message 📌

The setup utilizes an **Adder module** to combine a DC offset with the message signal, followed by a **Multiplier module** to modulate the carrier.

**System Block Diagram:**
1.  **DC + Message:** A 2kHz sine wave is added to a 1V DC offset.
2.  **Product:** This sum is multiplied by a 100kHz carrier sine wave.
3.  **Result:** The carrier's amplitude varies in proportion to the message's instantaneous value.

![Image](https://github.com/user-attachments/assets/d56549e6-0bab-44a3-896a-4f5c33f81594)

# Part B: Speech Modulation
The 2kHz sine wave is replaced with the **Speech module** output. Observations show that the "envelope" of the AM signal tracks the complex fluctuations of human speech.

# AM Signal using Speech Module
![Image](https://github.com/user-attachments/assets/c699fd5a-26d2-4ce5-b4f0-cedc20bd7572)

# Simulation 
https://github.com/user-attachments/assets/204a16ad-8426-46a6-ab01-0553296196aa

# Results and Discussion 🖋📒

- Question 1: In what way is the Adder module's output different from the original 2kHz sine?

Answer:  The output of the Adder module is no longer the same as the original 2 kHz sine wave because it now includes a DC offset. This causes the entire waveform to shift upward, placing most or all of it in the positive 
voltage range.

- Question 2:  What feature of the Multiplier output suggests it is an AM signal?

Answer:The Multiplier’s output can be identified as an AM signal because the outline or envelope of the high-frequency carrier follows the same shape as the lower-frequency message signal.

- Question 3: Is one of the signals in the AM complex a 2kHz sinewave?

Answer: None of the individual components in the AM spectrum is actually a 2 kHz sine wave. Although the envelope appears to have that frequency, the true frequencies present are the carrier, the carrier plus 2 kHz, and the carrier minus 2 kHz.

- Question 4: Why is there a signal out of the Multiplier even when not speaking (Speech module)?
- 
Answer: A signal still appears at the Multiplier output even with no speech input due to the DC term in the modulation equation. When the message is zero, the expression (DC+0)×carrier still produces a carrier with constant amplitude.

# Reflection/Learning Summary 💡

- Through the series of experiments using the oscilloscope and the Emona Telecoms-Trainer 101, I gained a deeper understanding of how theoretical telecommunications concepts are applied in real hardware systems. In Experiment 1, I learned not just how to operate a cathode ray oscilloscope (CRO), but also why proper setup is essential for obtaining accurate measurements. Adjusting the vertical and horizontal controls, configuring the trigger, and using the CAL output helped me understand how waveforms are displayed and how peak-to-peak voltage, period, and frequency are measured. This experiment strengthened my foundation in reading and interpreting AC signals, which became crucial in the next experiments.

- In Experiment 2, I was introduced to the Emona Telecoms-Trainer 101 and saw how the block diagrams in textbooks translate into actual circuits. Working with modules like Master Signals, Speech, Buffers, Adders, and Phase Shifters made me appreciate how each block represents a specific mathematical or functional operation. By listening to the speech module and observing the resulting signals, I understood how real audio is converted into electrical form. The Buffer and Adder experiments showed how signals can be conditioned, combined, or altered, while the Phase Shifter demonstrated how phase differences affect signal addition. The VCO experiment also taught me the idea of frequency control, where adjusting a DC voltage can vary the output frequency in real time.

- Experiment 3 further solidified the connection between equations and hardware behavior. By modeling expressions like
Output = Signal A + Signal B and
Output = Signal A + Signal B (with phase shift)
I saw how even small mismatches in gain or phase create measurable differences in the output. Ideal calculations predicted perfect addition or complete cancellation, but real results showed slight deviations, reminding me that practical systems always include imperfections such as measurement errors, component tolerances, and loading effects. These hands-on observations helped me understand why theoretical models must always consider real-world limitations.

- Finally, Experiment 4 tied together the concepts of signals, addition, multiplication, and phase by constructing an actual Amplitude Modulation (AM) system. Seeing how the carrier’s amplitude changes according to the message—first with a simple sinewave and later with speech—made the AM equation feel intuitive and visual. I learned how the envelope of the modulated wave represents the message, why the spectrum contains the carrier ± message frequencies, and how the DC offset ensures that modulation still occurs even with silence. Observing the effect of speech on the AM signal also showed me how communication systems encode real information onto high-frequency carriers for transmission.

- Overall, these experiments gave me a strong, practical understanding of signal behavior in telecommunications. I learned how equipment like oscilloscopes and functional modules reveal the true nature of electronic signals, how mathematical operations like addition, multiplication, and phase shifting occur physically, and how real-world factors affect theoretical expectations. Most importantly, I realized that telecommunications is not just about equations—it is about how these equations come alive through hardware, waveforms, and observable behaviors. This hands-on experience significantly deepened my confidence and comprehension of analog communication principles.









