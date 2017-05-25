# RNA-Puzzzles_format
The submission format of RNA-Puzzles.
It has been notified that different prediction methods of RNA 3D structure may generate different structure formats. Generally, they follow the PDB formatting rules but with many variations. For example, different chain id, deleting certain columns, atom deletions at the 5' end, etc. <br/>
However, such format variations is prone to subtle bias in structure comparison and the results of RNA-Puzzles. For example, atom deletion at the 5' end result in a shorter structure, which may lead to better RMSD. <br/>
To avoid such potential bias is the will of the RNA-Puzzles community concluded from the 1st RNA-Puzzles meeting. We have agreed to strict format control.<br/>

RNA-Puzzles follows the [1992 PDB format](http://www.rcsb.org/pdb/file_formats/pdb/pdbguide2.2/PDB_format_1992.pdf). 
* Chains are numbered from A, B, C ...
* Residues of each chain are numbered from 1, 2, 3...
* Atom names and residue names are according to the [rna_puzzles_format.py] (https://github.com/RNA-Puzzles/RNA-Puzzzles_format/blob/master/rna_puzzles_format.py) script.

## Citation: 
The Protein Data Bank.
Berman HM, Westbrook J, Feng Z, Gilliland G, Bhat TN, Weissig H, Shindyalov IN, Bourne PE.
Nucleic Acids Res. 2000 Jan 1;28(1):235-42.
PMID: 10592235


## Author:
Please contact [Chichau](mailto:z.miao@ibmc-cnrs.unistra.fr) if you have any problem related to this program.

## URL: 
https://github.com/RNA-Puzzles/RNA-Puzzzles_format

## Scripts:
rna_puzzles_format.py is a script used to generate a standard formatted PDB file for given sequences in a fasta file.   
Please refer to '2gdi.fa' for an example.   
To use:  <br/>
* $python rna_puzzles_format.py [fasta file] [number of model(optional)] >out.pdb
Real case: <br/>
* $python rna_puzzles_format.py 2gdi.fa 5 >out.pdb

<br/>
format_check.py is a script used to check the format of a submitted PDB file by referring to a standard PDB file of good   format. If more than 1 error exist, a 'xx.format_check.txt' file is generated to include all the error reports.   <br/>
To use:  <br/>
* $python format_check.py [To_be_checked.pdb] [Reference.pdb]
Real case: <br/>
* $python format_check.py 2gdi.pdb out.pdb
<hr/>


## Examples:
examples can be found at:
https://github.com/RNA-Puzzles/RNA-Puzzzles_format/tree/master/example
