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
Datasets| Public networks | Private networks | Public authors list | Private authors list | 
----|----|----|----|----
[y-2013](https://drive.google.com/drive/folders/1LbVCgFoKtWF98CVdQ_cdfPxfy-BwY0kV?usp=sharing) | [√](https://drive.google.com/file/d/1R_pwaOltJE_luJhgOfy21ZF_OnM25dFg/view?usp=sharing) | [√](https://drive.google.com/drive/folders/1klugWDnxI4Uhw4k32Y4CM13V8mmkaQbP?usp=sharing) | [√](https://drive.google.com/file/d/1m7xe8ue2d0aLWGtaN3TD3rOALDJ8G-nS/view?usp=sharing) | [√](https://drive.google.com/file/d/1hflsJUPGg05wOtu0qQiBGbae5CxY01J3/view?usp=sharing) 
[y-2014](https://drive.google.com/drive/folders/1oNpLKe7kqC_OGKgJddPNYrgvFtqqd9s4?usp=sharing) | [√](https://drive.google.com/open?id=1bXUzJXx4bwK4fAfBgcHtZMVS9_PFfKQx) | [√](https://drive.google.com/open?id=1y7vpsPVfEhcLOmz4WchUP3fvcVALGyWe) | [√](https://drive.google.com/open?id=1bXUzJXx4bwK4fAfBgcHtZMVS9_PFfKQx) | [√](https://drive.google.com/open?id=1sjPNv4vOvt4QXkgsTTWTDucHE-KFm53l) 
[y-2015](https://drive.google.com/drive/folders/1dqimeQLSKcaCjBXmBY_2quSgKxUCw7zr?usp=sharing) | [√](https://drive.google.com/open?id=129ZksL622Q_YTNPP_tH43tbMRhuYUJdT) | [√](https://drive.google.com/open?id=1AhK04-RXCApZdmVCdcrQCRTz1Uf5eKHF) | [√](https://drive.google.com/open?id=1RdDkdwgTbNSoGSt3_HQp8z_BrflwyqW0) | [√](https://drive.google.com/open?id=1W8cAONtRocJ_NxERET-tO7j6DUsjiWIe)  
[y-2016](https://drive.google.com/drive/folders/19p7FAZj-KMCvDG8Mk0zyct3s0OGEhmgB?usp=sharing) | [√](https://drive.google.com/open?id=1YC2sVQF3lVr8mm-grDr0xolSRhM-05ME) | [√](https://drive.google.com/open?id=1J7KJqlA3m9j3-bXjJAe5YOz8FwdHVWB1) | [√](https://drive.google.com/open?id=1E-5le1mAait60e3I0B5FDuFEso3C0AL_) | [√](https://drive.google.com/open?id=1BmwkaerV1K3qUpRRF_lor2RrBa34Ie-f)  

#### Data format ####

1. **Public networks and Private networks**
	
	Each line is two authors taking "\t" as separator which stands for a co-author relationship. 
	

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
