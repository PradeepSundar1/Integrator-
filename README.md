## Experiment No: 4
INTEGRATOR USING OP-AMP (μA741)
## Aim
To design and simulate an Integrator circuit using μA741 in Proteus Design Suite and verify that the output is proportional to the integral of the input voltage.
## Apparatus Required
•	μA741 Op-Amp
•	Resistor R = 10 kΩ
•	Capacitor Cf = 0.01 µF
•	Signal Generator
•	Dual Power Supply (±15V)
•	CRO / Oscilloscope
•	Connecting wires
## Circuit Diagram

![WhatsApp Image 2026-02-23 at 9 35 31 AM](https://github.com/user-attachments/assets/a6fd575b-202e-4f14-ad43-7413a425b5a6)

## Connection Details:
•	Input signal → Resistor (R) → Inverting terminal (Pin 2)
•	Feedback capacitor (Cf) → Between Output (Pin 6) and Pin 2
•	Non-inverting terminal (Pin 3) → Ground
•	Pin 7 → +15V
•	Pin 4 → −15V
## Theory
An Integrator circuit produces an output voltage proportional to the integral of the input voltage.
## Working Principle:
•	When input is constant → output is ramp signal
•	Output is inverted
•	Output depends on time
For Sine Wave Input:
•	Output lags input by 90°
•	Output amplitude decreases with frequency
## Procedure
1.	Open Proteus software.
2.	Select μA741, resistor, capacitor, signal generator, and CRO.
3.	Connect circuit in integrator configuration.
4.	Apply ±15V power supply.
5.	Set input waveform (1V, 1kHz).
6.	Run simulation.
7.	Observe input and output waveforms on CRO.
## Tabulation
| S.No | Input Signal              | Frequency | Expected Output                       | Practical Observation                           |
| ---- | ------------------------- | --------- | ------------------------------------- | ----------------------------------------------- |
| 1    | Square Wave               | 100 Hz    | Positive & negative spikes (impulses) | Sharp spikes at rising & falling edges observed |
| 2    | Triangular Wave           | 100 Hz    | Square Wave                           | Square waveform obtained                        |
| 3    | Sine Wave                 | 100 Hz    | Cosine Wave (90° lead)                | Phase-shifted sine (cosine) observed            |
| 4    | Square Wave (higher freq) | 1 kHz     | Higher amplitude spikes               | Narrower and sharper spikes seen                |
| 5    | Sine Wave (higher freq)   | 1 kHz     | Higher amplitude cosine               | Output amplitude increased                      |

## Waveforms

![WhatsApp Image 2026-02-23 at 9 35 30 AM](https://github.com/user-attachments/assets/8f56cd83-5b9b-4755-92f8-cb4f919280ac)

![WhatsApp Image 2026-02-23 at 9 35 31 AM (1)](https://github.com/user-attachments/assets/d17d9b18-0ee4-47e9-8270-95f8abdb3048)

![WhatsApp Image 2026-02-23 at 9 35 31 AM (2)](https://github.com/user-attachments/assets/af8721c0-8d1f-4fd7-b48a-71950929b686)

## Result
The Integrator circuit using μA741 Op-Amp was successfully designed and simulated in Proteus.
The output waveform is proportional to the integral of the input signal.
The circuit behaves as an integrator.
## Conclusion
•	Output lags input by 90° (for sine input).
•	Output amplitude decreases with increase in frequency.
•	Used in waveform generation and analog computation.
## Viva Questions
1.	What is an integrator circuit?
2.	Write the output equation of integrator.
3.	Why does output lag input?
4.	What happens at very low frequency?
5.	What is practical integrator?

## Answer
1. An integrator is an op-amp circuit in which the output voltage is proportional to the integral of the input voltage. It uses a resistor at the input and a capacitor in the feedback path.
2. Vout = -(1/RC)(Vin/dt)
3. For a sine wave input, integration converts sine into –cosine, which introduces a –90° phase shift. Therefore, the output lags the input by 90°.
4. At very low frequency, the gain becomes very high. This may cause output saturation and drift due to DC components and offset voltage.
5. A practical integrator is a modified integrator circuit that includes a resistor in parallel with the feedback capacitor to prevent excessive gain at low frequencies and improve stability.
