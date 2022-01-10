# Final_year_research_project: Healthcare pathway analysis: optimal matching and classification

This is a research project performed under the supervision of Nicolas Savy, Lecturer-researcher at Toulouse Mathematics Institute (IMT) and Romain Demeulemeester, PhD Student at Toulouse University Hospital Centre (CHU). The result of this project will hopefully be used for the study and determination of stable healthcare pathways for thyroid cancer patients.

## Presentation of our work

Several methods of sequence analysis are implemented using the R software in order to obtain a typology for different pathways.  We also wish to characterize the stability of our clusterings.  

We  perform  our  research  on  an  example dataset from McVicar and Anyadike-Danes (2002) called the MVAD dataset.  It is included in TraMineR, an R package used to discover characteristics of sequential data based on the course of its events.  This dataset originates from a survey that aimed to evaluate the transition from school to work of 712 individuals. It summarizes their monthly activity on a period of 72 months, from July 1993 to June 1999. The  possible  states  for  each  month  were:  ”employment”,  ”joblessness,  “higher  education”,”further education”, ”school” and ”training”.

In this research project, we first conduct an exploratory analysis on our sequential data. Then,  we  perform  a  panel  of  clustering  methods  based  on  the  Optimal  Matching  distance in  order  to  determine  groups  formed  by  the  individuals  and  the  predominant  pathways  of each  group.   Finally,  we  grant  some  time  to  studying  the  stability  of  the  clusters  we  have just formed and finding a global indicator of this stability.  This is a very important aspect because it allows to control these different clusters as well as whether or not the trajectories are representative enough.  We use different techniques from the literature and compare them in order to evaluate their efficiency. 
