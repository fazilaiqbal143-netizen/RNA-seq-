

# **🔬 Introduction (short)**

This study performs a reference-based RNA-Seq analysis using the Galaxy platform to understand gene expression patterns across samples. The workflow includes quality control, alignment to a reference genome, visualization, and downstream analyses such as PCA and heatmap generation to assess variability and expression differences.



1. FastQC (Quality Control)

FastQC was used to assess the quality of raw sequencing reads. It evaluates parameters such as per-base quality scores, GC content, and sequence duplication to ensure the data is suitable for downstream analysis.



2. Read Trimming

Low-quality bases and adapter sequences were removed to improve the accuracy of alignment. This step ensures that only high-quality reads are used in further analysis.



3. Alignment using STAR

Reads were aligned to the reference genome using the STAR aligner. This step maps RNA-Seq reads to their genomic locations, enabling identification of expressed genes and splice junctions.



4. Alignment Visualization (IGV)

Alignment results were visualized in IGV to inspect read coverage across the PE gene. This helps confirm proper mapping and identify expression patterns between samples.

5. Sashimi Plot

Sashimi plots were generated to visualize exon usage and splice junctions. These plots help in understanding alternative splicing events across the samples.


6. JBrowse2 Visualization**

JBrowse2 was used to interactively explore alignment data on genomic coordinates. It provides an intuitive view of read distribution and gene structure.


7. STAR Coverage (Strand-specific)**

Strand-specific coverage tracks were generated using STAR. Reads from strand 1 are shown in blue and strand 2 in red, allowing visualization of transcription direction and strand bias.



8. PCA Analysis

Principal Component Analysis (PCA) was performed to assess variation between samples. It reduces data dimensionality and helps identify clustering patterns based on gene expression profiles.


9. Heatmap (Sample-to-sample variability)**

A heatmap was generated to visualize similarities and differences between samples. It highlights expression patterns and clustering, helping to identify related or distinct samples.



Conclusion 

The RNA-Seq analysis pipeline successfully mapped reads, visualized gene expression, and identified variability between samples. Tools like PCA and heatmaps revealed sample relationships, while genome browsers confirmed accurate alignment and expression patterns, providing a comprehensive understanding of the dataset.


