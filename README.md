FlowerAI
    An AI that detects different types of flowers
This Project is a Classification AI to detect different types of flowers, by using a dataset from kraggle, with five different types of plants, i retrained the imagenet model in order to detect these specific flowers when inputed with an image, it creates another image with the classification on the top left with the percentage of confidence.

to install it, you need to clone the ropositary and go to the FlowerAI
cd {flowerAI path}

next, you need to set the net and dataset variables
    NET=models/flowermodel
    DATASET=dataset/flowerimages
finally, run this code to see how it works on an image
    imagenet.py --model=$NET/resnet18.onnx --input_blob=input_0 --output_blob=output_0 --labels=$DATASET/labels.txt $DATASET/test/cat/01.jpg cat.jpg
find the image and click on it and at the top left it should say the flower it recognizes with the perfcentage
