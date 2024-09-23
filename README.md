# Image Classifier Using Pretrained Classifier 

## Project Overview
This project, from the Udacity-AI with Python Programming course, implements an image classifier that identifies dog breeds using pretrained deep learning models. The classifier is designed to process images of dogs and classify them into their respective breeds based on a dataset of labeled images.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation
To run this project, you will need to have Python installed along with the following libraries:
- TensorFlow
- NumPy
- Matplotlib
- Pillow

You can install the required libraries using pip:
```bash
pip install tensorflow numpy matplotlib Pillow
```
Usage:
Clone the repository.
```
git clone <repository-url>
cd <repository-directory>
```
Prepare your dataset of dog images in the pet_images folder.
Run the image classifier:
```
python check_images.py --dir pet_images/
```
The program will output the classification results, including the accuracy of the model and the time taken for classification.

Project Structure
```
├── check_images.py 
# Main script to run the image classification

├── pet_images/           
# Directory containing images of dogs

├── dognames.txt        
# File containing dog breed names

└── README.md             # Project documentation
```

Results
```
The classifier was tested with three different models (VGG, ALEXNET, RESNET), and the results showed varying accuracy levels. The total elapsed runtime for each model was also recorded. The images are 40 images from the ImageNet database.

Example Output
*** Results Summary for CNN Model Architecture VGG ***
N Images            :  40
N Dog Images        :  30
N Not-Dog Images    :  10
pct_match           :  87.5
...
** Total Elapsed Runtime: 0:0:31
```

FINAL RESULT:
~~~
The VGG model was the most accurate model, having highest scores in:
% of non-dogs predicted as so (100%)
% of dogs predicted as so (100%)
% of dog breeds correctly identified (93.3%)
~~~