# social_network_link_prediction

# Problem statement

Most social media platforms, including Facebook, can be structured as graphs. The registered users are interconnected in a universe of networks. And to work on these networks and graphs, we need a different set of approaches, tools, and algorithms (instead of traditional machine learning methods).

The interactions among these entities generate unimaginable amounts of data in the form of posts, chat messages, tweets, likes, comments, shares, etc. This opens up a window of opportunities and use cases we can work on.

That brings us to Social Network Analytics (SNA). We can define it as a combination of several activities that are performed on social media. These activities include data collection from online social media sites and using that data to make business decisions.
The benefits of social network analytics can be highly rewarding. Here are a few key benefits:
1. Helps you understand your audience better
2. Used for customer segmentation
3. Used to design Recommendation Systems
4. Detect fake news, among other things

Link prediction is one of the most important research topics in the field of graphs and networks. The objective of link prediction is to identify pairs of nodes that will either form a link or not in the future

# Facebook Dataset

The data is obtained from the link below.
Data source : https://snap.stanford.edu/data/

These are the statistics of the facebook dataset :-

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/2df4d8cc-ef92-4551-a42c-eb075c7d2d5f)


This is how the dataset preview looks like :-

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/a585ca18-1f30-4f59-926c-1bfb1b0bb12f)


This is how the graph of the above dataset looks like:-
![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/c44adfe0-3753-40e1-ad3c-86bdb0a55cb4)

# Link Prediction Methods


1. Triadic Closure:
If two vertices are connected to the same third vertices, the tendency for them to share a connection is Triadic Closure.

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/7b510115-4193-4601-83be-18be40dddc5b)



2. Jaccard Coefficient:
It is calculated by the number of common neighbours normalised by the total number of neighbours. It is used to measure the similarity between two finite sample sets, and is defined as the size of the intersection divided by the size of the union of the sample sets.

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/27c0cb0e-971e-487e-8e52-8b0ffc394eac)

3. Resource Allocation Index:
It is defined as a fraction of a resource that a node can send to another through their common neighbours. Among a number of similarity-based methods to predict missing links in a complex network, Research Allocation Index performs well with lower time complexity. 

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/2d270d6d-87a5-4dbb-8124-5b66f5c687f7)


4. Adamic Adar Index:
This method is similar to Resource Allocation Index, but assigns lower importance to common neighbours that are more connected.

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/ac1f674f-942e-4047-a7fe-9a66870cb2f3)



5. Preferential Attachment:
Preferential attachment means that the more connected a node is, the more likely it is to receive new links Nodes with higher degree get more neighbours.

![image](https://github.com/smitsekhadiaa/social_network_link_prediction/assets/90528630/2b7a757a-e2c9-4e9a-93e6-89629192829a)


These measures capture different aspects of node similarity and can be used alone or in combination to improve link prediction performance. The choice of the measure depends on the characteristics of the network and the specific goals of the analysis.


# Classification technique through ML models

We can  use similarity based measures as features for classification in ML models.
To improve generalisation and prediction, we can add a set of features like: 
1. jaccard_followers 
2. jaccard_followees 
3. cosine_followers 
4. cosine_followees 
5. inter_followers 
6. inter_followees 
7. adar index 
8. is following back

## ML Algorithms used for classification

1. Random Forest:
2. Support Vector Machine (SVM):
3. Artificial Neural Networks (ANN):


# Applications of Link Prediction
Link prediction has a wide range of applications across various fields where relationships or connections between entities play a crucial role. Some notable applications of link prediction include:

1. Social Networks:
Identifying potential friendships or collaborations between users in social networks.
Recommending new connections to users based on their existing network.

2. Collaboration Networks:
Predicting potential collaborations between researchers, authors, or scientists.
Recommending potential collaborators for academic or research projects.

3. E-commerce:
Recommending products or services based on the purchasing patterns of users.
Predicting potential partnerships or collaborations between businesses.

4. Fraud Detection:
Identifying potentially fraudulent activities by predicting links between suspicious entities.
Detecting anomalous patterns in financial transactions.

5. Online Dating:
Recommending potential matches based on user preferences and behaviours.
Predicting the likelihood of forming a connection between users.

6. Supply Chain Management:
Predicting potential links between suppliers, manufacturers, and distributors.
Optimizing supply chain logistics and relationships.



# Team Members:
1. Dhrumil Raigagla - 201080061
2. Smit Sekhadia - 201080047
3. Pratham Shah - 201080056
4. Rushabh Gala - 201080072


