# Mini Places Challenge Data
This is the expanded data set for MIT's 6.819 Computer Vision Mini Places Challenge. The original data set was sampled from the [Places2 dataset](http://places2.csail.mit.edu/), which contains 10+ million images belonging to 400+ unique scene categories. The challenge data will be a subset of the full Places2 dataset, coming from 100 scene categories and consisting of 100,000 images for training, 10,000 images for validation, and 10,000 images for testing. For more information on the challenge, check out its [details](https://github.com/CSAILVision/miniplaces).

## About the Data Set
There are three types of image data for this competition, all coming from the larger Places2 dataset: training data (TRAINING), validation data (VALIDATION), and test (TEST). There is no overlap in the three splits of data.  All three splits contain images belonging to 100 scene categories.

```
               Number of images
   Dataset     TRAIN        VALIDATION   TEST
  ------------------------------------------------
   MiniPlaces  100,000      10,000       10,000
```

Every image in the training, validation and test sets has a single image-level label specifying the presence of one object category.

Challenge database statistics is as follows:

```
  Training: 	100,000 images, with 1000 images per category
  Validation:	10,000 images, with 100 images per category
  Test:		10,000 images, with 100 images per category
```

The 3 sets of images (training, validation and test) are available as a single tar archive. All images are in JPEG format. For the challenge, images have been resized to 128x128 to make the data manageable for students.

To expand the data set, we zoomed and cropped, rotated and blurred each image (separately). As a result, the data set now looks like the following:

| Dataset             | TRAIN        | VALIDATION  | TEST |
| --------------------| -------------| ------------| -----|
| MiniPlaces          | 100,000      | 10,000      | 10,000 |
| AugmentedMiniPlaces | 400,000      | 10,000      | 10,000 |

## Prepared by
- Maryam Archie
- Sandeep Silwal

## Reference
Link: [Places2 Database](http://places2.csail.mit.edu), [Places1 Database](http://places.csail.mit.edu), [Mini Places Challenge](https://github.com/CSAILVision/miniplaces)

Please cite the following [places journal paper](http://places2.csail.mit.edu/PAMI_places.pdf) if you use the data or pretrained CNN models.

```
 @article{zhou2017places,
   title={Places: A 10 million Image Database for Scene Recognition},
   author={Zhou, Bolei and Lapedriza, Agata and Khosla, Aditya and Oliva, Aude and Torralba, Antonio},
   journal={IEEE Transactions on Pattern Analysis and Machine Intelligence},
   year={2017},
   publisher={IEEE}
 }
```

Please contact Bolei Zhou (bzhou@csail.mit.edu) if you have questions or comments on the general design of the MiniPlaces challenge. If you an MIT student taking 6.819/6.869: Advances in Computer Vision, please contact the [teaching staff](http://6.869.csail.mit.edu/) for any course-related problems.
