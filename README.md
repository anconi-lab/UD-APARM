Quick Guide to UD-APARM

1.	Introduction
The UD-APARM software constructs supramolecular systems from two isolated cartesian coordinates. 
UD-APARM reads two simple text files comprising the cartesian coordinates of each molecule that will form the supramolecular system to be studied. 
To run UD-APARM, you have to use the following files:

ud-aparm-molecule_1.xyz 

ud-aparm-MOLECULE_2-REFERENCE.xyz

ud-aparm.inp
__________________________________________
ud-aparm-molecule_1.xyz

a file that contains the XYZ cartesian coordinates (with atomic number or symbol) of the molecule to be handled over a cartesian reference system. Usually, the smaller molecule. 
__________________________________________
ud-aparm-MOLECULE_2-REFERENCE.xyz

a file that contains the XYZ Cartesian coordinates of the fixed in space molecule (usually the greater molecule in a supramolecular system).

__________________________________________
ud-aparm.inp

a file that contains instructions to the UD-APARM software (input).

2.	Installation
The pre-compiled Linux UD-APARM file ("ud-aparm-linux") can be downloaded from https://github.com/anconi-lab/UD-APARM. 
After creation of the directory "/home/ud-aparm" in your linux distro, into .bashrc ncludes the following line:

alias ud-aparm='/home/ud-aparm/ud-aparm-linux'

After editing such a file, download run-test-ud-aparm.tar.gz and extract the files: 

>tar  -xzvf run-test-ud-aparm.tar.gz

At run-test-ud-aparm , run UD-APARM to test

>./ud-aparm-linux

Change the input (ud-aparm.inp) for testing and use some visualization software to study the supramolecular systems obtained. 

With UCSF Chimera installed, you can see the supramolecular systems and vectors that define the relative position between the molecules (.bild files). 
The parameters for supramolecular characterization are discussed in the following publication:
Relative Position and Relative Rotation in Supramolecular Systems through the Analysis of the Principal Axes of Inertia: Ferrocene/Cucurbit[7]uril and Ferrocenyl Azide/β-Cyclodextrin Case Studies. ACS Omega 2020, 5, 10, 5013–5025. 
3.	UD-APARM input
 

![image](https://user-images.githubusercontent.com/86429259/206524981-a87520c7-b431-4de3-b05e-3c07ab0f8b42.png)

4.	How to cite and License
The ideas related to the implementation are descr¬ibed in the contribution published in ACS Omega (Cleber P. A. Anconi, ACS Omega 2020, 5, 5013 – 5025). The codes were improved and revised since the publication. Therefore, the version employed in your work should be identified. For reproducibility, the present version does not handle high symmetric molecules, such as benzene. The multiple possible values for the supramolecular parameters for highly symmetric systems are under investigation. 

LICENSE INFORMATION: To download and use APARM and UD-APARM, you are required to read and agree to the following terms:
(a) Currently, UD-APARM is free of charge for both academic and commercial usage. Anyone can freely distribute the original or their improved versions to others.
(b) UD-APARM can be distributed as a free component of commercial code. 
(c) UD-APARM is utilized in your work. The original ACS Omega paper MUST BE cited in your work (with the version of the software used): 
Anconi, C. P. A.  ACS Omega 2020, 5, 5013 – 5025. UD-APARM, version 1.18. 
(d) There is no warranty of the correctness of the results produced by UD-APARM. The author does not hold responsibility in any way for any consequences arising from the use of the UD-APARM software.
