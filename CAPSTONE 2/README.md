# BEHOLDER - Attractiveness in Human Faces

In this experiment we implemented a new broad benchmark dataset called BEHOLDER to achieve multiparadigm analysis of facial attractiveness. The dataset has a total of over 8,000 frontal face images with varied characteristics (sex, race, ages) and a broadly generalized attractiveness score averaged over at least 15 ratings from other humans. 

Benchmark analysis was performed for the beauty scores, and the data reveals the efficacy of CNN networks for this type of problem. The experiment results in a model that can be run against any human face, male or female, and will return an accurate (according to other humans) representation of its attractiveness. However, the limitations are a posed face, either smiling or resting, a simple background, and a straight neutral angle facing the camera head-on. 
These are limitations that can be worked around by enriching the images with random rotations, saturations, crops and other manipulations that could be a continuation of the work presented herein.

Because the BEHOLDER dataset generation is designed for multi-paradigm implementations, our work can be tailored to various models for specific functions, such as appearance-based or shape-based facial image classification / regression / ranking. 
The BEHOLDER dataset was tested using various combinations of features, predictors and deep learning models, where the tests show the precision of the data collection. We only presented the best results achieved across the experimentation.
