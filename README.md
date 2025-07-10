# Web Application Coverage Dataset for Test Suite Reduction Research

This repository contains the **coverage dataset** created for the SEKE 2025 research paper:

> **Enhancing Automated Test Efficiency: A Hybrid Machine Learning Approach for Test Suite Reduction in Gray-Box Web Application Testing**  
> Elsa Paulson, Renee Bryce  
> Accepted at the 2025 International Conference on Software Engineering and Knowledge Engineering (SEKE)  
> DOI: [10.18293/SEKE2025-071](https://doi.org/10.18293/SEKE2025-071)

## 📘 Overview

We present the **first publicly available dataset of Playwright-based test coverage reports** for gray-box testing of web applications. This dataset is designed to support further research in:

- Test redundancy analysis  
- Test suite reduction (TSR)  
- Machine learning-based test optimization

The dataset covers **seven open-source web applications**, each tested using automated Playwright scripts.

## 📁 Contents

Each app folder includes:

- A set of **test case coverage reports**
- Each coverage file provides:
  - Covered **source line numbers**
  - **Execution count** per line (i.e., how many times a line was hit during test execution)

Example file format:

```json
{
  "scriptId": "app1.js",
  "url": "http://localhost/app1",
  "functions": [],
  "ranges": [
    { "startOffset": 51, "endOffset": 102, "count": 3 }
    /* ... */
  ]
}
