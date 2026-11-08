# Project proposal
# CHEM 527 Final Project Proposal

**Title:** Evaluating Single-Wavelength and Multiwavelength UV-Vis Fitting Methods for Determining the Apparent pKa of Methyl Orange

### 1. Research Question 

How does the choice of single-wavelength versus multiwavelength nonlinear fitting affect the estimated apparent pKa of methyl orange and its associated fitting uncertainty?

Methyl orange is an acid–base indicator whose UV-Vis absorption spectrum changes with its protonation state. These changes can be analyzed to determine its apparent acid dissociation constant (pKa). My project will compare two fitting approaches to investigate how the amount of spectral information used influences the estimated pKa and its uncertainty.

### 2. Dataset and Source

I will use *Raw UV-Vis Absorption Spectra of pH Indicator Dyes* by Satoru Goto (2026), published on Mendeley Data.

- **Dataset:** https://data.mendeley.com/datasets/jp2j9hz6v9/1
- **DOI:** 10.17632/jp2j9hz6v9.1
- **Accessed:** November 8, 2026
- **File:** `20160621MO-pH.xlsx`, worksheet `in H2O`

The aqueous dataset contains 551 wavelength measurements from 250 to 800 nm, recorded at 1 nm intervals across 12 pH conditions ranging from 2.0 to 7.0. This provides 6,612 absorbance measurements with no missing values in the selected data. Wavelength is measured in nanometers, while absorbance and pH are dimensionless.

### 3. Proposed Analysis

I will begin by plotting the absorption spectra at different pH values to identify wavelengths that respond strongly to changes in protonation. Preliminary inspection indicates that the greatest absorbance change across pH occurs near 531 nm, with a difference of approximately 1.017 absorbance units (AU).

I will use nonlinear curve fitting with a two-state acid–base equilibrium model to estimate the apparent pKa at a selected wavelength. I will then compare this result with a multiwavelength fit using a shared pKa parameter.

To evaluate the two approaches, I will compare fitted parameter uncertainties, residuals, and the sensitivity of the estimated pKa to excluding individual pH conditions.

### 4. Data Sufficiency, Limitations, and Fallback Plan

The dataset contains substantial pH-dependent absorbance changes across the visible spectrum, supporting its use for acid–base equilibrium analysis. Preliminary calculations indicate that 203 wavelengths between 350 and 650 nm show absorbance changes greater than 0.1 AU across the measured pH conditions.

However, the dataset contains no independent replicate measurements, and only four spectra fall between pH 2.5 and 4.0, limiting the information available around the main transition. The fully protonated endpoint may also be incompletely characterized. Therefore, fitting uncertainty cannot be interpreted as experimental reproducibility.

If multiwavelength fitting is unreliable or does not provide a meaningful improvement, I will compare pKa estimates obtained at several individual wavelengths and evaluate their sensitivity to wavelength selection. I may also compare the estimated pKa with a published reference value.

