# NanoAODProduction
NanoAODProduction

Install:

    #Enter into lxplus8-machine or lxplus9-machine
    scram project CMSSW_15_0_2
    cd CMSSW_15_0_2/src/
    cmsenv
    git cms-init
    git cms-checkout-topic bmarzocc:NanoAODv15_MustacheVars_15_0_2 #if you want to add additional Mustache variables variables
    git clone git@github.com:bmarzocc/NanoAODProduction.git
    git checkout Summer24NanoAODv15
    scram b -j 10

Run:

    cd NanoAODProduction/Summer24NanoAODv15/test/
    cmsRun step6_MINIAODSIM_cfg.py #Produce MINIAOD with additional Mustache info
    cmsRun step7_NANOAODSIMv15_cfg.py #Produce Summer24NanoAODv15 samples
