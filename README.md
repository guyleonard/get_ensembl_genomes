# Get ENSEMBL Genomes
A quick and easy way to download all of the CDS, GFF or peptides of predicted genes from the taxa available across the different ENSEMBL Genome portals.

**NB** Neither this tool nor myself are affiliated witih ENSEMBL, so please use at your own risk and responsibly.

## Usage
Decide which genome portal you wish to download from, currently you can choose:
 * f for Fungi
 * m for Metazoa
 * a for Plants (Archaeplastida)
 * p for Protists
 
 Then decide which version of the database you wish to download, the current version is 47 as of May 2020.
 
 Peptides (protein/AA) are the default option.
 
```bash
Usage: ./bin/get_ensemble_genomes [-f | -m | -a | -p] -V <int> (-c) (-g)
Databases:
		 -f Ensembl DB: Fungi
		 -m Ensembl DB: Metazoa
		 -a Ensembl DB: Plants
		 -p Ensembl DB: Protists
Version:
		-V Ensembl DB: Version
Other:
 		-c CDS (genes) instead of peptides (default)
 		-g GFF3 instead of FASTA
```

For example, to download the CDS for Metazoa:
```bash
./bin/get_ensemble_genomes -m -V 47 -c
```

or to download the gff3 files for Plants:
```bash
./bin/get_ensemble_genomes -p -V 47 -g
```

# Broken?
Sometimes names change or names are slightly different in the table than they are on the ftp, let me know and I'll update to catch the exceptions.
