  **Title:** Analysis and Modelling Lab 
  **Subtitle:** General Computational Skills 
  **Project:** Day 4: Data management with SQL
  **Author:** Julia Fotheringham  
  **Affiliation:** University van Amsterdam
  **Date:** January 31, 2019
 **Software:**
Data was processed in:
 DB Browser for SQLite, Version 3.10.1
Qt Version 5.7.1
SQLCipher Version 3.15.2

>**Data Resources:** 

The data tables were sourced from Hamish Wilman, Jonathan Belmaker, Jennifer Simpson, Carolina de la Rosa, Marcelo M. Rivadeneira, and Walter Jetz. (2014) [Elton Traits 1.0: Species-level foraging attributes of the world’s birds and mammals](https://doi.org/10.6084/m9.figshare.c.3306933.v1). Ecology 95:2027.
>**Contents of Data Table:** 

The Data tables created addressed the following queries:

>Define by scientific name (genus, Species) which bird species over 1000g utilise the aerial foraging strategy

	SELECT  Scientific as Lrge_AerialHntr
	FROM BirdFuncDat
	where ("ForStrat-aerial" >=1) and ("BodyMass-Value" >=1000)

Identify reference details for the source of mammalian body mass values and order by reference ID number lowest to highest.

	SELECT MamFuncDatSources.FullReference, MamFuncDat.Scientific as Sci_Name, MamFuncDatSources.Ref_ID
	FROM MamFuncDatSources
	JOIN MamFuncDat
	ON MamFuncDatSources.Ref_ID = MamFuncDat."BodyMass-Source"
	group by MamFuncDat.Scientific
	order by MamFuncDatSources.Ref_ID


Attribute tables for the SQL database can be found at:
https://github.com/jfoth/AML/blob/master/JFotheringham_Comp_Skills_Day4_new_attribute_tables
