# VoiceFilter-LibriSPeech
Pytorch model for voice filtering trained with LibriSpeech
                                                                
Embedder chkpt: https://drive.google.com/file/d/1LCdZNsvx6BEzVzy50BSCRAtvbrZtE6sV/view?usp=sharing
Filter chkpt(mse loss, train 1000h on LS 61k epochs, 8 days with gtx 1080ti) Google Drive: https://drive.google.com/file/d/1RRDGBFnyL5po1VXpkfJ_yRQryZ6fEWPW/view?usp=sharing

Examples for this checkpoint are in lib "Dialogs test"

You can try system like this:
"python3 inf.py -c [config yaml] -e [path of embedder pt file] --checkpoint_path [path of chkpt pt file] -m [path of mixed wav file] -r [path of reference wav file] -o [output directory] "
