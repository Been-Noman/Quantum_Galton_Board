# ⚛️ Project: Quantum Walks and Monte Carlo 

A collection of quantum circuit implementations designed to simulate **quantum probability distributions** using `Qiskit`. This repository explores quantum analogs of **classical distributions** through clever gate constructions and ancilla-controlled operations.

---

## 🚀   Team Name 

Turing's Church

---

## 🔬   Team Members 

1. Noman Bin Morshed (Wiser ID: gst-KYPWNvuRHBmt1oc)

---

## 🧠 Project Summary

This project showcases three unique quantum circuits that simulate:

1. **Quantum Hadamard Walk** – simulates a discrete-time quantum walk using Hadamard, CSWAP, and coin-flip logic.
2. **Quantum Exponential Distribution** – spreads amplitude exponentially using RX and CSWAP gates.
3. **Quantum-inspired Normal Distribution** – mimics bell-shaped distributions using ancilla-driven amplitude control.

All circuits are built, simulated, and visualized using `Qiskit` and `matplotlib`.

The solutions presented here are based on the approach described in the paper *"Universal Statistical Simulator"* by Mark Carney and Ben Varcoe. The implementation builds on the observation that the method outlined in the paper closely resembles a diffusion process. Pauli-X gates are employed to initialize the starting site of diffusion. Hadamard or rotation gates are then used to control the amplitude across the multiqubit system. Controlled swap (CSWAP) gates are applied to direct the amplitude to specific diffusion sites. Ancilla qubits play a dual role—facilitating the diffusion of amplitude throughout the multiqubit configuration and enabling the resetting of qubits. This methodology is not limited to normal, exponential, and Hadamard quantum walk distributions; it can be extended to simulate a wide range of probability distributions.

---

## 📁 Directory Structure

```bash
.
├── Quantum Hadamard Walk.ipynb                    # Quantum Hadamard Walk
├── Quantum Exponential Distribution.ipynb         # Quantum Exponential Distribution
├── Normal Distribution.ipynb                      # Quantum Bell/Normal-like Distribution
├── README.md                                      # Project documentation

