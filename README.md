# Customer Segmentation Project

## 1. Business Case
A global company has experienced a **decline in sales** over the past six months. Despite an **established customer base** and a diverse catalog, revenue has been steadily declining. The marketing team has tried various strategies, such as discounts and general promotions, but these tactics have not been able to stop the decline in sales.

Given this situation, management believes that they should start implementing strategies based on the purchasing **profile of each customer**.

Thus, they have identified an opportunity to apply a **customer segmentation** strategy based on RFM (Recency, Frequency, Monetary Value) analysis with the ultimate goal of improving the company's performance.

![image alt](https://github.com/GeorgeWLZD/customers_segmentation/blob/83c86646cf13101dc99a2701f7d72d6cf74609fe/img/map.jpg)

## 2. Data Structure

This is the dataset with 8 variables about the customer consumption. A sample with 1000 rows can be found in the folder called *data*. This data was preprocessed in order to develop the clustering model.

![image alt](https://github.com/GeorgeWLZD/customers_segmentation/blob/09849241193f78b810668e3fa2cef244f557fad4/img/sample.JPG)

As we see the total dataset has 525461 rows, and we have categorical and numerical data.

![image alt](https://github.com/GeorgeWLZD/customers_segmentation/blob/e26a34fe3c8c6921a5d4129412fd997a1a1a66bb/img/info.JPG)

## 3. Clustering Results

I performed the agglomerative and K-means algorithms to reach a solution, and to find the proper one I used the inertia metric and the silhouette plot. Based on this clustering analysis I identified 4 customer segments, which are the following

#### Newcomers (segment 1, size: 949 | 23%)
- These are customers with low spending and low purchase frequency. However, their high recency indicates they have made a purchase relatively recently. 
- Likely **new customers** or those testing the brand.

#### Casuals (segment 2, size: 848 | 21%)
- This group has **moderate values across all dimensions**. They spend occasionally, purchase somewhat frequently, and have a moderate recency. 
- They are engaged at a basic level but have **untapped potential**.

#### At-Risk (segment 3, size: 2000 | 49%)
- These customers have low spending and frequency, but their moderate recency indicates they are **still somewhat engaged**. 
- They are on the verge of becoming inactive and require attention to **prevent churn**.

#### Big Spenders (segment 4, size: 270 | 7%)
- These are the **most valuable customers**. They spend a lot, purchase frequently, but their low recency indicates they haven’t made a recent purchase. 
- They are **highly loyal** but at risk of disengaging if not re-engaged.

Here we can **visualize the profiles** of each segment:

![image alt](https://github.com/GeorgeWLZD/customers_segmentation/blob/c26057d3d4c90e8f58dc4011029b13208979f752/img/segments.png)

## 4. Business Recommendations

#### Develop Newcomers segment
- Implement **onboarding campaigns** to introduce them to the brand’s value.
- Use **cross-selling** or upselling strategies to encourage larger and more frequent purchases.
- Provide **personalized promotions** tied to their initial purchase to build loyalty early on.

#### Develop Casuals segment
- Encourage more frequent purchases by offering **targeted discounts** or **limited-time offers**.
- Introduce them to a **loyalty program** to incentivize higher spending.
- Provide **product bundles** or curated recommendations based on past purchases to spark their interest.

#### Reignite At-Risk segment
- Launch **win-back campaigns** with special offers like “We miss you!” or personalized discounts to reactivate them.
- Explore their **past purchase behavior** to craft tailored recommendations.
- Use incentives, such as ****free shipping** or **discounts**, to motivate immediate action.

#### Focus on Big Spenders segment
- Create exclusive **VIP programs** offering early access to products, premium discounts, or **personalized rewards**.
- Send **tailored reminders** showcasing new products or promotions to reignite interest.
- Conduct **surveys** or **feedback requests** to understand why their activity has declined and take corrective action.
