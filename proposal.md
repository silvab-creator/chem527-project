# Project proposal

**Title:** Evaluating Single-Wavelength and Multiwavelength UV-Vis Fitting Methods for Determining the Apparent pKa of Methyl Orange

### 1. Research Question 

How does the choice of single-wavelength versus multiwavelength nonlinear fitting affect the estimated apparent pKa of methyl orange and its associated fitting uncertainty?

Methyl orange is an acid–base indicator whose UV-Vis absorption spectrum changes with its protonation state. These changes can be analyzed to determine its apparent acid dissociation constant (pKa). My project will compare two fitting approaches to investigate how the amount of spectral information used influences the estimated pKa and its uncertainty.

### 2. Dataset and Source

I will use the publicly available dataset *Raw UV-vis absorption spectra of pH indicator dyes for singular-value analysis of overlapping chemical equilibria* by Satoru Goto (2026), published on Mendeley Data.

- **Dataset:** https://data.mendeley.com/datasets/jp2j9hz6v9/1
- **DOI:** 10.17632/jp2j9hz6v9.1
- **Accessed:** November 8, 2026
- **File:** `20160621MO-pH.xlsx`, worksheet `in H2O`

The aqueous dataset contains 551 wavelength measurements from 250 to 800 nm at 1 nm intervals across 12 pH conditions ranging from 2.0 to 7.0, providing 6,612 absorbance measurements with no missing values. Wavelength is measured in nanometers, while absorbance and pH are dimensionless. The reported experimental conditions include a temperature of 25.0 °C and an ionic strength of approximately 0.10 mol/L NaCl.

### 3. Proposed Analysis

I will first visualize the UV-Vis absorption spectra to identify wavelengths sensitive to changes in methyl orange protonation. Preliminary inspection indicates that the largest absorbance change occurs at 531 nm (1.017 AU), making this a reasonable starting wavelength for analysis. The spectra also show a near-common intersection around 470 nm, which is consistent with a two-state acid–base equilibrium.

I will estimate the apparent pKa using single-wavelength nonlinear fitting with a two-state equilibrium model, then compare the result with a multiwavelength fit using a shared pKa parameter. I will evaluate the fitted parameter uncertainties, residuals, and sensitivity of the results to excluding individual pH conditions.

### 4. Data Sufficiency, Limitations, and Fallback Plan

The dataset contains substantial pH-dependent spectral changes, with 203 wavelengths between 350 and 650 nm exhibiting absorbance differences greater than 0.1 AU. This supports comparing single-wavelength and multiwavelength fitting methods.

However, only four pH conditions fall between 2.5 and 4.0, limiting the information available around the main acid–base transition. The dataset also lacks independent replicate measurements and reported pH uncertainties, and the dataset description does not specify the dye concentration. These limitations may affect the reliability of the fitted pKa and the interpretation of its uncertainty.

If multiwavelength fitting proves unreliable, I will evaluate the sensitivity of single-wavelength pKa estimates to wavelength selection. If the methyl orange measurements are insufficient to constrain the equilibrium model, I will investigate another pH indicator available in the same published dataset.

