# SNOMED CT Clinical Note Entity Linking Challenge

## Problem Description
This competition aims to link text spans in clinical notes to specific topics within the SNOMED Clinical Terms (CT) terminology, utilizing the MIMIC-IV-Note dataset from the Beth Israel Deaconess Medical Center and SNOMED CT, a comprehensive clinical terminology.

## Overview
Participants are required to:
1. Obtain the challenge dataset from PhysioNet.
2. Download SNOMED CT taxonomy.
3. Train an entity linking model using `train_annotations.csv`.
4. Evaluate the model with `scoring.py`.
5. Submit the code for leaderboard scoring.

## Data Access
- **MIMIC-IV Note**: A vast collection of de-identified hospital discharge notes.
- **SNOMED CT**: A detailed clinical terminology used for documentation and reporting.

### Steps to Access
1. Register and complete training for data handling on PhysioNet.
2. Download the `mimic-iv_notes_training_set.csv` upon access approval.

## Using SNOMED CT
- Utilize the May 2023 release of SNOMED CT for entity linking.
- Explore terms, hierarchies, and defining relationships within SNOMED CT to enhance model accuracy.

## Annotations
The `train_annotations.csv` provides annotations for training, with fields for `note_id`, `start`, `end`, and `concept_id`.

## Performance Metric
- Evaluated on a class macro-averaged character intersection-over-union (IoU).
- Higher IoU values indicate better accuracy.

## Submission Format
- Submit a `main.py` script that predicts span classifications for the test set.
- Outputs should be consolidated into a `submission.csv` file.

Good luck to all participants! For more guidance, visit the user forum.
