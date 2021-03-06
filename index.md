---
title       : Modeling Lake Morphometry and Trophic State
subtitle    : Presentation for TNC Lake Classifcation Steering Committee
author      : Jeff Hollister
logo        : epa-seal.png
biglogo     : epa-seal.png
job         : US EPA, Research Ecologist
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
--- &twocol w1:45% w2:55%




## Overview

***=left

1. Lake Morphometry
2. USGS Sparrow
3. Modeling TN, TP, and Chl a 
4. Cyanobacteria Research at EPA

***=right

<img src="assets/img/Lila1.jpg" style="height: 600px;margin-top:-95px;"/>

--- .segue bg:url(assets/img/Lila2_80.jpg)

## Lake Morphometry

--- &twocol w1:50% w2:50%

## Lake Morphometry

***=left

- Northeastern US: Past Work
 - Volume: [Hollister and Milstead, 2010](http://dx.doi.org/10.1080/07438141.2010.504321)
 - Depth: [Hollister et al. 2011](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0025764)
- Rest of Country: Current Work
 - Full Suite of Lake Morphometry
 - Draft for ~380,000 lakes
 - [R package available from Github](https://github.com/USEPA/lakemorpho)
 
***=right

Inlcuded Morphometry Metrics        |
------------------------------------|
Surface Area                        |
Shoreline Length                    |
Shoreline Development               |
Maximum Depth                       |
Mean Depth                          |
Lake Volume                         |
Maximum Lake Length                 |
Mean Lake Width                     |
Maximum Lake Width                  |
Fetch from a specified bearing      |

---

## Basics on Depth


<img src="assets/img/journal.pone.0025764.g002.png" style="height: 600px;margin-left:290px;margin-top:-50px;"/>

--- &twocol w1:48%% w2:48%

## Validation, Correction and Assessment

***=left

Source    |HUC        |Mean Corr  |Mean RMSE (m)  |
----------|-----------|-----------|---------------|
NLA 2007  | 01        |0.82       |5.95           |
NLA 2007  | 02        |0.69       |5.02           |
Web       | 01 & 02   |0  .72     |7.0            |


***=right

<img src="http://www.plosone.org/article/fetchObject.action?uri=info:doi/10.1371/journal.pone.0025764.g003&representation=PNG_L" style="width:100%;">

--- &twocol w1:48%% w2:48%

## Validation, Correction and Assessment

***=left

Source    |HUC        |Mean Corr  |Mean RMSE (m)  |
----------|-----------|-----------|---------------|
NLA 2007  | 01        |0.82       |5.95           |
NLA 2007  | 02        |0.69       |5.02           |
Web       | 01 & 02   |0  .72     |7.0            |


***=right

<img src="assets/img/Figure4.jpg" style="width:100%;">

--- .segue bg:url(assets/img/Pooecetes_gramineus_-USA-8_small_80.jpg)

## Extending USGS SPARROW

<span style="color:white;font-size:60%;position:absolute;bottom:0px;left:10px;">Photo Credit:<a style:"color:white;" href="http://www.flickr.com/photos/59323989@N00"> Seabamirum</a></span>


--- &twocol w1:40% w2:60%

## USGS SPARROW

***=left
- Nutrient Load Model
- Multiple Scales
 - National Scale
 - Regional Scale


***=right

<img src="http://wi.water.usgs.gov/rna/9km30/images/SPARROW_model.jpg" style="margin-top:-50px;") />
<span style="font-size:60%;position:absolute;bottom:0px;left:10px;">Map Credit: http://wi.water.usgs.gov/</span>

--- &twocol w1:30% w2:60%

## USEPA Modeling

***=left
- Concentrations in Lakes
 - SPARROW Assumes a Flat Lake
- Our Addition
 - Modeled Residence Time: [Milstead et al. 2013](http://www.plosone.org/article/info%3Adoi%2F10.1371%2Fjournal.pone.0081457) 

***=right
<table><colgroup span="1"><col span="1"><col span="1"><col span="1"><col span="1"><col span="1"><col span="1"><col span="1"></colgroup><thead><tr><th colspan="1" rowspan="1"></th><th colspan="3" rowspan="1"><strong>Nitrogen Results</strong></th><th colspan="3" rowspan="1"><strong>Phosphorus Results</strong></th></tr><tr><th colspan="1" rowspan="1"><strong>Hypothesis</strong></th><th colspan="1" rowspan="1"><strong>rmse</strong></th><th colspan="1" rowspan="1"><strong>adjR2</strong></th><th colspan="1" rowspan="1"><strong>aic</strong></th><th colspan="1" rowspan="1"><strong>rmse</strong></th><th colspan="1" rowspan="1"><strong>adjR2</strong></th><th colspan="1" rowspan="1"><strong>Aic</strong></th></tr></thead><tbody><tr><td colspan="1" rowspan="1">H<sub>0</sub></td><td colspan="1" rowspan="1">0.26</td><td colspan="1" rowspan="1">0.43</td><td colspan="1" rowspan="1">24.7</td><td colspan="1" rowspan="1">0.43</td><td colspan="1" rowspan="1">0.35</td><td colspan="1" rowspan="1">154.3</td></tr><tr><td colspan="1" rowspan="1">H<sub>1</sub></td><td colspan="1" rowspan="1">0.31</td><td colspan="1" rowspan="1">0.53</td><td colspan="1" rowspan="1">21.4</td><td colspan="1" rowspan="1">0.47</td><td colspan="1" rowspan="1">0.45</td><td colspan="1" rowspan="1">141.9</td></tr><tr><td colspan="1" rowspan="1">H<sub>2</sub></td><td colspan="1" rowspan="1">0.28</td><td colspan="1" rowspan="1">0.43</td><td colspan="1" rowspan="1">8.7</td><td colspan="1" rowspan="1">0.46</td><td colspan="1" rowspan="1">0.30</td><td colspan="1" rowspan="1">152.7</td></tr><tr><td colspan="1" rowspan="1">H<sub>3</sub></td><td colspan="1" rowspan="1">0.31</td><td colspan="1" rowspan="1">0.48</td><td colspan="1" rowspan="1">6.2</td><td colspan="1" rowspan="1">0.48</td><td colspan="1" rowspan="1">0.38</td><td colspan="1" rowspan="1">158.2</td></tr><tr><td colspan="1" rowspan="1">H<sub>4</sub></td><td colspan="1" rowspan="1">0.27</td><td colspan="1" rowspan="1">0.51</td><td colspan="1" rowspan="1">-8.4</td><td colspan="1" rowspan="1">0.44</td><td colspan="1" rowspan="1">0.42</td><td colspan="1" rowspan="1">141.6</td></tr><tr><td colspan="1" rowspan="1">H<sub>5</sub></td><td colspan="1" rowspan="1">0.28</td><td colspan="1" rowspan="1">0.49</td><td colspan="1" rowspan="1">4.0</td><td colspan="1" rowspan="1">0.44</td><td colspan="1" rowspan="1">0.40</td><td colspan="1" rowspan="1">140.2</td></tr>

<tr style="background: #559b6a; color: white;"><td colspan="1" rowspan="1" style="color: white;">H<sub>6</sub></td><td colspan="1" rowspan="1"><strong>0.21</strong></td><td colspan="1" rowspan="1"><strong>0.62</strong></td><td colspan="1" rowspan="1"><strong>-69.9</strong></td><td colspan="1" rowspan="1"><strong>0.36</strong></td><td colspan="1" rowspan="1"><strong>0.54</strong></td><td colspan="1" rowspan="1"><strong>94.1</strong></td></tr>

<tr><td colspan="1" rowspan="1">H<sub>7</sub></td><td colspan="1" rowspan="1">0.27</td><td colspan="1" rowspan="1">0.52</td><td colspan="1" rowspan="1">-5.1</td><td colspan="1" rowspan="1">0.44</td><td colspan="1" rowspan="1">0.41</td><td colspan="1" rowspan="1">142.0</td></tr><tr><td colspan="1" rowspan="1">H<sub>8</sub></td><td colspan="1" rowspan="1">0.27</td><td colspan="1" rowspan="1">0.52</td><td colspan="1" rowspan="1">-4.6</td><td colspan="1" rowspan="1">0.44</td><td colspan="1" rowspan="1">0.42</td><td colspan="1" rowspan="1">142.3</td></tr></tbody></table>


--- &twocol w1:50% w2:50%

## Modeled Trophic State

***=left

- Predictions
 - TN
 - TP
 - Chl *a*


***=right

<img src="assets/img/journal.pone.0081457.g007.png" style="margin-top:-110px;max-height:650px;"/>

--- &twocol w1:40% w2:60%

## Availability

***=left
- Morphometry:
  - Draft for Conterminus US
  - Validation ongoing
  
- Trophic State:
 - New England - HUC01
 - Mid-Atlantic - HUC02

***=right

<img src="https://water.usgs.gov/wsc/imageregions.jpg" />
<span style="font-size:60%;position:absolute;bottom:0px;left:10px;">Map Credit: http://water.usgs.gov/</span>

--- .segue bg:url(http://www.pca.state.mn.us/artwork/newscenter/tab-littlerocklake.jpg)

## Cyanobacteria

<span style="color:white;font-size:60%;position:absolute;bottom:0px;left:10px;">Photo Credit: http://www.pca.state.mn.us/</span>

--- 

## Our Project

 > We are trying to combine what we know from field data, 
 > what we know from modeled data, and what we (think) we know
 > about cyanobacteria and create predicitve models of the 
 > probability of bloom events.
 

<img src="assets/img/function.jpg" style="margin:auto; width:100%;" />



--- .segue bg:url(assets/img/DSC00195_80_900-1200.jpg)

## Thanks and Questions

<span style="color:white;font-size:60%;position:absolute;bottom:0px;left:10px;">Photo Credit: Elizabeth Herron, URI Watershed Watch</span>






