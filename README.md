# SCUT-EPT_Dataset_Release

The SCUT-EPT Dataset for the research of offline handwritten Chinese text recognition (HCTR) in educational documents is now released by Deep Leaning and Visual Computing Lab of South China University of Technology. The dataset can be downloaded through the following link:

- [Baidu Cloud](https://pan.baidu.com/s/1h4d1ogn_MAnE_X0LNHowYg)  (Password : bk3x , Size = 1.08GB)
- [OneDrive](https://1drv.ms/u/s!AlPCATpK8Ix6aQ2mqpavf5rXLWI) 

Note: The SCUT-EPT dataset can only be used for non-commercial research purpose. For scholars or organization who wants to use the SCUT-EPT database, please first fill in this [Application Form](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/Application_Form/Application_Form_for_Using_SCUT-EPT_2019.doc) and send it via email to us (eelwjin@scut.edu.cn, or lianwen.jin@gmail.com). When submiting the application form to us, please list or attached 1-2 of your publications in recent 6 years to indicate that you (or your team) do research in the related research fields of OCR, handwriting analysis and recognition, document image processing. At present, this dataset is only freely open to scholars in the above-mentioned fields. We will give you the decompression password after your letter has been received and approved. 

For any person/institute/company who do not works in the field of OCR or document analysis and recognition, please contact us to obtain a commercial license. 

## Description

The SCUT-EPT Dataset contains 50,000 text line images, including 40,000 for training and 10,000 for testing, selected from examination papers of 2,986 volunteers. In addition to the common problems in HCTR, Dataset SCUT-EPT also encounters novel challenges in examination paper, including character erasure, text line supplement, character/phrase switching, noised background, nonuniform word size and unbalanced text length, as shown in **Figure 4**. 
**Character erasure**, also known as crossed-outs, often accompanies with crossed lines to strike out characters;
**Text line supplement** occurs with additional text line supplement appearing below or above the normal text line;
**Character/phrase switching** is the phenomenon where writers add special symbols to switch relevant written characters or phrases for better understanding;
**Noised background** refers to underlines below characters, dense grids between characters, etc. in contrast to most of the handwritten datasets whose backgrounds are very clean;
**Nonuniform word size** refers to the nonuniform word size of characters, especially when comparing Chinese character with digit, letter and symbol;
**Unbalanced text length** usually comes from different types of questions that result in different length of answers in the exam papers.

![image](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/images/FigureChallengeSamples.png)

As shown in **Table 1**, there are totally 4,250 classes in our dataset SCUT-EPT, including 4,033 commonly used Chinese characters, 104 symbols, and 113 outlier Chinese characters, where outlier Chinese character means that the Chinese character is outside the character set of the popular CASIA-HWDB1.0-1.2. It should be noted that there is no intersection between the training set and the testing set, i.e., students who contribute to the training set will not play a part in the testing set. The total character samples in the SCUT-EPT dataset is 1,267,161, with approximately 25 characters each text line. 

![image](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/images/TableDataset.png)

In **Figure 1**, we provide the class distribution as well as typical samples of each grade. It is clear that the class distribution is extremely unbalanced, classes with 10 or fewer samples occupy a proportion of 41% while 3% of classes has more than two thousand samples each class. The imbalance distribution can bring hidden danger to the recognition system, because classes with few samples can barely be recognized in the real application. The rest of the classes, about 56%, have samples distributed from 10 to 2000. Typical samples of each grades, as demonstrated in Fig.~\ref{FigureDistribution}, are in line with common sense, for example, characters like \`我' and \`有' are popular used in daily life while \`喟' and \`鸩' are rarely used.

![image](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/images/FigureDistribution.png)

The shape of the text line image, especially the width size, plays an important role in recognition system.  Therefore, we present the sample distribution (at logarithmic axis) with respect to image text width in **Figure 2**, and draw scatter distribution of text line images with respect to their height and width in **Figure 3**. 
In **Figure 2**, we observe that images with width between 1,200 and 1,400 pixels occupies the vast majority (about 70%) of samples, while most other intervals have approximate two thousand samples. Besides, for each width interval, we visualize the character number proportion for text lines. Not surprisingly, wider images tend to possess more characters, but there is still a considerable part of wide text line images have fewer than 10 characters. In **Figure 3**, part of the text line images are represented as points in the picture with respect to their height and width. In line with the statistics in **Figure 2**, the majority of the sample points in **Figure 3** have a width distribution between 1,200 and 1,400 pixels, with height ranging from 30 to 100 pixels, leaving the remaining points sparsely spread in the picture.
Note that we distinguish sample points of training set from those of testing set by using different shape and color of points in **Figure 3**.
It can be observed that the training set and testing set of SCUT-EPT share similar sample distribution.

![image](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/images/FigureWidthandnumber_FigureWidthandheight.png)

## Experiment Results

We produce state-of-the-art seq-to-seq methods for text recognition problem on SCUT-EPT in **Table 5**.  Since our solution for SCUT-EPT dataset is based on deep-learning technique and deep-learning-based methods dominate state-of-the-art result on most of the handwritten datasets, we only make comparison for this kind of methods.

![image](https://github.com/HCIILAB/SCUT-EPT_Dataset_Release/blob/master/images/TablePreviousMethods.png)

## Citation and Contact
Please consider to cite our paper when you use our dataset:
```
@article{zhu2018scut,
  title={SCUT-EPT: a New Dataset and Benchmark for Offline Chinese Text Recognition in Examination Paper},
  author={Zhu, Yuanzhi and Xie, Zecheng and Jin, Lianwen and Chen, Xiaoxue and Huang, Yaoxiong and Zhang, Ming},
  journal={IEEE Access},
  year={2018},
  publisher={IEEE}
}
```
For any quetions about the dataset please contact Prof. Jin([eelwjin@scut.edu.cn](mailto:eelwjin@scut.edu.cn)).


