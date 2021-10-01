# ellipse_perimeter
Few programs in FOCAL (HP41) for 
a) ellipse perimeter calculation
b) ellipse isoperimeter curve representation
c) calculus and analysis (error calculation) of curves which define isoperimetercurves of ellipse


These functions together creates a vivarium of functions which are compatible with others regarding memory (register) sharing; 
and compatible with other FOCAL functions of modules ADVANTAGE (SOLVE) or MATH (SOL).


Some programs use the printing functionality of HP-IL: it can be modified easily for having the data only being printed into the HP41 screen. 


However, the recommended setup is an HP41 connected to pyILPER on a PC via a PILBOX 
(in this case, the printing will be done on a window in the PC and the results can be easily transfered to complementary analysis 
at DESMOS.COM for example via a copy/paste of a PC editor).


Way for using the programms: read the TXT files and put them direct into the HP41 or

a) download the files in a PC

b) use the application hp41uc with "hp41uc.exe /t=SCPEREL.TXT /r /k". see https://sourceforge.net/projects/hp41uc/

c) upload the .raw file into the HP41 emulator V41 https://hp.giesselink.com/v41.htm

d) and use the programms there

e) ... or more ...

f) install pyILPER on your PC (see anaconda package)

g) transfer the programs from V41 into pyILPER

h) connect your HP41 with the PC via pilbox. Here you can order a pilbox http://www.jeffcalc.hp41.eu/hpil/index.html#pilbox

i) download the programs from pyILPER into your HP41; then use them


List of programs; look at the description in the TXT files for using them.


PEREL3 and PEREL4: calculate the perimeter given a and b (2 different convergences). No dependencies.


PERELS: calculate the perimeter of an ellipse according the best suitable method. Dependencies: PEREL3 and PEREL4.


BPEREL: calculate the other half-parameter of an ellipse by a given perimeter. Dependencies: PERELS, SOLVE from SandMath 
(or "SOL" from Math module by replacing the Line 
XEQ "SOLVE" 
with 
ASTO 06
XEQ "SOL"


SCPEREL: output several isoperimeter points of an ellipse by a given perimeter. Dependency: BPEREL, HP-IL (for outputs logging into printer/screen).


CMPPERE: compare 
a) ellipse perimeter calculation based on infinite serial calculations and 
b) ellipse perimeter calculation based on other method
Dependencies: BPEREL, HP-IL (for outputs logging into printer/screen), new function "CALPERE" (or other tbd).


CALPERE: calculate the ellipse perimeter based on a cycloid adjusted with the Bohr Magneton electron Adjustment factor. 
Dependencies: "SOLVE" from Sandmath, HP-IL (for outputs logging into printer/screen). 


Final word: 
these functions which can be used in the HP41 must be understood in the terms of mocks in the area of agile working. 
They are "Good enough" functions for quick evaluations of new ideas in ellipse-perimeter calculus.
Any functions with precise results will have to be checked and released on higher precision calculators (HP71 for example) 
and perhaps larger 64bits processors before any further use or creating mathematical conclusions.
All the functions are NOT for any legal and productive use in the real world. Just use it in order to developp your creativity and thoughts.
And: contact me if you want to share new thoughts or have any question.
