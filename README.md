# Single-Cycle Processor (Logisim)

## Overview
A 32-bit single-cycle processor implemented in Logisim, based on lecture-provided datapath architecture.
The processor is extended to correctly execute the given test program.
See singl

## Key Specifications
- 32-bit architecture
- Single-cycle execution
- 32-register register file (x0 is hard-wired to zero)
- Instruction Memory (ROM) / Data Memory (RAM)
- Memory access uses address bits [7:2] only
- Word-aligned instructions

## Datapath
- PC update via PC+4 or control-flow target
- ALU-based execution with Zero flag for branching
- Immediate extension controlled by instruction type
- Write-back from ALU, memory, or PC+4

## Supported Instructions
- Arithmetic / logic
- Load / store
- Branch
- **JALR (added as an extension)**

## Notes
- Control signals are generated combinationally
- Clock period is limited by the single-cycle critical path
- Design focuses on correctness and clarity rather than performance

## Files
- `single_cycle_processor.circ`: Logisim circuit files
- `single_cycle_processor_image.png`: Circuit Diagram
