# Machine-Learning-models-for-Flight-Price-Analysis

## Table of contents
* [Motivation](#Motivation)
* [Aim](#Aim)
* [Introduction](#Introduction)
  * [Problem Statement](#problem-statement)
  * [Dataset description](#dataset-description)
* [Methodology applied](#methodology-applied)
  * [Libraries used](#libraries-used)
  * [Data exploration](#data=exploration)
  * [Feature selection](#feature-selection)
  * [Model creation](#model-creation)
    * [Random Forest regressor](#random-forest-regressor)
    * [Decision Tree regressor](#decision-tree-regressor)
    * [Linear Regression](#linear-regression) 
  * [Cross Validation](#cross-validation)
* [Results exercepts](#code-exercepts)
* [Conclusion](#conclusion)
* [Acknowledgments](#acknowledgments)


## Motivation

To step into the world of data science and machine learning, I aimed to work on basic machine learning models and the other stages required for the same. The motivation arose after viewing various data driven insights that were uncovered from Kaggle notebooks people worked on. Adding to this, people used the same dataset to deliver different results which piqued my interest and I wished to work with the data as well.

## Aim

I worked on a dataset <a href="https://www.google.com/" target="_blank">Google</a>





|Airline                          |Date_of_Journey|Source  |Destination|Route                            |Dep_Time|Arrival_Time|Duration|Total_Stops|Additional_Info             |Price|
|---------------------------------|---------------|--------|-----------|---------------------------------|--------|------------|--------|-----------|----------------------------|-----|
|IndiGo                           |24/03/2019     |Banglore|New Delhi  |BLR → DEL                        |22:20   |01:10 22 Mar|2h 50m  |non-stop   |No info                     |3897 |
|Air India                        |1/05/2019      |Kolkata |Banglore   |CCU → IXR → BBI → BLR            |05:50   |13:15       |7h 25m  |2 stops    |No info                     |7662 |
|Jet Airways                      |9/06/2019      |Delhi   |Cochin     |DEL → LKO → BOM → COK            |09:25   |04:25 10 Jun|19h     |2 stops    |No info                     |13882|
|IndiGo                           |12/05/2019     |Kolkata |Banglore   |CCU → NAG → BLR                  |18:05   |23:30       |5h 25m  |1 stop     |No info                     |6218 |
|IndiGo                           |01/03/2019     |Banglore|New Delhi  |BLR → NAG → DEL                  |16:50   |21:35       |4h 45m  |1 stop     |No info                     |13302|
|SpiceJet                         |24/06/2019     |Kolkata |Banglore   |CCU → BLR                        |09:00   |11:25       |2h 25m  |non-stop   |No info                     |3873 |
|Jet Airways                      |12/03/2019     |Banglore|New Delhi  |BLR → BOM → DEL                  |18:55   |10:25 13 Mar|15h 30m |1 stop     |In-flight meal not included |11087|
