# An Introduction
We will investigate the neural substrate of decision making by analyzing the neural activity during a mouse behavioral task. In the task, mice are required to choose between two stimuli while neural activity is recorded using Neuropixel probes, a type of high-density electrophysiological recording tool. We will train a decoder to predict the choice of the mouse from neural activity obtained from 42 brain regions, that include cortical and subcortical areas like basal ganglia, hippocampus, thalamus, visual and frontal cortex. We hypothesize that (1) population activity from the supplementary motor (M2) cortex will have the highest predictive power regarding the choice of all the brain regions, because this brain area is known for contributing to control of movement. (2) We predict that a time-window shortly before the response onset will allow our model to predict the response of the mouse with higher accuracy, because the decision to move would manifest a little earlier than the response. To investigate 1 we will use a machine learning approach comparing different supervised learning algorithms like XGBoost, Gradient boosting, Naive Bayes. These models will learn some parameters of the data available that will be used in order to map different activities with different responses. To investigate 2 we will divide the signal into different time-windows relative to the events in the experiment (stimulus onset, response) to see when the upcoming choices are modeled with greater accuracy. The results obtained by these methods will allow us to respond to our research questions concerning the relevant neuronal activity during the decision making process.
Keywords:
Steinmetz, Single neuronCognitive Process,Decision Making,Dimensionality reduction,Machine learning, Classification problem, Neuropixel.
# Research Questions
Is a time-window is more important for predicting the response with more accuracy? 
![image](https://user-images.githubusercontent.com/12738794/127223424-34543ee1-89fb-4d30-ae8b-b1788dd6cd9b.png)



# Dataset
Neuropixels recordings during visual discrimination from Steinmetz et al 2019. Also accessible in Neurodata Without Borders (NWB) format here and via the Open Neurophysiology Environment (ONE) interface here.
Recordings with eight Neuropixels simultaneously during spontaneous behavior from Stringer, Pachitariu, et al 2019.
An example dataset recorded with a Neuropixels probe, with original raw data available.
An example dataset recorded with two Neuropixels probes, from Jun, Steinmetz, Siegle, Denman, Bauza, Barbarits, Lee, et al 2017.

### Neurons 

| Name  | Description | Notes |
| ------------- | ------------- | ------------ |
| [Steinmetz ](https://github.com/nsteinme/steinmetz-et-al-2019) | mice recordings of Neuropixel. Also accessible in Neurodata Without Borders (NWB) format here and via the Open Neurophysiology Environment (ONE) . | Includes a PyTorch dataloaders for classification.  |


