## Public-Private networks ##

### Introduction ###

We investigate the relationships of the authors and the research interests of the authors. In this repository, we offer all the links of the datasets and report some basic statistics. 

### Datasets ###

We investigate our research based on the dblp[1]. We divide the datasets into two parts based on the first publication of the papers. 

Datasets| n | m | n' | m'| ∂ 
----|----|----|----|----|---
[y-2013]() | 1,882,970 | 5,234,008 | 927,516 | 3,197,915 | 0.8654
[y-2015]() | 1,882,970 | 6,689,827 | 636,675 | 1,742,096 | 0.8977
[y-2016]() | 1,882,970 | 7,503,744 | 427,868 |  928,179  | 0.921
	
	1. n is the number of the authors in the public networks.
	2. m is the number of the co-authors relationships in the public networks.
	3. n' is the number of the authors in the private networks.
	4. m' is the number of the co-authors relationships in the private networks.
	5. ∂ is the common average research interests. 

### Downloads ###

#### links ####
Datasets| Public networks | Private networks | Public authors list | Private authors list 
----|----|----|----|----
[y-2013]() | [√](https://drive.google.com/file/d/1JvZeZnM7-oUsRtC2WyskOWLaHOjtTvoz/view?usp=sharing) | [√](https://drive.google.com/file/d/1EyQzjfyC5qUd1Hs1JyWGOIQOxru4whxa/view?usp=sharing) | [√](https://drive.google.com/file/d/1biPxG2xAvXrESVHru_Mu5LazWRB4zmZ9/view?usp=sharing) | [√](https://drive.google.com/file/d/1VgYL_KRdbw9oE5U6VntVp4Ws9sFhdrxF/view?usp=sharing) 
[y-2015]() | [√](https://drive.google.com/file/d/1fcemi02O5v64My_jirC4leGlduILVWXV/view?usp=sharing) | [√](https://drive.google.com/file/d/1teFxJImlIZSWCZn6U-JfEynhq0oBH_QW/view?usp=sharing) | [√](https://drive.google.com/file/d/175GUUSPvl2WsPGOdelMsti3NiujwN8fk/view?usp=sharing) | [√](https://drive.google.com/file/d/1Tq3Vm2cL8Vi9ZfpeThV_J2KCobXyhoVu/view?usp=sharing)  
[y-2016]() | [√](https://drive.google.com/file/d/1W4YcS8DISsnOFAPob4dXkK63_VBvl-25/view?usp=sharing) | [√](https://drive.google.com/file/d/1PkWDUj2nrWS9OYQP7T6Rqilk0Tz0Dzmg/view?usp=sharing) | [√](https://drive.google.com/file/d/1FS3fRDMXE4U-4FlJAOJ21bCLl3v0iv9G/view?usp=sharing) | [√](https://drive.google.com/file/d/16lnxtopnmZrda61-ZcUptr7gpSOTf_x5/view?usp=sharing)  

#### Data format ####

1. **Public networks and Private networks**
	
	Each line is two authors which takes "\t" as separator which stands for a co-author relationship. 
	

	Sample line:
	
	```
	5	2
	
	3	6
	
	2	9
	```	
	In this case, there are three co-author relationships. 

2. **Public authors list and Private authors list**

	Each line is a author and his/her research interests which wrapped up in a "#" pair. #author name# #author id# #research interests#
	
	Sample:
	
	```
	#Xin Huang# #241109# #networks;graph;community;knowledge;network;#
	```
### Reference ###

1. [dblp](http://dblp.uni-trier.de)
2. 