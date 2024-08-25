# DNA to RNA to Amino Acid Translator

(this is part of my college assignment "Bioinformatics")
This Python program converts a DNA sequence into its complementary DNA strand, transcribes it into RNA, and then translates the RNA sequence into an amino acid sequence. The program follows the biological processes of transcription and translation.

## Table of Contents
- [Introduction](#introduction)
- [How It Works](#how-it-works)
- [Usage](#usage)
- [Example](#example)
- [Requirements](#requirements)

## Introduction

This program is designed to simulate the transcription and translation processes of DNA in a biological system. It takes a DNA sequence as input, transcribes it into RNA, and then translates the RNA sequence into an amino acid sequence. 

The process includes:
- **Transcription**: Converting the DNA sequence into its complementary DNA strand and then into RNA by replacing thymine (T) with uracil (U).
- **Translation**: Converting the RNA sequence into an amino acid sequence based on codons (triplets of RNA bases).

## How It Works

1. **Transcription**:
   - The program first generates the complementary DNA strand by replacing:
     - G with C
     - C with G
     - A with T
     - T with A
   - Then, it converts thymine (T) to uracil (U) to generate the RNA sequence.

2. **Translation**:
   - The RNA sequence is divided into codons (triplets), and each codon is translated into the corresponding amino acid.
   - The translation stops when a stop codon (UAA, UAG, UGA) is encountered.

## Usage

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/dna-to-rna-translator.git
    cd dna-to-rna-translator
    ```

2. Run the program:
    ```bash
    python dna_to_rna_translator.py
    ```

3. Enter a DNA sequence when prompted.

4. The program will output the complementary DNA strand, the RNA sequence, and the corresponding amino acid sequence.

## Example

### Input:
```bash
Enter DNA sequence: TCGGTGAATCTGTTTGAT
```

### Output:
```bash
Complementary DNA strand: AGCCACTTAGACAAACTA
RNA sequence: AGCCACUUAGACAAACUA
Amino Acid sequence: SHLDKL
```

(Note: The Amino Acid sequence will vary depending on your codon table implementation.)

## Requirements

- Python 3.x
