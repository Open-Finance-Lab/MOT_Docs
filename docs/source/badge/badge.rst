Badging System
==============

After evaluating a model using the Model Openness Tool (MOT), each model is assigned an **openness class badge** based on the completeness and licensing of its components. This badge makes it easy to communicate the transparency and reproducibility of a model at a glance.

Openness Classes
----------------

Each badge reflects the model's classification under the **Model Openness Framework (MOF)**:

- **Class I – Full Open Science Bundle**  
  🟢 Includes all key artifacts: code, data, checkpoints, and documentation under open licenses.

- **Class II – Tooling Open**  
  🟡 Provides code and documentation but may lack key components like data or trained weights.

- **Class III – Basic Model Release**  
  🔴 Includes minimal release (e.g., just model weights or inference code) with limited openness.

Badges are automatically generated after a model is evaluated using the MOT.

Badge Examples
--------------

Each badge is available as an embeddable image in SVG format and includes a link to the model’s detail page.

Example Class I badge embed (HTML):

.. code-block:: html

   <a href="https://mot.isitopen.ai/model/my-model-name">
     <img src="https://mot.isitopen.ai/badge/my-model-name/badge.svg"
          alt="MOF Class I Badge">
   </a>

Example Markdown format for GitHub README:

.. code-block:: markdown

   [![MOF Class I Badge](https://mot.isitopen.ai/badge/my-model-name/badge.svg)](https://mot.isitopen.ai/model/my-model-name)

Badge Customization
-------------------

Badges are generated automatically and include:

- The MOF class level (I, II, or III)
- A color-coded bar (green, yellow, or red)
- A link to the MOT model page for verification

Currently, custom design is not supported. However, you can host the badge yourself or embed it anywhere that accepts standard HTML or Markdown.

Where to Use Your Badge
------------------------

You are encouraged to display the badge in:

- GitHub repository README
- Hugging Face model card
- Academic papers or technical blogs
- Project websites
- Documentation portals

This promotes transparency and helps users quickly assess model openness.

More Information
----------------

- See :doc:`../intro/mof` to learn how openness levels are determined.
- To evaluate your model and generate a badge, visit: https://mot.isitopen.ai/model/evaluate
- To submit your badge to the public catalog, see :doc:`../submit/submit_model`
