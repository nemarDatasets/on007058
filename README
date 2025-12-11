# EEG Dataset for "Auditory representations of words during silent visual reading"

This dataset contains the raw and processed EEG data accompanying the paper.
If you use these data in your research, please cite the above paper.

---

## Dataset Description

The dataset includes raw EEG recordings in **BrainVision format**:

* `.eeg`
* `.vhdr`
* `.vmrk`

All participants’ data follow the **BIDS (Brain Imaging Data Structure)** specification.

### Event Annotations

Each run includes an **events file** with onsets, durations, trial types, and event values for all trials.

### Stimulus Presentation

Participants viewed word stimuli forming naturalistic narratives, presented on a grey background with a central fixation cross.

Trigger | Type |
| :--- | :--- 
 `S111` | Onset of a word in a unique story
 `S71` | Onset of a word in a repeated story

### Additional Triggers

* **Run onset:** `S71`
* **Run end:** `S78`

---

## Derivatives

Processed data files are stored in the `./derivatives` folder.  
This folder contains the processed EEG, as well as the accompanying meta-data and feature embeddings.

### MetaData

The following files are found in the `./derivatives/MetaData/` sub-folder:

#### Story–Run–Session Match Table
**Path:** `./derivatives/MetaData/session_story_run`  
**Description:**  
A table matching each recording session to the specific story and run it contains.

#### Story Indexes for Each Epoch
**Path:** `./derivatives/MetaData/story_epoch_match`  
**Description:**  
Provides the specific story index corresponding to each epoch in the processed EEG data.

#### Expected Index for Each Epoch
**Path:** `./derivatives/MetaData/expect_or_not`  
**Description:**  
Indicates whether the epoch was expected or unexpected.  
**Values:**  
- `1` = expected  
- `0` = unexpected

### Processed EEG Data

The preprocessed EEG signals are located in: `./derivatives/eeg_processed/`


Data are organized by channel, where each channel file has the following specifications:

- **Shape:** `(nWords, nTimepoints)`  
- **nWords:** number of words (epochs)  
- **nTimepoints:** number of time points per epoch

### Corresponding Feature Embeddings

Feature (embeddings) are stored in: `./derivatives/Features/`

These feature files follow the same word-level indexing (`nWords`) as the EEG data:

- **Shape:** `(nWords,)`  
- **nWords:** number of words (epochs) in the EEG data

---

## References

* Appelhoff, S., Sanderson, M., Brooks, T., Vliet, M., Quentin, R., Holdgraf, C., Chaumon, M., Mikulan, E., Tavabi, K., Höchenberger, R., Welke, D., Brunner, C., Rockhill, A., Larson, E., Gramfort, A., & Jas, M. (2019). **MNE-BIDS: Organizing electrophysiological data into the BIDS format and facilitating their analysis.** *Journal of Open Source Software, 4*(1896). [https://doi.org/10.21105/joss.01896](https://doi.org/10.21105/joss.01896)
* Pernet, C. R., Appelhoff, S., Gorgolewski, K. J., Flandin, G., Phillips, C., Delorme, A., & Oostenveld, R. (2019). **EEG-BIDS, an extension to the brain imaging data structure for electroencephalography.** *Scientific Data, 6*, 103. [https://doi.org/10.1038/s41597-019-0104-8](https://doi.org/10.1038/s41597-019-0104-8)