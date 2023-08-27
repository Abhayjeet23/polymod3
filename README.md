


## Multiplication Verification Circuit ##
This repository contains a Circuit Template in Circom 2.0.0 that checks whether the value c is the multiplication of a and b. This template defines three component gates: AND, NOT, and OR, which are then used to construct the main circuit for multiplication verification.

## Table of Contents ##
Background
Circuit Template
Components
Usage
Contributing
License
## Background ##
The purpose of this circuit is to verify whether a given value c is the result of multiplying two input values a and b. It utilizes basic logic gates to construct the verification logic.

## Circuit Template ##
The main circuit template is defined in the GivenCircuit template. It uses component gates like AND, NOT, and OR to create a custom circuit. The GivenCircuit template takes two input signals, a and b, and produces an output signal Q that represents whether c is the multiplication of a and b.

## Components ##
This repository includes three circuit component templates:

AND: Implements the logical AND gate, taking two inputs a and b, and producing an output out equal to a * b.

NOT: Implements the logical NOT gate, taking an input in and producing an output out that follows the logic 1 + in - 2 * in.

OR: Implements the logical OR gate, taking two inputs a and b, and producing an output out equal to a + b - a * b.

## Usage ##
To use this circuit template, you can follow these steps:

Make sure you have Circom 2.0.0 installed on your system.

Clone this repository or download the code from main.circom.

Modify the values of a and b in the GivenCircuit template to match your desired input values.

Compile the circuit using Circom:

shell
circom main.circom
Generate the constraint system and witness:

shell
snarkjs wc circuit.r1cs witness.wtns
Use your preferred SNARK library to generate and verify proofs based on the compiled circuit, constraint system, and witness.

## Contributing ##
Contributions to this repository are welcome. Feel free to open issues and pull requests for any improvements, bug fixes, or suggestions.

## Author ##
Abhayjeet Singh

## License ##
This project is licensed under the MIT License.
