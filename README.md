# ICME2023_AVMST
## Modality-Fusion Spiking Transformer Network for Audio-Visual Zero-Shot Learning (ICME 2023)
Wenrui Li, Zhengyu Ma, Liang-Jian Deng and Xiaopeng Fan.  
The code is based on [AVCA](https://github.com/ExplainableML/AVCA-GZSL) and tested on Ubuntu 20.04 with torch 1.13.
### Downloading features
The features and dataset structure could download and placed the same as AVCA.
## Evaluation
### Dowloading pre-trained models
[Here](), you can download our trained AVMST models and baselines which are located in `pretrain_model.zip`
Put the content of `pretrain_model.zip` in the `runs/` folder.
### Test on three benchmark datasets
Here is an example for evaluating AVMST on Vggsound-GZSL using SeLaVi features.
``` 
python get_evaluation.py --load_path_stage_A runs/attention_ucf_vggsound_main --load_path_stage_B runs/attention_vggsound_all_main  --dataset_name UCF --AVMST 
```
## References 
Please cite our paper if you find the work useful:
```
@inproceedings{Li2023avmst,
  author    = {Wenrui Li, Zhengyu Ma, Liang-Jian Deng and Xiaopeng Fan},
  title     = {Modality-Fusion Spiking Transformer Network for Audio-Visual Zero-Shot Learning},
  booktitle = {IEEE International Conference on Multimedia and Expo (ICME))},
  year      = {2023}
}
```
