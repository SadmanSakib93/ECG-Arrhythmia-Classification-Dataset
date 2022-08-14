# **ECG-Arrhythmia-Classification-Dataset**
### **Link to the Dataset**
https://www.kaggle.com/datasets/sadmansakib7/ecg-arrhythmia-classification-dataset

### **Context**
The dataset contains features extracted two-lead ECG signal (lead II, V) from the MIT-BIH Arrhythmia dataset (Physionet). In addition, we have programmatically extracted relevant features from ECG signals to classify regular/irregular heartbeats.
[Link from PhysioNet](https://physionet.org/content/mitdb/1.0.0/). The dataset can be used to classify heartbeats for arrhythmia detection.  


### **Content**
Brief details of the dataset are as follows:
There are four ECG arrhythmia datasets in here, each employing 2-lead ECG features. Datasets obtained from PhysioNet are [MIT-BIH Supraventricular Arrhythmia Database](https://physionet.org/content/svdb/1.0.0/), [MIT-BIH Arrhythmia Database](https://physionet.org/content/mitdb/1.0.0/), [St Petersburg INCART 12-lead Arrhythmia Database](https://physionet.org/content/incartdb/1.0.0/), and [Sudden Cardiac Death Holter Database](https://physionet.org/content/sddb/1.0.0/).
2. In each of the datasets, the first column, named "record" is the name of the subject/patient.
3. Each data contain five classes/categories: N (Normal), S (Supraventricular ectopic beat), V (Ventricular ectopic beat), F (Fusion beat), and Q (Unknown beat). The column "type" contains the class information.
4. The remaining 34 columns contain 17 features for each ECG lead (17 features for lead-II and 17 features for lead-V5)
5. The short description of the features for all four datasets can be found in the following figure. Note that the features are consistent across all four datasets to be comparable when applying Machine Learning models.
|          Feature Group         	|     Lead A and B    	
|:------------------------------:	|:-------------------:	
|          RR Intervals          	|      Average RR     	
|                                	|          RR         	
|                                	|       Post RR       	
|  Heartbeat Intervals features  	|     PQ Interval     	
|                                	|     QT Interval     	
|                                	|     ST Interval     	
|                                	|     QRS Duration    	
| Heart beats amplitude features 	|        P peak       	
|                                	|        T peak       	
|                                	|        R peak       	
|                                	|        S peak       	
|                                	|        Q peak       	
|       Morphology features      	| QRS morph feature 0 	
|                                	| QRS morph feature 1 	
|                                	| QRS morph feature 2 	
|                                	| QRS morph feature 3 	
|                                	| QRS morph feature 4 	
6. Please refer to the following paper for details of each feature and the methodology followed to generate these features from raw ECG data:
[Harnessing Artificial Intelligence for Secure ECG Analytics at the Edge for Cardiac Arrhythmia Classification](https://www.taylorfrancis.com/chapters/edit/10.1201/9781003028635-11/harnessing-artificial-intelligence-secure-ecg-analytics-edge-cardiac-arrhythmia-classification-sadman-sakib-mostafa-fouda-zubair-md-fadlullah)


### **Acknowledgements**

- When using this dataset, please cite the [original paper](http://ecg.mit.edu/george/publications/mitdb-embs-2001.pdf).
- Also, please cite [this paper](https://www.taylorfrancis.com/chapters/edit/10.1201/9781003028635-11/harnessing-artificial-intelligence-secure-ecg-analytics-edge-cardiac-arrhythmia-classification-sadman-sakib-mostafa-fouda-zubair-md-fadlullah) as this is the work that demonstrated the feature extraction phase from the original dataset.
- Might want to checkout [another relevant paper](https://ieeexplore.ieee.org/abstract/document/9344639).


### **Inspiration**

The inspiration of this dataset is to help the research community to build proof-of-concept machine learning-based models for arrhythmia detection. However, this dataset is for experimental simulation only and may not be suitable for production-ready models to treat hospital patients.
