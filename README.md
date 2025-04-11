# NanoAODProduction
NanoAODProduction

Install:

    #Enter into lxplus8-machine 
    scram project CMSSW_13_3_1_patch1
    cd CMSSW_13_3_1_patch1/src/
    cmsenv
    git cms-init
    git cms-checkout-topic bmarzocc:NanoAODv13_EGMVars_13_3_1_patch1
    git clone git@github.com:bmarzocc/NanoAODProduction.git
    scram b -j 10

Run:
    cd NanoAODProduction/NanoAODv13/test/
    cmsRun step_NanoAODv13_Run2_UL16_preVFP_cfg.py 
