## Public-Private networks ##

### Introduction ###

We investigate the relationships of the authors and their research interests. In this repository, we offer all the links of the datasets and report some basic statistics. 

### Datasets ###

We investigate our research based on the dblp[1]. We divide the datasets into two parts based on the first publication of the papers. 

Datasets| n | m | n' | m'| ∂ 
----|----|----|----|----|---
y-2013 | 1,791,688 | 5,187,025 | 825,170 | 2,636,570 | 0.0858634262805
y-2014 | 1,791,688 | 5,893,083 | 686,292 | 1,930,512 | 0.0873812023198
y-2015 | 1,791,688 | 6,605,428 | 515,549 | 1,218,167 | 0.0869090560066
y-2016 | 1,791,688 | 7,378,090 | 263,937 |  445,505  | 0.0828958851282
	
	1. n is the number of the authors in the public networks.
	2. m is the number of the co-authors relationships in the public networks.
	3. n' is the number of the authors in the private networks.
	4. m' is the number of the co-authors relationships in the private networks.
	5. ∂ is the common average research interests. 

### Downloads ###



#### links ####
Datasets| [y-2013](https://drive.google.com/file/d/10EJEX-dLpoKO3yBlnbMTjpTE1WPIjU3a/view?usp=sharing) | [y-2014](https://drive.google.com/file/d/10Ca3uuMXSIEwZngpY7vdNW71GBFkO3iU/view?usp=sharing) | [y-2015](https://drive.google.com/file/d/10Ca3uuMXSIEwZngpY7vdNW71GBFkO3iU/view?usp=sharing) | [y-2016](https://drive.google.com/file/d/103v05vJoHQO3xCzK5wHG8fG9o2YZ6brH/view?usp=sharing) | 
----|----|----|----|----

#### Data format ####

1. **Public networks**
	
	Each line is two authors taking "\t" as separator which stands for a co-author relationship (author\_1, author\_2). 
	

	Sample line:
	
	```
	5	2
	
	3	6
	
	2	9
	```	
	In this case, there are three co-author relationships. 
	
2. **Private networks**

	We also randomly sample 50 private graphs for testing, e.g., 51673.g if a private graph for the author with id = 51673. Each line is an edge with its weight.  
	
	Sample line:
	
	```
	1113300	212609	1
	
	51673	382773	1
	
	867747	382773	1
	```
	
	In this case, there are three co-author relationships. 
	
3. **Public authors list**

	Each line is a author and his/her research interests which wrapped up in a "#" pair. #author name# #author id# #research interests#
	
	Sample:
	
	```
	#Xin Huang# #241109# #networks;graph;community;knowledge;network;#
	```
	
4. **Combined Private graphs**

	Since each vertex is associated with a private graph, we also combine all the private graphs in a file. 
	
	(1) The first line is a triple <Author name, # of vertices(n), # of edges(m)>.
	
	(2) The next n lines are the vertices in this private graph.  Each line is a triple <Author name, author id, research interests in this private graph>
	
	(3) The next m lines are the edges in this private graph. Each line is a tuple <src, dst>
	
	Sample:
	
	```
	#Francesco Paolo Schena# #3# #3#
	```
	```
	#Francesco Paolo Schena# #326160# #nephropathy;end;disease;classification;neural;#

	#David Naso# #4363# #nephropathy;end;disease;classification;neural;#

	#Giulio Binetti# #241721# #nephropathy;end;disease;classification;neural;#
	```
	```
	#4363# #326160#
	
	#326160# #241721#
	
	#4363# #241721#
	```
	

 
### Reference ###

1. [dblp](http://dblp.uni-trier.de)
