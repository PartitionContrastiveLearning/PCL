# Source Codes and Datasets for "Datasets, Tasks, and Training Methods for Benchmarking Large-scale Hypergraph Learning." 
- Sunwoo Kim*, Dongjin Lee*, Yul Kim, Jungho Park, Taeho Hwang, and Kijung Shin**
(*: Equal Contribution / **: Corresponding Author)
- Submitted to ICDE 2023. 
- For any (possible) issue regarding datasets or codes, feel free to contact kswoo97@kaist.ac.kr.

## Dataset Description

We provide hypergraph datasets at **https://www.dropbox.com/sh/qhz6rqol5mue4wc/AAByciJuLNba8uGv8MdMpbf-a?dl=0**. 
We provide 
- Each dataset's feature, node label, original hyperedge information, split hyperedge information (for task 1)
- Each dataset's partitioned hypergraph (# of Partition $|P|$ / DBLP:4, Trivago:32, OGBN_MAG:128, AMINER and MAG: 256)
- For DBLP, Trivago, OGBN_MAG, we also provide partitioned hypergraph **P-IOS** partition.  

Refer to README file in dataset folder for more details regarding datasets.

## Code Description 

### Overview
In this repository, we provide source codes for
- Obtaining performance on proposed task 1 (hyperedge disambiguation)
- Obtaining performance on proposed task 2 (local clustering)

### Dataset
For dataset one aims to run the code, files of corresponding dataset in **URL** should be located in scr/data folder. 
For example
```
src
  |_ data
      |_ aminer
            |_ aminer_X_vec.pt
            |_ aminer_y.pt
            |_ aminer_E.pt
            |_ ...
```

### Hyperparameters

We provide hyperparameter combination for reproducibility of experimental results.  
Refer to best_hyperparameter directory, where we saved each dataset-model combination's best hyperparameter as .json files.

### How to implement codes
