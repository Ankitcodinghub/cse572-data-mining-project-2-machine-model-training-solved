# cse572-data-mining-project-2-machine-model-training-solved
**TO GET THIS SOLUTION VISIT:** [CSE572: Data Mining Project 2: Machine Model Training Solved](https://www.ankitcodinghub.com/product/cse572-data-mining-project-2-machine-model-training-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;67000&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;4&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (4 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSE572: Data Mining Project 2: Machine Model Training Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (4 votes)    </div>
    </div>
<h2>Purpose</h2>
In this project you will use a training dataset to train and test a machine model. The purpose is to distinguish between meal and no meal time series data.

<h2>Objectives</h2>
Students will be able to:

<ul>
<li>Develop code to train a machine model.</li>
<li>Assess accuracy of machine model.</li>
</ul>
&nbsp;

<h2>Technology Requirements</h2>
Python 3.6 to 3.8 (do not use 3.9).&nbsp; scikit-learn==0.21.2 pandas==0.25.1

Python pickle

<h2>Project Description</h2>
In this project you will train a machine model to assess whether a person has eaten a meal or not eaten a meal.&nbsp; A training data set is provided.

<h2>Directions</h2>
Meal data can be extracted as follows:

From the InsulinData.csv file, search the column Y for a non NAN non zero value. This time indicates the start of meal consumption time tm. Meal data comprises a 2hr 30 min stretch of CGM data that starts from tm-30min and extends to tm+2hrs.

No meal data comprises 2 hrs of raw data that does not have meal intake.

Extraction: Meal data

Start of a meal can be obtained from InsulinData.csv. Search column Y for a non NAN non zero value. This time indicates the start of a meal. There can be three conditions:

<ul>
<li>There is no meal from time tm to time tm+2hrs. Then use this stretch as meal data</li>
<li>There is a meal at some time tp in between tp&gt;tm and tp&lt; tm+2hrs. Ignore the meal data at time tm and consider the meal at time tp instead.</li>
<li>There is a meal at time tm+2hrs, then consider the stretch from tm+1hr 30min to tm+4hrs as meal data.</li>
</ul>
Extraction: No Meal data

Start of no meal is at time tm+2hrs where tm is the start of some meal. We need to obtain a 2 hr stretch of no meal time. So you need to find all 2 hr stretches in a day that have no meal and do not fall within 2 hrs of the start of a meal.

&nbsp;

Handling missing data:

You have to carefully handle missing data. This is an important data mining step that is required for many applications. Here there are several approaches: a) ignore the meal or no meal data stretch if the number of missing data points in that stretch is greater than a certain threshold, b) use linear interpolation (not a good idea for meal data but maybe for no meal data), c) use polynomial regression to fill up missing data (untested in this domain). Choose wisely.

&nbsp;

Feature Extraction and Selection:

You have to carefully select features from the meal time series that are discriminatory between meal and no meal classes.

&nbsp;

Test Data:

The test data will be a matrix of size N×24, where N is the total number of tests and 24 is the size of the CGM time series. N will have some distribution of meal and no meal data.

Note here that for meal data you are asked to obtain a 2 hr 30 min time series data, while for no meal you are taking 2 hr. However, a machine will not take data with different lengths. Hence, in the feature extraction step, you have to ensure that features extracted from both meal and no meal data have the same length.

Output format:

You have to output an N×1 vector of 1s and 0s, where if a row is determined to be meal data, then the corresponding entry will be 1, and if determined to be no meal, the corresponding entry will be 0.

This vector should be saved in a “Result.csv” file.

&nbsp;

Given:

Meal Data and No Meal Data of subject 1 and 2

Ground truth labels of Meal and No Meal for subject 1 and 2

&nbsp;

Using Python, train a machine model to recognize whether a sample in the training data set represents a person who has eaten (Meal), or not eaten (No Meal). The training data set contains ground truth labels of Meal and No Meal for 5 subjects.

You will need to perform the following tasks:

<ol>
<li>Extract features from Meal and No Meal training data set.</li>
<li>Make sure that the features are discriminatory.</li>
<li>Train a machine to recognize Meal or No Meal data.</li>
<li>Use k fold cross validation on the training data to evaluate your recognition system.</li>
<li>Write a function that takes a single test sample as input, and outputs 1 if it predicts the test sample as meal or 0 if it predicts test sample as No meal.</li>
</ol>
&nbsp;

<h2>Submission Directions for Project Deliverables</h2>
Two python files: a) train.py and b) test.py

The train.py reads CGMData.csv, CGM_patient2.csv and InsulinData.csv, Insulin_patient2.csv, extracts meal and no-meal data, extracts features, trains your machine to recognize meal and no-meal classes, and stores the machine in a pickle file (Python API pickle).

The test.py reads test.csv which has the N x 24 matrix and outputs a Result.csv file which has N x 1 vector of 1s and 0s, where 1 denotes meal, 0 denotes no meal.

Assume that CGMData.csv, CGM_patient2.csv and InsulinData.csv, Insulin_patient2.csv files are all in your compilation and execution folder. Avoid using static paths.

&nbsp;

<h2>Evaluation</h2>
You will be evaluated on your code as well as the accuracy of your results based on a set of Meal and No Meal data that is not included in the training set.

50 points for developing a code in Python that takes the given dataset, extracts Meal and No Meal data and trains a machine model

20 points for developing a code in Python that implements a function to take a test input and run the trained machine to provide the class label as output

30 points will be evaluated on the accuracy, F1 score, Precision and Recall results obtained by your machine. This will be compared against class average to determine the final score.

&nbsp;

&nbsp;
