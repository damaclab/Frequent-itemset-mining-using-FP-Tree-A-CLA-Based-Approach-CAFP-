# CAFP
Frequent Itemset Mining Using FP-Tree: A Cellular Learning Automata Based Approach

## Description
 CAFP uses Cellular Learning Automata (CLA) and multiple FP tree structures for frequent itemset mining that is efficient in both time and memory requirements. 
 Dense dataset (DDS) has been proposed for compact representation of the larger input transaction dataset. This optimizes both time and memory as a larger dataset scan can be avoided in successive mining steps.

## Citation details
If you use the source code in your work please reference this work by citing the following paper:

Ghosh, M., Roy, A., Sil, P. et al. Frequent itemset mining using FP-tree: a CLA-based approach and its extended application in biodiversity data. Innovations Syst Softw Eng 19, 283–301 (2023). https://doi.org/10.1007/s11334-022-00500-3

## Execution Environment
The experiments have been executed on a system with the following specifications:
- Processor: Intel i7-10870H @2.21GHZ, 4 core CPU
- Memory: 16GB 2666MHz DDR4
- Operating System: Windows 10, 64-bit


### Prerequisites

1. Installed Java version should be >= 8
2. Dependency used : [guava-22.0.jar](https://mvnrepository.com/artifact/com.google.guava/guava/22.0) (Has been included in this project)

## HOW TO EXECUTE

First <b>download</b> the <b>CAFP.jar</b> file.

Execution command --
```
CAFP.jar "input file path" "delimiter" "output file path" "minsup value as a fraction"
```
<br>
Each of these parameters represent -- <br>
<b>"input file path"</b>            : the path to an input file containing a transaction database.<br>
<b>"delimiter"</b>                  : the delimiter between each item in the input file.For example it will be "," for csv files<br>
<b>"output file path"</b>           : the output file path for saving the result (if null, the result will also be printed).<br>
<b>"minsup value as a fraction"</b> : the minimum support threshold.<br>
 <br>

For using it in editors -
1.Clone this repository 
2.Open it in your desired editor
3.Build it using maven with goals clean and install
4.As an example execute MainTest.java in main package.

## EXAMPLE
To execute it download the <b>CAFP.jar</b> file , <b>sample.txt</b> and type the following command --<br>
```  
CAFP.jar "sample.txt" " " "output.txt"  0.5
```

## Comparison Algorithms
CAFP algorithm has been compared against the following state-of-the-art algorithms: 
- EClat
- FPGrowth*
- LCM
- DFIN
- PrePost

We used the publicly available implementation of these algorithms from SPMF(https://www.philippefournier-viger.com/spmf/), a publicly available data mining library, written in Java.
The implementation for CAFP is in Java.

## Datasets
Several real datasets have been used for the comparison of the algorithms.
The datasets are openly accessible benchmark datasets that can be used to test how well the algorithms work. These are designed particularly for mining tasks and can be downloaded from the FIMI repository (http://fimi.ua.ac.be). 
- T10I4D100K
- Retail
- Pumsb
- Mushroom
- Chess
- Connect
- Accident

## ORIGINAL PAPER
* **Moumita Ghosh, Anirban Roy, Pritam Sil, Kartick Chandra Mondal** - *Frequent Itemset Mining Using FP-Tree: A CLA-based Approach and Its Extended Application in Biodiversity* - [Link To Paper](https://link.springer.com/article/10.1007/s11334-022-00500-3)
