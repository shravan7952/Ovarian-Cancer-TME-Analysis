# 🧬 Ovarian Cancer Tumor Microenvironment (TME) Analysis

This project explores the **Tumor Microenvironment (TME)** in **ovarian cancer** using bulk RNA-sequencing data. By applying computational deconvolution techniques, we estimate immune and stromal cell compositions across patient samples, uncover distinct immune phenotypes, and provide visual insights into TME heterogeneity.

> 🧪 *A personal research project to understand cancer biology through data.*

---

## 📁 Dataset

- **Source**: [The Cancer Genome Atlas (TCGA)](https://portal.gdc.cancer.gov/)
- **Data Type**: Bulk RNA-seq (Illumina HiSeq platform)
- **Samples**: 508 ovarian cancer tumor samples (~530 files processed)
- **Deconvolution Tool**: [xCell](https://xcell.ucsf.edu/) — estimates ~40 immune and stromal cell types per sample.
- **Processed Files**:
  - `xcell_deconvoluted_cleaned.csv`
  - `xcell_deconvolution_output.csv`
  - `TCGA_Merged_RNASeq_TPM_Matrix.zip`
  - `final_expression_matrix.csv`

---

## 🧾 Objectives

- Estimate the abundance of immune and stromal cell types per tumor.
- Visualize cellular composition and variation across patients.
- Analyze interactions between TME components.
- Identify distinct **TME subtypes** or **immune archetypes**.
- Generate informative, publication-style figures.

---

## 🔍 Key Analyses

### ✅ Cell Abundance & Distribution
- **Bar Charts**: Mean abundance of top TME cell types (e.g., M1 Macrophages, NK cells).
- **Violin Plots**: Full distribution of all ~40 cell types showing inter-patient variability.

### ✅ TME Heterogeneity & Variation
- **Density Plots**: Focused on the 10 most variable cell types, highlighting sample diversity.

### ✅ Inter-Cellular Relationships
- **Correlation Matrix (Heatmap)**: Shows positive/negative correlations between cell types—revealing cellular co-occurrence or mutual exclusion.

### ✅ Identifying TME Subtypes
- **Hierarchical Clustering Heatmap**: Reveals patient groupings based on immune profiles.
- **UMAP Projection**: 2D dimensionality reduction clusters patients into clear subtypes (e.g., *immune hot*, *immune cold*).

---

## 🛠️ Tools & Libraries

- **Programming Language**: R
- **Packages**:
  - `xCell` for TME deconvolution
  - `ggplot2`, `pheatmap`, `cowplot` for plotting
  - `dplyr`, `tidyr` for data wrangling
  - `uwot`, `stats` for clustering & UMAP

---

## 📁 Folder Structure

```

Ovarian-Cancer-TME-Analysis/
├── data/
│   ├── xcell\_deconvoluted\_cleaned.csv
│   ├── xcell\_deconvolution\_output.csv
│   ├── TCGA\_Merged\_RNASeq\_TPM\_Matrix.zip
├── scripts/
│   └── (R scripts for each analysis step)
├── figures/
│   ├── violin\_plot.jpg
│   ├── top10\_cells\_mean\_score.png
│   ├── top10\_cells.png
│   ├── density\_plot.png
│   ├── correlation\_matrix.jpg
│   ├── hierachial\_clustering.png
│   ├── clustered\_heatmap\_celltypes.jpg
│   └── UMAP.jpg
└── README.md

```

---

## 📌 Future Enhancements

- Correlate TME subtypes with **clinical outcomes** (e.g., survival, treatment response).
- Integrate with **genomic/transcriptomic alterations** for multi-omics insights.
- Apply to **single-cell RNA-seq** data for finer granularity.
- Develop **interactive dashboards** using Shiny or Plotly.

---

## 🤝 Contributing

Contributions are welcome!  
Feel free to fork this repository or open an issue to discuss improvements or ideas.

---

## 📬 Contact

**Shravan Srikanthan**  
🔗 [LinkedIn](https://www.linkedin.com/in/shravan-s-7b53a494/)  
📧 [Email](mailto:shravan0601200@gmail.com)

---

> *"Decoding the tumor microenvironment helps us understand how cancer evades, resists, and sometimes gets defeated by the immune system."*
```

