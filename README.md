# MovieLens
Created during a recommendation challenge for hiring. The notebook touches on content-based filtering, collaborative filtering, and an ensemble approach by the end. 


## What is a recommendation system
- A subclass of information filtering system; to capture the user’s preference, or “recommend” similar items.​
- Nowadays, we see it in place of almost every commercial application; Daraz, Amazon, Netflix etc.​
- There are many styles of recommendation systems:​
    1. Collaborative Filtering: User-Item, User-User​
    2. Content-based Filtering: Content, Metadata​
    3. Hybrid Recommenders: CB+CF ​



## Phase 1

##### In our first attempt at understanding the dataset provided;​
- Select movie titles, genres and years from movies​
- Select Tags ​
- Convert Genres to columns (Top 15), and turn them into a 0-1 matrix​
- Titles: what do we do?​
- Thought Process: Titles have a meaning, sequels should come together? ​
- We converted Titles into embeddings using TF.HUB USE encoder​
- We filtered Tags on their weight > 1, and converted them to embeddings as well ​
- Apply Cosine Similarity and retrieve intermediate predictions

![image](https://user-images.githubusercontent.com/57410389/115930124-615bde80-a4a2-11eb-902d-cc5f8d43154d.png)


## Phase 2

##### In our second attempt at dealing with data, we:​
- Gather insight on metadata: Actors, Directors, Tags, Country​
- Capture the embeddings of all the above​
- Join newly constructed data with the previous data frame​
- Observe the effect on results​
- This is often known as meta-data based recommendations​
- Reasons are many; movie buffs who spend their entire time browsing movies possess enough information to know which actors - they like and dislike, what directors captures their interest the most and so on.

![image](https://user-images.githubusercontent.com/57410389/115930320-af70e200-a4a2-11eb-9005-c1d463220d69.png)

![image](https://user-images.githubusercontent.com/57410389/115930348-bac40d80-a4a2-11eb-94b3-fd29b4c781cf.png)


## Phase 3

##### The final step and the most important : ​
- Collaborative Filtering; User – Item collaboration​
- Ensemble Method​
- Hybrid Recommender: Personalized Suggestions for every user!​
- Flask API​
- Convert intermediate recommender to a function​
- Write up Ensemble Method function​
- Convert Hybrid Recommender to a function​
- Connect the dots – Recommend away!

![image](https://user-images.githubusercontent.com/57410389/115930522-10001f00-a4a3-11eb-9744-92745a153fca.png)

![image](https://user-images.githubusercontent.com/57410389/115930601-33c36500-a4a3-11eb-8f4d-766913740d0d.png)



## Tech

For this project, there  were a number of libraries used, namely:

- Pandas 
- Numpy
- Tensorflow 
- Surprise 
- Sklearn 
- Matplotlib
- NLTK 
- re 
- Flask


