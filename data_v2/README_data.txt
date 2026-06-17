The data provided can be used at different stages of the coding process.

***********************************
PLEASE NOTE - original data contained variables of interest (e.g. functional traits and sampling measures) which were not used in this study. 
However, this additional information was not yet standardised or validated. 
This will be done at a future date and released as an official database. 
If you made use of the original data, PLEASE VALIDATE THE DATA WITH THE SOURCE LITERATURE!
************************************

00_Primate_Studies.zip - contains the raw data collated from studies of primates should the reader want to run the very initial cleaning

01_Primate_Database_Initial.csv - database of initial XY points and occurrences. SEE THE README.TXT FILE IN MAIN DIRECTORY FOR EXPLANATION OF VARIABLES see the README.txt file in main directory for explanation of variables. 

	This .csv file is output of script 00_InitialDatabase.R and can be used to run code from script 01_ForestRasterGeneration.

03_Primate_Database_Patches.csv - database of patch sizes (in hectares) associated with the XY points of occupancy. 

	This .csv file is output of script 02_PatchGeneration.R and can be used to run code from script 03_2_PatchCombinationsGeneration.R onwards

	#Description of additional variables

04_Primate_Database_PatchCombinations.csv - database of patch combinations i.e. combinations of one or more patches totalling a predefined threshold of cumulative habitat amount.

	This .csv file is output of script 03_2_PatchCombinationsGeneration.R and can be used to run code from script 04_BrmModel.R onwards

06_FigS1_PatchDistribution - table of summary statistics of patches at level of IUCN threatened status. Used in 06_Figures_SM.R script to produce histograms.

06_FigS1_PatchDistribution - table of summary statistics of patch combinations at level of IUCN threatened status. 06_Figures_SM.R script to produce histograms.


Other files:

assessments.csv - used to assign IUCN threatened categories to species in 00_InitialDatabase.R script

dinerstein_lookup.csv - used to assign Dinerstein canopy cover thresholds in 00_InitialDatabase.R script. 
			
		i.e. the optimal canopy cover threshold that should be used with Hansen et al 2013 Global Forest Change Maps within each biome.

monkey2.png - used in methods figures produced in 05_1_Figures_Methods.R script


################################################################################################

Variable Descriptions:

	01_Primate_Database_Initial.csv 


	Source = the study that the primate patch occupancy data was taken from
	X = longitude coordinate in decimal degrees
	Y = latitude coordinate in decimal degrees
	Country = country of study
	Realm = biogeographical realm of study
	Family = family that species belongs to 
	Genus = genus that species belongs to
	Occurrence = presence or absence. presence = 1, absence = 0
	Taxon_ITIS = taxonomic name used by ITIS

	
	03_Primate_Database_Patches.csv

	#Add descriptions here of additional variables produced for this database

	04_Primate_Database_Patch_Combinations.csv

	#Add descriptions here of additional variables produced for this database
