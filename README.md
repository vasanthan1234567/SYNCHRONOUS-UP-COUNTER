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

![Screenshot 2025-05-05 144747](https://github.com/user-attachments/assets/5620d585-fefe-4700-9e98-a3312bcd5c71)


/* Program for flipflops and verify its truth table in quartus using Verilog programming. 

Developed by: NAME: VASANTHAN .N
RegisterNumber:212224240180
*/

**RTL LOGIC UP COUNTER**

![Screenshot 2025-05-05 143959](https://github.com/user-attachments/assets/1483ec5a-71a5-4b26-b62b-61c3ac11b202)

**TIMING DIAGRAM FOR IP COUNTER**

![Screenshot 2025-05-05 144642](https://github.com/user-attachments/assets/7fab73d9-dad1-4ac4-b18a-071bf8925734)

**TRUTH TABLE**

![326162211-b75ef146-b4c8-4718-87fa-c3d60f2c4dce](https://github.com/04Varsha/SYNCHRONOUS-UP-COUNTER/assets/149035374/a8caffaa-dc40-44b8-82dd-a12604a04eaa)


**RESULTS**

Thus the 4 bit counter is implemented successfully.
