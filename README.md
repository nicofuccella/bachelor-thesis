# Integrating ECLAIR static analysis in IDEs using the Language Server Protocol

## Description
This repository contains the final report for my bachelor's degree thesis at the University of Parma.
This bachelor thesis was supervised by Roberto Bagnara and was completed as part of my undergraduate studies in Computer Science at the University of Parma.

[Download PDF](https://github.com/nicofuccella/bachelor-thesis/raw/master/Tesi.pdf)

The base template for this thesis was provided by the University of Parma.

## Abstract
ECLAIR is a powerful platform for software verification with a strong focus on the development of high-integrity systems,
including safety-and security-critical systems. ECLAIR works on the desktop and on the server to analyze entire projects
to find possible defects. Following the “shift-left” trend (that is, performing verification activities starting from the early
development phases), the work described in this thesis aims at providing a proof-of-concept of “immediate feedback software verification” using ECLAIR.
This entails giving feedback to developers about their code correctness while they’re writing the code, directly in the IDE they use for development and without slowing down their work.
One of the challenges to be faced is the compatibility with multiple IDEs and editors. The proliferation of such coding environments, each one with its own extension standards and practices,
urges a decoupling between the IDE’s extension/plugin interface and the verification-specific smarts. The Language Server Protocol aims precisely at that: having a standardized protocol for communications between a Language Server and the IDE,
a single Language Server can be reused for multiple development environments. The transition from the traditional way in which static analysis results are consumed to this “immediate feedback” modality presents another challenge:
analysis time becomes critical and a fully satisfactory solution requires sophistication in the static analysis techniques (such as incrementality and parallelism).
We developed a proof-of-concept implementation of the integration of ECLAIR with IDEs using the Language Server Protocol. This thesis describes the underlying ideas, the challenges,
the possible solutions explored during the implementation of the proof-of-concept, the lessons learned, and the further developments that,
in our opinion, have the potential of turning the prototype into a fully fledged software development tool.

## Usage
```sh
$ pdflatex Tesi.tex

$ bibtex Tesi

$ pdflatex Tesi-frn.tex

$ pdflatex Tesi.tex
```
