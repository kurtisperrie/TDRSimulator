TDR Simulator

TRN553 Web Tool Project
By Kurtis Conant

⸻

Concept

This web tool demonstrates how a Time Domain Reflectometer (TDR) operates by simulating the step response of a transmission line terminated with different load impedances.

When a signal encounters an impedance mismatch at the load, part of the signal is reflected toward the source. This simulator visualizes that reflection at the source port, showing how its magnitude, polarity, and timing depend on the load conditions.

⸻

Equations

Reflection Coefficient
Γ = (ZL − Z0) / (ZL + Z0)

Initial Voltage
Vi = E · Z0 / (Zs + Z0)

Reflected Voltage
Vr = Γ · Vi

Return Loss
RL = −20 log |Γ| (dB)

Reflection Arrival Time
t = 2 · TD

⸻

How It Works

Each slider corresponds directly to a physical parameter. Zs and Z0 set the source and line impedance. TD controls the one-way propagation delay. ZL determines the reflection coefficient (Γ).

The five preset terminations automatically adjust the load impedance to represent common transmission line conditions.

⸻

Design Choices

The site is intentionally minimal, using a clean white single-page layout. A calculation panel is located directly below the oscilloscope so users can observe values updating in real time as parameters change.

Selecting a preset displays the termination type along with a short description. Brief instructions are included at the bottom of the page to guide the user.

⸻

Limitation

The model assumes a lossless transmission line. In reality, conductor and dielectric losses attenuate the signal. This causes the reflected waveform at the source to be smaller than what the simulator predicts, particularly for long transmission lines or high-frequency signals.

⸻

References

Anthropic. (2024). Claude AI [Large language model]. Used for web tool creation.

Maghera, H. (n.d.). TRN355 course lecture slides: Week 4 – Step response, reflections and TDR measurements. Seneca Polytechnic.
