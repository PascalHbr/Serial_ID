# Serial_ID

You need a model saved in ../models.

Download model with:

"curl -O -J -L https://uc97f437ebc03c4a4491dfe64421.dl.dropboxusercontent.com/cd/0/get/BKEogRzGEL3xm6woeJB_M8u1CdZcwBpgQj78RVGU7xu1exFL2o5zeknr9WC3EG8XgG_0nuwCwA7uOjGMhwycmrbzRFBoUwEl4FOnMXmTEZNmcaSuecevEadFSKTMtFlMg6muDDqCaDpQZmvfglz6qDCO/file?_download_id=14030996444504784793725676232234883445768887723076994877840363146&_notify_domain=www.dropbox.com&dl=1"

For training, run:

python3 train.py --train_data train_dataset --Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn --saved_model ../models/TPS-ResNet-BiLSTM-Attn.pth --FT --valid_data test_dataset --num_iter 10000 
