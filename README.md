# Code Repository for the thesis "Speech-to-text model for keyword spotting applications in the Papiamento language within a healthcare environment"

**Author**: Joel Rajnherc and collaborators • Bachelor Thesis Project • SISSTEM • University of Aruba

---

## 1. Overview
This repository accompanies the bachelor thesis by Joel Rajnherc entitled _"Speech-to-text model for keyword spotting applications in the Papiamento language within a healthcare environment"_. The goal of the thesis was to explore a keyword spotting model for the Papiamento language, which is spoken in Aruba, Bonaire, and Curaçao. A future aspirational goal is the creation of end-to-end voice interfaces in Papiamentu or Papiamento that can be embedded in various applications, including healthcare.

The repository provides an implementation in PyTorch through a runnable notebook and linkage with the remote dataset. This is a classification task, trained on a dataset of almost 280 participants, containing a total of 16766 spectrogram arrays, each 1 second long, with 6 different keywords in Papiamento. Additionally, it includes an unknown class for samples that do not contain any of the keywords.

![Spectrogram Sample, one for each of the seven classes.](readme_supplemental/one-sample-per-class-2-rows.png)

<table style="max-width: 800px; margin: auto;">
    <tr>
        <td align="center">Dolor</td>
        <td align="center">Masha Danki</td>
        <td align="center">No</td>
        <td align="center">Resultado</td>
        <td align="center">SSImSan</td>
        <td align="center">Si</td>
        <td align="center">Unknown</td>
    </tr>
    <tr>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/dolor.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/masha_danki.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/no.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/resultado.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/ssimsan.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/si.wav"></audio>
        </td>
        <td>
            <audio controls controlsList="nodownload noplaybackrate noremoteplayback nofullscreen" style="width: 115px;" src="readme_supplemental/unknown.wav"></audio>
        </td>
    </tr>
</table>

---

Our first attempt with the dataset achieved a 97.20% accuracy on the test set using a convolutional neural network (CNN).

Think you can beat that?
We warmly invite fellow students and researchers to take on the challenge: improve the model, experiment with new techniques, and push the boundaries of keyword spotting in Papiamento. If you manage to set a new state-of-the-art, submit a pull request and claim your spot at the top!

> **Note:** The dataset is also separately available on Zenodo at the following address: [Zenodo Dataset](https://zenodo.org/record/1234567).

## 2. Quick start
Run the notebook in the free-tier cloud: <a target="_blank" href="https://colab.research.google.com/github/University-of-Aruba/papiamento-keyword-spotting/blob/main/notebook/papiamento-keyword-spotting.ipynb"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>

## 3. Setup on a Local Environment

1. Create a Python virtual environment using the command line interface

   for `python`:
   ```bash
   python -m venv .venv
   ```
   or `python3`:
   ```bash
   python3 -m venv .venv
   ```
   , then activate it on Linux/macOS with
   ```bash
   source .venv/bin/activate
   ```
   or on Windows (PowerShell) with
   ```bash
   .\.venv\Scripts\Activate.ps1
   ```
   . In case of access issues in PowerShell, run
   ```bash
   Set-ExecutionPolicy Unrestricted -Scope Process
   ```

   then retry activating the environment.
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Start Jupyter:

   from the command line 
   ```bash
   jupyter notebook
   ```
   which opens a browser at the address of your local Jupyter server. From there, open the file under `notebook/papiamento-keyword-spotting.ipynb`. Alternatively, you can open this file from your preferred code editor with Jupyter support (e.g., VS Code).

## Project Structure
- Notebooks and scripts for experiments
- requirements.txt for dependencies
- .gitignore to exclude unnecessary files

## Usage
- All code and results are provided for reproducibility.
- See individual notebooks for details.

Crafted with ❤️ following FAIR principles.