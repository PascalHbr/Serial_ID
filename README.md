# Serial_ID

You need a model saved in ../models.
Download model with "curl -O -J -L https://uc013f5ffb678053875b37808008.dl.dropboxusercontent.com/cd/0/get/BJx6ipg83PDVASxctfD5-iN3SoWGOGso_Sm4Le_NIESchoGyKFlXUNRuN3Tk9IL-bX-rYSLRhvJ76vKZeW_zRISU7S2kTeQ0eDMYYQ5SWRB_G_Ixm9idWPFFHEzC0b9_ez0/file?_download_id=311912871436862752273396724680060220893539963916345488061336430886&_notify_domain=www.dropbox.com&dl=1"

For training, run:

python3 train.py --train_data train_dataset --Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn --saved_model ../models/TPS-ResNet-BiLSTM-Attn.pth --FT --valid_data test_dataset --num_iter 10000 
