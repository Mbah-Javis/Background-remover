# Background-remover
 
The JaNetDataset is a custom dataset made using 500 images from [Helen_1](http://www.ifp.illinois.edu/~vuongle2/helen/data/helen_1.zip). The images where resized to thesame shape using `transform_image_resolution.py` by using  
```python transform_image_resolution.py -d helen_1/ -s 800 600``` in the commandline and thesame directory with the helen_1 folder. After the images where resized to thesame shape, I used this [label](https://github.com/tzutalin/labelImg) tool to label the images. 
When all the images where labeled, i divided them into two that is one for training and the other for testing 
`train = 300` and `test = 200` 
