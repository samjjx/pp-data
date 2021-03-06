## Public-Private networks ##

### Introduction ###

We investigate the relationships of the authors and their research interests. In this repository, we offer all the links of the datasets and report some basic statistics. 

### Datasets ###

We investigate our research based on the dblp[1]. We divide the datasets into two parts based on the first publication of the papers. The dataset we used was published on 2019/01/01.

Datasets| n | m | n' | m'| ∂ 
----|----|----|----|----|---
y-2013 | 2,221,139 | 5,432,667 | 1,265,175 | 6,007,245 | 0.107000024123
y-2014 | 2,221,139 | 6,186,831 | 1,150,642 | 5,322,474 | 0.108253774729
y-2015 | 2,221,139 | 7,012,003 | 1,018,652 | 4,518,645 | 0.109794362055
y-2016 | 2,221,139 | 7,864,133 | 870,054   | 3,628,517 | 0.112118661251
y-2017 | 2,221,139 | 8,794,753 | 690,588   | 2,658,750 | 0.11562333225
	
	1. n is the number of the authors in the public networks.
	2. m is the number of the co-authors relationships in the public networks.
	3. n' is the number of the authors in the private networks.
	4. m' is the number of the co-authors relationships in the private networks.
	5. ∂ is the common average research interests. 

### Downloads ###



#### links ####
Datasets| [y-2013](https://drive.google.com/file/d/1QCvpmLADUuhxPRYjPiFwPs2RMcSRn9vh/view?usp=sharing) | [y-2014](https://drive.google.com/file/d/1yw5iyVdEoE4OXMlGy46JfBjytonExDjK/view?usp=sharing) | [y-2015](https://drive.google.com/file/d/1wP3B4gt9ooalyQQRvCIk1mTDJA-WhAhy/view?usp=sharing) | [y-2016](https://drive.google.com/file/d/1M7wif77hyGzu4D5cST8E57Bxqfx2RSS8/view?usp=sharing) | [y-2017](https://drive.google.com/file/d/1_wr0rWcqNuDT4m9KyiPzTJDcMAXRkwAw/view?usp=sharing)
----|----|----|----|----|----

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

1. [dblp](https://dblp.org/xml/release/)
