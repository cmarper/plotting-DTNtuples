# plotting-DTNtuples
Plotting scripts for DTNtuplizer

## Installation

* Create the singularity to run el7 on lxplus (to run on python instead of python3):
```
cmssw-el7
```

* Install the package:
```
cmsrel CMSSW_11_3_0
cd CMSSW_11_3_0/src/
cmsenv
git clone https://github.com/jaimeleonh/DTNtuples.git -b unifiedPerf DTDPGAnalysis/DTNtuples
# put these repo files under DTDPGAnalysis/DTNtuples/test
scramv1 b -j 5
```

## Execution
* Modify allLegends.py, runEffs.py, runResols.py with new filename

* Run efficiencies and resolutions
```
python runEffs.py -n (output en ./plotsEff)
python runResols.py -n (output en ./summaryPlots)
```
