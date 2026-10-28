---

### 3. Sprint Reflection Document:

# Learning Sprint #3: Reflection

### Deepening Conceptual Understanding
Building this interactive visualizer transformed abstract software security concepts into visible, observable behavior. Prior to completing Problem 2 and Problem 4, side-channel attacks and algorithmic complexity vulnerabilities felt theoretical. In standard coursework, we often evaluate functions purely based on functional correctness—whether the function outputs `true` or `false`. 

However, implementing the side-channel oracle showed how auxiliary outputs (like diff counts or microsecond execution timing delays) turn an intractable exponential search space (O(k^n)) into a trivial linear recovery (O(n*k)). Likewise, examining the Algorithmic Complexity (AC) vulnerabilities demonstrated how unoptimized nested algorithms allow untrusted input to weaponize worst-case computational complexity against availability.

### AI-Assisted Workflow
To build this application, our team used an AI-assisted workflow:
1. **Prompt Engineering & Architecture Design:** We prompted the AI with the core security invariants identified in the sprint problems (such as the character-by-character side-channel leakage from `passCheck.c` and nested collision detection bottlenecks).
2. **Rapid Prototyping:** The AI generated the single-file static HTML5/JavaScript scaffold, eliminating external library bloat and ensuring zero-dependency browser compatibility.
3. **Iterative Refinement:** We refined the simulation by having the AI implement both a vulnerable oracle and a constant-time secure oracle, adding step-by-step latency bars to clearly illustrate how side-channel measurements manifest to an outside observer.
4. **Verification & Testing:** We validated that the automated attacker accurately recovered variable-length secrets and verified that enabling the constant-time mode neutralized the exploit.