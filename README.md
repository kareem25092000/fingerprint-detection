- this project is to build AI model that takes a group of fingerprints and add the feature vector for every id to the system under the id for that person as for later you can see if the fingerprint for that person already exsist or not .
- so there are two mods for the system :
  1 ) add fingerprints
  2 ) find if a fingerprints exsist or not
- the model is a CNN classifier and the feature vector is the output of the CNN-part (head of the network)
- the comparison that leads to see if a fingerprints exsist or not is by taking the euclidean distance of the feature vector of the input image to the exsisting feature vectors to see if it belongs or not and the minimum distance that is less than a threshold is the match
- every id has five potential fingerprints (regards left or right hand):
  1 ) thumb finger
  2 ) little finger
  3 ) middle finger
  4 ) index finger
  5 ) ring finger
- if the classifier outputs a classification less than 0.7 then the image can't be classified
- the data that been used is on kaggle : <https://www.kaggle.com/datasets/ruizgara/socofing>
- the code that is on kaggle : <https://www.kaggle.com/code/kareemalmamlouk/fingerprint-detection>
