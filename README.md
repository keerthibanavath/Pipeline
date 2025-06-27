# Pipeline
COMPANY: CODETECH IT SOLUTIONS 
NAME: BANAVATH KEERTHI
INTERN ID: CT08DM1225
DOMAIN : VLSI
DURIATION: 8 WEEKS
MENTOR: NEELA SANTOSH
COMPANY: CODETECH IT SOLUTIONS NAME: AVULA BHUVANA PREETHI INTERN ID: CT08DN1058 DOMAIN : VLSI DURIATION: 8 WEEKS MENTOR: NEELA SANTOSH

Designing a 4-stage pipelined processor involves dividing instruction execution into 4 distinct stages, such that each stage performs a part of the instruction cycle. For simplicity, we'll implement three basic instructions: ADD, SUB, and LOAD. This processor will be implemented in Verilog, with a testbench that demonstrates pipelining in action. Pipeline Stages IF (Instruction Fetch) ID (Instruction Decode and Register Read) EX (Execute / ALU Operations) MEM/WB (Memory Access for LOAD or Write Back for ADD/SUB) Instruction Format 8-bit instruction: [7:6] – Opcode [5:3] – Destination Register [2:0] – Source Register / Memory Address Pipeline Behavior On the waveform viewer (like GTKWave), you will observe: At T1: Instruction fetched. At T2: Decode while next instruction is fetched. At T3: Execute while decode and fetch happen. At T4: Write Back while EX, ID, and IF stages are all active for other instructions. This is the binary encoding of:

Opcode: 00 → ADD Dest reg: 001 → R1 Src reg: 000 → R0 So: ADD R1, R1, R0 Conclusion This design successfully demonstrates how a pipelined processor can improve efficiency by executing different stages of multiple instructions in parallel. While the current implementation is simple and does not handle hazards (like data dependencies or control hazards), it serves as a foundational model for understanding pipelining in computer architecture. Future improvements can include support for multiple instructions, branch handling, data forwarding, and hazard detection mechanisms.
