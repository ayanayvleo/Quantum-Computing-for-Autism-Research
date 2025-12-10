# Quantum Computing for Autism Research

![Python](https://img.shields.io/badge/python-3.9+-blue.svg)
![Qiskit](https://img.shields.io/badge/qiskit-latest-purple.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-in%20development-orange.svg)

## Overview

Exploring quantum computing applications for understanding neurodiversity and autism spectrum patterns. This project uses IBM's Qiskit framework to build quantum circuits that could potentially analyze complex, high-dimensional data related to autism.

## Motivation

As an autism mom, I've experienced firsthand how complex and individual the autism spectrum is. Traditional computational approaches often struggle with the multidimensional nature of autism-related data. Just when you think you understand the patterns, something new emerges. Every child is different. Every day is different.

This project explores whether quantum computing's ability to handle high-dimensional spaces and complex pattern recognition could offer new insights into understanding neurodiversity - not through labels or categories, but through truly individualized understanding.

## The Challenge

Autism involves countless interacting factors:
- Neural connectivity patterns
- Sensory processing variations
- Genetic markers
- Environmental influences
- Behavioral characteristics
- Individual developmental trajectories

Classical computing approaches often require simplification or categorization. Quantum computing offers the potential to explore these complex, interconnected dimensions more naturally.

## What's Inside

- **Quantum Circuits**: Built with Qiskit for pattern recognition
- **Gate Operations**: Exploration of RZ, RX rotations and quantum state manipulation
- **Measurement Analysis**: Quantum state measurements and histogram visualizations
- **Research Notes**: Documentation of learning journey and findings

## Technologies Used

- **Qiskit** - IBM's open-source quantum computing framework
- **IBM Quantum Platform** - Access to real quantum hardware
- **Python 3.9+** - Primary programming language
- **OpenQASM 3.0** - Quantum assembly language
- **Matplotlib** - Data visualization

## Installation

```bash
# Clone the repository
git clone https://github.com/ayanayvleo/quantum-autism-research.git
cd quantum-autism-research

# Install required packages
pip install -r requirements.txt

# Set up IBM Quantum account (required for hardware access)
# Get your API token from https://quantum.ibm.com
```

## Quick Start

```python
import qiskit.qasm3
from qiskit_ibm_runtime import QiskitRuntimeService

# Initialize quantum circuit
qasm = """
OPENQASM 3.0;
include "stdgates.inc";
bit[4] c;
rz(-pi/2) $1;
rx(pi/2) $1;
rz(pi/2) $1;
cz $1, $0;
rz(pi/2) $0;
rx(2.7707963267948967) $0;
rz(pi/2) $0;
c[0] = measure $0;
"""

# Run on quantum hardware or simulator
# See /circuits directory for complete examples
```

## Current Status

🚧 **Early Stage Research** - This project is in active development as I learn quantum computing and explore its potential applications.

### What's Working
- Basic quantum circuits executing on IBM hardware
- Measurement and visualization of quantum states
- Pattern recognition exploration with 2-qubit systems

### In Progress
- Scaling to more complex circuits
- Implementing quantum machine learning algorithms
- Exploring variational quantum eigensolvers (VQE)
- Data encoding strategies for autism-related patterns

## Project Goals

**Short Term**
- Master quantum computing fundamentals
- Build increasingly complex quantum circuits
- Explore quantum feature mapping techniques
- Document learning process for others

**Long Term**
- Develop quantum machine learning models for pattern recognition
- Investigate applications in neurodiversity research
- Collaborate with autism research communities
- Contribute to understanding individualized support approaches

## Why Quantum Computing?

Quantum computers excel at:
- **High-dimensional optimization** - Finding patterns in complex data spaces
- **Parallel exploration** - Processing multiple possibilities simultaneously through superposition
- **Complex correlations** - Identifying relationships that classical computers struggle with
- **Feature mapping** - Transforming data into quantum states for novel analysis

These capabilities align well with the complexity of autism spectrum analysis, where traditional approaches often miss nuanced patterns.

## Repository Structure

```
quantum-autism-research/
├── circuits/           # Quantum circuit implementations
├── notebooks/          # Jupyter notebooks for exploration
├── results/            # Measurement data and visualizations
├── docs/              # Documentation and learning notes
├── requirements.txt   # Python dependencies
└── README.md         # You are here
```

## Learning Resources

New to quantum computing? Here are resources I found helpful:

- [Qiskit Textbook](https://qiskit.org/textbook/) - Free, comprehensive introduction
- [IBM Quantum Learning](https://learning.quantum.ibm.com/) - Interactive courses
- [Qiskit Documentation](https://qiskit.org/documentation/) - Official API docs
- [Quantum Computing Stack Exchange](https://quantumcomputing.stackexchange.com/) - Community Q&A

## Contributing

This is a learning project, but I welcome:
- Feedback on approach and methodology
- Suggestions for quantum algorithms to explore
- Collaborations with researchers in quantum computing or autism research
- Resources and papers related to quantum ML in healthcare

Feel free to open issues or reach out directly!

## Limitations and Disclaimers

- This is exploratory research and learning project
- Current quantum hardware is noisy and limited in scale
- No claims are made about diagnostic or clinical applications
- Results should be interpreted as proof-of-concept exploration
- This project does not replace evidence-based autism research or clinical practice

## About Me

I'm Ayana Leonard - a software developer with a BS and MS in Computer Science and an MBA. I'm a single mom in tech and an autism advocate. I started this project because I believe emerging technologies like quantum computing could eventually help us understand neurodiversity in deeper, more individualized ways.

**Connect with me:**
- GitHub: [@ayanayvleo](https://github.com/ayanayvleo)
- LinkedIn: [Ayana Leonard](https://www.linkedin.com/in/ayana-leonard/)

## Future Directions

- Expand circuit complexity and qubit count
- Implement variational quantum algorithms
- Explore quantum neural networks
- Investigate quantum support vector machines
- Connect with autism research datasets (with proper permissions)
- Collaborate with quantum computing and neurodiversity communities

## Acknowledgments

- **IBM Quantum** - For providing access to quantum hardware and the Qiskit framework
- **The Qiskit Community** - For excellent documentation, tutorials, and support
- **The Autism Community** - For inspiration and the reminder that every individual is unique
- **My daughter GG** - For being my "why" and teaching me that complexity is beautiful

## License

MIT License - See LICENSE file for details

## Citation

If you use this work in your research or projects, please cite:

```
Leonard, A. (2025). Quantum Computing for Autism Research. 
GitHub repository: https://github.com/ayanayvleo/quantum-autism-research
```

---

*"What if 'too far out' became your reason to start?"*

**Status**: Active Development | **Last Updated**: December 2025
