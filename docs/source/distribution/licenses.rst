Select and Verify Licenses
==========================

Choosing the correct license is a critical step in promoting openness, reuse, and trust for your model.

Licenses must be **valid SPDX licenses** to be accepted by the Model Openness Tool (MOT). This ensures compatibility with the openness evaluation system and compliance with recognized open standards.

Acceptable Licenses
-------------------

MOT evaluates models based on whether they use open and recognized SPDX licenses. A full list of valid SPDX licenses can be found at:

- https://spdx.org/licenses/

When submitting a model, MOT will automatically verify the license string against the SPDX list.

Best Practices
--------------

- ✅ Use an open license such as `MIT`, `Apache-2.0`, or `BSD-3-Clause`.
- ⚠️ Avoid custom or proprietary license strings that are not SPDX-compliant.
- 📄 Include a `LICENSE` file in your model repository for transparency.

SPDX and MOF
------------

The **Model Openness Framework (MOF)** emphasizes SPDX license usage as part of its reproducibility and openness metrics. See the :doc:`intro/mof` page for how licensing influences MOF scoring.

License Verification Example
----------------------------

MOT verifies licenses during submission. For example:

json
{
  "license": "Apache-2.0"
}

