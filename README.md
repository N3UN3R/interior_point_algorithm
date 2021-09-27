# interior_point_algorithm
This repository contains an implementation of an interior point algorithm for p2p elcectricity trading


getHouseholdData.py
- contains functions that generates list of currently
  active households and python dictionarys for current
  supply and demand values of producer and consumer households

currentlyActiveCostDict.py
- builds a cost-dictionary for all currently active households
  and ensures the needed format


constraintMatrix.py
- contains functions that build the needed constraints for
  the linear programming problem

orderedDemandSupplyValues.py
-  ensures that the order of the constraints and the supply
   and the demand dictionaries is the same


interior_point_algorithm.py
-  runs the interior-point algorithm
-  builds the objective function
-  analyses if demand > supply, demand < supply or demand = supply
-  builds righthandside constraints b
-  ensures proportional fairness
