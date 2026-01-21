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

# Learnings 📘

The experiment demonstrated how mathematical equations can be represented and analyzed using actual electronic circuits. It showed that telecommunications signals are not only theoretical concepts but can also be modeled physically using functional blocks such as the Adder and Phase Shifter modules of the Emona Telecoms-Trainer 101. By applying identical and phase-shifted sinewave signals, the experiment highlighted how addition and cancellation of signals occur in real systems and how these results compare with theoretical predictions.

The activity also reinforced the importance of understanding how phase relationships affect signal behavior. The setup using a 180° phase shift clearly illustrated that two signals with equal amplitude and opposite phase ideally cancel each other, although real setups always show small deviations due to hardware limitations. Additionally, the experiment emphasized that gain settings, phase accuracy, loading effects, and oscilloscope measurement precision all play roles in why actual outputs differ slightly from calculated values.

Through analyzing these variations, the experiment provided deeper insight into the difference between ideal mathematical modeling and practical electronic implementation. It also demonstrated how critical accurate phase and amplitude control are in telecommunications systems, especially when dealing with signal addition and cancellation. Overall, the experiment strengthened the understanding of how communication equations translate into real-world signal behavior and highlighted the importance of careful measurement, module configuration, and error analysis in laboratory work.





