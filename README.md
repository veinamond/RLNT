# RLNT
Repository containing source codes for the RLNT solver, that is a modified 
variant of Relaxed_LCMDCBDL_newTech. It allows one to separately 
enable / disable the following heuristics such as:
SLS - stochastic local search component + rephasing
DL - Duplicate Learnts
CB - Chronological Backtracking
LCM - Learnt Clause Minimization
DIST - Distance heuristic from Maple_LCM_Dist

Turning the heuristics on and off is done via manipulation of 
preprocessor directives, e.g. #ifdef SLS.
Thus, to enable SLS one has to insert the line
#define SLS
into solver.h 

The Ipasir folder contains the ipasir-enabled variant of RLNT which can
be used in SAT Competition Incremental Track evaluations. 
