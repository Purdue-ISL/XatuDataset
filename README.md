# Video session data used to evaluate Xatu

This dataset contains video session data used to evaluate the Xatu system. If you use this dataset, please cite our paper:

Y. Nam, J. Gao, C. Bothra, E. Ghabashneh, S. Rao, B. Ribeiro, J. Zhan, H. Zhang: "Xatu: Richer Neural Network Based Prediction for Video Streaming", in ACM SIGMETRICS 2022.

# Overview:

The dataset contains information for 20996 video sessions. The MetaInfo.txt file contains the meta information regarding each session. Session\<ID\>.txt contains the information about the chunks in each session. The session\<ID\>.txt files are present in the SessionInfo directory.

# MetaInfo.txt 
(the fields in each line are comma separated values.)

* Session ID (an anonymized ID generated by us as described above which identifies a session)
* CDN ID (anonymized ID which describes which CDN the session is served by)
* ISP ID  (anonymized ID which describes which ISP the session is served by)
* City ID (anonymized ID which describes which city the session corresponds to)
* Day and hour  (Integers that denote which day since the start of data collection that the session started at, and which hour. E.g., Day = 39, and  Hour = 16 means the session started at hour 16 on Day 39. Hour is an integer between 0 and 23).

# Session\<ID\>.txt 
(the fields in each line are comma separated values.)

* Chunk ID (an integer that goes as 1, 2, 3,.. corresponding to which video chunk we are referring to).
* Download start time (d_start): Time when the download of i_th chunk starts in seconds.
* Download end time (d_end): Time when the download of i_th chunk ended in seconds.
* Bandwidth (bw) of i_th chunk download in MegaByte per second.
* Time to first byte (ttfb): Time to get the first byte of i_th chunk in seconds.
* Chunk size (size): Size of i_th chunk in MegaBytes.

# Contact
For any questions, please contact Chandan Bothra (cbothra@purdue.edu) and Sanjay Rao (sanjay@ecn.purdue.edu).
