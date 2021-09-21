# cmstau
In refer to 

(1) https://cms-pdmv.cern.ch/mcm/public/restapi/requests/get_test/BPH-RunIISummer19UL16pLHEGEN-00001

(2) https://cms-pdmv.cern.ch/mcm/public/restapi/requests/get_test/BPH-RunIISummer19UL16SIM-00001

(3) https://cms-pdmv.cern.ch/mcm/public/restapi/requests/get_test/BPH-RunIISummer19UL16DIGIPremix-00001

(4) https://cms-pdmv.cern.ch/mcm/requests?prepid=BPH-RunIISummer19UL16HLT-00001&page=0&shown=127

(5) https://cms-pdmv.cern.ch/mcm/requests?prepid=BPH-RunIISummer19UL16RECO-00001&page=0&shown=127	

(6) https://cms-pdmv.cern.ch/mcm/public/restapi/requests/get_test/BPH-RunIISummer19UL16MiniAOD-00001

My customized files can be found in the py directory.
Where I applied no Pileup in (3).
And tried various pythia options in (2)

LHE files are either 

p p > ta+ ta-

or

mu+ mu- > ta+ ta- 

or

add model taudecay_UFO

import model sm__taudecay_UFO-full

  generate mu+ mu- > ta+ ta- ,  ta- > vt mu- vm~ / w+ w- , ta+ > vt~ pi+

  generate mu+ mu- > ta+ ta- ,  ta- > vt pi- pi- pi+, ta+ > vt~ pi+ 

  generate mu+ mu- > ta+ ta- ,  ta- > vt pi- pi- pi+, ta+ > vt~ mu+ vm / w+ w-

