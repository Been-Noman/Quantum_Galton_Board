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

1. **Quantum-inspired Normal Distribution** – mimics bell-shaped distributions using ancilla-driven amplitude control.
2. **Quantum Exponential Distribution** – spreads amplitude exponentially using RX and CSWAP gates.
3. **Quantum Hadamard Walk** – simulates a discrete-time quantum walk using Hadamard, CSWAP, and coin-flip logic.

All circuits are built, simulated, and visualized using `Qiskit` and `matplotlib`.

The solutions presented here are based on the approach described in the paper *"Universal Statistical Simulator"* by Mark Carney and Ben Varcoe. The implementation builds on the observation that the method outlined in the paper closely resembles a diffusion process. Pauli-X gates are employed to initialize the starting site of diffusion. Hadamard or rotation gates are then used to control the amplitude across the multiqubit system. Controlled swap (CSWAP) gates are applied to direct the amplitude to specific diffusion sites. Ancilla qubits play a dual role—facilitating the diffusion of amplitude throughout the multiqubit configuration and enabling the resetting of qubits. This methodology is not limited to normal, exponential, and Hadamard quantum walk distributions; it can be extended to simulate a wide range of probability distributions.

To model realistic execution conditions, hardware noise models based on "FakeGeneva", a "Fake Backend" provided by IBM were incorporated. Circuit optimization techniques, including standard transpilation and AI-assisted transpiling, were employed to enhance performance. For smaller circuits, fidelities remained high—around 90%—and the optimized versions effectively reproduced the desired probability distributions across multiple levels. While fidelity dropped to approximately 60% for systems involving more than 10 qubits, the optimized circuits still demonstrated strong alignment with the target distributions. Importantly, no leakage from the ideal results was observed, ensuring the reliability of the simulation outcomes.

---

## 🧠 Project Presentation Deck

Link: [Presentation Deck](https://1drv.ms/p/c/cba382d5b6a0311d/EaeYENPkpuJBg_CDo1HajbcBZv7NW0B0Wm1rHb1S66KJfA?e=P1Q6yI)

---

## 📁 Directory Structure

```bash
.
├── Task-1:       Universal Statistical Simulator Summary.pdf                  # Paper Summary
├── Task-2:       Normal Distribution.ipynb                                    # Quantum Bell/Normal-like Distribution
├── Task-3-a:     Quantum Exponential Distribution.ipynb                       # Quantum Exponential Distribution
├── Task-3-b:     Quantum Hadamard Walk.ipynb                                  # Quantum Hadamard Walk
├── Task-4&5-a:   Normal Distribution Error Modeling & Analysis.ipynb          # Quantum Bell/Normal-like Distribution Under Thermal Noise
├── Task-4&5-b:   Exponential Distribution Error Modeling & Analysis.ipynb     # Quantum Exponential Distribution Under Thermal Noise
├── Task-4&5-c:   Hadamard Walk Error Modeling & Analysis.ipynb                # Quantum Hadamard Walk Under Thermal Noise
├── Presentation Deck.pptx                                                     # Project presentation
├── README.md                                                                  # Project documentation



