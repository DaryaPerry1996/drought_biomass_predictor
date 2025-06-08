# Drought Biomass Random Forest Regresssor

## Introduction
### Background
In the Mediterranean climate, plants have evolved under conditions of low soil-water and nutrient availabilities and have acquired a series of adaptive traits that, in turn exert strong feedback on soil fertility, structure, and protection. As a result, plant-soil systems constitute complex interactive webs where these adaptive traits allow plants to maximize the use of scarce resources.( Sardans et al. 2013) . The long-term evolutionary adaptation to drought of Mediterranean plants allows them to cope with moderate increases of drought without significant losses of production and survival in some species.
Mediterranean-type climates are defined by temperate, wet winters, and warm or hot dry summers, winter storms bring precipitation and the summers are dry. (Seager et al. 2019)
All Mediterranean Regions are overall semiarid as a result of the highly seasonal precipitation and long dry summers and all struggle with water resources at the best of times. Lying between the more arid subtropics and the more humid extratropics they are locations of impactful climate variability and are highly vulnerable to intense and protracted droughts (e.g., Hurrell 1995; Smith et al. 2000; Risbey et al. 2009; Seager et al. 2014a; Cook et al. 2016; Garreaud et al. 2017).
The effects of climate change on Mediterranean ecosystems are profound and multifaceted, impacting soil moisture, pasture productivity  and biogeochemical cycles. These changes threaten the sustainability and functionality of these ecosystems, necessitating urgent attention and adaptive management strategies.
Rising global temperatures have led to decreased soil moisture, particularly in Mediterranean regions, which is critical for crop growth and ecosystem stability (Huang et al. 2024). The reduction in soil moisture can lead to increased aridity, affecting plant health and agricultural productivity.
 Climate change is altering the productivity and nutritional quality of pastures in Mediterranean silvopastoral systems, with increased temperatures and reduced rainfall negatively impacting biomass and nutrient composition(Martins-Noguerol et al., 2023).
Mediterranean forests are experiencing disruptions in carbon, nitrogen, and phosphorus cycles due to combined effects of drought and warming, leading to significant ecological consequences(Serrano et al. 2023). These changes can alter nutrient availability and soil organic matter, impacting overall ecosystem functioning.
### Projected changes:
The Mediterranean region is one of the most responsive areas to climate change and was identified as a major “hot-spot” based on global climate change analyses.
The Mediterranean has long stood out in successive generations of global climate models (GCMs) as being particularly sensitive to rising concentrations of greenhouse gases. Models overwhelmingly project, across all scenarios, a large reduction in precipitation, more than in other land regions in relative terms (Fig. 1b) (Giorgi and Lionello 2008; Planton et al. 2012). A large part of that decline occurs during winter, with enhanced drying over northwestern Africa [from 230% to 240% in December–February (DJF) precipitation] and the eastern Mediterranean (from 220% to 225%). In summer, significant warming and drying is also projected for the northern Mediterranean (Brogli et al. 2019).
All models predict a steady and significant warming across all study areas, accompanied by moderate changes in total annual precipitation, though with some seasonal variations. Future drought patterns in the Mediterranean region were analyzed based on the maximum duration of heat waves, their peak temperatures, and the number of consecutive dry days. The findings indicate an expected increase in both the duration and intensity of heat waves, as well as a rise in the maximum number of consecutive dry days across most study areas. (Valeria Todaro et al., 2022)
The projected impacts of climate change pose significant risks to both societies and the environment in the Mediterranean region. A decline in future precipitation combined with increased evapotranspiration could easily trigger critical water shortages, especially in areas where water resources are already at precarious levels (Iglesias et al. 2007; García-Ruiz et al. 2011). Rising temperatures associated with climate change are expected to affect human health (Diffenbaugh et al. 2007), disrupt plant life cycles (Gordo and Sanz 2010), and elevate fire risk (Moriondo et al. 2006). Of particular concern are the consequences for agriculture, with studies highlighting potential reductions in crop yields and food security (Iglesias et al. 2011; Bindi and Olesen 2011; Tanasijevic et al. 2014; Saadi et al. 2015). In essence, climate change is likely to decrease the availability of crucial ecosystem services (Schröter et al. 2005).
While the evidence highlights the severe impacts of climate change on Mediterranean ecosystems, it is also essential to consider the potential for adaptive management strategies that could mitigate these effects and promote ecosystem resilience. Understanding the nature and effect of Climate relations on mediterranean ecosystems is crucial in order to develop such strategies.
### Random Forest and other ML Models:
Machine learning models are highly useful in understanding the effects of climate on biomass due to their ability to handle complex datasets, integrate diverse variables, and provide accurate predictions. These models can effectively analyze the intricate relationships between climate variables and biomass, offering insights that traditional methods may not capture.
 Machine learning models, such as random forests and support vector machines, can manage large datasets with numerous variables, including both biotic and abiotic factors, which are crucial for accurate biomass estimation( e.g: Huntington et al. 2020 , Liu et al. 2023 , Xiao He et al. 2022 ·)
These models have demonstrated high accuracy in predicting biomass under various climate scenarios. For instance, random forest models have been used to predict sorghum yields and forest biomass with high precision, considering factors like greenhouse gas emissions and irrigation practices (e.g:  Huntington et al. 2020 , Xiao He et al. 2022, · Ghosh et al. 2018 )
These characteristics make random forest regressors an excellent candidate for providing Insights into Climate-Biomass Relationships.
This study aims to examine the effects of climate factors (temperature, rainfall patterns)  under the different drought treatments and categorize complex relations between climate factors on above-ground biomass in Mediterranean climate . More specifically, our study focuses on achieving the following objectives: (1) to utilize a random forest regressor model to predict above-ground biomass (2) to extract influental climate  factors and describe the nature of their influence.
## Materials and Methods:
Biomass data from 2002-2010:
Biomass samples were cultivated in plots in the matta rainout shelters under three different drought treatments I,C,D. During this time period the biomass was harvested in 15 plots (5 per treatment) with 10 replications per plot, each replication is a 20 x 20 cm quadrate within the plots.
Treatment I was irrigated 33% more then the natural precipitation.
Treatment C received the naturally occurring precipitation.
Treatment D received 66% of the naturally occurring precipitation ( 33% of the plot was covered such that only 66% of rainfall reached the plots)
Biomass data from 2011-2017- The samples were collected from rainout shelters under three different treatments I,C,D this data did not include the individual samples but rather the mean of all plots and replications per year per treatment.
Biomass data from 2018-2024: the samples were collected from rainout shelters under four different treatments  D,D66-HF,D66-LF,C from 2018 until 2021(treatments D66-HF,D66-LF were not used in the final training of the model) . from 2021 all D treatments were changed to D66 treatments. During this time period the biomass was harvested in 5 Blocks with 4 plots(Treatments) per Block 5 Replications per plot (one treatment per plot or 4 treatments per block). 
Treatment D66 recieved 33% of the naturally occurring precipitation( 66% of the plot was covered such that only 33% of rainfall reached the plots)
The biomass samples were harvested yearly in April then dried and weighed in the lab.

##Relation of annual above ground biomass measurements with varying Drought condition :
![image](https://github.com/user-attachments/assets/2a946101-e390-46bc-8fa8-632d5448b3a2)

 
As can be seen in the above plot the relation between the level of drought and the biomass cannot be described in a linear formula. 
(add the total reduction of biomass to see that there exists a cause effect relationship)
This study aims to uncover the nature of influence and the effects of climate factors (temperature, rainfall patterns) on the biomass results.
##Meteorological data and Climatic indices:
2021-2024: field measurements from Matta (from Zentra Cloud database). This dataset contains hourly VPD (vapor pressure deficit)(Kpa), temp(C°), precipitation(mm), this was reformatted into a dataset containing daily minimum maximum and average values of temperature and daily total precipitation and maximum precipitation rate
2003-2014 : field measurements from Matta. This dataset contains daily precipitation (mm) and daily average minimum and maximum temperature (C°) and daily relative humidity (RH) (%) measurements. The RH measurements were recorded only from 2011.
2014-2021: due to some gaps in the Matta meteorological database, these climate indices were extracted from Rosh Tzurim and Tzur Hadassa meteorological stations located near the Matta plots.
Using linear regression we received the following correlation between average temperatures in Matta and average temperatures in Rosh Tzurim:

![image](https://github.com/user-attachments/assets/389aa484-e8ee-4a8b-9b69-cd101687bd27)

We supplemented the missing temperature values from 2014-2020 in the matta data from Rosh Tzurim hourly average temperature values, these were adjusted according to the transformation extracted from the linear regression. The average temps and daily min max temps were extracted from hourly temperature values of each day.
Using linear regression we received the following correlation between daily precipitation in Matta and daily precipitation in Tzur Hadassa:

 ![image](https://github.com/user-attachments/assets/012c1d4c-145c-449a-934a-02139f2c128f)

We supplemented the missing precipitation values from 2014-2020 in the matta data from the Tzur Hadassah daily precipitation values, these needed to be adjusted according to the transformation extracted from the linear regression, this we applied after yearly aggregation.
Using linear regression we received the following correlation between relative humidity in matta and relative humidity in Rosh Tzurim:

  ![image](https://github.com/user-attachments/assets/fac4ff47-4510-4b3d-a189-a0a57840a02b)

We supplemented the missing RH values in the Matta data, from 2004-2011 and from 2015-2020 with the relative humidity in Rosh Tzurim after transformation according to the equation extracted from the linear regression.
###VPD Climate Indice:
Air can only hold a certain amount of water vapor at a given temperature before it starts condensing back to liquid water (in forms such as dew or rain). The maximum amount of water vapor that air can hold at a certain temperature is called “saturation vapor pressure” or SVP. First we calculate svp as follows:
![image](https://github.com/user-attachments/assets/0672da68-4c8f-4f9a-bf9f-643fede65ec1)

Similarly, the current actual amount of water vapor in the air is called the “actual vapor pressure” or AVP.
AVP / SVP x 100 = RH%
RH is the proportion of water the air is currently holding vs. its maximum capacity. This is defined as “Relative” humidity.
thus we can calculate AVP from the relative humidity as follows:
AVP= (RH x SVP)X1/100
the vapor pressure deficit is the difference between the actual vapor pressure and the maximum vapor pressure in the air at the current temp. In general hot air has a higher capacity for vapor retention, its SVP is larger than cold air.
VPD = SVP – AVP
The climate indices were extracted in two different time frames:
•	Hydrological Climate indices: the climate indices calculated only from the hydrological year. The period of time commonly used for which precipitation totals are measured this is the period of time with the highest correlation between precipitation and negligible changes in storage (soil water). We defined a hydrological year from October to April
•	Seasonal climate indices extracted separately according to each season which we defined as follows- Autumn : October-November, Winter: December-February, Spring: March-April
###Combining and Adjusting the data
We combined the Biomass and Climate Data so that every Biomass sample was joined with the climate indices of the hydrologic year preceding its harvest. In a separate dataframe we combined each Biomass sample with the seasonal climate indices of the year preceding its harvest.
After combining the Biomass sample data with the indices of the appropriate time frame we adjusted the cumulative precipitation values and the total rainy days according to each treatment.
3 more indices were calculated:
Drought indice which we defined as the percent of natural precipitation that the sample received.
SDII which is the The Simple Daily Intensity Index (SDII), the average rainfall rate on “wet days” (PPT ≥ 1mm), measured in mm/day, during the period of interest (year, season or month).
###Climate Indices:
For each given time period the following climate indices were extracted:
•	Cummulative precipitation- total sum of all daily precipitation values
•	Simple Daily Intensity Index (SDII):  the average rainfall rate on “wet days” (PPT ≥ 1mm), measured in mm/day, during the period of interest (year, season or month).
•	Average temperature
•	no. of consecutive dry days, defined as days with <1mm precipitation
•	no. of consecutive wet days, defined as days with>1mm precipitation
•	no. of rain events if an rain event was separated by one day from another rain event this was calculated as one rain event in total.
•	Average difference between daily Tmin and Tmax (Daily Temperature Range, DTR)
•	Average VPD (calculated as listed above)
•	Cumulative precipitation of previous year.
•	Drought indice  defined as the percent of natural precipitation that the sample received.

##Training the Random Forest Regressor
We trained two different models and compared them:
•	one model trained on the seasonal climate indices.
•	one models trained on the hydrological yearly climate indices
We used one hot encoding for non numerical values the frequency values this translated categorical data into indicative binary data in this case translated a frequency column into two binary columns frequency NF detailing 1 if the type of frequency was a natural frequency and 0 if not and Frequency HF detailing 1 if the treatment applied was HF and 0 otherwise (the third column LF doesn’t add information and can be extrapolated from the other two columns)
We split the data into test and train data such that the test size was 20% of the total data, then trained and evaluated a random forest regressor on the 4 different data categories during which we ran the model training on several different indice combinations to determine if certain indices negatively effect the models reliability.
##Results
Model trained on Hydrological Indices with only natural frequency treatments:

![image](https://github.com/user-attachments/assets/a8360cbb-bbfd-4b70-8cfd-dafcf921e381)
 
the r-squared was generally maximized when all indices were included
Model trained on Seasonal Indices with only natural frequency treatments:

![image](https://github.com/user-attachments/assets/3bcc9af7-010d-41fe-9e3a-a4aa14a836ad)
 
Descriptive statistical Biomass values for all, training, and validation datasets:
The coefficient of variation of all, training and validation were all close to each other

![image](https://github.com/user-attachments/assets/ce4c61db-2f32-4ea3-a17d-e8b0acc62250)

###Reliability of the models:
All models consistently returned a non negative r-squared value , because of the level of randomness in the model creation this value varies across multiple runtimes but was generally larger then 0.5 in most models. this indicates the models capabilities of explaining over 50% in the variance in biomass. All models were significantly better at predicting the biomass results then using the mean.
The points discussed in conclusions were consistent in all runtimes.
###Feature Importance:
The feature importance was analysed using SHAP and Gini importance,
Gini Importance: The importance of a feature is computed as the (normalized) total reduction of the criterion brought by that feature. The criterion is the Gini impurity, which measures the impurity of a node in a decision tree, with more substantial weight to the most important features. Therefore, Gini importance is also known as the total decrease in node impurity.
SHAP values are a common way of getting a consistent and objective explanation of how each feature impacts the model's prediction.
SHAP values are based on game theory and assign an importance value to each feature in a model. Features with positive SHAP values positively impact the prediction, while those with negative values have a negative impact. The magnitude is a measure of how strong the effect is.
the importance calculated by Gini importance and by SHAP were highly similar. with differences in features of similar importance. the similarity between the two importance calculations can be seen below:

![image](https://github.com/user-attachments/assets/09436bc8-97c0-40fa-9e53-de6153ec82d8)

![image](https://github.com/user-attachments/assets/b64af77f-1de1-41dd-87f8-9cc3b31b54ba)

 
###Feature correlation:
Using Pearsons correlation we analysed the dependence between the different features in the model the results were not indicative of any interaction not easily explained by natural weather behaviour, such as the DTR of spring being correlated to the DTR of winter, or correlations that were improbable such as one between the average temp and the drought treatment applied ,such a correlation is by chance as there is no possible interaction between the two indices. There were also correlations between indices for example SDII and cumulative precipitation which is used in order to calculate the SDII. The following images are the heatmaps graphing the Pearson correlation between the features.

![image](https://github.com/user-attachments/assets/9975180d-4fbf-44e4-8d51-1a42a9ebf581)

 
###SHAP Summary ScatterPlot
Scatter plot explanation: Y-axis indicates the feature names in order of importance from top to bottom. X-axis represents the SHAP value, which indicates the degree of change in log odds. Each point represents a row of data from the original dataset. The colour of each point on the graph represents the value of the corresponding feature, with red indicating high values and blue indicating low values.
For instance, In both of the seasonal scatter plots below we can see in the winter average temperature the blue points, low feature in this case low temperature points correspond to high SHAP values meaning they have a positive effect on biomass and the red points correspond with high temperature values have a negative effect on biomass. Furthermore we can see an opposite directional correlation in the DTR high DTR has a positive effect on biomass and low DTR has a negative effect on biomass.

![image](https://github.com/user-attachments/assets/2bc1dbc1-e499-4e31-8efc-ccd12ac90f5e)

![image](https://github.com/user-attachments/assets/6dec7d59-ec2f-4354-8128-80cba0bbccc3)


 
##Discussion:
###Drought percentage:
During the hydrological periods the drought level had the relatively high feature importance over other models, the correlation is identical in all the models a positive correlation between the percent of natural precipitation and the biomass. This is indicative of the definition of a hydrological year or water year which takes into account months with the highest correlation between precipitation and negligible changes in storage (soil water). The correlation was positive between percent of natural precipitation and Biomass in this model and all other models.
Daily Temperature Range and Average Temperature:
In both hydrological models the daily temperature range was most important consistently and the correlation is a positive correlation, increase in the daily temperature range correlates with increase in the biomass.
In general across all models the Daily Temperature Range had very high or highest significance. From a seasonal perspective the Spring and Winter daily temperature range had highest significance consistently.
Across all models the relationship between the DTR and the biomass was a positive one, increase in the DTR results in increase in the biomass, this gives an indication that during spring and winter months high temperatures followed by low temperatures have a positive effect on biomass whereas an increase in the average winter temperatures was shown to have a negative effect on biomass as can be seen in both the nf and the af seasonal scatterplots. furthermore, we can see that the winter and spring average temp were most significant off all seasonal average temperatures.
###Spring and Winter DTR
in the Seasonal models the Spring DTR and Winter DTR were of high importance consistentl.
Previous Year Precipitation:
In both the hydrological models the previous years precipitation was consistently more important than the current yearly precipitation. This could be because of soil water retention properties which help to minimize the effects of temporary droughts.
###Vapor Pressure deficit:
 In the seasonal models Springs VPD was the most important and in the hydrological model the VPD was similarly important. In the hydrological model the VPD was generally of greater importance then precipitation indices, this could be an indication that the atmospheric water budget has a greater effect than precipitation on the plants hydration.

##Conclusions
To summarize the various models trained on the data showed reliability (R squared generally above 0.5)  and detailed a non linear relation between key climatic features such as Daily temperature range Vapor Pressure Deficit and previous year precipitation. Our results highlight that Biomass in Mediterranean climates is related to these climate variables; and the variance explained by the models greatly increased when including these indices. The relationship between the Biomass and the Climate is a complex one but ML models like this one can be used in order to better determine key factors in this complex relationship. Our model showed the Mediterranean landscape had a relatively strong resilience to drought factors and the feature importance of the drought was not most important in determining biomass. There are many possible biological explanations for this as was detailed such as the evapotranspiration from the plant having a stronger effect than precipitation and the water retention properties of the soil.

