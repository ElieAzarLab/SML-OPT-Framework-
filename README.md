# SML-OPT-Framework

This repository contains the code used for a project funded by the India-Canada Centre for Innovative Multidisciplinary Partnerships to Accelerate Community Transformation and Sustainability (IC-IMPACTS), especially [1]. The code was developed to allow for the creation of machine-learning (ML) surrogates of EnergyPlus -- a Building Performance Simulation (BPS) software -- outputs [2], then integrating the surrogates into an optimization framework (created using pymoo [3]) that also includes an energy supply model (created using NREL-pySAM [4]), with the aim of optimizing for energy demand & supply, thermal comfort, and costs (capital & operational).

While the examples given here are for an archetypal office in Ottawa, ON, Canada, the framework was designed to be adjustable to fit different climate and building contexts, provided the user has a working understanding of EnergyPlus (and Eppy [5]), ML, and Python. Seeing as the framework utilizes UNSGA-III, the framework can be scaled to accomodate from 1 to 15 objective functions, though the user is highly recommended to consult the original UNSGA-III papers before changing the number of objective functions coded in the repository, as well as the paper that this code supports ([1],[6]). Note also that the results found here differ very slightly from the ones in the paper due to the stochasticity of the optimization algorithm.

Earlier versions of this framework (not published due to incompleteness of scope/redundancy with what is found in this repository) were used for the following papers ([7-10]), which the user is encouraged to explore in addition to [1]. See also [11] for a tutorial on using pymoo with ML surrogates. 

[1] S. Qiblawi et al., "A many-objective building retrofit optimization framework leveraging reduced-order surrogate and physics-based models." [UNPUBLISHED]

[2] J. Woods et al., EnergyPlusTM v.23.2.0. (2023). National Renewable Energy Laboratory (NREL), United States. doi: 10.11578/dc.20240605.1

[3] J. Blank and K. Deb, “Pymoo: Multi-Objective Optimization in Python,” IEEE Access, vol. 8, pp. 89497–89509, 2020, doi: 10.1109/ACCESS.2020.2990567 (see https://github.com/anyoptimization/pymoo)

[4] P. Gilman et al., “PySAM (Python Wrapper for System Advisor Model ‘SAM’) [SWR-19-57],” National Renewable Energy Laboratory (NREL), Golden, CO (United States), PySAM, Aug. 2019. doi: 10.11578/dc.20190903.1 (see https://github.com/NREL/pysam)

[5] https://github.com/santoshphilip/eppy

[6] H. Seada and K. Deb, “A Unified Evolutionary Optimization Procedure for Single, Multiple, and Many Objectives,” IEEE Transactions on Evolutionary Computation, vol. 20, no. 3, pp. 358–369, Jun. 2016, doi: 10.1109/TEVC.2015.2459718

[7] S. Krishnan et al., "Evaluating the Capabilities of Surrogate Modeling Techniques in Predicting Hourly Building Energy Consumption." InEC3 Conference 2024 2024 Jul 14 (Vol. 5, pp. 0-0). European Council on Computing in Construction.

[8] E. Markarian et al., "Evaluating the Capabilities of Machine Learning Surrogate Modeling to Support High-Resolution Building Performance Simulation." In Advances in Information Technology in Civil and Building Engineering. ICCCBE 2024. Lecture Notes in Civil Engineering, vol 629. Springer, Cham. https://doi.org/10.1007/978-3-031-87364-5_14

[9] E. Markarian et al. "Informing building retrofits at low computational costs: a multi-objective optimisation using machine learning surrogates of building performance simulation models." Journal of Building Performance Simulation, 1–17. https://doi.org/10.1080/19401493.2024.2384487

[10] S. Qiblawi et al., "Informing Building Retrofits Using Surrogates of Physics-Based Simulation Models: A Comparison of Multi-Objective Optimization Algorithms," 2024 Winter Simulation Conference (WSC), Orlando, FL, USA, 2024, pp. 798-809, doi: 10.1109/WSC63780.2024.10838892.

[11] https://github.com/DataGasmic/EuroPython2023-Solving-MO_Constrained-Optimisation-with-Pymoo
