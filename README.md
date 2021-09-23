# PathContainer

Computational pathology, a rapidly growing field, has proven to be effective and efficient in clinical diagnosisand therapeutic response prediction. However, processing Gigapixel images from Whole Slide Imaging(WSI) is extremely time-consuming. In the entire image processing pipeline, the tasks of patch-wise tilingand feature extracting are typically the most time consuming steps in large-scale patch-wise classificationand  WSI-wise  segmentation.  However, the selection of pretrained models (e.g.,  ImageNet) and featuredimensions of existing studies are generally subjective and difficult to standardize. In this paper, we presenta containerized toolkit called PathContainer, which provides flexible patch-wise transfer learning operations. Specifically, the PathContainer (1)tiles and extracts image patches from WSIs with the flexibility of thepatch  sizes, and (2) computes features with four different transfer learning methods, including ImageNetand BIT pre-trained ResNet50 models with different output dimensions.

## Setup
Please follow the instruction to download the [docker](https://docs.docker.com/get-docker/), and [NVIDIA Container Toolkit](https://docs.nvidia.com/datacenter/cloud-native/container-toolkit/install-guide.html#docker). 
Then you need to download the [PathContainer Image](https://hub.docker.com/repository/docker/zheyuzhu/pathcontainer) from DockerHub.

## Run your own dataset
```
docker run --rm -v [input directory]:/input/:ro -v [output directory]:/output -it pathcontainer
```

## Results
After running the code, you will get a list of folder in the output directory. 

## Example output
