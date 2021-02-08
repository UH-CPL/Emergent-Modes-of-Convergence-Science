Required Files:
------------------------------------------------------------
Node Files:
1. Node_US_3cat.csv
2. Node_Europe_3cat.csv
3. Node_Australasia_3cat.csv

Edge Files:
1. Edge_US_3cat_1999.csv
2. Edge_Europe_3cat_1999.csv
3. Edge_Australasia_3cat_1999.csv
1. Edge_US_3cat_2004.csv
2. Edge_Europe_3cat_2004.csv
3. Edge_Australasia_3cat_2004.csv
1. Edge_US_3cat_2009.csv
2. Edge_Europe_3cat_2009.csv
3. Edge_Australasia_3cat_2009.csv
1. Edge_US_3cat_2014.csv
2. Edge_Europe_3cat_2014.csv
3. Edge_Australasia_3cat_2014.csv






Steps:
--------------------------------------------------------------
1. Load Node and edge files of 2014
2. Set color based on cip_type
3. Run all the Statistics algorithms
4. Set node size based on degree
5. Apply all layouts
6. Use Filter Degree and create new workspace. Named FULL_2014.
7. Use Filter Giant Component for giant component and create new workspace. Named GIANT_2014.
8. Save images for 2014
9. Use Filter Attributes Equal y_2009 = 1. Create another  workspace. Named FULL_2009
10. Delete edges from new workspaces. Then add new edges for that year.  
11.  Set node sizes based on below logic.
12. Use Filter Attributes Equal y_2009 = 1 in  GIANT_2014. Create another  workspace. Named 2009
13. Delete edges from new workspaces. Then add new edges for that year.
14. Use Filter Giant component and create new workspace. Named it GIANT_2009
15. Set node sizes based on below logic.
16. Save Images.
17. Repeat steps 12 to 16 for year 2004 and 1999





Coloring Logic:
--------------------------------------------------------------------
 1. Health             : Orange
 2. Neuro/Biology      : GREEN
 3. Sci/Eng            : MAGENTA





Layouts Design:
--------------------------------------------------------------------
1. Circle pack layout:
	Hierarchy1:	cip_type (Attribute)

2. Force atlas 2:
	Approximate Repulsion	false
	Stronger Gravity	true
	Gravity	0.5
	Dissuade Hubs	true
	LinLog mode	true
	Prevent Overlap	true

3. Rotate : for better looks
4. Expansion:
 	Scale factor	1.02


Node Size Calculation:
--------------------------------------------------------------------
 Highest degree in US         : 148
 Highest degree in Europe     : 195
 Highest degree in Australasia:  40

 Node Size from 5 to 100

For 2014,
 US node size range          ( 5 to 76 )  
 Europe node size range      ( 5 to 100 ) 
 Australasia node size range ( 5 to  21 ) 

For 2009,
 US node size range          ( 5 to 52 ) 
 Europe node size range      ( 5 to 67 ) 
 Australasia node size range ( 5 to 17 ) 
 

For 2004,
 US node size range          ( 5 to 36 ) 
 Europe node size range      ( 5 to 22 ) 
 Australasia node size range ( 5 to  10 )  



For 1999,
 US node size range          ( 5 to 24 )  
 Europe node size range      ( 5 to 17 ) 
 Australasia node size range ( 5 to  6 ) 
 



Node Reduced for 2014
----------------------------------------------------------------

North America: (total 3908)
	   Category             Color		Initial Number		Giant Component Number		% reduced
	1. Neuro/Biology      : GREEN		    2114			442			            79.09
 	2. Health             : Orange		    1552			240			  		84.54
 	3. Sci/Eng            : MAGENTA		     242			 39			  		83.88

Europe: (total 3088)
	   Category             Color		Initial Number		Giant Component Number		% reduced
	1. Neuro/Biology      : GREEN		    2008			351			  		82.5
 	2. Health             : Orange		     951			146			  		84.6	  
 	3. Sci/Eng            : MAGENTA		     129			  9			  		93    


Australasia: (total 1826)
	   Category             Color		Initial Number		Giant Component Number		% reduced
	1. Neuro/Biology      : GREEN		    773				134			  	82.66
 	2. Health             : Orange		    771				104			  	86.5
 	3. Sci/Eng            : MAGENTA		    282				7			  	97.5

	




