---
layout: default
title: Why "Code" by Charles Petzold is the First Book Every Programmer Should Read
---

# Why "Code" by Charles Petzold is the First Book Every Programmer Should Read

[← Back to Home](../)

---

## What This Book Did to My Thinking

Before this book, I knew how to write code. I could make programs work. But I did not understand what was actually happening. There was a gap between my keyboard and the result on screen. Magic gap. Black box.

This book killed the magic. Now I see the chain.

When I press a key:
- Physical switch closes
- Electrical current flows
- Voltage changes propagate through circuits
- Transistors flip states
- Bits change in memory
- Pixels update on display

With keyboard, I change physical reality. Not metaphor. Actual electrons moving because I pressed plastic.

This understanding changes everything.

---

## What I Actually Learned

### Numbers are not what I thought

I "knew" binary before. 1s and 0s. Computer stuff. But I did not understand that decimal is also just a code. We use 10 symbols because we have 10 fingers. Nothing special about it.

Binary uses 2 symbols. Same math, different base. Place value works identical. 101 in binary means (1×4) + (0×2) + (1×1) = 5. Same logic as 101 in decimal meaning (1×100) + (0×10) + (1×1).

We use binary not because computers are mysterious. We use it because electricity has two natural states: on and off. High voltage, low voltage. Current flows, current stops.

Physics chooses the encoding. Not computer scientists.

### Everything is transformation

The book builds from bottom up:
1. Electricity and simple circuits
2. Switches that control current
3. Relays that amplify and chain
4. Logic gates (AND, OR, NOT) from switches
5. Adders from gates
6. Memory (flip-flops) from feedback loops
7. CPU from all components together
8. Software as instructions controlling hardware

Each layer builds on previous. Nothing appears from nowhere. When you see the full stack, programming stops being abstract symbol manipulation. It becomes control of physical systems through layers of abstraction.

### Simple rules create infinite complexity

AND gate: output 1 only if both inputs 1.
OR gate: output 1 if any input 1.
NOT gate: flip the input.

Three rules. That is it. From these three operations, you can build anything. Calculators. Memory. Processors. The computer I am typing on.

Not different magic at each level. Same simple logic, composed and layered.

### Memory is just feedback

This was big insight for me. How does circuit "remember"? Connect output back to input. Loop. Now state persists until you change it explicitly.

Flip-flop is two gates feeding each other. Set it once, it stays. Reset it, it flips and stays. This is one bit of memory. Scale it up: millions of flip-flops = gigabytes of RAM.

No special memory substance. Just loops.

---

## Why This Matters for Programming

When you understand the full chain from electrons to software:

**Debugging becomes intuition.** You reason about what machine is actually doing, not just pattern-matching error messages.

**Learning new languages becomes fast.** All languages compile to same fundamental operations. Syntax differs, substrate is identical.

**You write better code.** Understanding memory, CPU cycles, data representation helps you make smarter choices about performance and structure.

**Impostor syndrome decreases.** You are not copying tutorials hoping they work. You understand the system.

---

## How to Read This Book

Do not rush. Petzold builds each chapter on previous ones. If you skip, you miss the foundation.

Read with paper nearby. Draw the circuits. Work through the binary conversions yourself. Understanding comes from doing, not just reading.

Take your time. This is not book to finish. This is book to absorb.

---

## My Chapter Notes

Below are my detailed notes for reference.

### Part One: Foundations of Communication

**Chapter 1: Best Friends**
Core idea: communication requires shared codes. Two kids want to talk at night using flashlights. But light alone is not communication. They need system both understand.

**Chapter 2: Codes and Combinations**
Morse code: only dots and dashes. Two symbols. Yet it represents entire alphabet. Frequent letters get short codes (E is single dot). This is information theory before Shannon formalized it.

**Chapter 3: Braille and Binary Codes**
Braille uses 6 positions. Each raised or flat. 2^6 = 64 patterns. This is exactly how computers think. Not "what symbol" but "which positions are on or off."

**Chapter 4: Anatomy of a Flashlight**
Understanding circuits starts with electricity. Battery creates voltage. Circuit must be complete for current to flow. Switch breaks or completes circuit. A switch is a decision. On or off. 1 or 0.

**Chapter 5: Seeing Around Corners**
You can control something at distance using electricity. This is telegraph principle. Information travels at speed of electricity.

**Chapter 6: Telegraphs and Relays**
Relay is fundamental building block. Weak signal activates electromagnet, pulls armature, closes separate circuit. Input controls output, electrically isolated. You can chain relays.

**Chapter 7: Our Ten Digits**
Our number system is arbitrary. We use 10 symbols because 10 fingers. Place value: in 234, the 2 means 200 because of position. Nothing special about 10. Any base works.

**Chapter 8: Alternatives to Ten**
Binary (base 2): uses 0 and 1 only. Place values: 1, 2, 4, 8, 16, 32... Binary 1011 = 8+0+2+1 = 11 decimal. Why binary? Electricity has two natural states.

**Chapter 9: Bit by Bit**
Bit = Binary Digit. Smallest piece of information. Byte = 8 bits = 256 values.

### Part Two: Building Logic from Switches

**Chapter 10: Logic and Switches**
George Boole created algebra for logic. True/False. AND, OR, NOT. Claude Shannon (1937): Boolean algebra maps to electrical switches. Birth of digital logic.

**Chapter 11: Gates and Circuits**
AND gate: two switches in series. OR gate: two switches in parallel. NOT gate: normally-closed relay. NAND gate is universal: you can build any gate from NAND alone.

**Chapter 12: A Binary Adding Machine**
Half adder: adds two bits, outputs Sum and Carry. Sum = XOR, Carry = AND. Chain full adders for multi-bit numbers. Machine that can add can do anything.

**Chapter 13: But What About Subtraction?**
Two's complement: flip bits, add 1. Same adder handles positive and negative. No special hardware needed.

**Chapter 14: Feedback and Flip-Flops**
Memory requires feedback. Connect output to input. SR flip-flop: two NOR gates cross-connected. This is 1 bit of memory.

**Chapter 15: Bytes and Hex**
Hexadecimal groups 4 bits into one symbol. 0-9 then A-F. Binary 11011010 = Hex DA. Compact and direct mapping.

**Chapter 16: An Assemblage of Memory**
RAM: many flip-flops organized systematically. Address lines select byte, data lines carry value. With N address lines: 2^N locations.

### Part Three: The Computer

**Chapter 17: Automation**
Fetch-decode-execute cycle: Read instruction, decode operation, execute, update program counter, repeat. This is heartbeat of every CPU.

**Chapter 18: From Abaci to Chips**
Mechanical → vacuum tubes → transistors (1947) → integrated circuits → microprocessors (1971). Logic has not changed. Only implementation shrinks.

**Chapter 19: Two Classic Microprocessors**
Intel 8080: 8-bit data, 16-bit address, registers A/B/C/D/E/H/L. Instruction types: data movement, arithmetic, logic, control flow.

**Chapter 20: ASCII and a Cast of Characters**
ASCII: 7-bit encoding, 128 characters. Digits 0-9 are codes 48-57. Uppercase and lowercase differ by 32.

**Chapter 21: Get on the Bus**
Bus: shared wires. Address bus, data bus, control bus. Memory-mapped I/O: devices accessed like memory addresses.

**Chapter 22: The Operating System**
OS provides: file system, process management, memory management, device drivers. Abstraction: you write print(), OS handles hardware.

**Chapter 23: Fixed Point, Floating Point**
IEEE 754: sign bit + exponent + mantissa. 0.1 cannot be exactly represented. This is why 0.1 + 0.2 ≠ 0.3.

**Chapter 24: Languages High and Low**
Machine code → assembly → high-level. Each abstraction hides complexity below.

**Chapter 25: The Graphical Revolution**
Text mode → graphics mode → GUI. Event-driven programming.

---

## Core Themes

1. **Everything is encoding.** Information takes any physical form with agreed mapping.
2. **Binary is practical, not magical.** Physics chooses it.
3. **Complex from simple.** AND, OR, NOT build everything.
4. **Memory is feedback.** Loops that persist.
5. **Abstraction hides complexity.** Each layer serves the one above.
6. **Physical and logical connect.** Keyboard changes reality.

---

## Crash Course Computer Science (YouTube)

After reading Petzold, watch this series for visual reinforcement. 40 episodes, ~10 minutes each.

Playlist: [https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo](https://www.youtube.com/playlist?list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)

The book gives deep understanding. The videos give visual memory. Both together strengthen your mental model.

---

*If you read one book about computers, read this one. Everything else makes more sense after.*

[← Back to Home](../)
