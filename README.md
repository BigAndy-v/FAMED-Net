# FAMED-Net
[FAMED-Net: A Fast and Accurate Multi-scale End-to-end Dehazing Network.](https://chaimi2013.github.io/Research/FAMED-Net/)

The code has been tested on Ubuntu 14.04 with CUDA 8.0.

## Installation
Install the caffe-master-FAMED-Net and compile the Matlab interface. 

If you use Ubuntu 16.04, please modify Makefile and Makefile.config. 

Download the AOD-Net model and FPC-Net model from [AOD-Net](https://github.com/Boyiliee/AOD-Net) and [FPC-Net](https://github.com/chaimi2013/FPCNet), rename them as "AOD_Net.caffemodel" and "FPC-Net.caffemodel", and put them into the "model" folder.

## Folder Structure
    caffe-master-FAMED-Net
        The caffe source code
    FAMED-Net
        -fast-guided-filter
            Fast guided filter code [1]
        -generateData
            Generating HDF5 training files
        -model
            Folder containing dehazed models of AOD-Net, FPC-Net, and FAMED-Net
        -results
            Folder containing dehazed results
        -stats
            Codes and data for generating the learned statistical priors of different models
        -testImgs
            Test hazy images
        -utils
            PSNR, SSIM (from [2]), and store2hdf5 functions
        -testDemoObjectiveEval_ForTestSet_FastGF
            Main script for objective evaluation on RESIDE SOTS test set
        -testDemoSubjectiveEval_ForImgs_FastGF
            Main script for subjective evaluation on single hazy test image

## Reference
    [1]. Fast guided filter, [Kaiming He](http://kaiminghe.com/eccv10/index.html)
    
    [2]. A Benchmark for Single Image Dehazing, [RESIDE](https://sites.google.com/view/reside-dehaze-datasets)
            
## Citation
Please cite our paper in your publications if it helps your research:

    @article{zhang2019famednet, 
        author={Zhang, Jing and Tao, Dacheng}, 
        journal={IEEE Transactions on Image Processing}, 
        title={FAMED-Net: A Fast and Accurate Multi-scale End-to-end Dehazing Network}, 
        year={2019}, 
        volume={}, 
        number={}, 
        pages={1-1}, 
        doi={10.1109/TIP.2019.2922837}, 
        ISSN={1057-7149}, 
        month={}
    }

## Contact
[Email](zj.winner@163.com)
