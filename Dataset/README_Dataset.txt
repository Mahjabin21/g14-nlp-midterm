DATASET README G14 — Bangla Telecom and Mobile-Banking Customer-Care
Classification Course: CSC4233 | Section B | Group: G14

1.  DATASET SOURCE Original dataset: Bengali Telecom Customer Care
    Speech Hugging Face:
    https://huggingface.co/datasets/kawshikbuet17/bengali-telecom-customer-care-speech

The original dataset is used as the source for preparing Bangla
customer-care utterances. Please consult the dataset page for the
original dataset description, version, and license information. Retain
the original attribution and license when redistributing or reusing the
source data.

2.  PROJECT DATASET The project’s final annotated dataset contains 2,682
    unique Bangla sentences. Each sentence is assigned to one of six
    classification categories:

-   mobile_money
-   bank_service
-   telecom_sim_pack
-   security_otp
-   complaint_helpline
-   generic_dialogue

The final labels are the group’s prepared gold labels for the
experiments in this project.

3.  FILE DESCRIPTIONS The files included in this folder may include:

-   gold_labels_final.csv Final annotated dataset. Main fields:
    sentence_id, sentence, label, and label_source.

-   master_sentences.csv Master sentence-level dataset. Main fields:
    sentence_id, sentence, doc_id, and owner. Sentences extracted from
    the same original document share a doc_id.

-   final_adjudication_decisions.csv Records of adjudication decisions
    made during the annotation process.

-   M1_independent.csv Member 1’s independent annotation file.

-   M2_independent.csv Member 2’s independent annotation file.

-   M3_independent.csv Member 3’s independent annotation file.

-   M1_change_log.csv Records of label changes and related notes from
    Member 1’s annotation-repair process. This is a change log, not the
    complete original keyword-prediction file.

Not every submission package necessarily needs every intermediate
annotation file. Keep the files that are actually included in the final
ZIP, and do not rename or alter their contents without updating the
notebook and report.

4.  IMPORTANT DATA FIELDS

-   sentence_id: Unique identifier for a sentence.
-   sentence: Bangla customer-care utterance.
-   label: Final class assigned to the sentence.
-   label_source: Records the source or method associated with the final
    label, where available.
-   doc_id: Identifier of the original source document; sentences from
    the same document share this identifier.
-   owner: Annotation ownership information, where available.

5.  DATA PREPARATION AND USE The project applies Bangla text
    preprocessing, including Unicode normalization, tokenization,
    optional stopword removal, and optional light stemming. Multiple
    preprocessing configurations are compared in the notebook.

For model evaluation, the project uses a grouped train/validation/test
split designed to keep document and template-related groups together
across splits. A separate random split is also evaluated for comparison.

The notebook should be treated as the executable record of the dataset
preparation and experiments. The report’s dataset counts, split sizes,
and evaluation results must match the outputs reproduced by the
submitted notebook.

6.  REPRODUCIBILITY

-   Use the final notebook in the 01_Source_Code folder.
-   The notebook should load the dataset from its public source as
    specified in the code.
-   Include the dataset files in this folder as a backup, as required by
    the project submission instructions.
-   Do not manually edit labels or experimental results after
    evaluation.
-   If any dataset file is updated, rerun the relevant notebook cells
    and ensure the report reflects the updated results.

7.  ATTRIBUTION Original dataset authors and source:
    https://huggingface.co/datasets/kawshikbuet17/bengali-telecom-customer-care-speech

Project group: G14 | CSC4233 | Section B

Prepared for the G14 course project submission.
