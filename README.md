# 作业2 复现schoenberger_phd_thesis Table 3.3: Results for our local feature benchmark. Fountain行

1.阅读INSTRUCTIONS.md并配置环境 准备数据  

2.运行理解代码 scripts/matching_pipeline.m

3.运行理解代码 

scripts/reconstruction_pipeline.py

4.可视化论文图片结果

## 文件组成

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/%E6%96%87%E4%BB%B6%E7%BB%84%E6%88%90.png)




## SIFT

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_Matlab.png)



![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_Matlab_result.png)



![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/%E6%96%87%E4%BB%B6%E7%BB%84%E6%88%90_2.png)



SIFT结果：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_result.png)



## SIFT-PCA

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_Matlab.png)



### SIFT-PCA遇到的问题：

1、

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_error.png)



![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_correct.png)

2、

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_error_2.png)



![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_correct_2.png)



SIFT-PCA结果：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/SIFT_PCA_result.png)



## DSP-SIFT

DSP-SIFT结果：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/DSP_SIFT_result.png)



## ConvOpt

opencv版本：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/ConvOpt_opencv_version_.png)



实现步骤：

1、先运行feature_extraction_convopt.py，获取描述子

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/ConvOpt_descriptor.png)



2、在Matlab中注释调用描述子获取的程序，只运行匹配操作

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/ConvOpt_Matlab.png)



ConvOpt结果:

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/ConvOpt_result.png)



## TFeat

下载TFeat项目：[GitHub - vbalnt/tfeat: TFeat descriptor models for BMVC 2016 paper &quot;Learning local feature descriptors with triplets and shallow convolutional neural networks&quot;](https://github.com/vbalnt/tfeat)

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/TFeat_github.png)



实现步骤：

1、先在Matlab中运行feature_extraction_tfeat.m，代码是检测每个图像中的关键点，并提取与这些关键点相关的图像补丁（patches），然后将这些补丁存储到文件中

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/TFeat_patch.png)



2、再运行feature_extraction_tfeat.py，获取描述子

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/TFeat_descriptor.png)

3、在Matlab运行匹配程序



TFeat结果：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/TFeat_result.png)



## LIFT

下载LIFT项目：[GitHub - cvlab-epfl/LIFT: Code release for the ECCV 2016 paper](https://github.com/cvlab-epfl/LIFT)

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/LIFT_github.png)



实现步骤：

1、编译c-code文件夹下的代码：



2、配置feature_extraction_list.sh路径

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/LIFT_setting.png)



3、运行feature_extraction_lift.sh



4、运行feature_extraction_list.py，获取描述子



LIFT结果：

![](https://github.com/GDUTCV/homework-02-feature-descriptor-lijiayu1125/blob/main/result/LIFT_result.png)
