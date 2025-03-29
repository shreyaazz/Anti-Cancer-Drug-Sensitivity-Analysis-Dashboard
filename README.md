# Anti-Cancer Drug Sensitivity Analysis Dashboard

Original Data Source: The raw data is publicly available and can be accessed from the GDSC database (https://www.cancerrxgene.org/)

Dataset from Kaggle: Genomics of Drug Sensitivity in Cancer (GDSC)
https://www.kaggle.com/datasets/samiraalipour/genomics-of-drug-sensitivity-in-cancer-gdsc

### 1. Overview Metrics (Top Section)
The top section of the dashboard provides key summary statistics:

- Drugs: The total number of drugs included in the dataset. -> 110

- Cancer Types: The number of cancer types analyzed. -> 30

- Most Sensitive Cancer: The cancer type that shows the highest sensitivity to a drug. -> PAAD

- Most Potent Drug: The drug that exhibits the highest potency against cancer types. -> N-acetyl cysteine

Additionally, there are slicers for Cancer Type, Drug, and Target, allowing dynamic filtering of the data. The Reset button helps clear all applied filters.

Initial Preview of Dashboard:
![Image](https://github.com/user-attachments/assets/fefd89c9-82be-44a0-a29f-cb21755782dc)

### 2. Sensitivity Analysis Table (Left Panel)
This section highlights which cancer types are most sensitive to a drug:

- Drug: Lists the most potent drug, which is N-acetyl cysteine.

- Cancer Type: Displays the cancer types where the drug is most effective.

- ln(IC50): Represents the logarithm of the IC50 value, which measures drug sensitivity (lower IC50 means higher sensitivity).

Here, Pancreatic Adenocarcinoma (PAAD) shows the highest sensitivity to N-acetyl cysteine.

### 3. Drug Effectiveness (Violin Plot - Center Panel)
This visualization addresses the question "Are all drugs equally effective?" by showing:

- Violin plots for different cancer types, displaying the distribution of drug response.

- Median and Mean values of drug response for each cancer type.

This helps in understanding the variability in drug responses across different cancers. hereas a wider violin plot suggests greater variability in drug sensitivity across different samples.

### 4. Drug Target Pathways (Right Panel - Bar Chart)
This bar chart answers "Where do these drugs target?" by displaying the frequency of drugs affecting specific pathways:

Top Target Pathways:

- DNA replication (12.4K occurrences)

- PI3K/MTOR signaling (8.6K occurrences)

- Chromatin histone modification (6.4K occurrences)

- Genome integrity, Mitosis, Apoptosis, Metabolism, and ERK MAPK signaling

This section provides insights into the most commonly targeted mechanisms by these anti-cancer drugs.

### 5. Drug Link Analysis (Bottom Left - Chord Diagram)
This chord visualization shows "Which drugs have the most successive links?":

- It maps drugs to their associated cancer types.

Preview to analyze broad spectrum of a drug:
![Image](https://github.com/user-attachments/assets/9519b642-8cd8-4bde-9ebe-ecc71117e3c7)


A higher number of links suggests a broad-spectrum drug, whereas fewer links indicate targeted therapies.

### 6. Drug Sensitivity vs. Response (Bottom Right - Scatter Plot)
This scatter plot examines "How Drug Sensitivity Impacts Response?":

- X-axis: Drug pIC50 concentration which is the negative logarithm of the IC50 value (half-maximal inhibitory concentration), a logarithmic measure of compound potency.

- Y-axis: Drug response (higher values indicate better response).

- Color-coded datapoints: Different cancer types.

This helps visualize the correlation between drug concentration and therapeutic response, which is critical in evaluating treatment effectiveness.

### Key Insights from the Dashboard
- N-acetyl cysteine is the most potent drug in the dataset, showing high sensitivity for PAAD (Pancreatic Adenocarcinoma).

- Cancer types vary widely in their drug responses, as seen in the violin plot.

- DNA replication and PI3K/MTOR pathways are the most targeted by anti-cancer drugs, indicating their crucial role in cancer progression.

- Some drugs have broad-spectrum effects, while others are highly specific to certain cancers.

- Drug sensitivity correlates with response, helping researchers and clinicians predict treatment outcomes.

This dashboard provides valuable insights for precision oncology, helping researchers identify effective drug candidates and understand drug-cancer interactions.

# Authors

# Acknowledgements
- This dataset is originally sourced from the Genomics of Drug Sensitivity in Cancer (GDSC) project, a joint effort between the Wellcome Sanger Institute (UK) and the Massachusetts General Hospital Cancer Center (USA). The GDSC project is one of the largest public resources for information on drug sensitivity in cancer cells and molecular markers of drug response. Original Data Source: The raw data is publicly available and can be accessed from the GDSC database (https://www.cancerrxgene.org/).
- Samira Alipour: provider of the Kaggle dataset  https://www.kaggle.com/datasets/samiraalipour/genomics-of-drug-sensitivity-in-cancer-gdsc
  
