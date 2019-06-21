# svmerge
Merge SVs according to reciprocal overlap
-----------------------------------------

## Quick Start

`./svmerge in.bed`

--------------

## Requirements

`svmerge` is designed for UNIX systems

* perl 5.X :camel:
* bedtools 2.X.X in environment path

------------------

## Installation:

Copy or download the perl script and make it executable

`chmod +x svmerge`

--------------------

## Usage

```
Tool:     svmerge 
About:    Merge SVs according to reciprocal overlap

Usage:    svmerge <bed file> [overlap]

Required Arguments:
    bed file        bed file of SVs to merge. Can be bgzipped

Optional Arguments:
    overlap         minimum reciprocal overlap requirement [default 0.8]

Notes:
    svmerge takes a bed file as input and merges SVs according to a defined
    minimum reciprocal overlap. 

    svmerge requires bedtools to be in the environment path.

    svmerge is written for UNIX systems

    svmerge will create temporary files in the current working directory. 
    
    Output will be in the form of a chain file linking the consensus SV to 
    the merged position.
         
         bed_file_svmerged.bed: consensus SV ---> merged SV 

Author:
    Danny Antaki, <dantaki at ucsd dot edu>
```
