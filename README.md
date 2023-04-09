# ICME2023_AVMST
## Modality-Fusion Spiking Transformer Network for Audio-Visual Zero-Shot Learning (ICME 2023)
Wenrui Li, Zhengyu Ma, Liang-Jian Deng and Xiaopeng Fan.  
The code is based on [AVCA](https://github.com/ExplainableML/AVCA-GZSL) and tested on Ubuntu 20.04 with torch 1.13.
### Inportant
The version of [spikingjelly](https://spikingjelly.readthedocs.io/zh_CN/latest/index.html) we used is 0.0.0.0.12. Installing different versions can cause performance differences.
### Downloading features
The features and dataset structure could download and placed the same as [AVCA](https://github.com/ExplainableML/AVCA-GZSL).
## Evaluation
### Dowloading pre-trained models
[Here](https://drive.google.com/file/d/1HK9_dwysfQv56smXYK4lRA7dvSKpE_DE/view?usp=sharing), you can download our trained AVMST models and baselines which are located in `pretrain_model.zip`
Put the content of `pretrain_model.zip` in the `runs/` folder.
### Test on three benchmark datasets
Here is an example for evaluating AVMST on Vggsound-GZSL using SeLaVi features.
``` 
python get_evaluation.py --load_path_stage_A runs/attention_ucf_vggsound_main --load_path_stage_B runs/attention_vggsound_all_main  --dataset_name VGGSound --AVMST 
```
## Acknowledgement
We appreciate the code provided by [AVCA](https://github.com/ExplainableML/AVCA-GZSL), which is very helpful to our research.

## References 
If you find this work useful, please consider citing:
```
@inproceedings{Li2023avmst,
  author    = {Wenrui Li, Zhengyu Ma, Liang-Jian Deng and Xiaopeng Fan},
  title     = {Modality-Fusion Spiking Transformer Network for Audio-Visual Zero-Shot Learning},
  booktitle = {IEEE International Conference on Multimedia and Expo (ICME))},
  year      = {2023}
}
```
```
@inproceedings{mercea2022avca,
  author    = {Mercea, Otniel-Bogdan and Riesch, Lukas and Koepke, A. Sophia and Akata, Zeynep},
  title     = {Audio-visual Generalised Zero-shot Learning with Cross-modal Attention and Language},
  booktitle = {Conference on Computer Vision and Pattern Recognition (CVPR)},
  year      = {2022}
}
```
