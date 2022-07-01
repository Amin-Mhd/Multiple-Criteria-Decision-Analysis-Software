# Multiple Criteria Decision Analysis Software
Multiple Criteria Decision Analysis is one of the most popular problems in the globe due to its wide application in real-life situtations. Buying a new car, selecting appropriate supplier for a company, etc. can be defined as Multiple Criteria Decision Analysis problem. There are several methods to solve Multiple Criteria Decision Analysis problems yet the [Ordinal Priority Approach (OPA)](https://ordinalpriorityapproach.com/) is one of the most recent MCDA methods. 

## Ordinal Priority Approach (OPA)

The Ordinal Priority Approach is a novel Multiple Criteria Decision Analysis method which works based on the ordinal data. It can calculate the weights of experts, criteria, and alternatives at the same time. The OPA believes that human cannot provide precise values for comparing the experts, criteria, and alternatives. Therefore, using the preferences can be helpful to solve the problem. There are several types of solver for the Ordinal Priority Approach, including [Web-Based](https://ordinalpriorityapproach.com/opasolver.html), [Excel-Based](https://zenodo.org/record/4453887), [Matlab-Based](https://www.mathworks.com/matlabcentral/fileexchange/106890-opa-solver-a-solver-for-multi-criteria-decision-analysis). However, we are going to implement the OPA into the LINGO software here. The important papers on the OPA can be found [here](https://ordinalpriorityapproach.com/index.php?s=2-opa-papers). The LINGO software can be downloaded from [here](https://www.lindo.com/lindoforms/downlingo.html).  

### Example 1: Individual Decision Making
Here, we aim to buy a new car based on some pre-defined criteria. The decision problem is shown on the following figure:

![This is an image](https://ordinalpriorityapproach.com/images/7.jpg)

The expert believes that the preference of the criteria are as follows:

P > S > G > F

Moreover, the expert suggested the following preference for each car in each criterion:

In criterion P : A > C > B

In criterion S : C > A > B

In criterion G : B > C > A

In criterion F : B > A > C

Since there is one expert, the problem is individual decision-making. Therefore, in the **1-Individual Decision-Making.lg4**, we define the criteria, and alternatives as follows:

```
sets:

Experts/E/:Experts_color,W_Experts;
Criteria/G S P F/:W_Criteria;
Alternatives/A B C/:W_Alternatives;
Experts_Criteria(Experts,Criteria):Criteria_color;
Experts_Criteria_Alternatives(Experts,Criteria,Alternatives):Alternatives_color,W;
Experts_Alternatives(Experts,Alternatives);
Criteria_Alternatives(Criteria,Alternatives);

endsets
```

### Example 2: Group Decision Making
typing...
### Example 3: Calculate the weight of the criteria
typing...
