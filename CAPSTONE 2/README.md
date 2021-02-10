# BEHOLDER - Attractiveness in Human Faces

In this experiment we implemented a new broad benchmark dataset called BEHOLDER to achieve multiparadigm analysis of facial attractiveness. The dataset has a total of over 8,000 frontal face images with varied characteristics (sex, race, ages) and a broadly generalized attractiveness score averaged over at least 15 ratings from other humans. 

Benchmark analysis was performed for the beauty scores, and the data reveals the efficacy of CNN networks for this type of problem. The experiment results in a model that can be run against any human face, male or female, and will return an accurate (according to other humans) representation of its attractiveness. However, the limitations are a posed face, either smiling or resting, a simple background, and a straight neutral angle facing the camera head-on. 
These are limitations that can be worked around by enriching the images with random rotations, saturations, crops and other manipulations that could be a continuation of the work presented herein.

## Introduction

Appraisal of facial attractiveness seems natural to humans, but an actual definition of facial beauty remains elusive. Lately, human attractiveness prediction projects, which intend to achieve an automatic, human-consistent, facial attraction evaluation through a computational model, are becoming increasingly popular in pattern recognition and machining learning groups. It has potential use in facial makeup, image recapture, esthetic surgery and more. 

From the computational point of view, attractiveness prediction remains a challenging problem. Numerous data-driven models were implemented in this experiment to tackle this issue.

## Data Sources

The data set was acquired from open and private sources. The first set was retrieved from the SCUT-FBP5500 dataset. Dubbed ‘SCUT-5500’ or ‘SCUT’, it includes face attractiveness ratings of 5,500 young men and women of Asian and Caucasian ethnicity. All the images are labelled with beauty scores ranging from [1, 5] by a total of 60 volunteers.

The second dataset is the London Face Research Lab dataset that’s publicly available. Images were taken in London, UK, in April 2012. Attractiveness ratings, on a [1-7] scale for 2513 people (ages 17-90).

The third set is the 10k Adult Faces Database. This database contains 10,168 natural face photographs and several features for 2,222 of the faces, including attractiveness ratings by peers.

## Model

Run in google colab due to lack of local resources, we applied a transfer learning technique to build upon one of the best performing CNN architectures at the time of writing. NASNet-Large with the famous ‘imagenet’ weights will be our foundation.

## Discussion

Because the BEHOLDER dataset generation is designed for multi-paradigm implementations, our work can be tailored to various models for specific functions, such as appearance-based or shape-based facial image classification / regression / ranking. 
The BEHOLDER dataset was tested using various combinations of features, predictors and deep learning models, where the tests show the precision of the data collection. We only presented the best results achieved across the experimentation.
