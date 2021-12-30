# Fraud-Prediction-Pyspark
<ins>Problem Overview</ins>

We intent to see about potential frauds taking in medicare insurance. The total Medicare spending increased exponentially due to frauds in Medicare claims.
Some of the most common types of frauds by providers are:. Duplicate submission of a claim for the same service. Misrepresenting the service provided. 
Charging for a more complex or expensive service than was actually provided. We would see a big data use case to see how pyspark can help in our analysis,
and as well as assists to provide ML computation to predict the fraud cases.

<ins>Approach and Methodology</ins>

- The dataset being in different parts, we wanted to merge them finally in order to get the final dataset. In doing so we used inner joins and thereafter we got the data that we were looking for. It was important to structure the data in pyspark format, in order to use it appropriatelty.
- We used different types of techniques like groupby, describe, different types of plots to assist us in our EDA process. This is an important phase as we want to some insights to our story.
- Pyspark supports .toPandas method which enables us to code in pandas, making EDA quite easier.
- We remove the irrelevant columns to go for modelling, most of the NaN values constituted about 80% in density, hence it was dropped from the dataframe.
- For modelling in Pyspark, we used Vectorassembler to enocde our data, which would help in processing our inputs and finally we use Decision trees to model our data.

<ins>Insights, analysis and Modelling</ins>
- On average approximately $17530 were the reimbursments in insurance that has been claimed by many customers. This amount constitutes to both Fraud and Non fraud cases.
- Different procedures had different no. of fraud cases where 9904 and 8154 (data code is encoded to mantain confidentiality) had the highest amount of frauds, also these cases constitute to Surguries, medical visits etc.
- Most fraudlent cases were observed for age range above 65, this explains the fact that older people are getting targeted for such cases more. Also, this is in case of medicare insurance, but in general there are many scams, phishing activities etc, which is targetting the section of this age range of people in the US.
- Most of the beneficiary details are for Race 1. 80% beneficiaries are of same race which is Race 1 which means Maximum population in the dataset originated from this race.
- Our intent for modelling was to apply a classification based algorithm to assit in the predicting the fraud cases, provided that we have the required parameters for the same. Hence, we used decision trees to assit in the modelling phase. We could have went for different approaches like going for boosting techniques, hyperparameter tuning, cross validations etc. but the objective was to learn how a classification algorithm can be used in Pyspark.

<ins>Future Scope</ins>
- With organization seeking help in need of open-source solutions, the program when integrated to live databases, would be able to track such cases which will help real time risk management. 
- A business intelligence tool, with support of Python scripts, can help in creation of dashboards, that will help the particular user /organization to keep a record and monitoring of NPA’s/such cases with ease.
- Classifying and forecasting the frauds based on the timelines, due which more standardization of such cases can be done and assisting in effective time series analysis

<ins>Summary/Conclusion</ins>

We do see a no. of frauds that has taken place in regard to different diagnosis and claims as well as we see a uncommon age range being targeted for the same. In context to what we understand is to have a well informed and a capability to have some decision support in order to foresee how frauds can be tackled. If a firm for instance has a history of piled up data, being inclined to a big data requirement, we have pyspark to assist in the computational feasibility of it and we see how addition of MLlib provides a decisional based support to predict the fraud cases. Risks, frauds are quite common these days and an effective risk management framework can help organizations to make better decisions to prevent and minimize such instances.
