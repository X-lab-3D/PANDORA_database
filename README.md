# Database for PANDORA

## Installation


1) Clone this repository with git:
   ```
   git clone https://github.com/X-lab-3D/PANDORA_database.git
   ```
   
2) Move to the PANDORA_database folder you just cloned:
   ```
   cd PANDORA_database
   ```

3) Uncompress the database file:
   ```
   tar -xvf ./data/csv_pkl_files/database.tar.xz -C ./data/csv_pkl_files/
   ```

4) Copy the folder inside your PANDORA installation (fill in <path_to_PANDORA>:
   ```
   cp -r ./data/ <path_to_PANDORA>/PANDORA_files/
   ```
   OR move the folder inside your PANDORA installation:
   ```
   mv -r ./data <path_to_PANDORA>/PANDORA_files/
   ```
   
5) Repath your database:

   To properly use the database object, you need to specify the absolute path to the PDB template structures.
   You can either do it every time you load the database or do it just once and save it to a new database (as shown below).
   Use in python 3:
   ```python
   from PANDORA.Database import Database

   db = Database.load('<path_to_PANDORA>/PANDORA_files/data/csv_pkl_files/database.pkl')
   db.repath('<absolute_path_to_PANDORA>/PANDORA_files/data/PDBs', save='<path_to_PANDORA>/PANDORA_files/data/csv_pkl_files/database_repath.pkl')
   ```
6) Enjoy using PANDORA!

## Data Structure

```
data/  
 └──csv_pkl_files/  
    ├──Human_MHC_data.fasta    Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IMGTHLA/Latest/hla_prot.fasta  
    ├──NonHuman_MHC_data.fasta Non-Human MHC reference sequences parsed from https://raw.githubusercontent.com/ANHIG/IPDMHC/Latest/MHC_prot.fasta  
    └──database.tar.xz PANDORA database object. To be uncompressed (as explained in this README) before usage.  
 └──PDBs/  
    └──pMHCI/   Collection of pMHCI template structures. The same structures have been used for the manuscript benchmark experiment as cross validation targets.  
```
