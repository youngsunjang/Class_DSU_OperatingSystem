# Class_DSU_OperatingSystem

## OpenMP and Sequential Programming
1. How to compile your program?
2. How to run your program?

Due to complicated issues emerging during compile- and run-time related to many libraries, path registration, and dependencies, this program is strongly recommended to run in Google Colab's environment.

Copying and pasting my uploaded python file to Google Colab, it's easily to compile and run the program.
File name: Skip-gram_OpenMP_Sequential.py

However, for your convenience, please visit my github repository (https://github.com/youngsunjang/Class_DSU_OperatingSystem).
(1) Open the github repository by copying and pasting the link above to a web browser.
(2) Click the file 'Skip-gram_OpenMP_Sequential.ipynb'.
(3) Click the icon 'Open in Colab'. (Recommend to be logged in Google Account)
(4) Check if the machine set to Host (CPU). For doing this, plese follow below steps:
   i. Click the 'Runtime' on menu bar.
   ii. Click the 'Change return type' in the sub-menu
   iii. Click the button 'CPU' in the Hardware accelerator section.
   iv. Click the 'Save'
(5) Upload data file ('New_data.txt').  For doing this, plese follow below steps:
   i. Download the file from the github link
   ii. Click the icon 'Files' located in the left of Colab editor
   iii. Once the 'Files' pane gets expanded, drag the downloaded file to this area to upload the file to storage session.
(6) Run each cell in the Colab editor, one by one from top to bottom.
   * if a message of warning ('This notebook was not authored by Google') pops up, ignore it and click the 'Run anyway'.




3. What is the average running time of your program?

The performance displayed below differs somewhat from the results observed in the Colab environment, because below is the execution on my local laptop environment. Additionally, the running time, even under the same NP conditions, may vary among the 10 repetitions due to potential influences from my PC's usage at the time. When I executed other heavy programs, such as video play, concurrently on the laptop, the running time may extend. 

I conducted 10 repetitions for each NP option to calculate the average running time. The following records represent the running times for each of the 10 repetitions. All experiment ensured the same accuracy performance.

* As noted in section 5 below, the required library PyTorch already employed the OpenMP method, NP=1 experiment can be regarded as Sequential program's performance.

NP=1 (Sequential)
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655\\
Elapsed Time: 350.84901762008667 seconds\\
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655\\
Elapsed Time: 343.2357666492462 seconds\\
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 344.023868560791 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 341.5191717147827 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 340.1362421512604 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 342.741557598114 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 342.25909781455994 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 352.66613388061523 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 357.25474739074707 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 365.0220322608948 seconds

NP=2
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 296.04875588417053 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 287.94748282432556 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 237.90127038955688 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 264.5040957927704 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 251.1345591545105 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 245.18237400054932 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 322.1634156703949 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 305.09377789497375 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 258.77007365226746 seconds
Epoch 1950, loss = 3.4129061698913574, accuracy = 0.2850042601533655
Elapsed Time: 257.36603021621704 seconds

NP=3
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 330.15155267715454 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 229.37725162506104 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 210.58707785606384 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 261.2154231071472 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 275.11957478523254 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 214.41710495948792 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 212.8665885925293 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 199.00910091400146 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 254.14104843139648 seconds
Epoch 1950, loss = 3.4145970344543457, accuracy = 0.2850042601533655
Elapsed Time: 262.2793278694153 seconds

NP=4
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 232.39578890800476 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 231.2735686302185 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 195.7581045627594 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 190.83921337127686 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 187.00310492515564 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 194.1915681362152 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 200.29467010498047 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 202.2070996761322 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 204.31884098052979 seconds
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 205.73759961128235 seconds




4. What are the expected output results when I run your program?

The number of model training ('Epoch'), the error rate of model's prediction ('loss'), and the model performance ('accuracy').
The accuracy is one metric for evaluating NN models. Informally, accuracy is the fraction of predictions a model got right. Formally, accuracy has the following definition:

Accuracy = Number of correct prediction of model / Total number of prediction of model

e.g.,
Epoch 1950, loss = 3.4139177799224854, accuracy = 0.2850042601533655
Elapsed Time: 205.73759961128235 seconds




5. Any descriptions which may help me to compile, run, and verify your answers. (FYI: I check every programming assignment turned in!)

The program imports all necessary libraries, including PyTorch and its sub-libraries, Pandas, Numpy, and more. Notably, PyTorch plays a fundamental role in constructing the program among these libraries. It transforms raw input data into torch.tensor-typed real numbers, making it machine-readable input. The tensor data type proves highly convenient for massive vector operations like addition, multiplication, and division, establishing its widespread use in NN programs. Additionally, the tensor data type easily supports multi-dimensional conversion. 
Furthermore, with regard to CPU parallelism, PyTorch supports OpenMP as the default mode. This implies maximum parallel programming throughout the program whenever a PyTorch-based language is employed using the OpenMP method.

## GPU Programming
1. How to compile your program?
2. How to run your program?

Due to complicated issues emerging during compile- and run-time related to many libraries, path registration, and dependencies, this program is strongly recommended to run in Google Colab's environment.

Copying and pasting my uploaded python file to Google Colab, it's easily to compile and run the program.
File name: Skip-gram_GPU.py

However, for your convenience, please visit my github repository (https://github.com/youngsunjang/Class_DSU_OperatingSystem).
(1) Open the github repository by copying and pasting the link above to a web browser.
(2) Click the file 'Skip_gram_GPU_A100_V100.ipynb', when either A100 GPU or V100 GPU is available. 
    Click the file 'Skip-gram_GPU_T4GPU.ipynb', when T4 GPU is available.
(3) Click the icon 'Open in Colab'. (Must be logged in Google Account)
(4) Check if the machine set to Device (GPU). For doing this, plese follow below steps:
   i. Click the 'Runtime' on menu bar.
   ii. Click the 'Change return type' in the sub-menu
   iii. Click the button 'A100 GPU' or 'V100 GPU' or 'T4 GPU' in the Hardware accelerator section.
        * If you are not a Colab Pro subscribed user, the only option is T4 GPU.
   iv. Click the 'Save'
(5) Upload data file ('New_data.txt').  For doing this, plese follow below steps:
   i. Download the file from the github link
   ii. Click the icon 'Files' located in the left of Colab editor
   iii. Once the 'Files' pane gets expanded, drag the downloaded file to this area to upload the file to storage session.
(6) Run each cell in the Colab editor, one by one from top to bottom.
   * if a message of warning ('This notebook was not authored by Google') pops up, ignore it and click the 'Run anyway'.




3. What is the average running time of your program?

The performance displayed below differs somewhat from the results observed in the Colab environment, because below is the execution on my local laptop environment. Additionally, the running time, even under the same NP conditions, may vary among the 10 repetitions due to potential influences from my PC's usage at the time. When I executed other heavy programs, such as video play, concurrently on the laptop, the running time may extend. 

I conducted 10 repetitions for each NP option to calculate the average running time. The following records represent the running times for each of the 10 repetitions. All experiment ensured the same accuracy performance.

* As noted in section 5 below, the required library PyTorch already employed the OpenMP method, NP=1 experiment can be regarded as Sequential program's performance.
* T4 GPU has slight performance decrease due to slight change in model training condition, but there's a very minor gap.

V100 GPU

Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 35.24060797691345 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 34.569284439086914 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 29.726160287857056 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 28.800009965896606 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 29.840426206588745 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 29.600542783737183 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 30.688892364501953 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 28.950028896331787 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 30.624762773513794 seconds
Epoch 1950, loss = 3.4115867614746094, accuracy = 0.2850042601533655
Elapsed Time: 29.694819927215576 seconds


A100 GPU

Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 30.75859260559082 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.35645294189453 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.604503393173218 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.474350214004517 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 29.62126350402832 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.408024549484253 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.458804607391357 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.370119333267212 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.417228937149048 seconds
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.52726149559021 seconds


T4 GPU

Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 38.023916721343994 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 35.69511651992798 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 35.99100470542908 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 36.111114501953125 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 36.10673499107361 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 36.331968784332275 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 36.540855169296265 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 36.968337297439575 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 37.01098704338074 seconds
Epoch 1950, loss = 3.6092190742492676, accuracy = 0.28486225504118146
Elapsed Time: 37.30700445175171 seconds



4. What are the expected output results when I run your program?

The number of model training ('Epoch'), the error rate of model's prediction ('loss'), and the model performance ('accuracy').
The accuracy is one metric for evaluating NN models. Informally, accuracy is the fraction of predictions a model got right. Formally, accuracy has the following definition:

Accuracy = Number of correct prediction of model / Total number of prediction of model

e.g.,
Epoch 1950, loss = 3.4162163734436035, accuracy = 0.2850042601533655
Elapsed Time: 28.52726149559021 seconds





5. Any descriptions which may help me to compile, run, and verify your answers. (FYI: I check every programming assignment turned in!)

The program imports all necessary libraries, including PyTorch and its sub-libraries, Pandas, Numpy, and more. Notably, PyTorch plays a fundamental role in constructing the program among these libraries. It transforms raw input data into torch.tensor-typed real numbers, making it machine-readable input. The tensor data type proves highly convenient for massive vector operations like addition, multiplication, and division, establishing its widespread use in NN programs. Additionally, the tensor data type easily supports multi-dimensional conversion. 
Furthermore, with regard to CPU parallelism, PyTorch supports OpenMP as the default mode. This implies maximum parallel programming throughout the program whenever a PyTorch-based language is employed using the OpenMP method.
