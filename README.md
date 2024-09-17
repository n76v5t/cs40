java c
DSCI 216 Stochastic Computing 
Fall 2024 
Proj#2 
Disk Array Design 
Due:  9/17/2024@ 11:59:59pm
Outcomes 
Upon completion of this project students will gain experience with reliability analysis and the construction of and experimentation with simulations of probabilistic systems comprised of interacting parts.
The Assignment 
Invented in 1987, Redundant Array of Inexpensive Disks (RAID), represented a significant improvement in performance and significant cost savings by demonstrating that through algorithmic means, disk performance could be improved by aggregating inexpensive devices versus using a single expensive high performance device. In this assignment, after considering motivating questions,  you will model a RAID 10 system and evaluate the impact on performance due to mirroring. 
The evolution of RAID begins with RAID 0. This technology begins with multiple disks. In RAID 0 (Figure 1), blocks of file storage are scattered across multiple disks, namely stripes. Because different parts of the same file are accessed on multiple physically different devices, all of the disk stripes must run in order for file operations to succeed. That is, pieces of the same file exist across different physical disks. In order toreador write a file, each of the disks in which a piece of a file is stored must run. In the RAID 0 example below (Figure 1) we have two stripes. Thus, in order toreador write a file, pieces of the file on each device must be accessed. 

Figure 1.  RAID 0, disk stripes
The nextstep in the evolution of RAID continued with RAID 1. This technology begins with multiple disks. In RAID 1 (Figure 2), a complete copy of all the blocks for a file are maintained on each of multiple physically different devices. These complete copies, namely mirror disks, are able to accept read/write requests for a file. Because each mirror maintains its own complete copy of the file, only one mirror must run in order for a file operation to succeed.

Figure 2.  RAID 1, disk mirrors
A key innovation in the evolution of RAID combined RAID 0 (striping) and RAID 1 (mirroring) to form. mirrored stripes, namely RAID 1+0 or RAID 10 (Figure 3). In RAID 10, we combine striping and mirroring. That is we maintain stripe disks (Disk 1 and Disk 3), but a complete copy of the stripes is also maintained (Disk 2 and Disk 4). The impact of RAID 10 is both a performance improvement attributed to striping as well as robustness attributed to the mirroring. 

Figure 3.  RAID 10:  disk stripe + mirror
Questions 
•   What type of dependency is represented by striping?  Draw a probabilistic dependence graph representing RAID 0 (Figure 1) consisting of two devices 代 写DSCI 216 Stochastic Computing Fall 2024 Proj#2 Disk	Array DesignR
代做程序编程语言Disk 1 and Disk 2
•   What type of dependency is represented by mirroring? Draw a probabilistic dependence graph representing RAID 1 (Figure 2) consisting of two devices, Disk 1 and Disk 2.
•   What type of dependency is represented by mirroring and striping?  Draw a probabilistic dependence graph representing RAID 10 (Figure 3) consisting  of four devices, Disk 1, Disk 2, Disk 3,and Disk 4.
Experiment 
•   You are building a RAID 10 storage array. You employ three-disk striping and decide to use, some number k-many mirrors.
•   You can decide how many mirrors you use for mirrored-striped RAID 10 storage array.
•   The base price for a “perfectly” reliable disk (0.01 failure rate) is $75
•   As the reliability decreases in percentage increments, the cost for each disk proportionately reduces in price. For example, a disk with 5% failure rate reflects a 5% reduction in cost per disk, while a disk with 10% failure rate reflects a 10% reduction in cost per disk.
•   Assume that every disk in your storage array has the same failure rate
•   In aJupyter Notebook, design and execute an experiment to determine:
o The most cost effective, most reliable, highest-performance
o How many mirrors you have?
o How many disks your RAID 10 array has
o Total cost of your RAID 10 array
•   Make sure you test your code and write your experiments to try different parameterizations.
•   Please remember to describe your design and document your results
Reflection 
•    How did you go about starting and solving the project
•   Were there any surprises or unexpected issues?
•   What did you learn from this project?
Submitting Your work 
1.   Create a folder using your name FirstNameLastNameProj2. If your name is John Smith your folder would be called JohnSmithProj2.
2.   In your folder, place a single MS-Word or PDF document containing all of your written work. All images and text must be in this document.
3.   In your folder, place your Jupyter Notebook. Remember that your Jupyter notebook is an IPYNB file.    DO NOT copy and paste or save the HTML version.
4.   In your folder, place your reflection document
5.   Compress your folder using ZIP only (no 7-Zip, notar, no rar).
6.   Submit your zip file to Canvas using the project submission site.
Note:  Verify that what you submit runs by decompressing your
archive to anew location and ensuring that it runs standalone.
Make sure your program does not depend on being in a specific directory because the instructor does not have any files that are  not part of your submission. Make sure your program runs from a clean Jupyter Environment.

         
加QQ：99515681  WX：codinghelp
