# THK2004.github.io
BookRecSys_THK
## README

BookRecSys is my final capstone project for ML4AI (Machine Learning for AI) course, organized by CoTai center. The project provides a simple recommender system for books based on data compiled from Amazon by Cai-Nicolas Ziegler. It contains 1.1 million ratings of 270,000 books by 90,000 users. The ratings are on a scale from 1 to 10.

Here is the dataset link: http://www2.informatik.uni-freiburg.de/~cziegler/BX/ 

## Representation

This is the PowerPoint file i used for representation. It contains the process i built this recommender system at the beginning, also my viewpoint in Machine Learning Pipeline,  $X\to Z\to \hat{y}$ and TEFPA.

https://drive.google.com/file/d/1lV2snWVvaTmx7jF53HUlPk-MzhayWpON/view?usp=sharing

## How to use

- Run the code in google colab with GPU, skip Personalized part.
- Find out the Id of your favourite book in Amazon.
- Find out its order in my book lists with ```np.where(books_in_orders=='ISBN')```. 
- Put it in my code and see the recommended one.

## Source Code

From Google Collab: https://colab.research.google.com/drive/1bn9Kn4dtmvvJOLh_GDTPxaUKkGcFf_3Z?usp=sharing

## About changes

After perceiving some problems and receiving new ideas from the representation. My project has some updates:

- Instead of filling 0 in utility matrix, it is normalized with the mean value. The users who only rate 0 are excluded.
- Using MLP for personalized models.

## Known problems

Measure to know how good is this RecSys.

Can't pickle a dictionary of keras models.
