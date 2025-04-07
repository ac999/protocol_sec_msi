# Security Protocols Analysis Repository

![GitHub](https://img.shields.io/badge/license-MIT-blue.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/ac999/protocol_sec_msi)

This repository contains academic work on security protocol modeling and verification completed during the Master's in Information Security program at Alexandru Ioan Cuza University of Iasi, under the guidance of Lecturer, Ph.D. Cătălin Bîrjoveanu.

## Table of Contents
- [Overview](#overview)
- [Repository Structure](#repository-structure)
- [Tools Used](#tools-used)
- [Projects](#projects)
  - [Homework 1](#homework-1)
  - [Homework 2](#homework-2)
  - [Multi-protocol Attacks](#multi-protocol-attacks)
  - [Group Authentication Presentation](#group-authentication-presentation)
- [Getting Started](#getting-started)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Overview

This repository contains formal models and analyses of various security protocols using specialized verification tools. The work focuses on:
- Protocol design and specification
- Formal verification using CL-AtSe and Scyther tools
- Analysis of security properties (authentication, secrecy, etc.)
- Group authentication protocols
- Multi-protocol attack scenarios

## Repository Structure

```
.
├── HW1/                      # Homework 1 - Basic protocol design
│   ├── proj.hlpsl            # HLPSL protocol specification
│   └── README.md             # Assignment description
│
├── HW2/                      # Homework 2 - Protocol improvements
│   ├── protocol_hw2.spdl     # Scyther protocol specification
│   └── README.md             # Assignment description
│
├── multiprotocol-attacks/    # Multi-protocol attack analysis
│   ├── Protocolv0.spdl       # Original protocol version
│   ├── Protocolv1.spdl       # Modified protocol version
│   ├── Protocolv0_v1.spdl    # Combined protocol analysis
│   └── README.md             # Analysis results
│
├── presentation/             # Group authentication presentation
│   ├── group_protocols_auth.bib  # Bibliography
│   ├── group-auth-dlp1-neq2.spdl # Protocol specification
│   ├── Prezentare_*.bib      # Presentation bibliography
│   └── Prezentare_*.tex      # Presentation LaTeX source
│
├── .gitignore                # Git ignore rules
└── README.md                 # This file
```

## Tools Used

- **CL-AtSe**: For analyzing HLPSL protocol specifications
- **Scyther**: For formal verification of security protocols
- **LaTeX**: For academic presentation and documentation
- **Git**: Version control

## Projects

### Homework 1
**Design and verification of a basic authentication protocol**

- Models a client-server authentication protocol with session key establishment
- Uses HLPSL language for specification
- Verified using CL-AtSe tool
- Based on Example 2 from the AVISPA tutorial

Key files:
- `proj.hlpsl`: Protocol specification
- `README.md`: Assignment description

### Homework 2
**Analysis and improvement of NSL protocol variant**

- Models and verifies a modified Needham-Schroeder-Lowe protocol
- Proposes and tests six protocol improvements
- Uses Scyther for formal verification

Key files:
- `protocol_hw2.spdl`: Protocol specification
- `README.md`: Analysis of improvements

### Multi-protocol Attacks
**Analysis of cross-protocol attacks**

- Contains three versions of authentication protocols
- Demonstrates how similar protocols can be vulnerable when run concurrently
- Includes visual verification results from Scyther

Key files:
- `Protocolv0.spdl`: Original protocol
- `Protocolv1.spdl`: Modified protocol
- `Protocolv0_v1.spdl`: Combined analysis

### Group Authentication Presentation
**Formal analysis of group authentication protocols**

- Presents framework for group authentication protocols
- Formal verification using Scyther
- Analysis of security properties (authentication, secrecy, etc.)

Key files:
- `Prezentare_*.tex`: Presentation LaTeX source
- `group_protocols_auth.bib`: Bibliography
- `group-auth-dlp1-neq2.spdl`: Protocol specification

## Getting Started

To reproduce the analyses:

1. Install required tools:
   - [Scyther](https://www.cs.ox.ac.uk/people/cas.cremers/scyther/)
   - [CL-AtSe](http://www.avispa-project.org/)

2. For protocol verification:
   ```bash
   scyther --verify protocol_hw2.spdl
   ```

3. To compile the presentation:
   ```bash
   pdflatex Prezentare_*.tex
   bibtex Prezentare_*.aux
   pdflatex Prezentare_*.tex
   pdflatex Prezentare_*.tex
   ```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Lecturer, Ph.D. Cătălin Bîrjoveanu for guidance
- University of Agder researchers for foundational work on group authentication protocols
- Developers of Scyther and CL-AtSe verification tools
