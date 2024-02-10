# CVEsImpactDataset
## Efficiency of consensual transformation matrix 
The consensually agreed, by our experts, matrix is available at [Matrix_Consensual.xlsx](Transformation_matrices/Matrix_Consensual.xlsx).
It allows for an easy attribution of effects to CVEs.

As a ground truth measure we have taken Vector Changer (VC) results from surveys in [CVEs](CVEs).
As model prediction we have taken each CVE and followed path of: CWE (from NVD) through Technical Impacts (from [https://cwe.mitre.org](https://cwe.mitre.org)) and finishing on Vector Changers (from mentioned transformation matrix)

To establish baseline for future research, we estimated its efficiency by defining classical classifier characteristics: 
- True Positive (TP),
- True Negative (TN),
- False Positive (FP),
- False Negative (FN).

Definition are as follows
- TP - model marked the same as expert;
- TN - model did not mark VCs and expert also did not mark them;
- FP - model marked more permissive VCs than expert;
- FN - model marked less permissive VCs than expert.

With the following definition, counts of corresponding classifier characteristics were as follows:
- TP = 63;
- TN = 6;
- FP = 58;
- FN = 8.

Giving us following performance metrics (definitions as in [Wikipedia's "Precision and Recall" article](https://en.wikipedia.org/wiki/Precision_and_recall]))
- Precision of **0.52**;
- Recall of **0.89**;
- F1 of **0.66**.

# To cite paper
TBD

