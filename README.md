
## Project Discussions 
1. I used the TFOD API to train the detection model. The API expects TFRecords as its inputs. So, before we have to generate the TFRecord data from the dataset.
2. Augmentation used 
- Horizontal flips
- Random crops
3. I used the SSD MobileDet Network to detect products from shelf images of grocery stores. MobileDet is more parameter efficient than MobileNetV2-based detectors.
- I have also added the hyperparameters config file for the training process.
- I trained the model for 10000 steps with a learning rate: 0.8.
- The Trained model exists with the loss:0.2736276 and mAP:0.68955684 at step: 10000.
 
4. I have also added the Tensor Board to view the trained progress report graphs. 

5. Evaluation: I generated the recall and precision scores (for 0.5 Intersection Over Union) on the test dataset with the trained model.

6. The Trained model infers how many products are likely to be present inside a given shelf image and I also created the output detection deliverables as "image2product.json" file and also added the "metrics.json" file (according to your requirement) 

## Major Requirements

1. TensorFlow == 1.5
2. Pandas
3. NumPy
4. Matplotlib
5. SciPy
6. OpenCV


## Reference Links
- https://github.com/tensorflow/models/tree/master/research/object_detection
- http://www.fypsolutions.com/opencv-python/ssdlite-mobilenet-object-detection-with-opencv-dnn/
- https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/
- https://github.com/anirbankonar123/CorrosionDetector/
- https://github.com/sayakpaul/Grocery-Product-Detection.git
- https://github.com/gulvarol/grocerydataset.git
```bash
https://github.com/moneshj

```


