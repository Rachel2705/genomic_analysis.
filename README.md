# genomic_analysis.
# Genomic Analysis Script

This Python script utilizes the Biopython library to perform various analyses on genomic data retrieved from the National Center for Biotechnology Information (NCBI) using its E-utilities. The script covers tasks such as fetching genomic data, reverse complementing sequences, calculating GC skew, visualizing genomic features, and generating files compatible with the UCSC Genome Browser.

![GC Skew Plot]([gc_skew_plot.png](https://github.com/Rachel2705/genomic_analysis./blob/main/gc_skew_plot.png))

## Requirements
- Python 3
- Biopython
- Matplotlib

## Setup
1. Install the required libraries:
   ```bash
   pip install biopython matplotlib
   ```

2. Update the `Entrez.email` variable in the script with a valid email address. This is required for using NCBI's E-utilities.

## Usage
Replace the placeholder accession number (`"JX573431.1"`) in the script with the actual accession number you want to analyze.

```python
# Replace 'your_accession_number' with the actual accession number you want to analyze
accession_number = "JX573431.1"
```

Run the script:

```bash
python genomic_analysis_script.py
```

## Functionality

### 1. Fetch Genomic Data
The script fetches genomic data from NCBI using the provided accession number.

### 2. Reverse Sequences
It reverses the retrieved genomic sequence to its complement.

### 3. Calculate GC Skew
The script calculates and visualizes the GC skew of the reversed sequence.

### 4. Annotate Genes
It extracts and prints information about genes, including their locations and descriptions.

### 5. Extract Gene Sequences
The script extracts gene sequences and stores them for further analysis.

### 6. Create BED File
It generates a BED file (`gene_locations.bed`) containing information about gene locations.

### 7. Create Track File
A track file (`trackDb.txt`) is created for use with the UCSC Genome Browser, providing a custom track description.

### 8. Calculate Coverage
The script calculates coverage based on genomic features.

### 9. Plot Coverage
It generates a coverage plot and saves it to a file.

### 10. Visualize Gene Locations
The script visualizes gene locations on the genomic sequence and saves the plot to a file.
