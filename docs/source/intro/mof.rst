Model Openness Framework (MOF)
==============================

The **Model Openness Framework (MOF)** is a structured, license-aware framework designed to assess the openness and completeness of machine learning model releases. It was created to prevent "open-washing"—the practice of claiming models as open without providing sufficient artifacts or legal clarity.

Framework Overview
------------------

MOF evaluates models across three levels of openness:

- **Class I (Full Open Science Bundle)**: Includes all critical artifacts—training code, datasets, model checkpoints, and documentation—released under open licenses.
- **Class II (Tooling Open)**: Provides sufficient materials to reproduce the model (e.g., training/evaluation code) but may omit key artifacts like datasets or model weights.
- **Class III (Basic Model Release)**: Minimal release, often including only model weights and limited documentation.

Each release is also evaluated for *completeness*, based on the presence of 16 specific components (described below).

The 16 MOF Components
---------------------

Each model submission is assessed across the following 16 components:

1. **Model Card**
2. **Data Card**
3. **Training Data**
4. **Test Data**
5. **Preprocessing Code**
6. **Training Code**
7. **Evaluation Code**
8. **Inference Code**
9. **Model Architecture**
10. **Model Checkpoints**
11. **Hyperparameters**
12. **Results**
13. **Diagrams**
14. **Research Paper**
15. **Licenses**
16. **README / Docs**

Each component is marked as:

- ✅ Released under a clearly open license (e.g., Apache-2.0, MIT, CC-BY-4.0)
- ⚠️ Released but with unclear/restrictive terms
- ❌ Not released

These annotations help determine the overall openness classification.

Licensing Considerations
------------------------

MOF emphasizes the use of SPDX-recognized licenses. Recommended licenses include:

- **Code**: Apache-2.0, MIT, BSD-3-Clause
- **Data**: CC-BY-4.0, CDLA-Sharing, ODbL
- **Documentation**: CC-BY-4.0

Models released with proprietary or ambiguous licenses may not qualify as fully open even if the components are technically present.

Openness Badges
---------------

After evaluation, a model is awarded an openness class badge:

- ``Class I`` → 🟢 Full Open Science Bundle
- ``Class II`` → 🟡 Tooling Open
- ``Class III`` → 🔴 Basic Release

These badges help users quickly understand the transparency and reproducibility of a model.

For more information, see the original paper:  
`The Model Openness Framework <https://arxiv.org/abs/2403.13784>`_

