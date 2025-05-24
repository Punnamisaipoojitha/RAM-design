# RAM-design

*COMPANY* : CODTECH IT SOLUTIONS

*NAME* : PUNNAMISAIPOOJITHA

*INTERN ID* : CT04DL863

*DOMAIN* : VLSI

*DURATION* : 4 WEEKS

*MENTOR* : NEELA SANTOSH

*DESCRIPTION OF THE TASK* :

This VHDL code describes a synchronous RAM (Random Access Memory) module named `sync_ram`, which performs read and write operations on the rising edge of a clock signal. The design is generic, allowing the user to specify the data width (`DATA_WIDTH`) and address width (`ADDR_WIDTH`) at the time of instantiation. By default, it defines an 8-bit wide data word and a 4-bit address bus, allowing access to $2^4 = 16$ memory locations.

The entity declaration defines the interface of the RAM module. The inputs include `clk` (clock), `we` (write enable), `addr` (address input), and `din` (data input). The output is `dout`, which delivers the data stored at the specified address. The generics make the design flexible and reusable for different RAM sizes by adjusting the width of data and address lines.

In the architecture, a RAM array named `ram` is declared using a user-defined array type `ram_type`, which maps address values to 8-bit vectors. The memory is initialized to all zeros using the `(others => (others => '0'))` construct. Another signal, `dout_reg`, is used to hold the output data temporarily so that it can be registered (synchronized with the clock) before being sent to the output port.

The process block is triggered on the rising edge of the clock (`rising_edge(clk)`), ensuring synchronous operation. If the write enable signal (`we`) is high, the data at the input (`din`) is written to the memory at the address specified by `addr`. Simultaneously, the content of the same address is read and assigned to `dout_reg`, regardless of whether a write is taking place. Finally, `dout` is continuously assigned the value of `dout_reg`, making the output available one clock cycle after the address is specified. This structure is typical of synchronous RAM and is useful in designing memory blocks in digital systems such as FPGAs and microprocessors.



*OUTPUT* :


<img width="754" alt="Image" src="https://github.com/user-attachments/assets/f9c92dc5-538a-4adb-8217-a599d07cd634" />


<img width="784" alt="Image" src="https://github.com/user-attachments/assets/4ffc3666-68ec-4d89-93ae-54989c5a47ef" />


<img width="785" alt="Image" src="https://github.com/user-attachments/assets/625c5972-68cb-4b17-927a-1ae08f729474" />


<img width="786" alt="Image" src="https://github.com/user-attachments/assets/d75bb37b-e2b3-4265-9895-4def992685f2" />



