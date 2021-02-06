# particle-identification
Data source:
https://archive.ics.uci.edu/ml/datasets/MiniBooNE+particle+identification

Made for a machine learning course as part of my data science certificate, this project uses data consisting of 50 features of 150K measured signals, identifying each signal as a neutrino particle or as background noise.

Neutrinos are very difficult to detect since they interact very little with matter, and require very large and sensitive detectors. The more sensitive an instrument, the more background noise, so correctly identifying signals allows scientists to pull meaningful information from large and noisy datasets. 

The first row of our data has two values, the number of neutrino signals and the number of background events. Below that we have the neutrino rows and then the background rows, both with 50 features. Not much feature transformation here, so this project compares the performance of two models: a random forest classifier and a neural network classifier

The labels of our dataset are either signal or background, and so this is a binary classification problem. The performance of both models were measured using their accuracy. Both models were pretty accurate, with the random forest classifier at 93.68% and the neural network at 94.92%, but training the neural network model was much, much quicker and required less lines of code, making it more practical to use and therefore my recommendation to use in order to label data from neutrino detectors.
