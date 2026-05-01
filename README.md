# FPGA AES-128 Encryptor/Decryptor

This repository contains the source code and constraints for an FPGA-based AES-128 implementation. The design includes both encryption and decryption modules with hardcoded keys.It is code I contributed to the [Echipa_SSH](https://github.com/owaseraph/Echipa_SSH) project.

## Features

* AES-128 encryption and decryption cores
* Hardware implementation optimized for FPGA
* UART interface exposed via JMODA ports for data input/output
* Includes source files (`src/`) and constraint files (`constraints/`)

## Notes

* Keys are fixed (hardcoded in the design)
* No testbench is included
* Designed for on-chip operation with external UART communication

## Usage

Synthesize and program the FPGA using your preferred toolchain(guranteed to work for Vivado), then communicate with the design over UART via the JMODA interface.

## Supported boards
* Artyx 7 basys 3

## Structure

* `sources_1/` – Verilog/VHDL source files
* `constr_1/` – Pin mappings and timing constraints
