# Serial_ID

You need a model saved in ../models.
Download model with "curl -O -J -L https://www.dropbox.com/sh/j3xmli4di1zuv3s/AAArdcPgz7UFxIHUuKNOeKv_a?dl=0&preview=TPS-ResNet-BiLSTM-Attn.pth"

For training, run:

python3 train.py --train_data train_dataset --Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn --saved_model ../models/TPS-ResNet-BiLSTM-Attn.pth --FT --valid_data test_dataset --num_iter 10000 
