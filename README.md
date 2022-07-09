# CT-image-segmentation-and-radiomics-feature-extration

param.yaml 为Pyradiomic Extractor的配置文件，用于配置filter以及提取的特征。

从[这里](https://pan.baidu.com/s/1n40vNR9wzNjHYwdkDgk_AA?pwd=b54i)(提取码：b54i)下载实验中用到的数据集。将下载的数据集分别存放到根目录下的CT_seg1和CT_seg2文件夹下。

模型文件从[这里](https://pan.baidu.com/s/1IqlUtqZI3jeDiwHrZ1Qorw?pwd=mscg)(提取码：mscg)下载, 下载完成后存放到根目录下。

运行下面的命令来训练TV_Unet模型:
```sh
 CUDA_VISIBLE_DEVICE=0 python main_TV_Unet_Split1.py
```

下载模型文件后可以直接运行下面的命令来训练TV_Unet模型:
```sh
 CUDA_VISIBLE_DEVICE=0 python main_TV_Unet_Split1.py --infer
```


