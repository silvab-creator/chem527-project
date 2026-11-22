# Judgment log: <Silvana>

## How I used AI in this project

(Final submission only.)

## Entries

### Nov 22: Choosing wavelengths for fitting

- **What the assistant suggested:** Use 531 nm for the first single-wavelength fit and 350–650 nm for the first multiwavelength fit.
- **What I did:** Checked the absorbance changes in the notebook. Recorded these wavelengths as starting choices for the planned fits.
- **Why, from my data:** The largest absorbance change across pH is 1.017 AU at 531 nm. Between 350 and 650 nm, 203 wavelengths change by more than 0.1 AU. These results support the starting choices. Later checks will compare other wavelengths and spectral ranges to see how much the estimated pKa changes.

### Nov 22: Checking the crossing near 470 nm

- **What the assistant suggested:** Check the crossing near 470 nm before fitting a two-state model.
- **What I did:** Used the notebook plots and the absorbance range across all 12 pH conditions to check the 450–490 nm region. Described the crossing as approximate.
- **Why, from my data:** The smallest range in this region occurs at 470 nm, where absorbance runs from 0.750 to 0.768 AU. The spread is 0.018 AU, so the spectra do not meet at exactly one value. A two-state model is a starting point, and the fitted residuals still need to be checked.