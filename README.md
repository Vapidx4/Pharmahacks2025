# Pharmahacks-25

Our submission for Pharmahacks 2025

We decided to work on Multiple Sequence Alignment (MSA) Challenge provided from McGill AntibioticMicrobial Resistence (AMR)

MSA is a critical bioinformatics task used to analyze similarities and differences across DNA, RNA, or protein sequences. This challenge is inspired by the leverages data from Borderlands Science (BLS)—a citizen science game that has collected millions of player-generated solutions to small-scale MSA problems.

# Project Goals
	1.	Leverage Player-Generated Data
Use the unique dataset from Borderlands Science, which consists of alignment solutions crowdsourced from thousands of players.

	2.	Develop Predictive Models
Build and refine models capable of predicting optimal alignment moves, enhancing the performance of computational MSA methods.

	3.	Advance MSA Techniques
Improve the accuracy and efficiency of MSA algorithms by incorporating insights gained from human solutions.

# Methods

In our code, we decided to use the DeepQ machine learning algorithm as this method uses reinforcement learning which seemed ideal for our specific challenge. 
After setting up overall strucuture of the AI model, several extra considerations were implemented based on trends found in the data. A heatmap of the frequency of gap insertions in the puzzles was generated allowing us to understand which sequence indexes were most common. This knowledge was then implemented in our code by affecting the action step and slightly nudging the values towards more common actions. The most common changes in sequences were also generated, allowing us to consider this new data in our model using the same method as mentioned above. 

With the provided training dataset, our model achieved an accuracy score of around 93%. 
