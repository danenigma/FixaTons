# FixaTons
A collection of Human FixationsDatasets and Metrics for Scanpath Similarity

## Citations
If you intend to use this collection of dataset for your research, please cite the technical report

    - FixaTons technical report: link

and also, all the correspondent pubblications for the dataset included:

    - MIT1003: http://people.csail.mit.edu/tjudd/WherePeopleLook/Docs/wherepeoplelook.pdf
    - TORONTO: http://journalofvision.org/7/9/950/
    - KOOTSTRA: http://www.csc.kth.se/~kootstra/index.php?item=602&menu=&file=http://dx.doi.org/10.1007/s12559-010-9089-5

## Download FixaTons

- Clone or download the folder with the code
- Download the zip file from https://www.dropbox.com/s/i5xw3xbgqdw6tk8/FixaTons.zip?dl=0 and extract its content in the same folder with the code

## Structure of FixaTons

________________________________________________________________________________

- FixaTons

    - DATASET_NAME

        - STIMULI : contains original images.
                  They can have different file format (jpg, jpeg, png,...)

        - SCANPATHS : contains one folder for each image

            - IMAGE_ID :
                  it contains one file for each scanpath of that image
                  scanpaths are matrices
                  rows of this matrices describe fixations
                  each fixation is of the form :
                  [x-pixel, y-pixel, initial time, final time]
                  Times are in seconds.

        - FIXATION_MAPS : contains a fixation map of each original image
            they are matrices of zeros (NON-fixated pixels) and 255's (fixated
            pixels). They can have different file format (jpg, jpeg, png,...)

        - SALIENCY_MAPS : contains saliency maps of each original image
            they are generated from human data. They can have different file
            format (jpg, jpeg, png,...)
            
________________________________________________________________________________

## How to use FixaTons (with python)


For an easy use of the dataset, python software is provided. This tools help you in different tasks:

    - List information
    - Get data (matrices)
    - Visualize data
    - Compute metrics
    - Compute statistics

For some example codes, please refer to the correspondent report or Tutorial.ipynb (jupiter notebook).

