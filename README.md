# DECISION MAKING DURING COVID19
![umbrella-1588167_640](/assets/umbrella-1588167_640.jpg)
This project is based on an current unpublished research on human decission making during COVID19 outbreak. The study has been carried out in five countries and it is currently collecting data in several other countries. 

The success of humanity is widely attributed to our species’ inordinate capability and motivation to engage in cooperative activities. Virtually all of our most important and complex achievements –language, technology, social institutions –are the product of individuals cooperating with each other. The maintenance of cooperation in large groups of unrelated individuals, such as human societies, is only possible thanks to social norms that regulate behaviour among group members and are shared by all members (Richerson et al., 2016; Tomasello & Vaish, 2012). From very early in development, humans are not only willing to endorse social norms, but crucially to punish violators of norms. Indeed, according to many scholars, both conformity to norms and third-party punishment are responsible for the evolution and stabilization of cooperation among humans.  
![team-386673_640](/assets/team-386673_640.jpg)


## TOPIC

The present project selected a part of the dataset in order to focus on how individuals’ cooperation tendency and group cohesion are influenced by the current situation of fear (to get ill, to suffer) and uncertainty (loss of control). 

The main predictor variable(target) is the psychological state generated by the COVID19 outbreak.

The former dataset was composed of samples from 5 different countries in which data were collected on: 

- Atruistic behavior
- Third party punishment
- Conformity to norms 
- Social decission making.

Here I analysed Individualistic and Collectivistic orientation in four different contexts, as I expose below.

## OBJECTIVES

Explore to what extent the individuals’ cooperation tendency and group cohesion are influenced by the current situation of fear (to get ill, to suffer) and uncertainty (loss of control) in different countries.

## METHODS

### The Dataset
The original dataset was composed by 563 datapoints with 51 behavioural measures, once the objectives were setted, the dataset was cleaned and treated by using [Pandas](https://pandas.pydata.org/) and [Numpy](https://numpy.org/).

### Features(VD) and Targets (VI)

The features to be analysed are the type of orientation, Collectivistic vs Indivdualistic, that individuals adopt under the four situations that were presented to the subjects:

**Targets**

- Small Scale Dilemma Neutral
- Small Scale Dilemma with COVID19
- Large Scale Dilemma Neutral
- Large Scale Dilemma with COVID19

**Features**

- Living country (categorical)
- Age (numeric)
- Children (ordinal)
- Education_Cat (ordinal)
- Job (categorical)
- Risk perception (ordinal-Likert)
- Conformity (numeric)

### Data Anayses and Visualization

The following technologies were used to explore and analyse data:

**MACHINE LEARNING MODELS AND STATISTICS**

Machine learning models with [Sckit-Learn](https://scikit-learn.org/stable/) and Stats with [Scipy](https://www.scipy.org/).
<ol>
<li>Supervised Machine Learning Models: To predict behaviors for each situation proposed</li>
<li>Multilabel Machine Learning Model: To test whether there is a model capable to predict behavior under four different situations</li>
<li>Unsupervised Machine Learning Model for one target: To test whether an unsupervised model was capable to classify behavior better than a supervised under the fourth situation (Large-scale Covid19)</li>
<li>Statistical Analyses: Fisher Exacts' test</li>
</ol

**Machine Learning Models were tested with responses from collegues, as we will see in results**

**DATA VISUALIZATION:**

* [Tableau](https://www.tableau.com/)
* [Plotly](https://plotly.com/) with [Dash](https://dash.plotly.com/) apps 
* [Matplotlib](https://matplotlib.org/)
* [Seaborn](https://seaborn.pydata.org/)

## RESULTS
**Machine Learning**
Supervised Classification ML models show that three out of the four conditions can be predicted with the studied models. Multilabel and Unsupervised models did not provide further information.
![Captura de pantalla 2020-08-06 a las 18.44.59](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2018.44.59.png)

**ML models capacity to predict new data were as follows**: 
 
- Small-Scale Neutral model accuracy was of the 0.5
- Small-Scale Covid19 model accuracy raised up to 0.8
- Large-Scale Neutral model accuracy was of 0.9 
- Large-Scale Covid19 model was of 0.6

**Statistical Analyses**
Fisher exacts' Chi Square show that the answers in Small-Scale Covid19 and Small-Scale Neutral were related, and also were those between Large-Scale Covid19 and Small-Scale Covid19,this is that individuals that are be individualistic or collectivistic in one situation tend to be also individualistic in the other situation proposed.



![Captura de pantalla 2020-08-06 a las 19.11.28](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2019.11.28.png)

**Tableau Dashboard** to visualize individualistic and collectivistic orientations by countries (right graph) together with risk perception and conformity punctuation (map on the left): 

![Captura de pantalla 2020-07-29 a las 17.24.45](/assets/Captura%20de%20pantalla%202020-07-29%20a%20las%2017.24.45.png)

**Plotly and Dash apps**

To provide an visual representation of data to researchers I added data visualization with Plotly and Dash to have the best visualization of data: 

![Captura de pantalla 2020-08-06 a las 18.05.51](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2018.05.51.png)

Some examples of the output from Dash:

![Captura de pantalla 2020-08-06 a las 18.03.55](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2018.03.55.png)

This visualization refers to the overall proportion of indivualistic and collectivistic orientation in the four situations studied.



![Captura de pantalla 2020-08-06 a las 18.04.20](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2018.04.20.png)

With these visualizations we can observe individualistic (black) and collectivistic (blue and yellow) reponses of each subject in two out of the four situations studied. Lines refer to the same datapoint (subject) in each item:  country, gender, risk perception, etc. 

![Captura de pantalla 2020-08-06 a las 18.04.49](/assets/Captura%20de%20pantalla%202020-08-06%20a%20las%2018.04.49.png)

Finally these visualizations refer to age (y), conformity (x), risk perception (size of the circle) and individualistic or collectivistic orientations (color). All these graphs are dynamic, individualistic or collectivistic orientations can be selected independently as in the first graph, and additional infromation is provided when clicking on the circles.



## CONCLUSIONS AND FURTHER STEPS

Data from this study come from real world data, which made predictions difficult to pre-evaluate, however results were richer than expected and will probably be used for its final analysis and publication. 

There are differences between individuals in their responeses regarding the situation studied as has been shown in machine learning models, besides two out of the four models were very accurate with new data, which was quite impressive given the small size of the new data(n=10) and the biased sample (collegues from the bootcamp).

Finally chi square showed that some responses are related, there are trends in people that make them give a type of response given the environment, age, children category, perception of risk and conformity variables must be taken into account when analysing these data in depth.

This one week study lacks of deeper statistical analysis that I would like to conduct by using [R](https://www.r-project.org/) language, I did not have time to study R and to conduct them but I have this taks in mind.

For a better performance I plan to create an API by using [FastAPI](https://fastapi.tiangolo.com/) in the next weeks, so researchers will be able to analyse their own data and make predictions with other countries. 
