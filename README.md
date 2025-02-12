
# Rust-NES

Just a hobby NES emulator.

## Purpose

I am attempting to make this emulator as hardware-accurate as possible, for two reasons:

- To see how good I actually am at modeling a real-world system in software
- I have no idea how accurate an NES emulator needs to be for it to play games well. I guess I will figure that out along the way, but I like to play things safe.

In addition, I want to learn more about real-time systems that require shared resources.

## Usage

- Compiling my example ROM (A really stupid test program):
    - Ensure you have freem's [asm6f](https://github.com/freem/asm6f) installed (available in Arch Linux as `asm6f` package)
    - `asm6f sample.asm`
- Running the Emulator:
    - Have the [Rust build system](https://www.rust-lang.org/tools/install) set up
    - `cargo run --release -- [ROM.nes]`

## Roadmap

- [X] Basic hardware layout
- [ ] Header decoding
- [ ] Memory Bus
    - [X] Correct hardware mapping
    - Mappers:
        - none yet! :P
- [ ] 6502 core (56 instructions, 151 opcodes)
    - [ ] ADC
    - [ ] AND
    - [ ] ASL
    - [ ] BCC
    - [ ] BCS
    - [ ] BEQ
    - [ ] BIT
    - [ ] BMI
    - [ ] BNE
    - [ ] BPL
    - [X] BRK
    - [ ] BVC
    - [ ] BVS
    - [ ] CLC
    - [ ] CLD
    - [ ] CLI
    - [ ] CLV
    - [ ] CMP
    - [ ] CPX
    - [ ] CPY
    - [ ] DEC
    - [ ] DEX
    - [ ] DEY
    - [ ] EOR
    - [ ] INC
    - [ ] INX
    - [ ] INY
    - [ ] JMP
    - [ ] JSR
    - [ ] LDA
    - [ ] LDX
    - [ ] LDY
    - [ ] LSR
    - [X] NOP
    - [ ] ORA
    - [ ] PHA
    - [ ] PHP
    - [ ] PLA
    - [ ] PLP
    - [ ] ROL
    - [ ] ROR
    - [ ] RTI
    - [ ] RTS
    - [ ] SBC
    - [ ] SEC
    - [ ] SED
    - [ ] SEI
    - [ ] STA
    - [ ] STX
    - [ ] STY
    - [ ] TAX
    - [ ] TAY
    - [ ] TSX
    - [ ] TXA
    - [ ] TXS
    - [ ] TYA
- [ ] PPU
- [ ] APU

## Helpful Resources

- Thanks to [NESDEV](https://www.nesdev.org/wiki) for their simply amazing work on documenting the NES hardware
- mass:werk's excellent [Instruction Set](https://www.masswerk.at/6502/6502_instruction_set.html) reference
- doppelganger's [Super Mario Bros. Disassembly](https://gist.github.com/1wErt3r/4048722) for giving me some good assembly code examples to reference.

