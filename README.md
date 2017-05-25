# RNA-Puzzzles_format
The submission format of RNA-Puzzles

## Citation: 
The Protein Data Bank.
Berman HM, Westbrook J, Feng Z, Gilliland G, Bhat TN, Weissig H, Shindyalov IN, Bourne PE.
Nucleic Acids Res. 2000 Jan 1;28(1):235-42.
PMID: 10592235
[http://www.rcsb.org/pdb/file_formats/pdb/pdbguide2.2/PDB_format_1992.pdf]

___
rna_puzzles_format.py is a script used to generate a standard formatted PDB file for given sequences in a fasta file.   
Please refer to '2gdi.fa' for an example.   
To use:  
*$python rna_puzzles_format.py [fasta file] [number of model(optional)] >out.pdb*  
___
format_check.py is a script used to check the format of a submitted PDB file by referring to a standard PDB file of good   format. If more than 1 error exist, a 'xx.format_check.txt' file is generated to include all the error reports.   
To use:  
*$python format_check.py [To_be_checked.pdb] [Reference.pdb]*  

