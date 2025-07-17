Submit Model
============

Once you've evaluated your model using the MOT, you can submit it to the public catalog at mot.isitopen.ai.

Submission Workflow
-------------------

1. **Prepare your evaluation artifacts**
   - Run the evaluation form via: https://mot.isitopen.ai/model/evaluate  
   - Download the output `MOF.json` and openness badge after submission :contentReference[oaicite:1]{index=1}  

2. **Fork the MOT GitHub repository**
   - Repository: `lfai/model_openness_tool` on GitHub  
   - Create a fork and clone it locally :contentReference[oaicite:2]{index=2}  

3. **Add your model to the `models/` directory**
   - Create a new folder with your *model name* (e.g., `my‑model‑v1/`)  
   - Add:
     - `MOF.json` produced by MOT
     - Model metadata file (optional) including description, version, license, contact info
     - Optional badge snippet (e.g., `![Open Model – Class I](… )`)

4. **Submit a Pull Request**
   - Push your branch to your fork
   - Open a PR against the `main` branch of `lfai/model_openness_tool`
   - In the PR description, include:
     - Link to your MOT evaluation page or JSON preview
     - Licensing info and distribution details
     - Verified openness classification (Class I/II/III)

5. **Community review process**
   - Your submission will undergo review by MOT maintainers and community members for:
     - Accurate mapping to MOF components
     - Valid SPDX license IDs in `MOF.json`
     - Completeness and reproducibility
   - After feedback, resolve comments and merge the PR

6. **Post-merge publication**
   - Once merged, your model appears in the MOT public catalog  
   - The catalog displays:
     - Model name, openness class badge, component breakdown, metadata :contentReference[oaicite:3]{index=3}  

Badge Usage Guidelines
----------------------

Embed the badge in your:
- README, blog posts, or model card
- Website or documentation portal

Badges visually communicate your model's openness level and link back to MOT for transparency.

