## Predicting Behavioral Phenotypes from Genomic Variants in Drosophila using Machine Learning

The genetic architecture underlying *Drosophila* behavior is complex. This project utilizes a memory-efficient pipeline to process VCF data and applies Random Forest regression to rank variant importance. By integrating machine learning with functional genomics, we identify and annotate key genomic loci that drive phenotypic variance.

## Methodology

The pipeline follows a four-stage architecture:

1. **Genomic Data Handling:** Memory-optimized parsing of large-scale VCF files.
2. **Machine Learning Modeling:** Utilization of `RandomForestRegressor` to quantify the predictive contribution of genomic variants.
3. **Feature Importance Analysis:** Systematic extraction and ranking of top-tier predictive variants.
4. **Biological Annotation:** Mapping predictive coordinates to functional genes using FlyBase JBrowse and the Coordinate Converter tool.

## Key Findings

* **Computational Efficiency:** Successfully optimized a pipeline capable of processing large-scale genomic data within constrained memory settings.
* **Predictive Insights:** Identified high-importance genomic candidate regions influencing behavioral traits, including **Food Intake**, **Aggression**, and **Waking Activity**.
* **Biological Discovery:** Mapped predictive variants to critical developmental and signaling genes, including:
* **`ush` (*u-shaped*)**: Transcription factor involved in developmental patterning.
* **`Ptth`**: Hormone signaling in growth and development.
* **`cold`**: Gene regulation.


## Repository Structure

```text
/Predicting-Behavioral-Phenotypes-in-Drosophila
├── data/               # Top predictive variant CSVs 
├── notebooks/          # Main project Jupyter Notebook (.ipynb)
├── results/            # Visualizations and importance plots
├── README.md           # Project documentation


```

## How to Reproduce

1. Clone this repository: https://github.com/mahamtaqi3-cloud/Predicting-Behavioral-Phenotypes-from-Genomic-Variants-in-Drosophila-using-Machine-Learning
2. Ensure your environment has `pandas`, `scikit-learn`, `matplotlib`, and `seaborn` installed.
3. Run the notebook `Predicting_Behavioral_Phenotypes.ipynb` in your Google Colab or local Jupyter environment.

