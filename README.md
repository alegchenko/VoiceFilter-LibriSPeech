# VoiceFilter-LibriSPeech
Pytorch model for voice filtering trained with LibriSpeech

### Download Checkpoints:
                                                                
1)Embedder chkpt: https://drive.google.com/file/d/1LCdZNsvx6BEzVzy50BSCRAtvbrZtE6sV/view?usp=sharing

2)Filter chkpt(mse loss, train 1000h on LS 61k epochs, 8 days with gtx 1080ti) Google Drive: https://drive.google.com/file/d/1RRDGBFnyL5po1VXpkfJ_yRQryZ6fEWPW/view?usp=sharing

Examples for this checkpoint are in lib "Dialogs test"

After downloading both chkpts you can try system:
```
python3 inf.py -c [config yaml] -e [path of embedder pt file] --checkpoint_path [path of chkpt pt file] -m [path of mixed wav file] -r [path of reference wav file] -o [output directory]
```

Train history:
![Снимок экрана от 2021-06-27 16-23-12](https://user-images.githubusercontent.com/68243701/123599088-6a10be00-d81f-11eb-89b0-5eea4bcb6e95.jpg)
