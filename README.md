# Healthcare pathway analysis: optimal matching and classification

This is a research project performed under the supervision of Nicolas Savy, Lecturer-researcher at Toulouse Mathematics Institute (IMT) and Romain Demeulemeester, PhD Student at Toulouse University Hospital Centre (CHU). The result of this project will hopefully be used for the study and determination of stable healthcare pathways for thyroid cancer patients.

## Presentation of our work

Several methods of sequence analysis are implemented using the R software in order to obtain a typology for different pathways.  We also wish to characterize the stability of our clusterings.  

We  perform  our  research  on  an  example dataset from McVicar and Anyadike-Danes (2002) called the MVAD dataset.  It is included in TraMineR, an R package used to discover characteristics of sequential data based on the course of its events.  This dataset originates from a survey that aimed to evaluate the transition from school to work of 712 individuals. It summarizes their monthly activity on a period of 72 months, from July 1993 to June 1999. The  possible  states  for  each  month  were:  ”employment”,  ”joblessness,  “higher  education”,”further education”, ”school” and ”training”.

In this research project, we first conduct an exploratory analysis on our sequential data. Then,  we  perform  a  panel  of  clustering  methods  based  on  the  Optimal  Matching  distance in  order  to  determine  groups  formed  by  the  individuals  and  the  predominant  pathways  of each  group.   Finally,  we  grant  some  time  to  studying  the  stability  of  the  clusters  we  have just formed and finding a global indicator of this stability.  This is a very important aspect because it allows to control these different clusters as well as whether or not the trajectories are representative enough.  We use different techniques from the literature and compare them in order to evaluate their efficiency. 

## Main results (cf. Conclusion)

State Sequence Analysis (SSA) is an effective way to extract a great deal of information from data relating to changes over time at an individual level, such as MVAD’s social data .

Thanks to optimal matching distance, we can build typologies of sequences by applying adapted clustering algorithms like hierarchical clustering or K-medoids algorithm.
Researchers are increasingly focusing on studying the stability of clusters formed by these algorithms. There are various methods and indicators for validation of results obtained by sequence clustering and for determining the optimal number of clusters. In this paper, we have used methods based on resampling without replacement, parametric bootstrapping and Jackknife.

Resampling allows to make a trade-off between the number of clusters and quality of clustering. However, the resampling size should be chosen so as not to change the structure of the data too much.

Parametric boostrap, which is a recent method for determining the optimal number of clusters, has not shown its relevancy in this study.

The jackknife method has allowed us to determine individuals that decrease stability and find which of their other characteristics influenced this behaviour.

Moreover, we have noticed that variation of information is more sensitive to stability than the Rand index. It detects more changes between two compared clusterings.
This study will hopefully help set the basis to constructing stable clusters for patients in healthcare.

To continue this project, we could try defining a method for choosing the costs used in the Optimal Matching algorithm with respect to cluster stability, predict the class of a new sequence based on the closest medoid (for example) and/or find covariates on which could depend clustering results.
