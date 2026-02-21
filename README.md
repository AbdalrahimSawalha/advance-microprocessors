# 8086 Memory Interface Design – Advanced Microprocessors 🔧

---

## 1. Overview 📘

This project presents the design of a complete memory interface system for the Intel 8086 microprocessor.

The design demonstrates how the 8086 communicates with external memory using address buses, data buses, and control signals. The system was designed using schematic tools and includes full memory organization and control logic implementation.

---

## 2. System Architecture 🧩

The memory interface consists of the following major components:

- Intel 8086 Microprocessor

- Address Bus (A1 – A19)

- Data Bus (D0 – D15)

- Memory Banks (Even and Odd banks)

- RAM Modules (64 KB each)

- Address Latches (SN74F373)

- Address Decoder (SN74F138)

- Bus Transceivers (74F245)

- Control Logic Circuits

---

## 3. Memory Organization 🗂️

The system uses banked memory architecture:

- Low Bank (Even addresses) → handles D0–D7

- High Bank (Odd addresses) → handles D8–D15

- Multiple 64 KB RAM modules

- Address decoding logic for memory selection

This allows proper 16-bit data access using two 8-bit memory banks.

---

## 4. Address Bus Operation 🧭

The address bus is used to select memory locations.

Functions include:

- Selecting RAM modules

- Enabling memory banks

- Providing memory addressing up to full range

Address signals are latched using SN74F373 for stable addressing.

---

## 5. Data Bus Operation 🔄

The data bus transfers data between the CPU and memory.

Includes:

- Lower data bus (D0–D7)

- Upper data bus (D8–D15)

- Controlled using bus transceivers (74F245)

This enables bidirectional data transfer.

---

## 6. Control Signals 🎛️

Control signals regulate memory operations:

- RD → Read control

- WR → Write control

- CE → Chip enable

- BHE → High bank enable

- ALE → Address latch enable

These signals ensure correct timing and memory access.

---

## 7. Address Decoding 🧠

Address decoding is implemented using SN74F138 decoder.

Functions:

- Select specific RAM modules

- Enable memory banks

- Control memory access regions

---

## 8. Project Objectives 🎯

The main objectives of this project are:

- Understand 8086 memory interface design

- Implement banked memory architecture

- Apply address decoding techniques

- Implement memory control logic

- Understand CPU-memory communication

---

## 9. Tools Used 🛠️

- EasyEDA (Schematic design)

- Intel 8086 Architecture

- Digital Logic Components

---

## 10. Author 👨‍💻

Abdalrahim Sawalha

---

## 11. Course 

Advanced Microprocessors

---
