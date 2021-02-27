# Serial_ID

You need a model saved in ../models.

For training, run:

python3 train.py --train_data train_dataset --Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn --saved_model ../models/TPS-ResNet-BiLSTM-Attn.pth --FT --valid_data test_dataset --num_iter 10000 
