# Data Preparation

## ImageNet-B
The dataset should be in the following format:

```
### ImageNet style


dataset
   images
        class1
             image1.jpeg
             image2.jpeg
             ...
        class2
             image1.jpeg
             image2.jpeg
             ...
        ...
   masks
        class1
             image1.jpeg
             image2.jpeg
             ...
         class2
             image1.jpeg
             image2.jpeg
             ...
         ...
    captions
        class1
             image1.txt
             image2.txt
             ...
         class2
             image1.txt
             image2.txt
             ...
         ...
```

## COCO-DC

```
dataset
   images or val2017       
         image1.jpeg
         image2.jpeg
         ...

   masks
         image1.jpeg
         image2.jpeg
         ...

    captions
         image1.txt
         image2.txt
         ...
    
    annotations
         instances_val2017.json

```


Captions can be generated for ImageNet-B and COCO-DC dataset using BLIP:
```
python dataset_utils/generate_captions_blip.py --dataset imagenet --data_path <>
```
A captions folder will be generated in the dataset folder.

ImageNet-B, ImageNet-B_1k, COCO-DC, and COCO-DC(classification) datasets will be publicly available after we get manuscript reviews.

