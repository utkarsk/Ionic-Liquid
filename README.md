# Ionic Liquid #

This repository is created by **Utkarsh Kapoor**, as part of the Ph.D. disseration, for the purpose of contributing to the ionic liquid research community; and allowing the user to get acquainted with running simulations. It contains:


* Force Field Parameters  
	1. Zhiping Liu United Atom FF  
	2. CL&P All Atom FF  
* Input Files for running MD simulations using GROMACS
* CASSANDRA input files for running MC Simulations for Phase Equilibria Properties

##### Utkarsh Kapoor, Oklahoma State University #####

## Download ##

git clone https://utkarshkapoor@bitbucket.org/utkarshkapoor/ionic-liquid.git

## Force Field Parameters Available ##

#### Zhiping Liu United Atom FF ####

* Cations  
	* 1-ethyl-3-methylimidazolium [EMIM]
	* 1-butyl-3-methylimidazolium [BMIM]
	* 1-hexyl-3-methylimidazolium [HMIM]
	* 1-octyl-3-methylimidazolium [OMIM]
	
* Anions
	* chloride [Cl]
	* methylsulfate [MeSO4]
	* bis(trifluoromethylsulfonyl)amide [NTf2]
	* acetate [OAC]
	* trifluoroacetate [TFA]
	* trifluoromethanesulfonate [TFS]


#### CL&P All Atom FF ####

* Cations 
	* 1,3 dimethylimidazolium     [MMIM]
	* 1-ethyl-3-methylimidazolium [EMIM]
	* 1-butyl-3-methylimidazolium [BMIM]
	* 1-hexyl-3-methylimidazolium [HMIM]
	* 1-octyl-3-methylimidazolium [OMIM]
	* 1-decyl-3-methylimidazolium [DMIM]
	* 1-dodecyl-3-methylimidazolium [XMIM]
	
* Anions
	* 1-n-octylsulfate [OtSO4]
	* chloride [Cl]
	* methylsulfate [MeSO4]
	* dimethylphosphate [Me2PO4]
	* acetate [OAC]
	* bis(trifluoromethylsulfonyl)amide [NTf2]
	* trifluoroacetate [TFA]
	* trifluoromethanesulfonate [TFS]
	* tris(pentafluoroethyl)trifluorophosphate [eFAP]
	* tetraborofluorate [BF4]
	* hexafluorophosphate [PF6]
	* dicyanamide [DCA]
	
#### Extra Force Field Parameters ####

* Gas Solutes
	* carbon dioxide [CO2]  (from the works of Shi and Maginn)
	* sulfur dioxide [SO2]  (from the works of Shi and Maginn)
	* ammonia [NH3]         (from the works of Shi and Maginn)
	* methane [CH4]         (from TRaPPE)

* Others
	* 1-n-octanol [C8H17OH]  (CL&P)
	* n-octane [C8H18]	     (CL&P)
	* water [H2O]            (SPC/E)

## GROMACS Input Files Available ##

* MDP Files
	* minimize (minimization using steepest descend)
	* annealing (to remove bad energy contacts)
	* nvt_eq (relaxation in NVT ensemble)
	* npt_eq (relaxation in NPT ensemble)
	* npt_prod (Production run - used for analysis)

* TOP Files (only for reference)
	* a top file for [BMIM]Cl[NTf2] mixture for using Zhiping Liu FF
	* a top file for [XMIM][OtSO4] for using CL&P FF

## CASSANDRA Input Files Available ##

* MCF (Molecular connectivity file)
	* 1-butyl-3-methylimidazolium [BMIM]        (Zhiping Liu FF)
	* chloride [Cl]                             (Zhiping Liu FF)
	* bis(trifluoromethylsulfonyl)amide [NTf2]  (Zhiping Liu FF)
	* methylsulfate [MeSO4]                     (Zhiping Liu FF)
	* carbon dioxide [CO2]                      (from the works of Shi and Maginn)
	* methane [CH4]                             (from TRaPPE)

* INP (INPUT file)
	* Gibbs Ensemble Monte Carlo (GEMC_NPT) Simulation (Both Equilibration and Production)
		* For Pure Gas Solubility in [BMIM]Cl[NTf2] mixture at a particular pressure
		* For Mixture of CO2/CH4 Solubility in [BMIM]Cl[NTf2] mixture at 100 bar pressure

* PDB 
	* Since CASSANDRA requires atom connectivity information, unlike GROMACS

## PDB Files Available ##
All the relevant cation, anion and gas solute mentioned above, PDB files are provided.

## Input Files for doing Thermodynamic Integration using MD in GROMACS ##
* MDP Files (for initial state only)
	* minimize
	* annealing 
	* nvt_eq
	* npt_eq 
	* npt_prod

* TOP Files (only for reference)
	* a top file for CO2 + [BMIM]Cl[NTf2] mixture for using Zhiping Liu FF


## GROMACS Tutorial ##

* TO BE ADDED SOON

## CASSANDRA Tutorial ##

* TO BE ADDED SOON

## References ##
U. Kapoor and J. K. Shah "Effect of Molecular Solvents of Varying Polarity on the Self-Assembly of 1-n-Dodecyl-3- methylimidazolium Octylsulfate Ionic Liquid" [J. Theor. Comput. Chem. 2018, 17, 1840004-1-1840004-26](https://www.worldscientific.com/doi/pdf/10.1142/S0219633618400047) 

U. Kapoor and J. K. Shah "Thermophysical Properties of Imidazolium-Based Binary Ionic Liquid Mixtures Using Molecular Dynamics Simulations" [J. Chem. Eng. Data, 2018, 63 (7), 2512-2521](https://pubs.acs.org/doi/abs/10.1021/acs.jced.7b01028)

U. Kapoor and J. K. Shah "Globular, Sponge-like to Layer-like Morphological Transition in 1-n-Alkyl-3-methylimidazolium Octylsulfate Ionic Liquid Homologous Series" [J. Phys. Chem. B, 2018, 122(1), 213-228](https://pubs.acs.org/doi/abs/10.1021/acs.jpcb.7b08397)

U. Kapoor and J. K. Shah "Preferential Ionic Interactions and Microscopic Structural Changes Drive Nonideality in Binary Ionic Liquid Mixtures as Revealed from Molecular Simulations" [Ind. Eng. Chem. Res., 2016, 55 (51), 13132-1314](https://pubs.acs.org/doi/abs/10.1021/acs.iecr.6b03314)



## About ##

Contributing Authors: Utkarsh Kapoor and Jindal K. Shah, Oklahoma State University

Contact: utkarsh.kapoor@okstate.edu

Funding: Gratitude is expressed to the National Science Foundation (NSF ACI-1339785 and NSF CBET-1706978) for funding the project.


