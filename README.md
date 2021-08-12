# CDDS-CESM
 
*Collection of documentation, tutorials, and notebooks highlighting how to set up, run, and analyze CESM/CAM simulations on the Cheyenne Supercomputer. This repo assumes basic knowledge of the CESM environment and Python. In order to get the most out of this repo, please review the provided documentation and tutorials linked below*

## Requirements
- Access to the Cheyenne Supercomputer
- Python 

## Documentation & Tutorials
[2020 CESM Tutorial Course](https://www.cesm.ucar.edu/events/tutorials/2020/coursework.html)
- Week long course (~8 hours per day)
- Broken down into Lectures, Practicals, and Talks
- Practicals are the most important parts of this course for setting up simulations

[CESM Quickstart Guide (CESM2.2)](https://escomp.github.io/CESM/versions/cesm2.2/html/)
- Community Earth System Model (CESM)

[CAM 6.0 User's Guide](https://ncar.github.io/CAM/doc/build/html/index.html)
- Community Atmosphere Model (CAM)

[CIME Documentation](http://esmci.github.io/cime/versions/master/html/index.html)
- Coupling Infrastructure for Modeling Earth (CIME)

## Cheyenne Environment
You can interface with Cheyenne using a linux terminal envrioment through SSH.  

## Workflow

#### Creating a Case

Once you have decided on a compset and grid resolution, you can run the case creation command. For your casename, you can specify a directory and name for your case to be created in. You need to also specify what project account you are going to use. 
```
./create_newcase --case CASENAME --compset COMPSET --res GRID --project PROJECT
```

#### Setting up the Case
This command creates scripts needed to run the model and namelist files. 

```
./case.setup
```

#### Building the Case

```
./case.build
```
or
```
qcmd -- ./case.build
```



## Changing SST Boundary Conditions
In order to prescribe SST/ICE, you must be using either an A or F compset. The first step is to create a case as shown above. Once 


## Notebooks


