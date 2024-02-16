# Cancer-type-prediction-with-GNN
### Implement a GNN to classify breast cancer patients in LUMINAL A / Luminal B 
#### The Data
The dataset consists of 100 patients. 
For each, we have the full gene expression levels as input (1022 features) and a label consisting of the patient breast cancer subtype: 
LUMINAL A or LUMINAL B.

#### Graph Representation
Firts, the dataset is represented with a Graph (network) where: 
1. Each network node corresponds to a patient
2. For each node (patient) the feature vector is the entire gene expression profile of the patient
3. Node labels are the patient class (Luminal A/ Luminal B)
4. Since edges are not provided, they are computed using Pearson correlation coefficient.

#### Task
The aim is to predict node labels. This is done:
1. With MLP
2. With GCN (Graph Convolution Network)
3. With GAT (Graph Attention Network)

