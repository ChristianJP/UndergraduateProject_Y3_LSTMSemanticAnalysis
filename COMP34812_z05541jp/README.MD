# Using Deep Learning Models to Analyse Investors’ Bearishness and Bullishness in Communities Behind NFTs


Data for training and testing was acquired from Discord using Discord chat exporter:
https://github.com/Tyrrrz/DiscordChatExporter/wiki/GUI%2C-CLI-and-Formats-explained

The chats were exported from 4 different Discord servers:
1. Dented Feels
2. Degen Toonz
3. Cosmic Cats
4. Cosmodinos

The floor talk chat was exported since conversations about prices occur there. The labelled data used for BERT & LSTM model can be found:
1. Dented Feels: https://drive.google.com/file/d/1Q5uEe5EEoAR6TrqIrAZ-tN3F2st1zkMb/view?usp=sharing
2. Degen Toonz: https://drive.google.com/file/d/1fk_XPRx6pv8eRuMCQdg-WQOyIRLu6ZuR/view?usp=sharing
3. Cosmic Cats: https://drive.google.com/file/d/18u3Am4ocfBZg6tsZAylk1p2pL0Rqg38L/view?usp=sharing
4. Cosmodinos: https://drive.google.com/file/d/190BUHsOtboEhdO1yZLjoNW1jljk8Wlpa/view?usp=sharing


Two models were developed to perform the classifcation:
1. Bi-directional LSTM Recurrent Neural Network (RNN)
2. BERT (transformer) based model

The code for training the models is in the notebooks in ./notebooks folder.

Saved models are available on the cloud:
1. LSTM: https://drive.google.com/file/d/1-2e6jWnsAS1Tq-7x4pQTgxG-LlheGvR8/view?usp=sharing
2. BERT: https://drive.google.com/file/d/1-5_xk4wkbrYlmf3jBxM1uTnOSvg9mkAO/view?usp=sharing


The models shown here are trained on Discord NFT Community messages, and can infer semantics between 
the categories  of 'Bearish' and 'Bullish' from un-seen data - shown in the demo notebooks.
This follows our original objective, in designing a soloution to understanding the overall emotion of NFT communities.  
This analysis can be done on multiple messages in a community in order to quantify overall levels of 'Bearish' or 'Bullish'.