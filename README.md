# Database for PANDORA

## Installation

1) Install git-lfs by following the instructions in this README: https://github.com/git-lfs/git-lfs/blob/main/README.md

2) Clone this repository with git-lfs:
   ```
   git lfs clone https://github.com/X-lab-3D/PANDORA_database.git
   ```

3) Uncompress the database folder:
   ```
   tar xzf pandora_database.tar.gz
   ```

4) Copy the folder inside your PANDORA installation:
   ```
   cp -r ./PANDORA_files /path/to/PANDORA/
   ```
   OR move the folder inside your PANDORA installation:
   ```
   mv -r ./PANDORA_files /path/to/PANDORA/
   ```
5) Enjoy using PANDORA!

```
data/  
 └──csv_pkl_files/  
    ├──Human_MHC_data.fasta    Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IMGTHLA/Latest/hla_prot.fasta  
    ├──NonHuman_MHC_data.fasta Non-Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IPDMHC/Latest/MHC_prot.fasta  
    └──pandora_database.tar.gz PANDORA database object. To be uncompressed with ```tar xvf database.tar.gz``` before usage.  
 └──PDBs/  
    └──pMHCI/   Collection of pMHCI template structures. The same structures have been used for the manuscript benchmark experiment as cross validation targets.  
```
