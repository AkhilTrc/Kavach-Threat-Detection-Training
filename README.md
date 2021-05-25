# Kavach-Threat-Detection-Prediction
Code for Generalized Threat Detection from Network traffic data (NSL-KDD), implemented using Convolutional Neural Network.

## Dataset
- Latest version of the NSL-KDD Cybersecurity Malicious-attack Network data:
1. KDDTrain+  - Training Data - Size (125973, 43)
2. KDDTest+   - Testing Data  - Size (22544, 43)
3. KDDTest-21 - Unseen Testing Data - Size (11850, 43)

## CNN Model Details
- This Convolutional Neural Network Model s designed to encompass the features and Data spread of the NSL-KDD Dataset. 
Consisting Network Server type labels, Packet Flag type labels, Network Protocol Type labels and dozens of other features 
which references Public Network traffic. Dataset references the Binary/Multi-class attack type labels for training purposes. 

- Training input set in the Comma Separated Vector (csv) format. 
- NSL-KDD Dataset pre-processing done accord to fitting the model. 

## CNN Model Training
- Feed pre-processed dataset into CNN model. 
- Using Crossvalidation and Train-Test split to train the model. 
- Model fit and Crossvalidated for 100 Epochs on a batch size of 128.

## Output
- Predicted output generated in Pandas DataFrame format and saved in system as a Comma Separated Vector (csv) file.

## Further Procedures
- Generated csv file is sent to the Cybersecurity team to exert appropriate counter-measures based on the Threat level and type forcasted.
