README - IEA_PLR_Dataset

Dataset Version 1.0.0 
Created on: 2025-04-13

---

Title  
Disentangling Emotional and Attentional Contributions to Pupillary Response using Auditory Stimuli and Visual Brightness Shifts

Description  
This dataset accompanies a study investigating pupillary and oculomotor responses when participants were exposed to emotionally charged auditory stimuli  
while simultaneously directing visual attention to objects of varying brightness.

All time-series data of pupil diameter and OKN slow-phase velocity included here have already undergone basic preprocessing (e.g., artifact removal, interpolation, normalization as noted).

---

1. OKN_LR.csv  
- Content: Preprocessed time-series data of the slow-phase velocity of optokinetic nystagmus (OKN).  
- Condition: Trials in which visual attention was shifted from leftward to rightward motion (Left-to-Right).  
- Format: Each column represents one trial, containing 11 seconds of data (from 5 seconds before to 6 seconds after the onset of the auditory stimulus).  
- Notes: All signals have been preprocessed and aligned relative to stimulus onset.

---

2. OKN_RL.csv  
- Content: Preprocessed time-series data of the slow-phase velocity of OKN.  
- Condition: Trials in which visual attention was shifted from rightward to leftward motion (Right-to-Left).  
- Format: Each column represents one trial, containing 11 seconds of data (from 5 seconds before to 6 seconds after the onset of the auditory stimulus).  
- Notes: All signals have been preprocessed and aligned relative to stimulus onset.

---

3. Pupil_BW.csv  
- Content: Preprocessed and z-score normalized pupil size data for the Black-to-White (BW) visual attention shift condition.  
- Format: Each column corresponds to one trial, containing 11 seconds of data (from 5 seconds before to 6 seconds after the auditory stimulus).  
- Normalization: Z-score normalization was applied within each 11-second trial window after preprocessing (e.g., blink removal, interpolation).

---

4. Pupil_WB.csv  
- Content: Preprocessed and z-score normalized pupil size data for the White-to-Black (WB) visual attention shift condition.  
- Format: Each column corresponds to one trial, containing 11 seconds of data (from 5 seconds before to 6 seconds after the auditory stimulus).  
- Normalization: Z-score normalization was applied within each 11-second trial window after preprocessing.

---

5. Pupil_emotion.xlsx  
- Content: Summary of pupil responses and emotion ratings for 40 auditory stimuli, based on the average data of 22 participants.  
- Columns:
  - sound_file: File name of the auditory stimulus  
  - original_ID: IADS-E stimulus ID (Yang et al., 2018)  
  - BW_condition: Mean z-scored pupil size in the BW condition  
  - WB_condition: Mean z-scored pupil size in the WB condition  
  - Pupil: Mean pupil size (z-score) during the 6 seconds following stimulus onset  
  - Arousal: Mean arousal rating for the stimulus (1–9 scale)  
  - Valence: Mean valence rating for the stimulus (1–9 scale)

---

General Notes:  
- All data are anonymized and labeled with pseudo-identifiers where applicable.  
- All time-series data have undergone basic preprocessing (e.g., blink or saccade artifact removal, interpolation, normalization).  
- Time windows span 11 seconds per trial (−5s to +6s relative to sound onset).  
- All files use UTF-8 encoding. .csv and .xlsx files can be opened with any standard spreadsheet or data analysis software.

---

Citation:  
If you use this dataset, please cite the following manuscript:  
"Disentangling Emotional and Attentional Contributions to Pupillary Response using Auditory Stimuli and Visual Brightness Shifts" (in preparation)

---

Contact:  
Kei Kanari  
Tohoku University  
Email: kei.kanari.a2@tohoku.ac.jp
