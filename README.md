# Pytorch-Model-to-TensorRT

## Convert a Pytorch model to TensorRT engin (optional: int8 engin)

### Required:

Python packages: in `requirements.txt` 

External: 

- CUDA == 9.0
- CUDNN == 7.3.1
- TensorRT == 4.0.2.6

### Data And Checkpoint Prepare

You shuold prepare data and model weights in like this way:
```
project  
│
└───data
│   │   test.txt
│   │   fake-test.txt
│   │   images
│   
└───checkpoint
    │   model_best.pth

```

The list of test file should follow this format:
```text
file0,label0
file1,label1
... ...
``` 

Or you can download the example from [BaiduYun](https://pan.baidu.com/s/1ecVcWXDbEwKl2D_PUuGmng) 

### Convert step:

```bash
python main.py
```

Additional steps are needed to set up the Tensor RT 4, given the reduced support & focus on the newer Tensor RT 5 by NVIDIA. Will list here some of the steps I encountered myself while stumbling to get it working these past few weeks.

Please refer to useful links.txt for resources to help out.
