# Project: ClimSim - Machine Learning for Climate Modeling


### [Full Project Description](doc/project3_desc.md)

<img src="https://leap-stc.github.io/ClimSim/_images/fig_1.png" alt="climsim" width="300"/>

Term: Fall 2023

+ Team 3
+ Team members
	+ Noreen Mayat
 	+ Miao Zhang
	+ Jason Cho
	+ Stephanie Shu
	+ Yihan Zhang 

+ **Project summary and goals:** In this project, we sought to help the ClimSim project by addressing the following questions through our exploration:
	+ Is the ClimSim GitHub repo with its associated "quick start" guide and demo notebooks set up in a way to provide data scientists an easy entryway to play with the data set and contribute ideas?
	+ Could one use collaborative cloud-based notebooks such as Google Colab or Huggingface Spaces to explore the dataset's numerous files on Huggingface?
	+ What data selection, visualizations and/or processing workflows could be created so that one could apply various ML/DL models on some aspects of the ClimSim data? This is especially interesting given the dataset is already on Huggingface, which hosts a large number of models for NLP and computer vision.
	+ What advanced ML/DL models could be applied to the ClimSim data set to improve the evaluation metrics?

+ **Findings:**
	+ We used a Zero-Inflated Poisson Model.
 	+ We chose this model because our data distirbution had an excess number of zeroes.
  		+ This model was more accurate for snow than for rain based on MAE scores.
  	+ PCA Dimension Reduction did not improve model performance.
  	+ We also used EN model as baseline to run other models.
  	+ Trained our own CNN model → accuracy of 0.9757
  	+ Other models we explored were: 2D CNN, MLP, ResNet.
  		+ 2D-CNN accuracy: 0.9541
  		+ MLP accuracy: 0.9639
  	+ Based on performance metrics (ex. RMSE, R2, MAE scores) we found 2D-CNN to have the best results. 

**Contribution statement**: ([default](doc/a_note_on_contributions.md)) We met to analyze our exploratory analysis and decided as a group on the zero-inflated Poisson model. Miao and Yihan, Jason, and Stephanie ran models on Google Colab. These were shared with the team. Miao merged these notebooks into one. Noreen reviewed and interpreted the model results, worked on the presentation slides, and organized the Github. All team members contributed equally in all stages of this project. All team members approve our work presented in this GitHub repository including this contributions statement.

Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
