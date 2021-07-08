# Movie-Recommandation-System
## Introduction
### What is Recommandation system
Recommandation system is simply a filteration programme whose prime goal is to predict "rating" or "prefrences" of a user towards a domain specific item. In my case the domain specific item is movie
### Different filtering strategies -
1. Content based filtering
2. Collabrative filtering
    #### 1. Content based filtering :- 
    This filtering strategy is based on the data provied about the items. The algorithm recommand products that are similar to the ones that a user has liked in past. this similarity (generally cosine similarity) is computed from the data that we have about the items aas well as user past prefrences.
    
    Disadvantages : -
    a. different products do not get much exposure to the user
    b. Businesses can not be expanded as the user does not try different products.
   
   #### 2. Collabrative filtering : -
   This filtration strategy is based on the combination of the user’s behavior and comparing and contrasting that with other users’ behavior in the database. The history of all users plays an important role in this algorithm.
   
   There are two types of collabrative filtering - 
   a. User based collabrative filtering : - The basic idea here is to find users that have similar past preference patterns as the user ‘A’ has had and then recommending him or her items liked by those similar users which ‘A’ has not encountered yet. This is achieved by making a matrix of items each user has rated/viewed/liked/clicked depending upon the task at hand, and then computing the similarity score between the users and finally recommending items that the concerned user isn’t aware of but users similar to him/her are and liked it.
   Disadvatages : - People taste changes time to time and as this algorithm based on user similarity it may pick up initially pattern between two users that after a while may changes.,
   There are more users than items therefore it become very difficulty to handle such large matricses., this algorithm is very susceptible to shilling attacks where fake user profiles consisting of biased prefrences are used to manipulate key decisions.
   
    b. Item based collabrative filtering : - The concept in this case is to find similar movies instead of similar users and then recommending similar movies to that ‘A’ has had in his/her past preferences. This is executed by finding every pair of items that were rated/viewed/liked/clicked by the same user, then measuring the similarity of those rated/viewed/liked/clicked across all user who rated/viewed/liked/clicked both, and finally recommending them based on similarity scores.
    Advantages :- unlike people taste movie doesn't change, there are usually a lot fewer items than people, shilling attacks are much harder because item can not be faked
