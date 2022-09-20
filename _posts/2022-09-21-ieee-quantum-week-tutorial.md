---
layout: post
title: "2022 IEEE Quantum Week Tutorial"
tags: tutorial
permalink: /2022-ieee-quantum-week-tutorial/
---

Today, we are presenting a [tutorial](https://qce.quantum.ieee.org/2022/tutorials-program/) at the 2022 IEEE Quantum Week.  Below are the installation instructions and links to resources presented.

![QR Code]({{ site.url }}{{ site.baseurl }}/assets/2022-ieee-tutorial-qrcode.svg)
https://qiskit-community.github.io/prototypes/2022-ieee-quantum-week-tutorial/

## Installation instructions

We recommend installing in a virtual Python environment.  The below instructions use `venv`, but you might wish to use `conda` instead if you are more familiar with it.

### Preliminaries

```sh
mkdir ieee-quantum-prototypes-tutorial
cd ieee-quantum-prototypes-tutorial
python3 -m venv venv
source venv/bin/activate
```

### Quantum Kernel Training

```sh
git clone https://github.com/qiskit-community/prototype-quantum-kernel-training.git
pip install -r prototype-quantum-kernel-training/requirements.txt
pip install -r prototype-quantum-kernel-training/requirements-dev.txt
```

### Quantum Random Access Optimization

```sh
git clone https://github.com/qiskit-community/prototype-qrao.git
pip install -e 'prototype-qrao/[notebook-dependencies]'
```

### Entanglement Forging

```sh
pip install entanglement-forging
```

### Zero Noise Extrapolation

### Start Jupyter notebook server locally

```sh
pip install tox notebook
jupyter notebook
```

## Prototype repositories and resources

- [Quantum Kernel Training prototype](https://github.com/qiskit-community/prototype-qrao) ([background information](https://github.com/qiskit-community/prototype-qrao/blob/main/docs/background/README.md), [tutorials](https://github.com/qiskit-community/prototype-qrao/tree/main/docs/tutorials))
- [Quantum Random Access Optimization prototype](https://github.com/qiskit-community/prototype-quantum-kernel-training) ([background information](https://github.com/qiskit-community/prototype-quantum-kernel-training/tree/main/docs/background), [tutorials](https://github.com/qiskit-community/prototype-quantum-kernel-training/tree/main/docs/tutorials))
- [Entanglement Forging prototype](https://github.com/qiskit-community/prototype-entanglement-forging) ([background information](https://github.com/qiskit-community/prototype-entanglement-forging/blob/main/docs/3-explanatory_material/explanatory_material.md), [tutorials](https://github.com/qiskit-community/prototype-entanglement-forging/tree/main/docs/1-tutorials))
