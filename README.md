# RAM-design

*NAME* : PUNNAMISAIPOOJITHA

*INTERN ID* : CT04DL863

*DOMAIN* : VLSI

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH

*DESCRIPTION OF THE TASK* :

This project focuses on the development of a simple synchronous RAM (Random Access Memory) module using Verilog Hardware Description Language (HDL). The RAM is designed to support basic memory operations—namely read and write—in a synchronous manner, controlled by a clock signal. The purpose of this module is to demonstrate the fundamental working principles of memory storage and retrieval in digital systems, a critical component of most computer architectures.

The RAM is implemented as a 16-word memory array, where each word is 8 bits wide, allowing for 16 unique addresses ranging from 0 to 15. The module includes inputs for the address, data, clock, and a write enable signal, along with an output for the data read from memory. When the write enable (we) signal is high during a rising clock edge, the data present on the data_in bus is written to the specified address. When the write enable is low, the module instead reads the data from the selected memory location and presents it on the data_out bus. All memory operations are triggered on the rising edge of the clock, ensuring synchronous behavior.

To verify the design, a comprehensive testbench was developed, which simulates various read and write operations. The testbench writes known data to specific memory addresses and subsequently reads from those addresses to confirm that the correct values are retrieved. The simulation demonstrates successful data storage and retrieval, confirming the functional correctness of the RAM design.

The final deliverables for this project include the Verilog source code for the RAM module, the testbench file for verification, and a simulation report showing the expected and actual results. This project serves as a hands-on exercise in memory design, reinforcing core concepts of synchronous digital systems, and forms a key component of the CodTech internship learning experience.


*OUTPUT* :

<img width="754" alt="Image" src="https://github.com/user-attachments/assets/f9c92dc5-538a-4adb-8217-a599d07cd634" />

<img width="784" alt="Image" src="https://github.com/user-attachments/assets/4ffc3666-68ec-4d89-93ae-54989c5a47ef" />

<img width="785" alt="Image" src="https://github.com/user-attachments/assets/625c5972-68cb-4b17-927a-1ae08f729474" />

<img width="786" alt="Image" src="https://github.com/user-attachments/assets/d75bb37b-e2b3-4265-9895-4def992685f2" />

