# Design-and-Simulation-of-1M-16-bit-RAM-Using-32K-8-RAM-Chips
Design and Simulation of 1M × 16-bit RAM Using 32K × 8 RAM Chips

# 1M × 16-bit RAM Design Using 32K × 8 RAM Chips

## Overview
This project presents the design and simulation of a 1M × 16-bit single-port memory system using multiple 32K × 8 RAM ICs in Logisim Evolution. The design demonstrates practical memory expansion, address decoding, and chip selection techniques used in digital systems.

## Key Features
- Memory expansion using standard RAM ICs
- Hierarchical address decoding
- 16-bit data bus construction from 8-bit RAM chips
- Single-port read/write operation
- Fully simulated and verified design

## Memory Specifications
| Parameter | Value |
|---------|------|
| Memory Size | 1M × 16 bits |
| Base RAM IC | 32K × 8 |
| Address Lines | 20 (A0–A19) |
| Data Bus Width | 16 bits |
| Memory Type | Single-Port RAM |

## Design Summary
### Address Organization
- A0–A14: Internal RAM addressing
- A15–A19: Chip selection using decoders

### Data Bus Expansion
Two 32K × 8 RAM ICs are connected in parallel to form a 16-bit data bus:
- Lower byte: D0–D7
- Upper byte: D8–D15

### Chip Selection Logic
4-to-16 decoders are used to generate chip select signals, ensuring that only one memory block is active at a time and preventing data bus contention.

### Control Signals
- WE: Write Enable
- OE: Output Enable
- CS: Chip Select

## Simulation
The complete design was implemented and verified in Logisim Evolution. Correct address decoding, read/write operations, and 16-bit data transfer were successfully validated.

## Tools Used
- Logisim Evolution
- Digital Logic Design
- Memory Interfacing Concepts



## Learning Outcomes
- Understanding of RAM expansion techniques
- Address decoding and chip select implementation
- Practical memory interfacing
- Scalable digital system design


## Author
Pushap Mohan Sharma  
B.Tech – Microelectronics & VLSI  
NIT Kurukshetra
