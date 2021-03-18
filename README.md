# Serial_ID

You need a model saved in ../models.

Download model with:

"curl -O -J -L https://ucb7de9e4bd6cc37865dca9a8065.dl.dropboxusercontent.com/cd/0/get/BK5rZSRqxbaZIZqVR-XQh7cZcLir-VpQQZFVC50lAUdsNed1gZ4m4NU4EmAznEyIu3z1GF8gBqs2Yr94gD4rXe9AdlfJfTVziGHYKQQ_49nx7MGbQmp09fmJXb13n0fwcz1Q404gpiAeK8oBLRiQ33FM/file?_download_id=662644634291795749989267350354416283216104673969856066319626059823&_notify_domain=www.dropbox.com&dl=1"

For training, run:

python3 train.py --train_data train_dataset --Transformation TPS --FeatureExtraction ResNet --SequenceModeling BiLSTM --Prediction Attn --saved_model ../models/TPS-ResNet-BiLSTM-Attn.pth --FT --valid_data test_dataset --num_iter 10000 
