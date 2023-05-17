# **Title: Customer Segmentation project**   

 
## **Team Members:**   

*Group 07*     

BAHRAMI MAZIYAR (maziyar.bahrami@studenti.luiss.it)  
REZAEI NILOOFAR (niloofar.rezaei@studenti.luiss.it)  
ZHUMAKAN AITGUL (aitgul.zhumakan@studenti.luiss.it)  


 
## **Introduction:**  
The goal of this project is to segment customers using the RFM (recency, frequency, monetary value) strategy in order to create personalized and relevant marketing messages that result in increased sales and customer loyalty. We will use the provided dataset, which includes information on orders, customers, sellers, payments, products, and geolocation data, to identify the optimal number of segments and assign each user to one of them. By understanding different customer segments, businesses can personalize their marketing messages and improve customer engagement, satisfaction, and loyalty.

## **Methods:**  
  
 
- i. Design Decisions:  

  - RFM Analysis: We chose RFM analysis as the primary method for customer segmentation because it captures key aspects of customer behavior: recency, frequency, and monetary value. These factors are crucial in understanding customer engagement, loyalty, and potential value to the business.  
 
  - Quintile Method: We opted to use the quintile method for customer segmentation to create distinct segments based on equal-sized groups. This approach allows for easy interpretation and practical implementation, making it suitable for businesses aiming to develop targeted marketing campaigns.  

  - K-means Clustering: In addition to the quintile method, we also decided to deploy k-means clustering as an alternative method for customer segmentation. K-means clustering is an unsupervised machine learning algorithm that can identify more nuanced customer segments based on their RFM scores. It provides flexibility in defining the number of clusters and allows for more granular insights into customer behavior and preferences.  

  - Determining the Optimal Number of Clusters: We used the elbow method and silhouette estimation to determine the optimal number of clusters. The elbow method determines the inflection point, and the silhouette score measures the compactness and separation of clusters.  

  - Applying K-means Clustering: After determining the optimal number of clusters, we applied the k-means clustering algorithm to group clients based on their RFM scores. Each client was assigned to one cluster based on its similarity to other clients within the same cluster.  
  
  
## **Experimental Design:**
					
- i. Main purpose: The main purpose of the experiments is to validate the effectiveness of the customer segmentation approach (RFM analysis and clustering) in improving business outcomes such as customer engagement, conversion rates, revenue generation, customer retention, and customer satisfaction.							
- ii.	Baselines:To compare our work with baselines, we used the K-means clustering algorithm as the main method for customer segmentation. This allowed us to create distinct clusters based on RFM scores and analyze the characteristics of each cluster. We compared the results of our clustering approach with the baselines to evaluate the effectiveness of our method in identifying meaningful customer segments. Additionally, we utilized statistical tests or evaluation metrics to measure the quality of the clustering results, such as the Silhouette Score.

- iii. Evaluation metrics  

  In our project, we employed the Silhouette Score as the primary evaluation metric for assessing the quality of our clustering algorithm. The      Silhouette Score measures both the cohesion and separation of the clusters by calculating the average silhouette coefficient for each data point. This coefficient represents how well the data point belongs to its own cluster compared to other clusters. The Silhouette Score ranges from -1 to 1, with higher values indicating better-defined and well-separated clusters.  
  We chose the Silhouette Score because it provides a comprehensive evaluation of the clustering algorithm by considering both the within-cluster similarity and between-cluster dissimilarity. It allows us to assess the overall effectiveness of the clustering algorithm in creating distinct and meaningful clusters. Higher Silhouette Scores indicate better clustering results, with values close to 1 indicating well-separated clusters and values close to -1 indicating poor clustering.  
  Additionally, we utilized the Calinski-Harabasz index as another evaluation metric. The Calinski-Harabasz index measures cluster cohesion and separation by calculating the ratio of between-cluster dispersion to within-cluster dispersion. A higher Calinski-Harabasz score indicates better-defined and well-separated clusters.  
  We used the Calinski-Harabasz index because it provides a quantitative measure of clustering performance. By comparing the index values for different numbers of clusters, we can determine the optimal number of clusters that maximize the separation and cohesion of the clusters. This helps in identifying the most meaningful and distinct customer segments in the dataset.  
  Using the Silhouette Score and Calinski-Harabasz index as evaluation metrics allows us to objectively assess the quality of the clustering results and make informed decisions about the number of clusters to use in our analysis. 
  
     
## **Results:**  
   
   
- i. The experiment was conducted using two different values for the number of clusters, k=3 and k=4. Both configurations showed promising results, but k=4 performed slightly better in terms of clustering quality and interpretability. The results are as follows:  
  - For k=3, the Silhouette score was 0.3612 and the Calinski score was 6032.31.   
  - For k=4, the Silhouette score improved to 0.3799, and the Calinski score increased to 6588.11.
    
  Higher Silhouette and Calinski scores indicate better clustering performance. Although the difference between the scores is not substantial, the     model with k=4 yielded slightly better results in terms of cluster separation and cohesion. Additionally, the clusters for k= 4 is more     intrepretable that it will be considered.

- ii. Customer Segmentation: The RFM analysis and clustering algorithm successfully segmented customers into distinct groups based on their recency, frequency, and monetary value.

  - High-Value Segment: Cluster 3 represents the high-value segment with the highest monetary value and purchasing amounts. These customers are likely to be the most valuable to the company and should be a focus for retention and loyalty programs.

  - Engagement Differences: Clusters 1 and 2 show similar frequency and monetary value characteristics. However, Cluster 2 consists of customers who have made more recent purchases compared to Cluster 1. This indicates that Cluster 2 customers are more engaged and may have a higher potential for upselling, cross-selling, or targeted marketing campaigns.

  - Lost Customers: Cluster 0 can be considered as the "Lost Customers" segment since they have the lowest recency and monetary value. These customers may require re-engagement strategies or specific approaches to win them back.

   By analyzing the results of customer segmentation, businesses can tailor their marketing strategies to each cluster, optimize customer engagement, and maximize revenue generation by focusing on high-value customers, engaging with active customers, and implementing targeted campaigns for specific segments.
  
    
    
## **Conclusions:**

Our work focused on RFM analysis and customer segmentation using clustering techniques. Through this project, we have demonstrated the value of understanding customer behavior and utilizing segmentation strategies to optimize marketing efforts and improve business outcomes. By tailoring strategies to different customer groups, businesses can enhance customer satisfaction, increase customer retention, and generate higher revenues.
  
The key takeaway from our work is that RFM analysis and segmentation provide valuable insights into customer behavior. However, it is important to note that our analysis solely relied on RFM scores and did not consider other demographic or behavioral factors that could further enhance customer segmentation. Incorporating additional data such as customer demographics, purchase history, and website interactions could provide a more comprehensive understanding of customer behavior and preferences.
  
Furthermore, while we determined that four clusters were optimal for this particular dataset, further exploration and experimentation can be conducted to determine the most suitable number of clusters for different datasets and business contexts.  

In conclusion, our work has laid the foundation for customer segmentation and personalized marketing strategies based on RFM analysis. However, there are ample opportunities for further refinement and expansion. By incorporating additional data sources, exploring advanced machine learning techniques, and conducting empirical studies to validate the proposed strategies, businesses can continually improve their customer segmentation approaches and foster long-term customer relationships in an increasingly competitive landscape.






  



				













