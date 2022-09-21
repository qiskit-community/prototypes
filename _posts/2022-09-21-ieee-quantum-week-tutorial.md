---
layout: post
title: "2022 IEEE Quantum Week Tutorial"
tags: tutorial
permalink: /2022-ieee-quantum-week-tutorial/
---

Today, we are presenting a [tutorial](https://qce.quantum.ieee.org/2022/tutorials-program/#pedrorivero) at the 2022 IEEE Quantum Week.  Below are the installation instructions and links to resources presented.

![QR Code]({{ site.url }}{{ site.baseurl }}/assets/2022-ieee-tutorial-qrcode.svg)
https://qiskit-community.github.io/prototypes/2022-ieee-quantum-week-tutorial/

## Installation instructions

[Python](https://www.python.org/) 3.7 or higher is required.  If you are on a Mac, you will be best to stick with Python 3.7, 3.8, or 3.9, as one of the dependencies (pyscf) has not been updated to work with Python 3.10.

We recommend installing in a virtual Python environment.  The below instructions use `venv`, but you might wish to use `conda` instead if you are more familiar with it.

### Preliminaries

The following commands create a new directory, then create and activate a virtual environment inside it.

```sh
mkdir ieee-quantum-prototypes-tutorial
cd ieee-quantum-prototypes-tutorial
python3 -m venv venv
source venv/bin/activate
pip install -U pip
```

### Quantum Kernel Training

```sh
git clone https://github.com/qiskit-community/prototype-quantum-kernel-training.git
pip install -r prototype-quantum-kernel-training/requirements.txt
pip install -r prototype-quantum-kernel-training/requirements-dev.txt
```

([full installation instructions here](https://github.com/qiskit-community/prototype-quantum-kernel-training/blob/main/INSTALL.md))

### Quantum Random Access Optimization

```sh
git clone https://github.com/qiskit-community/prototype-qrao.git
pip install -e 'prototype-qrao/[notebook-dependencies]'
```

([full installation instructions here](https://github.com/qiskit-community/prototype-qrao/blob/main/INSTALL.md))

### Entanglement Forging

Note that the Entanglement Forging prototype depends on [pyscf](https://pyscf.org/).  It is not available on Windows, and on macOS it has not been updated to work with Python 3.10.

```sh
pip install entanglement-forging
git clone https://github.com/qiskit-community/prototype-entanglement-forging.git
```

([full installation instructions here](https://github.com/qiskit-community/prototype-entanglement-forging/blob/main/docs/2-reference_guide/reference_guide.md#installation-instructions))

### Start Jupyter notebook server locally

```sh
pip install tox notebook
jupyter notebook
```

Then, navigate in your web browser to the URL displayed to the terminal.

## Prototype repositories and resources

- [Quantum Kernel Training prototype](https://github.com/qiskit-community/prototype-quantum-kernel-training) ([background information](https://github.com/qiskit-community/prototype-quantum-kernel-training/tree/main/docs/background), [tutorials](https://github.com/qiskit-community/prototype-quantum-kernel-training/tree/main/docs/tutorials))
- [Quantum Random Access Optimization prototype](https://github.com/qiskit-community/prototype-qrao) ([background information](https://github.com/qiskit-community/prototype-qrao/blob/main/docs/background/README.md), [tutorials](https://github.com/qiskit-community/prototype-qrao/tree/main/docs/tutorials), [explanatory video](https://www.youtube.com/watch?v=y-k4--0ZbGo), [Qiskit Algorithms tutorials](https://qiskit.org/documentation/tutorials.html#algorithms), [Qiskit Optimization tutorials](https://qiskit.org/documentation/optimization/tutorials/index.html#optimization-tutorials))
- [Entanglement Forging prototype](https://github.com/qiskit-community/prototype-entanglement-forging) ([background information](https://github.com/qiskit-community/prototype-entanglement-forging/blob/main/docs/3-explanatory_material/explanatory_material.md), [tutorials](https://github.com/qiskit-community/prototype-entanglement-forging/tree/main/docs/1-tutorials))
