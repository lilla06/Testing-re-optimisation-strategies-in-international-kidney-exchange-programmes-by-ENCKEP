# Testing-re-optimisation-strategies-in-international-kidney-exchange-programmes-by-ENCKEP
Testing re-optimisation strategies in international kidney exchange programmes by the ENCKEP simulator

## Config files
We used the modified config files to generate the datasets. These config files have modified PRA values based on real historical datasets.
The config_7.5.json was used for the tests on one pool (the 7.5 refers to the size of the pool), while the config_ES_modified.json, config_NL_modified.json and the config_UK_modified.json files were used for the multiple pool simulations to generate tha data for Spain, the Netherlands and fot the United Kingdom.

## Objective files
We used the general_objective.json file for most of the one pool simulations. The two exceptions are the cases when we tested the two new optimisation critera: to maximise the number of tested arcs we used the objective_max_num_tested_arcs.json file, and to maximise the number of inner arcs we used the objective_max_num_arcs_in_pools.json file.
For the multiple pool simulations we used the objective_UK_ES_NL.json in every case.

## Policy files
We used the policy_general.json for the general test. In the name of the other tests we used abbreviation.
- opti2/3/4/5: 2/3/4/5 optimisation rounds
- max2/4: teh maximum length of the cycles and chains are 2/4
- fixc: fixing the good cycles

For the multiple pool simulations:
- none: no collaboration
- indiv-first: consecutive policy
- all: all of the inner arcs are tested
- u: just in the UK inner arcs tested
- n: just in the Netherlands inner arcs tested
- s: just in Spain inner arcs tested
- g: all arcs are tested
