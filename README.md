# XOR Neural Network – Logic to Perceptron

This project implements the 2‑input XOR function in three ways:

1. As Boolean logic truth tables.
2. As a logic circuit in CircuitVerse using AND, OR, and NOT.
3. As a tiny 2‑layer “neural network” in Python using step‑function neurons.

## 1. XOR Logic

XOR is 1 if and only if the two input bits are different:

| A | B | XOR |
|---|---|-----|
| 0 | 0 | 0   |
| 0 | 1 | 1   |
| 1 | 0 | 1   |
| 1 | 1 | 0   |

In this project, XOR is built from:

- H1 = A AND B  
- H2 = A OR B  
- Output O = H2 AND NOT(H1)

## 2. CircuitVerse Implementation

The CircuitVerse circuit has:

- Inputs: `A`, `B`
- Hidden layer:
  - `H1 = A AND B`
  - `H2 = A OR B`
- Output layer:
  - `XOR_OUT = H2 AND NOT(H1)`

Truth table of `XOR_OUT` matches XOR: `0, 1, 1, 0`.

## 3. Python Neural Network Simulation

The same structure is implemented as a 2‑layer perceptron network:

