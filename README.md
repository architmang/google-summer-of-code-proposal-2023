# Google Summer of Code 2023

## [Organization: Red Hen Lab](https://www.redhenlab.org/home)
## Project Title:   Multimodal stance detection

### Project Description
While most Americans still obtain their news through television, this remains one of the understudied aspects of the information ecosystem. Although network news consumption has declined, cable news stations account for an increasing percentage of American television viewing. It is important to understand not only what stations people are consuming, but also what these stations are creating. Recent studies have shown that small differences in wording influence study participants to view certain groups as socially distant and less human. Even biased information—not necessarily extreme—can have real-world impacts ranging from micro-aggression and harassment to more serious violence. 

It is unclear how prevalent biases are among the three major cable news networks, FNC, CNN, and MSNBC. For instance, the study will investigate whether FNC is more likely to promote, neutralize, or debunk pro-gun control arguments over anti-gun control arguments compared with CNN. We propose to develop a stance detection method for television news programs using multimodal data. We focuse on topics: gun control, abortion, immigration, and covid/vaccination at the stance level, i.e., promoting, neutralizing, or debunking. 

<p align="center">
![image](https://user-images.githubusercontent.com/75172544/230663224-306df3f1-16c0-45f1-b1c5-ec0b7e5a9164.png)
</p>

A news program may cover more than one story, but the stance may vary from story to story. Thus, we divide a news program into segments consisting of coherent stories. We can perform stance detection on a topic-by-topic basis (or story-by-story) once we have identified consecutive sentences relating to the same topic using mixture topic models. The use of text, while useful for dividing a news program into segments of coherent stories, can be insufficient to capture stance, as much of the signal is transmitted via audio and image (facial expressions). We will hand code a limited set of videos that are intended to promote, neutralize, or debunk the topics under study. In light of the fact that manual coding is an expensive and time-consuming process, we use a small sample of annotated videos utilizing weak-supervised and unsupervised methods. We develop an embedding that incorporates both image and audio to develop a joint low-dimension representation of the data. Developing a deep variational autoencoder, we minimize the reconstruction error for images and audio jointly. Lastly, the embedding space data points will be used as inputs to weak-supervised and unsupervised models that infer the stance of a story.

### Project Summary
In this project, I propose to develop a stance detection method for television news using multimodal data. I will focus on the topics of gun control, abortion, immigration, and covid/vaccination at the stance level, i.e., promoting, neutralizing, or debunking. I will use a combination of segmentation, annotation, feature extraction, and supervised and unsupervised models to perform stance detection. I will evaluate the performance of our models using standard evaluation metrics and analyze the impact of different features on the performance of the models. I will also address ethical considerations such as bias and fairness in our approach. The proposed method will provide valuable insights into the prevalence of biases in cable news networks
