# Anti-Cancer_Drug_Activity_Prediction

Problem Definition:

It is a binary classification problem based on the graph data.
The task is to predict the anticancer activity of a chemical compound using the chemical structure of the compound.
The chemical compound can be positive or negative against lung cancer cell and thus labelled as either 0 or 1.

the data input and output:-

The data is in the form of graph which represents the chemical structure of the compound.
Each sample of data contains information about the atoms and the connections between atoms of the molecule.
So in this problem the features are the atoms and connections.
The input file is structure data file (SDF). It contains information about the chemical composition of a molecule. SDF file store information about position of individual atom in the chemical compound and also tells about the connections.


in this project, I used different trials like:

* change the "message_calculation_class" = 'GGNN' Compute new graph states by neural message passing and gated units on the nodes
* added hyperparameters num_edge_MLP_hidden_layers by 16 and use message_calculation_class" = 'RGCN' 
* used "message_calculation_class"= "RGAT" and hidden_dim by 32 and num_heads by 32 and after i check the accurracy and validation accuracy,
* change in "message_calculation_class"] = 'RGIN' and change in another hyperparameaters

data graph as it is "unbalanced" and with Balanced 
