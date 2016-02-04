# bag-of-words
The source code is from https://github.com/bikz05/bag-of-words
Revised a little and replaced function of opencv using 3.0 version

## Training the classifier
```
python findFeatures.py -t dataset/train/
```

## Testing the classifier
* Testing a number of images
```
python getClass.py -t dataset/test --visualize
```
The `--visualize` flag will display the image with the corresponding label printed on the image/

* Testing a single image
```
python getClass.py -i dataset/test/aeroplane/test_1.jpg --visualize
```

# Troubleshooting

If you get 

```python
AttributeError: 'LinearSVC' object has no attribute 'classes_'
```

error, then simply retrain the model. 
