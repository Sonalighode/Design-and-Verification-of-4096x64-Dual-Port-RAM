<h1> Design and Verifiation of 4096x64 Dual Port RAM </h1>

<h2> Intoduction</h2>

1. **Memory Capacity**: 4096 words, each 64 bits wide.
2. **Dual-Port Access**: Provides simultaneous read/write operations.
3. **Concurrent Operations**: Allows simultaneous access to different addresses.
4. **Addressing**: 12-bit wide address lines.
5. **Data Buses**: 64-bit data.
8. **Low Latency**: Quick data retrieval and storage.
9. **Applications**: Suitable for networking, video processing, and high-speed data transfer tasks.

<h2> Block Diagram </h2>

![image](https://github.com/user-attachments/assets/14f5c9a4-c82a-4f7e-97b7-aba5b1b341c1)

1. **clk (Clock)**: Synchronizes the operations of the RAM.
2. **rst (Reset):** Resets the RAM to a known initial state.
3. **data_in (Data Input)**: Carries the 64-bit data to be written into the RAM.
4. **wr_addr (Write Address)**: Specifies the 12-bit address location for writing data.
5. **rd_addr (Read Address)**: Specifies the 12-bit address location for reading data.
6. **write (Write Enable)**: Enables write operations when asserted.
7. **read (Read Enable)**: Enables read operations when asserted.
8. **data_out (Data Output)**: Carries the 64-bit data read from the RAM.

<h2> Simulation waveform </h2>

![image](https://github.com/user-attachments/assets/10b8ced4-7d06-4982-be2f-71bdde5d3994)

<h2> Verification Plan </h2>

1. **Transaction:**
   - Base class: Contained with read address, write address, input data, read and write control signals.
   - Extended classes: 3 classes for 3 different test cases applied for achieving greater coverage.

2. **Transactors:**
   - Generator: For generating random transactions.
   - Driver: Read and write drivers to drive address, input data and control signals for read and write operations respectively.
   - Monitor: Read and write monitor to collect the read adress and output data and forward to reference model and scoreboard.
   - Reference model: Functionality depicting the duv written using System Verilog.
   - Scoreboard: Comparing the transations recieved from reference model and read monitor and give the comparison results. Consists of covergroup as well for creating bins over read address and output data over a varied range.

<h2> Outputs </h2>

<h3> Test case 1 </h3>

![image](https://github.com/user-attachments/assets/411d2068-c30d-44af-9ee0-2ca46282984a)

![image](https://github.com/user-attachments/assets/a9595b32-54ba-4f89-b249-75378c27cfc0)

<h3> Test cse 2 </h3>

<h3> Test case 3 </h3>

<h2> Conclusion </h2>

Successfully caried out the design and verification steps for the dual port RAM using Mentor Graphics tools: Modelsim, Questasim.




