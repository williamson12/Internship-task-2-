5 Qubit Quantum Fourier Transform (QFT) Implementation
This repository contains a Python implementation of a 5-qubit Quantum Fourier Transform (QFT) using Qiskit. The QFT transforms quantum states from the computational basis into the Fourier basis, playing a key role in many quantum algorithms.

Objective
Understand the Quantum Fourier Transform (QFT).
Implement the 5-qubit QFT using Qiskit.
Theory
What is the Quantum Fourier Transform (QFT)?
The Quantum Fourier Transform (QFT) is a unitary transformation that acts on a quantum state and converts it from the computational basis to the Fourier basis. It is a critical component in many quantum algorithms, such as Shor’s algorithm for factoring.

The 1-qubit QFT is equivalent to applying a Hadamard gate.
The multi-qubit QFT involves applying Hadamard gates followed by controlled phase shift gates, also known as controlled U1 gates.
For an N-qubit QFT:

The rotation values are successively halved for each qubit, starting from π/2, π/4, π/8, and so on.
Swap gates are applied to reverse the qubit order, though these swaps can be omitted when QFT is at the end of the circuit.
Circuit Explanation
The circuit for a 5-qubit QFT includes:

Hadamard gate applied to each qubit to put it into superposition.
Controlled phase gates (U1) with decreasing rotation angles for each subsequent qubit.
Swap gates (optional) to reverse the qubit order.
Installation
To run the implementation locally, ensure you have the following dependencies installed:

Python 3.x
Qiskit
NumPy
Matplotlib (for drawing the circuit)
