# MAVEx Hierachical Model 

## Preprocessing
Please download the image features from [here](https://mavex.s3.us-east-2.amazonaws.com/new_image_features.zip) and unzip as 'image_features' <br>
Please download the image MAVEx features by following operations:
(1) mkdir h5py_accumulate. <br>
(2) download [file1](https://mavex.s3.us-east-2.amazonaws.com/h5py_accumulate/image_features/image_train_qid_ans2idx.pkl) to h5py_accumulate.<br>
(3) download [file2](https://mavex.s3.us-east-2.amazonaws.com/h5py_accumulate/image_features/image_train.hdf5) to h5py_accumulate.<br>
(4) download [file1](https://mavex.s3.us-east-2.amazonaws.com/h5py_accumulate/image_features/image_val_qid_ans2idx.pkl) to h5py_accumulate.<br>
(5) download [file1](https://mavex.s3.us-east-2.amazonaws.com/h5py_accumulate/image_features/image_val.hdf5) to h5py_accumulate.  <br>
Please download the vilbert pretrained model from [here](https://mavex.s3.us-east-2.amazonaws.com/pytorch_model_4.bin)<br>
Please download retrieved knowledge from [here](https://drive.google.com/file/d/1F_tKHOC5HIHdmm9KnUJV7wYMBZEgHQI0/view?usp=sharing)<br>

``mkdir save''<br>

## Training
(1) Train by runnning <br>
``CUDA_VISIBLE_DEVICES=0 ft_mavex.py --save_name demo --seed 7777 --from_pretrained pytorch_model_4.bin --num_epochs 120
