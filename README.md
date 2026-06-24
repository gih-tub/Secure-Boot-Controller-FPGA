# Secure Boot FSM

- A tamper-resistant secure boot FSM in SystemVerilog with one-hot encoding, parity protection, sticky fault latch, and state transition integrity checks, integrated with a BLAKE2b-512 hash core on Artix-7 FPGA (Basys3)
- Timing closure at 100MHz (WNS +0.263ns) via 4-stage round pipeline in the BLAKE2b compression function; post-route PPA: 4871 LUTs, 2605 FFs, 0.189W
- Functionally verified hash output against RFC 7693 test vectors and evaluated FSM resilience via directed RTL-level runtime fault injection and SystemVerilog Assertions (SVA) properties
- Reports under `/Reports`

# Block Diagram
<img width="1062" height="697" alt="image" src="https://github.com/user-attachments/assets/715604ff-c04c-4b91-ae42-ab2c745e17b1" />
