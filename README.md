# Customer-Analytics
Here I have developed models of customer Analytics. Steps: 1) customer segmentation 2) purchase probability (buy or not buy) 3) brand choice 4) purchase quantity
1) Customer segmentation using PCA (for dimension reduction) and K-means for clustering. customers are clusters into 4 groups.
1.2) Segements by (PCA + Kmeans): 
Segment 0: single and less eduacted people with low income in small cities --> fewer opportunities segment.
Segment 1: almost all men, low education but high income and live in big cities --> career-focused segment.
Segment 2: youngest group with average income and education and married --> standard segment.
Segment 3: highly educated and older people and in a family with high income --> well-off segment.

1.3) features for segmentation: Sex , Marital Status, Education = 1, 2, 3: high school, university, graduate school, Occupation = 0, 1, 2: unemployed, skilled, highly qualified, Settlement size = 0, 1, 2: small, medium, big city.

2) purchase probability: using logistic regression and 2 classes incident = 1 or 0 (buy or not buy). This model can be found in "Purchase Predictive Analytics". Results of different customer segments are also provided.
2.1) Features: mean price of all brands and mean promotion dummy (1 if the brand is on promotion, 0 if not)
2.2) price elasticity results are provided for each segement

3) Brand choice: using multinomial logistic regression to model the customer brand choice. 
3.1) features: prices of 5 brnads. 
3.2) price elasticity results are provided for each segement. moreover, cross elasticity results are provided for brand 5 and its competitor brand 4. in cross elasticity we are interested to evaluate how price change of a competitor brand (brand 4) would affect our own brand (brand 5) purchase probability. In this experiment our price is set to be constant and competitor brand price is variable. Note that formula of cross elasticity is a bit different than own elasticity.
4) Purchase Quantity: predictiong quantity that customer would buy using linear regression.
4.1) features: Price and Promotion
