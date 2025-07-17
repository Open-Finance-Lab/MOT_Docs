Submit a Model
==============

Once you’ve completed the evaluation process and received your openness classification, you can submit your model to the public Model Openness Tool (MOT) catalog.

Step 1: Complete the Evaluation Form
------------------------------------

Start by visiting the evaluation form:

https://mot.isitopen.ai/model/evaluate

After filling out your model information and licenses, the tool will generate:

- A downloadable `MOF.json` file
- A corresponding openness badge (Class I, II, or III)

These files are required for submission.

Step 2: Fork the Repository
---------------------------

To submit your model, fork the official GitHub repository:

https://github.com/lfai/model_openness_tool

Clone your fork locally:

.. code-block:: bash

   git clone https://github.com/your-username/model_openness_tool.git
   cd model_openness_tool

Step 3: Add Your Model Files
----------------------------

Inside the `models/` directory, create a new folder named after your model (e.g., `my-model-name/`). Include the following:

- `MOF.json` – produced by the evaluation tool
- Optional: a `README.md` with additional model info
- Optional: badge embed code snippet

Example structure:

.. code-block:: text

   models/
     my-model-name/
       MOF.json
       README.md

Step 4: Submit a Pull Request
-----------------------------

Push your changes and open a pull request to the `main` branch of the original repository. In the pull request description, include:

- A short summary of your model
- Licensing and openness details
- A link to your evaluation result (if hosted)
- Any additional notes for reviewers

MOT maintainers will review your submission to ensure it complies with the MOF evaluation framework.

Step 5: Appear in the Public Catalog
------------------------------------

After your pull request is approved and merged, your model will be listed in the MOT public catalog:

https://mot.isitopen.ai/

Your entry will display:

- Model name and version
- MOF openness classification badge
- Component-by-component license status
- Links to your model artifacts

Step 6: Share Your Openness Badge
---------------------------------

You can embed your badge in your documentation or model card to communicate transparency to users.

Example badge snippet (HTML):

.. code-block:: html

   <a href="https://mot.isitopen.ai/model/my-model-name">
     <img src="https://mot.isitopen.ai/badge/my-model-name/badge.svg"
          alt="MOF Class I Badge">
   </a>

Refer to :doc:`../badge/badge` for more information on badge usage.

