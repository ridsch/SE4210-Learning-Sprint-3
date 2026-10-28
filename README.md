# Side-Channel & Algorithmic Complexity Educational Visualizer

An interactive educational browser tool developed for **SE/CprE 4210 (Learning Sprint #3)** to demonstrate side-channel timing leaks and algorithmic complexity vulnerabilities.

## Core Features
- **Side-Channel Mismatch Leakage:** Visualizes the vulnerability explored in Problem 2 where leaking character mismatch counts allows an attacker to recover keys in $O(N \cdot |\Sigma|)$ trials rather than brute-forcing $O(|\Sigma|^N)$.
- **Constant-Time Comparison Sandbox:** Provides an interactive toggle to compare vulnerable branch-heavy validation against safe constant-time bitwise accumulation.
- **Automated Driver Simulation:** Features an active attacker script that runs in real-time to solve secret candidates one character at a time.

## How to Run
1. Clone this repository:
   ```bash
   git clone <repo-url>