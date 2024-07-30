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

![image](https://github.com/user-attachments/assets/3bfd564a-2a2b-409f-b17e-1dca9b2276e0)

1. **clk (Clock)**: Synchronizes the operations of the RAM.
2. **data_in (Data Input)**: Carries the 64-bit data to be written into the RAM.
3. **wr_addr (Write Address)**: Specifies the 12-bit address location for writing data.
4. **rd_addr (Read Address)**: Specifies the 12-bit address location for reading data.
5. **write (Write Enable)**: Enables write operations when asserted.
6. **read (Read Enable)**: Enables read operations when asserted.
7. **data_out (Data Output)**: Carries the 64-bit data read from the RAM.
