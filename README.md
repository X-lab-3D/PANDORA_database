# Database for PANDORA

## Installation


1) Clone this repository with git:
   ```
   git clone https://github.com/X-lab-3D/PANDORA_database.git
   ```
   
2) Uncompress the database file:
   ```
   tar -xvzf ./data/csv_pkl_files/database.tar.gz -C ./data/csv_pkl_files/
   ```

3) Copy the folder inside your PANDORA installation:
   ```
   cp -r ./data /path/to/PANDORA/PANDORA_files/
   ```
   OR move the folder inside your PANDORA installation:
   ```
   mv -r ./data /path/to/PANDORA/PANDORA_files/
   ```
   
4) Enjoy using PANDORA!

## Data Structure

```
data/  
 └──csv_pkl_files/  
    ├──Human_MHC_data.fasta    Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IMGTHLA/Latest/hla_prot.fasta  
    ├──NonHuman_MHC_data.fasta Non-Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IPDMHC/Latest/MHC_prot.fasta  
    └──database.tar.gz PANDORA database object. To be uncompressed with ```tar xvf database.tar.gz``` before usage.  
 └──PDBs/  
    └──pMHCI/   Collection of pMHCI template structures. The same structures have been used for the manuscript benchmark experiment as cross validation targets.  
```
