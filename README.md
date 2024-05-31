# LHCb particle classification
The data that we have from the source https://zenodo.org/records/1230552 is from LHC which shows the Compressed PID's from LHC with six classifications ["pion", "electron", "muon", "ghost", "proton", "kaon"] which are denoted here as ["a", "b", "c", "d", "e", "f"], and features are mentioned for each particle based on the readings at LHC. This data is a compressed version of the obscured data from particle identification in PID function of the LHC particle detection process.We have built a classification model here to predict the nature of the particle based on the readings that we receive.
![slide2-l](https://github.com/Neelesh1305/LHCb-particle-classification/assets/113800036/b13033f2-8de4-4391-a270-d3974dce9af7)

The data was trained on many regression models including Linear regression, Randomforest regressor, xgbregressor, fully connected neural networks, convolutional neural networks and recurrent neural networks. Though there is no presence of any time stamps in the data, reshaping the data and feeding it to a LSTM network gave results that are better than any other regression models. We received a test accuracy of around 75% with the rnn model used in the classification modeling.
## Results
The below shown are the results of the rnn model visualised in heatmaps of confusion matrix.
![Unknown-37](https://github.com/Neelesh1305/LHCb-particle-classification/assets/113800036/c8008028-ac80-4b1f-82db-cfa9bc83ce6c)

While the AOC curves pictured below the performance of the model on each particle's classification individually
![Unknown-36](https://github.com/Neelesh1305/LHCb-particle-classification/assets/113800036/f09ac3e4-ce19-462c-852b-261f7fed4fcb)

## References
1. Weisser, C. (2018, April 26). LHCb Particle Identification Compression Challenge. Zenodo. https://doi.org/10.5281/zenodo.1230552
2. Weisser, C. (2021, April 12). weissercn/LHCb_PID_Compression. GitHub. https://github.com/weissercn/LHCb_PID_Compression
3. horace. (2014, September 10). PPT - The readout system for the LHCb Outer Tracker PowerPoint Presentation - ID:4208460. SlideServe. https://www.slideserve.com/horace/the-readout-system-for-the-lhcb-outer-tracker
‌
