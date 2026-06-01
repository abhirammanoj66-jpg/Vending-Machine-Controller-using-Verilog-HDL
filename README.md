# Vending Machine Controller using Verilog HDL

## Overview

This project implements a Finite State Machine (FSM)-based Vending Machine Controller using Verilog HDL. The design accepts ₹5 and ₹10 coin inputs, dispenses a product when the required amount is reached, and returns change when excess money is inserted.

The design was simulated and verified using Xilinx ISE and ISim Simulator.

---

## Features

- FSM-based RTL design
- Supports ₹5 and ₹10 coin inputs
- Product price fixed at ₹15
- Automatic product dispensing
- Automatic ₹5 change return for excess payment
- Behavioral simulation verification

---

## FSM States

| State | Amount Stored |
|---------|---------|
| S0 | ₹0 |
| S5 | ₹5 |
| S10 | ₹10 |
| S15 | ₹15 |

---

## Working Principle

### Case 1: Exact Payment

Input Sequence:

₹5 → ₹10

Result:

- Product Dispensed
- No Change Returned

---

### Case 2: Excess Payment

Input Sequence:

₹10 → ₹10

Result:

- Product Dispensed
- ₹5 Change Returned

---

## Inputs

- clk
- rst
- coin5
- coin10

## Outputs

- dispense
- return5

---

## Tools Used

- Verilog HDL
- Xilinx ISE 14.7
- ISim Simulator

---

## Simulation

Behavioral simulation was performed using ISim Simulator to verify:

- State transitions
- Coin accumulation
- Product dispensing
- Change return operation

---

## Files

- vending_machine.v → RTL Design
- vending_machine_tb.v → Testbench
- waveform.png → Simulation Results

---

## Concepts Learned

- Finite State Machines (FSM)
- RTL Design
- Sequential Logic
- State Transition Design
- Digital System Design
- Verilog HDL
- Functional Verification

---

## Future Improvements

- Support for multiple products
- Variable product pricing
- Inventory management
- Display interface
- FPGA implementation
