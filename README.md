# Constituting Valence: An Emergentist-Predictive Approach to Affective Experience (EPET)

## 📌 Overview

This repository contains materials related to the manuscript:

**"Constituting Valence: An Emergentist-Predictive Approach to Affective Experience (EPET)"**.

The manuscript introduces **Emergent Predictive Experience Theory (EPET)**, a theoretical framework that integrates predictive processing (PP), global workspace theory (GWT), and embodied self-modeling to provide a constitutive explanation of affective valence.

## 📂 Repository Structure

*   `manuscript/`: Source files of the main manuscript in Markdown (`.md`), divided by sections. Contains `input_files.txt` (for anonymous PDF) and `input_files_full.txt` (for full PDF).
*   `manuscript/Supplementary_Materials/`: Source files (`.md`) for the Supplementary Materials. Contains `input_files_sm.txt`. Includes a `README.md` describing the SM contents.
*   `assets/`: Auxiliary resources (metadata `.yaml` files, common bibliography `.bib` file, CSL citation style).
*   `scripts/`: Utility scripts (e.g., `generate_filtered_bib.py`, `check_bib.py`).
*   `output/`: Directory for generated PDF files and filtered `.bib` files (excluded from Git by `.gitignore`).
*   `Makefile`: Defines build commands and dependencies.
*   `README.md`: This file.
*   `.gitignore`: List of files ignored by Git.
*   `LICENSE`: License file (CC BY 4.0 International).

## 📑 Manuscript Contents

The main manuscript addresses the following topics:

1. Introduction and problem formulation regarding affective valence.
2. Overview of contemporary PP/FEP theories of valence.
3. Philosophical critiques and conceptual gaps in existing PP models.
4. Detailed exposition of EPET architecture, highlighting roles of predictive hierarchy, precision modulation, interoception, and the predictive self-model.
5. Empirical support for EPET from neuroscience, psychology, and cognitive science.
6. Responses to philosophical critiques within EPET.
7. Discussion, implications, and directions for future research.

## 📚 Supplementary Materials

The Supplementary Materials include additional in-depth content:

* Appendix A: Formal definitions and technical clarifications.
* Appendix B: Empirical hypotheses derived from EPET.
* Appendix C: Detailed discussions of philosophical critiques of predictive processing approaches.

## 🔧 Building the Manuscript

To build the PDF documents from the source files, you need:

1.  **Pandoc:** A universal document converter.
2.  **A LaTeX Distribution:** Such as TeX Live or MiKTeX (XeLaTeX engine is used by default).
3.  **Python 3:** Required for the bibliography generation script.
4.  **Python `bibtexparser` library:** Install via `pip install bibtexparser`.
5.  **Fonts:** Ensure DejaVu fonts (Serif, Sans, Sans Mono) are installed.

**Build Commands (using Make):**

(Run these commands from the root directory of the repository)

*   **Build all main PDFs (Full, Anonymous, SM):**
    ```bash
    make all
    ```
*   **Build only the Full PDF (with author info & references):**
    ```bash
    make output/EPET_Constituting_Valence_1.0.pdf
    ```
*   **Build only the Anonymous PDF (for journal submission):**
    ```bash
    make output/EPET_Constituting_Valence_Anonymous_1.0.pdf
    ```
*   **Build only the Supplementary Materials PDF:**
    ```bash
    make output/EPET_Constituting_Valence_Supplementary_Materials_1.0.pdf
    ```
*   **Generate filtered bibliography files (optional, usually done automatically):**
    ```bash
    make output/references_for_submission.bib
    make output/references_for_sm.bib
    ```
*   **Clean the output directory:**
    ```bash
    make clean
    ```
*   **Count words (main manuscript, excluding bibliography):**
    ```bash
    make count_words
    ```

The `Makefile` handles dependencies, including the automatic generation of filtered `.bib` files required for PDF compilation.

## 📖 Citation

Please cite this manuscript (upon publication) as:

```bibtex
@unpublished{Kopnin2025,
  author      = {Kopnin, Andrey V.},
  year        = {2025},
  title       = {Constituting Affective Valence: An Emergentist-Predictive Model of Embodied Consciousness (EPET)},
  note        = {Manuscript in preparation (preprint available upon request)}
}
```

## 📄 License

All content in this repository, unless otherwise specified, is licensed under the [CC BY 4.0 International](LICENSE).
