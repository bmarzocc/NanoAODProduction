# NanoAODProduction
NanoAODProduction

Install:

    #Enter into lxplus8-machine or lxplus9-machine
    scram project CMSSW_15_0_15_patch4
    cd CMSSW_15_0_15_patch4/src/
    cmsenv
    git cms-init
    git cms-checkout-topic bmarzocc:NanoAODRunv15_NewDRNVars_15_0_15_patch4 #if you want to add additional DRN variables
    git clone git@github.com:bmarzocc/NanoAODProduction.git
    git checkout Run2v15
    scram b -j 10

Run:

    cd NanoAODProduction/NanoAODv15/test/
    cmsRun step_NanoAODv15_Run2_UL18_cfg.py 
