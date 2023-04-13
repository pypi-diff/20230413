# Comparing `tmp/proteinTools-0.1.7.tar.gz` & `tmp/proteinTools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinTools-0.1.7.tar", last modified: Fri Apr  7 21:21:48 2023, max compression
+gzip compressed data, was "proteinTools-0.1.8.tar", last modified: Thu Apr 13 06:22:58 2023, max compression
```

## Comparing `proteinTools-0.1.7.tar` & `proteinTools-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-07 21:21:48.820818 proteinTools-0.1.7/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-0.1.7/LICENSE
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-07 21:21:48.816911 proteinTools-0.1.7/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-0.1.7/README.md
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-07 21:21:48.607423 proteinTools-0.1.7/proteinTools/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       33 2023-04-07 21:21:20.000000 proteinTools-0.1.7/proteinTools/__init__.py
--rw-rw----   0 defrondeville.c (1825595208) users      (100)    36436 2023-04-07 15:45:47.000000 proteinTools-0.1.7/proteinTools/proteins.py
-drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-07 21:21:48.755741 proteinTools-0.1.7/proteinTools.egg-info/
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-07 21:21:48.000000 proteinTools-0.1.7/proteinTools.egg-info/PKG-INFO
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      220 2023-04-07 21:21:48.000000 proteinTools-0.1.7/proteinTools.egg-info/SOURCES.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-07 21:21:48.000000 proteinTools-0.1.7/proteinTools.egg-info/dependency_links.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-07 21:21:48.000000 proteinTools-0.1.7/proteinTools.egg-info/top_level.txt
--rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-07 21:21:48.825184 proteinTools-0.1.7/setup.cfg
--rw-rw----   0 defrondeville.c (1825595208) users      (100)      436 2023-04-07 21:20:51.000000 proteinTools-0.1.7/setup.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:22:58.145733 proteinTools-0.1.8/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)     1069 2023-04-05 17:13:20.000000 proteinTools-0.1.8/LICENSE
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-13 06:22:58.142732 proteinTools-0.1.8/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      269 2023-04-06 05:13:03.000000 proteinTools-0.1.8/README.md
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:22:58.029471 proteinTools-0.1.8/proteinTools/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)    44440 2023-04-13 05:14:53.000000 proteinTools-0.1.8/proteinTools/PT.py
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        0 2023-04-08 01:23:23.000000 proteinTools-0.1.8/proteinTools/__init__.py
+drwxrwx---   0 defrondeville.c (1825595208) users      (100)        0 2023-04-13 06:22:58.127477 proteinTools-0.1.8/proteinTools.egg-info/
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      451 2023-04-13 06:22:57.000000 proteinTools-0.1.8/proteinTools.egg-info/PKG-INFO
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      249 2023-04-13 06:22:57.000000 proteinTools-0.1.8/proteinTools.egg-info/SOURCES.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)        1 2023-04-13 06:22:57.000000 proteinTools-0.1.8/proteinTools.egg-info/dependency_links.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       48 2023-04-13 06:22:57.000000 proteinTools-0.1.8/proteinTools.egg-info/requires.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       13 2023-04-13 06:22:57.000000 proteinTools-0.1.8/proteinTools.egg-info/top_level.txt
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)       38 2023-04-13 06:22:58.149610 proteinTools-0.1.8/setup.cfg
+-rw-rw----   0 defrondeville.c (1825595208) users      (100)      512 2023-04-13 06:19:31.000000 proteinTools-0.1.8/setup.py
```

### Comparing `proteinTools-0.1.7/LICENSE` & `proteinTools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinTools-0.1.7/proteinTools/proteins.py` & `proteinTools-0.1.8/proteinTools/PT.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,128 +16,238 @@
 mg = mygene.MyGeneInfo()
 
 #Utility dictionaries containing element/mass mappings as well as FASTA mapping
 FASTAdict = {'ALA':'A', 'ALX':'B', 'CYS': 'C', 'ASP' : 'D', 'GLU': 'E', 'PHE': 'F', 'GLY': 'G', 'HIS': 'H', 'ILE': 'I', 'LYS':'K', 'LEU':'L', 'MET': 'M', 'ASN':'N', 'PRO':'P', 'GLN': 'Q', 'ARG':'R', 'SER': 'S', 'THR': 'T', 'VAL': 'V', 'TRP': 'W', 'UNK':'X', 'TYR':'Y', 'GLX':'Z'}
 atom_dict = {'H':1.01, 'C':12.01, 'O':16.00, 'N':14.01, 'P':30.97, 'F':18.998, 'S':32.06, 'B':10.81, 'K':39.1, 'I':126.904, 'BR':79.904, 'CL':35.453, 'CA':40.08, 'NA':22.99, 'MG':24.305, 'AL':26.98, 'CR':51.996, 'NE':20.179, 'BE':9.01, 'FE':55.847, 'CO':58.933,'AG':107.868, 'CD':112.41, 'NI':58.693, 'ZN':65.39, 'BE':9.0122, 'IN':114.818, 'SI':28.085, 'SC':44.956, 'TI':47.867, 'V':50.941, 'MN':54.938, 'CU':63.546, 'GA':59.723, 'GE':72.64, 'SE':78.96, 'KR':83.8, 'ZR':91.224, 'NB':92.906, 'PD':106.42, 'SN':118.71, 'SB':121.76, 'XE':131.293, 'BA':137.327, 'LA':138.91, 'LI':6.941, 'HG':200.59, 'PB':207.2, 'BI':208.98, 'PO':209, 'TI':204.3833, 'AU':196.9665, 'IR':192.217, 'PT':195.078, 'RE':186.207, 'W':183.84, 'TA':180.948, 'YB':173.04, 'EU':151.964, 'ND':144.25, 'CE':140.116, 'TH':232.04, 'U':238.029, 'PU':244, 'FR':223, 'PA':231.04, 'HO':164.93, 'SM':150.36, 'PR':140.908, 'TE':127.6, 'TC':98, 'Y':88.906}
 atom_keys = atom_dict.keys()
 
-#Subclass for individual atoms
 class atom:
+    """
+    Atom class
+
+    This class contains the essential parameters of an individual atom in a protein structural file, including the coordinates, element, atomic mass, parent residue, and line data.
+    """
     def __init__(self, element, x, y, z, data, residue = ''):
+        
         self.element = element
         self.x = x
         self.y = y
         self.z = z
         self.residue = residue
         self.data = data
         self.mass = atom_dict[self.element]
              
-#Subclass for individual protein residues
 class residue:
+    """
+    Residue class
+    
+    This class contains the essential parameters of an individual residue in a protein structural file, including the child atoms, protein sidechain, residue index, and type of amino acid.
+    """
     def __init__(self, amino_acid, index, chain):
+        
         self.amino_acid = amino_acid
         self.index = index
         self.atoms = []
         self.chain = chain
             
-    #Calculates center of residue
     @cached_property
     def center(self):
+        """
+        Residue Center of Mass
+    
+        This property returns the center of mass of the residue, which is generated from all atom components. 
+    
+        Returns
+        -------
+        list
+            A list consisting of the x, y, and z coordinate in 3D space of the residue center of mass position for the protein structural file.
+        """
         x, y, z, totmass = 0, 0, 0, 0
         for atom in self.atoms:
             x += atom.x
             y += atom.y 
             z += atom.z
             totmass += atom.mass
         x /= atom.mass
         y /= atom.mass
         z /= atom.mass
         return [x, y, z]
         
-    #Allows user to access residue atoms via indexing
     def __getitem__(self, key):
+        """
+        Residue Index
+    
+        This property returns the atom contained in the parent residue based on the index of the atom as it appears in the structural file.
+        
+        Parameters
+        ----------
+        index : int
+            The atom index
+
+        Returns
+        -------
+        class
+            Returns the atom class contained at the given index.
+        """
         try:  
             if isinstance(key, slice):
                 atoms = [i for index, i in enumerate(self.atoms) if index > key.start and index <= key.stop] 
                 return atoms
             else:
                 return self.residue_list[key]
         except IndexError:
             print('Atom index out of bounds!')
         except:
             pass
             
-    #Returns number of atoms in residue
     @lru_cache
     def __len__(self):
+        """
+        Residue Length
+    
+        This property returns the total number of atoms contained with the residue.
+    
+        Returns
+        -------
+        int
+            A number of all the atoms contained within the specific residue.
+        """
         return len(self.atoms)
         
-#Subclass for ligands in protein file (if present)
 class ligand:
+    """
+        Ligand Class
+    
+        This property returns the center of mass of the residue, which is generated from all atom components. 
+        """
     def __init__(self, ID):
         self.ID = ID
         self.sites = []
         self.atoms = []
         
-    #Downloads ligand from PDB database
+   
     def download(self, directory = os.getcwd()):
+        """
+        Download Ligand
+    
+        This method downloads the specific ligand structural file based on the ligand ID. 
+    
+        Parameters
+        ----------
+        arg1 : str
+            Directory structural file will be downloaded in. Defaults to current user directory.
+        """
         url = 'https://files.rcsb.org/ligands/download/' + self.ID + '_ideal.sdf'
         urllib.request.urlretrieve(url, directory + '/' + self.ID + '.sdf')
         
-    #Calculates the center of mass of the ligand position
     @cached_property
     def center(self):
+        """
+        Ligand Center of Mass
+    
+        This property returns the center of mass of the ligand, which is generated from all atom components. 
+    
+        Returns
+        -------
+        list
+            A list consisting of the x, y, and z coordinate in 3D space of the ligand center of mass position for the specific ligand pose registered within the file.
+        """
         x, y, z, totmass = 0, 0, 0, 0
         for atom in self.atoms:
             x += atom.x
             y += atom.y
             z += atom.z
             totmass += atom.mass
         x /= totmass
         y /= totmass
         z /= totmass
         return [x, y, z]
         
 #Main protein class
 class Protein:
+    """
+    Protein Class
+
+    This class represents an individual protein, it's provided ID and relevant structural file (generated via Alphafold or scraped from RCSB), and analytical methods and properties for biostatistics and bioinformatics purposes.
+    """
     def __init__(self, protein_name, protein_type = 'PDB', species = 'human'):
         self.protein = protein_name
         self.ID_type = protein_type
         self.species = species
         
         #Accepts Uniprots if they are the correct length and user forgot to specify
         if self.ID_type == 'PDB' and len(self.protein) > 4:
             self.ID_type = 'Uniprot'
         
         #length of each side chain
         self.chains = {}
         
-    #Returns length of protein
     def __len__(self):
+        """
+        Protein Length
+    
+        This property returns the total number of residues within the protein structural file.
+        
+        Returns
+        -------
+        int
+            The total number of residues within the protein.
+        """
         length = 0
-        for chain in self.chains:
-            length += self.chains[chain]
+        try:
+            for chain in self.chains:
+                length += self.chains[chain]
+        except:
+            length = 0
+            print('Protein structural file not downloaded!')
+            
         return length
     
-    #Allows user to access residues via indexing
     def __getitem__(self, key):
+        """
+        Residue Index
+    
+        This magic method allows the user to index the protein for individual residues by either slicing or accessing an individual residue.
+    
+        Parameters
+        ----------
+        slice : slice
+            A slice of the residues within the protein file.
+            
+        key : int
+            An index of the residue within the protein file.
+    
+        Returns
+        -------
+        class, list
+        Returns the class or the list of classes queried by the index.
+        """
         try:  
             if isinstance(key, slice):
                 residues = [i for index, i in enumerate(self.residue_list) if index > key.start and index <= key.stop] 
                 return residues
             else:
                 return self.residue_list[key]
         except IndexError:
             print('Residue index out of bounds!')
         except:
             print(traceback.format_exc())
             print('Protein file has not been downloaded yet! Download the protein with <protname>.download()')
-            
-    #Attempts to download protein file to a default directory (or a user-specified one)
+            )
     def download(self, destination = os.getcwd()):
+        """
+        Download Protein
+    
+        This method allows the user to download the simulated structural file of the specific protein from Alphafold (if a non-PDB ID is given) or a true structural file from RCSB (if a specific PDB ID is provided). Can identify process cif/mmcif files as well as .pdb files. Downloading the protein also collects all residue and atom information from the structural file, populating the attributes of the protein class.
+    
+        Parameters
+        ----------
+        destination : str
+            The destination of the protein file, defaulting to the current user directory.
+        """
         self.cif = False
                 
         #Downloads files from RCSB if they are PDB files
         if self.ID_type == 'PDB':
             try:
                 protname = self.protein + '.pdb'
                 urllib.request.urlretrieve('http://files.rcsb.org/download/' + protname, destination + '/' + protname)
@@ -340,32 +450,50 @@
                         counter += 1    
     
         #Generates FASTA sequence based on protein file
         self.FASTA = ''
         for id_residue in self.residue_list:
             self.FASTA += FASTAdict[id_residue.amino_acid]
     
-    #Method that outputs all atoms in a .csv file
     def to_csv(self, destination = os.getcwd()):
+        """
+        Atoms to CSV
+    
+        This method returns a .csv file of each individual atom of the protein and all contained attributes within the atom.
+    
+        Parameters
+        ----------
+        destination : str
+            Destiation of the csv file. Defaults to the user's current directory
+        """
         atoms_x, atoms_y, atoms_z, atoms_element, atoms_residue, residue_index, residue_chain = [], [], [], [], [], [], []
         for count, residue in enumerate(self.residue_list):
             for atom in residue.atoms:
                 atoms_x.append(atom.x)
                 atoms_y.append(atom.y)
                 atoms_z.append(atom.z)
                 atoms_element.append(atom.element)
                 atoms_residue.append(residue.amino_acid)
                 residue_index.append(residue.index)
                 residue_chain.append(residue.chain)
         atoms = pd.DataFrame.from_dict({'Atom x coordinate':atoms_x, 'Atom y coordinate':atoms_y, 'Atom z coordinate':atoms_z, 'Atom element':atoms_element, 'Atom residue':atoms_residue, 'residue index':residue_index, 'residue chain': residue_chain})
         atoms.to_csv(destination + '/Atoms' + self.protein + '.csv')
         
-    #Property for calculating center of mass of the protein
     @cached_property
     def center(self):
+        """
+        Protein Center of Mass
+    
+        This property returns the center of mass of the protein, which is generated from all atom components of each residue in the protein.
+    
+        Returns
+        -------
+        list
+            A list consisting of the x, y, and z coordinate in 3D space of the protein center of mass position for the protein structural file.
+        """
         try:
             x, y, z, totmass = 0, 0, 0, 0
             for res in self.residue_list:
                 for atom in res.atoms:
                     x += atom.x
                     y += atom.y
                     z += atom.z
@@ -373,17 +501,26 @@
             x /= totmass
             y /= totmass
             z /= totmass
             return [x, y, z]
         except:
             print('Protein not downloaded yet or downloaded incorrectly!')
     
-    #Property for obtaining list of ligand sites
     @cached_property
     def sites(self):
+        """
+        Docked Ligand Center of Mass
+    
+        This property returns the center of mass for each ligand position of each unique ligand type within the protein file.
+    
+        Returns
+        -------
+        dict
+            A dictionary containing the unique ligand identifier within the protein file (the key) and a list of the center of mass of each indivual ligand pose (the values)
+        """
         if self.ID_type != 'PDB':
             return 'Not a PDB file with valid binding sites!'
         else:
             sites = {}
             for ligand in self.ligand_list:
                 if len(ligand.sites) > 0:
                     try:
@@ -391,17 +528,31 @@
                     except:
                         sites[ligand.ID] = [ligand.sites]
                 else:
                     sites = 'No valid binding sites listed in PDB file!'
                     break
         return sites
     
-    #Method for indexing protein residues
     @lru_cache
     def residues(self, residue_index):
+        """
+        Residue Indexing
+    
+        This method allows for indexing residues with a numeric or a side chain-numeric (i.e. A244) identifier.
+    
+        Parameters
+        ----------
+        index : int, str
+            Numeric or string index of the residue.
+            
+        Returns
+        -------
+        class
+            Returns the residue class at the given index.
+        """
         try:
             try:
                 index = int(re.sub('[^0-9]', '', residue_index))
                 residue = self.residue_list[index]
                 if residue.index != index:
                     diff = residue.index - index
                     residue = self.residue_list[index - diff]
@@ -410,41 +561,79 @@
     
             residue_items = {'chain':residue.chain, 'AA':residue.amino_acid, 'index':residue.index, 'atoms':residue.atoms}
             res = pd.Series(residue_items, index = ['chain', 'AA', 'index', 'atoms'])
             return res
         except:
             return 'Index larger than number of residues!'
            
-    #Method for indexing protein atoms
     @lru_cache
     def atoms(self, atom_index):
+        """
+        Atom Indexing
+    
+        This method allows for indexing atoms with a numeric identifier.
+    
+        Parameters
+        ----------
+        index : int
+            Numeric index of the atom. 
+            
+        Returns
+        -------
+        class
+            Returns the atom class at the given index.
+        """
         ac = 0
         for res in self.residue_list:
             for atom in res.atoms:
                 if ac == atom_index:
                     atom_items = {'element':atom.element, 'x':atom.x, 'y':atom.y, 'z':atom.z, 'residue':atom.residue, 'data':atom.data}
                     atm = pd.Series(atom_items, index = ['element', 'x', 'y', 'z', 'residue', 'data'])
                     return atm
                 ac += 1
         return 'Index is larger than total number of atoms!'
     
-    #Method for reconstructing section of protein
     def concat(self, start, stop, destination = os.getcwd()):
+        """
+        Residue Concatenation
+    
+        This method allows for the concatenation of residues into a sub-structural file containing only the indexed residues.
+    
+        Parameters
+        ----------
+        start : int
+            Starting numeric index of the first residue.
+            
+        stop: int
+            Final numeric index of the last residue in the sub-structure.
+            
+        destination: str
+            Location of the downloaded sub-structure, defaults to the user's current directory.
+        """
         residues, atoms = [i for i in self.residue_list if i >= start and i < stop], []
         for res in residues:
             for atom in res.atoms:
                 atoms.append(atom.data)
                 
         with open(destination + '/' + self.protein + str(start) + 'to' + str(stop) + '.pdb', 'w') as f:
             for line in atoms:
                 f.write(line)
     
-    #Returns a uniprot identifier
     @cached_property
     def Uniprot(self):
+        """
+        Uniprot ID
+    
+        This properties allows for easy conversion of protein IDs to Uniprot IDs.
+
+        Returns
+        -------
+        str
+            Returns the Uniprot ID for the protein class.
+        """
         if self.ID_type.upper() == 'UNIPROT':
             return self.protein
         elif self.ID_type.upper() == 'PDB':
             try:
                 out = mg.querymany(self.protein, scopes = 'pdb', fields = 'uniprot', species = self.species)
             except:
                 out = mg.querymany(self.protein, scopes = 'pdb', fields = 'uniprot', species = 'all')
@@ -501,17 +690,26 @@
                 firstResultIndex = Data.index('primaryAccession')
                 uniprot = Data[firstResultIndex + 19:firstResultIndex + 25] 
                 return uniprot
             except:
                 print('Cannot find valid Uniprot ID for protein ' + self.protein + '!')
                 return 'N/A'
     
-    #Returns a PDB identifier
     @cached_property 
     def PDB(self):
+        """
+        PDB ID
+    
+        This properties allows for easy conversion of protein IDs to PDB IDs. A pandas dataframe containing the number of unique ligands, number of residues, and the resolution of the electron microscope used to image the protein is returned.
+
+        Returns
+        -------
+        df
+            Returns a dataframe containing relevant properties for all PDB IDs associated with the protein ID.
+        """
         def scrape_data(PDB):  
             resdf = pd.DataFrame()
             resolutions, residue_number, lignums, proteins = [], [], [], []
             for ID in PDB:
                 curr_lig, lignum = '', 0
                 protname = ID + '.pdb'
                 try:
@@ -621,17 +819,26 @@
                     pass
                 return scrape_data(PDB_IDs)
             except:
                 print('Cannot find valid PDB ID for protein ' + self.protein + '!')
                 return 'N/A'
         
     
-    #Returns HGNC identifier
     @cached_property
     def Gene(self):
+        """
+        Gene ID
+    
+        This properties allows for easy conversion of protein IDs to Gene IDs.
+
+        Returns
+        -------
+        str
+            Returns the Gene ID for the protein class.
+        """
         def search_uniprot(protein):
             url = 'https://rest.uniprot.org/uniprotkb/search?query=' + self.protein + '%20' + self.species
             Data = requests.get(url).text
             firstResultIndex = Data.index('geneName":')
             Gene = Data[firstResultIndex + 20:firstResultIndex + 31]
             Gene = Gene.split('"')[0]
             return Gene
@@ -655,17 +862,26 @@
                  except:
                      out = mg.querymany(self.protein, scopes = 'pdb', fields = 'symbol', species = 'all')
                  gene = out[0]['symbol']
                  return gene
              except:
                 return search_uniprot(self.protein)
             
-    #Returns ChEMBL identifier
     @cached_property
     def ChEMBL(self):
+        """
+        ChEMBL ID
+    
+        This properties allows for easy conversion of protein IDs to ChEMBL IDs.
+
+        Returns
+        -------
+        str
+            Returns the ChEMBL ID for the protein class.
+        """
         try:
             target = new_client.target
             gene_name = self.Gene
             res = target.filter(target_synonym__icontains=gene_name).only('target_chembl_id')[0]
             ChEMBL = res['target_chembl_id']
             return ChEMBL
         except:
@@ -676,43 +892,61 @@
                 ChEMBL = Data[firstResultIndex + 14:firstResultIndex + 34]
                 ChEMBL = ChEMBL.split('"')
                 return ChEMBL[0]
             except:
                 print('No ChEMBL ID found for ' + self.protein + '!')
                 return 'N/A'
          
-    #Property for obtaining protein ligands (if present in file)
     @cached_property
     def ligands(self):
+        """
+        Protein Ligands
+    
+        This property returns a series containing the ID of the primary ligand contained within the file, as well as the ID of all present confactors. Only returns ligands if the file is a PDB file with valid ligand structures contained.
+    
+        Returns
+        -------
+        df
+            A pandas dataframe containing the primary ligand IDs and cofactor IDs within the protein structural file.
+        """
         ligs = []
         for ligand in self.ligand_list:
             if ligand.ID not in ligs:
                 ligs.append(ligand.ID)
-        ligand = ligs[0]
-        cofactors = ligs[1:]
-        ligands = pd.DataFrame.from_dict({'Protein': self.protein, 'Primary Ligand':ligand, 'Cofactors':cofactors})
+            ligand = ligs[1]
+            cofactors = ligs[1:]
+        ligands = pd.DataFrame.from_dict({'Primary Ligand':ligand, 'Cofactors':cofactors})
         return ligands
     
-    #Property for obtaining protein binders. Searches ChEMBL, BindingDB, and STITCH
     @cached_property   
     def interactions(self):
+        """
+        Protein Interactions
+    
+        This property allows the user to query the Bioinformatics databases STITCH, BindingDB, and ChEMBL for relevant protein-ligand and protein-protein interactions. BindingDB interactions are contained in a dataframe containing the Kd constant in nanoMolar. ChEMBL IDs are returned along with the IC50 or DC50 values in nanoMolar. STITCH data represents a dictionary-embedded list of all proteins and ligands with network-based interactions. If valid data cannot be pulled from any site, their output datatypes will not be included in output.
+    
+        Returns
+        -------
+        list
+            A list containing two dataframes for BindingDB and ChEMBL protein-ligand intearction data, as well as a dictionary containing all STITCH interactors for the given protein ID with a high confidence of interaction.
+        """
         try:
             #Queries bindingDB for ligand interactions
             try:
                 Affinities, ligands = [], []
                 url = 'https://bindingdb.org/axis2/services/BDBService/getLigandsByUniprot?uniprot=' + self.Uniprot
                 mytree = ET.fromstring(requests.get(url, timeout=4).text)
                 for tree in mytree:
                     if 'affinities' in i.tree:
                         ligands.append(i[1].text)
-                        Affinities.append(float(i[3].text))
-                BindingDB = pd.DataFrame.from_dict({'Ligands':ligands, 'Kd (nM)': Affinities})
+                        Affinities.append(float(i[3].text) * 1000)
+                BindingDB = pd.DataFrame.from_dict({'Ligands':ligands, 'Kd': Affinities})
             except:
                 print('BindingDB request timed out!')
-            
+                
             #Queries STITCH for protein and ligand interactions
             try:
                 url = 'http://string-db.org/api/tsv-no-header/resolve?identifier=' + self.Uniprot
                 Result = [i for i in re.split(' |\t', requests.get(url).text.strip()) if i != '']
                 if Result[3].upper() == Result[3]:
                     Gene = Result[3]
                 else:
@@ -727,37 +961,32 @@
                         IDlist.append(ID)
                 STITCH = {'STITCH':set(IDlist)}
             except:
                 print('No compounds or proteins found in STICH!')
                 
             #Queries ChEMBL for ligand interactions
             try:
-                target, ligands, affinities = new_client.target, [], []
+                target, ligands, activities = new_client.target, [], []
                 activity = new_client.activity
                 activities = activity.filter(target_chembl_id=self.ChEMBL).filter(standard_type="IC50")
                 for act in activities:
-                    try:
-                        value = float(act['value'])
-                        if act['units'] != 'nM':
-                            if act['units'] == 'uM':
-                                value *= 1000
-                            elif act['units'] == 'pM':
-                                value /= 1000
-                    except:
-                        value = 'NaN'
-                   
+                    value = float(act['value'])
+                    if act['units'] != 'nM':
+                        if act['units'] == 'uM':
+                            value *= 1000
+                        elif act['units'] == 'pM':
+                            value /= 1000
                     try:
                         ligands.append(act['canonical_smiles'])
-                        affinities.append(value)
+                        activities.append(value)
                     except:
                         continue
-                
-                ChEMBL = pd.DataFrame.from_dict({'Ligands':ligands, 'IC50 (nM)':affinities})
+                ChEMBL = pd.DataFrame.from_dict({'Ligands':ligands, 'IC50 (uM)':activities})
+                ChEMBL = {'ChEMBL':chembl}
             except:
-                print(traceback.format_exc())
                 print('No compounds or proteins found in ChEMBL!')
             results = []  
             try:
                 results.append(BindingDB)
             except:
                 pass
             try:
@@ -778,14 +1007,13 @@
     - Add more ID conversions
     '''
 '''
 #For unit testing    
 if __name__ == '__main__':
     p = Protein('1HK4')
     p.download()
-    for item in p.interactions:
-        print(item)
+    print(p.ligands)
     #new = Protein(p.Uniprot)
     #new.download()
     #print(new.interactions)
     #print(protein.interactions)
 '''
```

