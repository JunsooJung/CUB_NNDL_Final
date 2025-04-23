This is Final project for University of Colorado Boulder, CSCI 5922-001-003: Neural Nets and Deep Learning course.

# Bird Image Classification


## Team
| Name                                  | Email                                      |
|---------------------------------------|--------------------------------------------|
| Junsoo Jung                           | junsoo.jung@colorado.edu                   |
| Wyatt Babb                            | wyatt.babb@colorado.edu                    |


## Files 

### inat_downloader.py
This is the main data collecting method. 

Using this command.
```shell
py inat_downloader.py -o 5000 -q research -l cc-by,cc-by-nc,cc0 -s medium
```
will download from 5000 uploaders with research grade images with maximum 500px on the longest side.

### inat_cleaner.ipynb

After download the images, There will be at least 5000 research grade images. But also there will be other images that user uploaded at the same time.

Mostly they are :
  - Same photo but slightly different angle.
  - Blurred photos
  - inaccurate photos

We found out that people usually post the best photo as a Main(first) photo, we decided to collect only the first images.

### Deep_Learning_Final_Prototype.ipynb

This is the main function file that doing the model structure and training.
