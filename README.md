# Final Project: Predict the popularity of shelter pet photos
Inspired by 
[PetFinder.my - Pawpularity Contest](https://www.kaggle.com/c/petfinder-pawpularity-score "PetFinder.my - Pawpularity Contest")

Blog site:
https://yaqiX.github.io/Assignment-09/

Binder: https://mybinder.org/v2/gh/yaqiX/FinalProj.git/HEAD

## Research Question Introduction
Before I settled in California, I was always thinking to adopt a cat. So after I finally settle, I check petfinder, if you're not familiar with it, it's a platform that helps you to find pets that are available for adoption.
I live in westwood and there are plenty of shelters but I end up adopt from a shelter 60 miles away after I saw the picture of our cat in [Petfinder](https://www.petfinder.com "Petfinder"). Without any reponse from the shelter, just one single picture in petfinder, we drove there immediately after we saw his cute cat paws. Before that we had been to many shelters and met so many stray animals, all after we saw some cute animal friends we would want to meet. Petfinder.com has options for shelters and rescuers to set up the pet profile, their basic features, but from my experience, the first sight from the pictures matters the most. I think this project can help improve people find their ideal animal friends, as well as more animal waiting to be adopted find their forever home. It can also guide shelters and rescuers to take better pictures to increase the chance that these animals being favored at the first sight. 
I also adopted a puppy in my home country China, where animal rescuing growing rapidly these few years. But we are not doing enough. I was also volunteering and helping local shelters, and writing a lot to government facilities for animal protection laws. I really hope this project can provide some insights, at least for myself, to improve animal rescue and promote stray animal adoption.

## About the Project data
Here's the link of data sources.
[Final Project Datasets: Petfinder Popularity of shelter pet photos prediction](https://www.kaggle.com/c/petfinder-pawpularity-score/data "Final Project Datasets: Petfinder Popularity of shelter pet photos prediction")
### - The Pawpularity Score 
The Pawpularity Score is derived from each pet profile's page view statistics at the listing pages, using an algorithm that normalizes the traffic data across different pages, platforms (web & mobile) and various metrics. Duplicate clicks, crawler bot accesses and sponsored profiles are excluded from the analysis.
### - Test and Train
The data is consisted of test data and train data. To be noted, the train.csv and test.csv files contain metadata for photos in the training set and test set, respectively. They featured each photo features such as photo quality, pet action, etc.

### - Usage of the data
The original data set is consisted of both tabular and picture data. I intended to analyze both, however, my macbook doesn't support tensorflow. I tried to set virtual environment but it worked really slow. And I was always confused. Now my laptop is having all kind of remaining problems with installing packages. So before I completely solve the problem, I have to leave the image processing and only work with numbers so far. It's sad that I finish this project solely on binder at last because I cannot even install packages like seaborn or numpy in my laptop.
### - Purpose of Photo Metadata
The Photo Metadata in this project is optional, manually labeling each photo for key visual quality and composition parameters by the PetFinder team.
These labels are not used for deriving the Pawpularity score, but it may be beneficial for better understanding the content and co-relating them to a photo's attractiveness. The end goal is to deploy AI solutions that can generate intelligent recommendations (i.e. show a closer frontal pet face, add accessories, increase subject focus, etc) and automatic enhancements (i.e. brightness, contrast) on the photos, so we are hoping to have predictions that are more easily interpretable.
## Methods
There are two parts of this projects. The first part is **exploratory data analysis and visualization**. In this part, I analyzed the Pawpularity Score distribution and the photo features.  The second part is **machine learning**. I applied the decision tree: classification and regression trees and came up with models that are able to predict the pawpularity score by features of pet picture.

