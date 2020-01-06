# Background-remover

A background remover project that uses a frozen model trained on JaNetDataset. The fronzen model was trained [here](https://colab.research.google.com/drive/105ESRoQXROdjkJkcWPoU4RwAAmOhtJ3G)<p></p>

Open this [notebook](https://github.com/Mbah-Javis/Background-remover/blob/master/Background%20Removal.ipynb) to see how the model was used to remove background from an image
<h3>Sample input</h3>
![](https://github.com/Mbah-Javis/Background-remover/blob/master/IMG_0031.JPG)

<h3>Output</h3>
![](https://github.com/Mbah-Javis/Background-remover/blob/master/output/IMG_0031.png)

<p></p>
The JaNetDataset is a custom dataset made using 500 images from [Helen_1](http://www.ifp.illinois.edu/~vuongle2/helen/data/helen_1.zip). The images where resized to thesame shape using `transform_image_resolution.py` by typing  <p></p>
```python transform_image_resolution.py -d helen_1/ -s 800 600``` 
<p></p>
in the command line and the same directory with the helen_1 folder. 
<p>After the images where resized to thesame shape, I divided the images into two that is trainging and testing images</p>

`train = 300` and `test = 200` 

<p></p>

I used this [label](https://github.com/tzutalin/labelImg) tool to label the images and each labele was saved as PICTURENUM.xml in train_ and test_ directories. 
<p></p>

The file `xml_to_csv.py` was used to extract the labesl from the .xml files of the train_ and test_ directories to `train_labels.csv` and `test_labels.csv`  
