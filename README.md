# Capstone
## Final Project of Data Intensive Applications

### The Relationship Between Obesity and Internet Use

                                              Gizem Kaya, Necdet Alperen Özil

  Determination and interpretation of the relationship between the percentage of obese people received from 200 countries between 1975 and 2016 and the percentage of people using the internet. We expect the relationship between these two features to be a linearly increasing correlation. Because we think that using the internet and technology together reduces the need for people to move. In this project, we investigated the emergence of the lack of movement, the main cause of obesity, with the spread of the internet and technology.

1. Table of Content
2. Problem
3. Data Understanding
4. Data Preparation
5. Modeling
6. Evaluation
7. References

##### Problem 

The growth and development speed of the world is accelerating day by day. This growth benefits us in terms of technological and increasing the quality and length of human life.

> For example, psychological counseling with internet connection can be very useful for an individual who is impossible to leave home.

However, although we think that the solution of many problems is effective, we should not forget that sometimes there may be side effects. The fact that the Internet brings distant things closer to us has made it easier for people not only in the field of health but also in many business areas. But, this not only facilitated the achievement of hard-to-achieve things, but also reduced the effort that people exerted to achieve them.

> For instance, people working remotely among countries can earn money without ever leaving their homes. Or when we want to see a friend, we can see his face without going to him or her.

These are the privileges that come to our feet thanks to the internet, without any long or tiring effort. But we know that acting is inherent in nature, benefiting human health and prolonging life by reducing heart conditions. Obesity is one of the main diseases that have been on the agenda for the last 10 years and emerged as a result of inactivity. We think obesity is caused by immobility, poor quality meals and eating too much food. We know that the use of the Internet completely fills our free time with the principles of social media and remote work. So much so that sometimes we don't have enough time to eat or eat. So we order fast food 'online' to meet our food needs. Although these fast food foods look great, we get hungry again and want to eat again because they are of poor quality. Thus, we both eat a lot and eat high-carb meals on the effect of the internet on us. Organizing eating habits in this way may cause obesity.

In the light of these thoughts, we tried to show the connection between countries by comparing the number of citizens who are obese with internet usage by years.

##### Data

We will use 3 different datasets in this project. The first is Internet Users, the second is Population, and the third is Obesity datasets.

Internet Users, that we found at The World Bank, includes percentage of the total number of people using the internet in 264 countries, with a separate representation for each year from 1960 to 2019. If we look at the data, we see that most of the data in the Internet Users dataset earlier than 2000 is missing. This deficiency also caught our attention when searching for a dataset, but it seemed reasonable that the Internet was not used at that time.
Population dataset, that we found at The World Bank, contains the population of in 264 countries between 1960 and 2019. If we look at the Population dataset, we can see the appearance of the Population and the Internet Users dataset are similar. Because the sources from which datasets are provided are the same. This means we can easily make operations on them.

Because some countries have few populations, the percentage of people using the internet may not yield reliable results about that country. For example, in 2000 the percentage of internet users of a country with a population of 100,000 was 80% does not indicate that the country is a very developed country. When we look at countries that could not have a population of more than 100,000 people by 2016, we often see that those countries are either newly established or underdeveloped. We will remove these countries because we think these countries are the outliers of our work.

Obesity dataset, that we found at Global Health Observatory Data Repository, shows the ratio of obese population of 195 countries of all years from 2016 to 1975 to real population by making gender discrimination in individuals over the age of 18. Since our other datasets are not seperated by gender, we will only use the column that applies to both sexes out of 3 columns that are male, female and both sexes. However we don't have a The data type of this dataset is percentage of defined population with a body mass index (BMI) of 30 kg/m2 or higher. And this data is calculated with Worldwide trends in body-mass index, underweight, overweight, and obesity from 1975 to 2016: a pooled analysis of 2416 population-based measurement studies with 128.9 million participants.
