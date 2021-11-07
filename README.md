# Neural_Network_Charity_Analysis

## Overview

Use Machine Learning and Neural Networks to analyze a set of charity data to determine success rates of organizations that are funded by Alphabet Soup. 

## Results

### Data Preprocessing
- What variables are considered the target for your model? IS_SUCCESSFUL was a key indicator in this
- What variables are considered to be the features for your model? Variables such as APPLICATION_TYPE, AFFILIATION, etc. 
- What variables are neither targets nor features, and should be removed from the input data? In the initial preprocessing, EIN and NAME were removed since identifiers truly don't impact this analysis, or at least, shouldn't.

### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why? I first selected 15 (layer1) and 5 (layer2) which ended up having the highest accuracy, most likely due to the removal of certain columns, but still. I used 2 layers and relu and sigmoid for activation functions.
- Were you able to achieve the target model performance? My first, non-optimized, model hit a 72.6% accuracy. The optimizations actually did the opposite. Unfortunately, that makes this answer a no. 
- What steps did you take to try and increase model performance? I removed columns that at a high-level looked erroneous, but I was wrong in this assumption. SPECIAL_CONSIDERATIONS, AFFILIATION, and ORGANIZATION were all removed, but I think if I were to dive back into this, I would have narrowed down less on the AFFILIATION because I think this was the removal problem. Actually, I want to run this back with the original neuron count and test this. BRB. Back ot 72.1%. AFFILIATION definitely is a key factor in this machine learning analysis because of the relationship it has with the key values here.

## Summary
Things that I found semi-circumstantial evidence to support would be that the data source needs to be all-encompassing of the connections in how data impacts each other. Thinking about the AFFILIATION removal, and then putting it back in, how it improved the accuracy by almost > 10% shows that this is paramount in being accurate. Diving into hidden_node_layers might be something to do externally, but given the dataset we were provided, I truly think making impactful connections from a logical perspective are the most important factor in creating an accurate model.
