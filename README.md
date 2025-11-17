### SYNCHRONOUS-UP-COUNTER

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**

/* write all the steps invloved */

**PROGRAM**

/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

![WhatsApp Image 2025-11-17 at 12 37 40_01907c7b](https://github.com/user-attachments/assets/80ac10fa-c53c-4647-8442-d0dfb7facb25)


Developed by:JUHI JAHAN T S RegisterNumber:25011334
*/

**RTL LOGIC UP COUNTER**
![WhatsApp Image 2025-11-17 at 12 32 44_15f87df1](https://github.com/user-attachments/assets/31c3f208-06ce-4afb-a9da-f16030e20213)

**TIMING DIAGRAM FOR IP COUNTER**
![WhatsApp Image 2025-11-17 at 12 40 03_fc2f5575](https://github.com/user-attachments/assets/b64c3c59-e314-4c79-932c-90d6bea91bc0)

**TRUTH TABLE**
![WhatsApp Image 2025-11-17 at 12 40 29_f32f901e](https://github.com/user-attachments/assets/7b1637ff-73e0-4da8-b09c-e19857f8f2bd)


**RESULTS**
Hence a 4 bit synchronous up counter is implemented correctly
