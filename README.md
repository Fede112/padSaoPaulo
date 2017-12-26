# padSaoPaulo
Welcome to Software Carpentry Etherpad!

This pad is synchronized as you type, so that everyone viewing this page sees the same text. This allows you to collaborate seamlessly on documents.

Use of this service is restricted to members of the Software Carpentry and Data Carpentry community; this is not for general purpose use (for that, try etherpad.wikimedia.org).

Users are expected to follow our code of conduct: http://software-carpentry.org/conduct.html

All content is publicly available under the Creative Commons Attribution License: https://creativecommons.org/licenses/by/4.0/



Social Dinner 

Just to remind you all: 

There will be a conference dinner on Thursday December 7th starting at 19:30. 
  
The dinner will be a courtesy by the institute, which is also included one non-alcoholic beverage.

Here is the map for the location: https://drive.google.com/open?id=1xKKrT5cB-cfoWqvc-EfZubhcUatZfBWc. And this is it on google maps http://bit.ly/2BQoofL

Dinner venue: BOVINU’S FAST GRILL - ALAMEDA Santos 2393 - Cerqueira César  São Paulo

Have a nice evening!!



Materials

Materials for the school can be found at 

- https://drive.google.com/open?id=1Jzy4eCoKVfnt_EUtUOPWiDQ-4G5N9zNr

Course feedback - at the end of each module please complete the form at  https://goo.gl/forms/BqEyG5rgjNpWd6ii2

There is a facebook group page for this school - please look up DataSãoPaulo17 : https://www.facebook.com/groups/DataSaoPaulo17/

Twitter hashtag #DataSãoPaulo17

CODATA-RDA photos @ Flickr https://www.flickr.com/photos/93319111@N04/albums/72157663343276228



Open Science

- https://www.icsu.org/cms/2017/04/open-data-in-big-data-world_long.pdf

Results from question on being "scooped".

I am worried about being scooped by someone I know YES 3 NO 15
I am worried about being scooped by someone I do not know YES 9 NO 11



Shell Lesson

If you have any questions for Abel you can contact him on abel.s.siqueira@gmail.com

- https://github.com/abelsiqueira/codata-ictp-saifr-2017-12-04/blob/master/class.md

$ wget https://github.com/abelsiqueira/codata-ictp-saifr-2017-12-04/raw/master/data_process_example.tar.gz
$ tar -xvzf data_process_example.tar.gz

$ cd data_process_example

$ for file in data/data*
>  do

>      myvar=$(basename $file .dat)
>      ./process_data $file > output/$myvar.out
>      wc -l $file > output/$myvar.wc
> done

Some shell commands:
cp
mkdir
mv
rm
mkdir
rmdir



Git (Version Control)

Simplified and community-driven man pages: https://tldr.sh/

The Excel Depression: http://www.nytimes.com/2013/04/19/opinion/krugman-the-excel-depression.html

Links for the slides:

    - https://jiffyclub.github.io/2015-07-06-scipy/slides-local_version_control.html
    - http://slides.com/abostroem/collaborating_using_git
    - http://slides.com/abostroem/deck-4

Official Software Carpentry lesson:

    - https://swcarpentry.github.io/git-novice/

I (Filipe Fernandes) am `ocefpaf` on GitHub.
You can ping me with @ocefpaf and ask for help.

Here is some extra philosophy about the usage of github in SPANISH, videos are included: https://tcpbros.github.io/

You might not need to read the whole thing but I'd love for you to read, about the `git commit` command. https://tcpbros.github.io/git/commit/



Introduction to R

- https://github.com/fernandomayer/CODATA - included scripts writen in the two days

Extra resources:

- SWC lessons page: https://software-carpentry.org/lessons/

- For those of you who are ready to start looking at more advanced R material, take a look at http://r4ds.had.co.nz R for Data Science. There are some lovely ideas here and discusses the Tidyverse which are a very powerful set of libraries.

Challenges for tue, afternoon:

## Create an object with the letters A, B, C repeated 15, 12,
## and 8 times, respectively

## Show where are the letter B in this object

## How many B letters are there in this vector? Use the
## function sum() to count this. See ?sum

## Create an object with 1000 random numbers from runif().
## How many numbers greater than 0.5 are there?

## Calculate the first 50 powers of 2 (e.g. 2^1, 2^2, etc).
## Calculate the square of integers from 1 to 50 (e.g. 1^2, 2^2, etc)
## How many pairs are equal? 2^n = n^2 ?

## Create the matrix
## 2 8 4
## 0 4 1
## 9 7 5

## Set names for rows and columns of this matrix

## Make a list with 2 components: a vector with A, B, C 
## repeated 2, 5, and 4 times respectively, and the matrix
## created before

## Give names to the components of this list

## Create a data frame so that the numbers 23, 34, 56, 21
## are associated with the letters A, B, C, D

Challanges for wed morning:

- http://swcarpentry.github.io/r-novice-gapminder/06-data-subsetting/
- http://swcarpentry.github.io/r-novice-gapminder/05-data-structures-part2/

## conditional selection

x <- c(5,15,42,28,79,4,7,14)
str(x)
x[x>15]
names(x)<- letters[1:length(x)]
char <- letters[1:length(x)]
char[x>30]
x[char %in% c("a", "c")]

char[ x %in% c(4,14)]
which(x>15)
which( char %in% c("a", "c"))

df <- data.frame(year = 2001:2005, obs = c(26,18,25,32,NA),
                 state = c(" SP", "RS", "SC", "SC", "RN"),
                 stringsAsFactors = FALSE)

df[df$year == 2004,]
df[df$state == "SC",]
df[df$state == "SC", "obs"]
df[df$state == "SC" & df$obs > 30, ]

subset(df, year == 2004)

## Create a data frame to store two variables:
## number of habitants and city. City A have 42 habitants,
## city B have 34, city C have 59, and city D have 18
## (numbers are in thousands).

## Show what city has less than 30 habitants.

## Make a new column stating that cities A and C are at
## the east part of the country and that cities D and Df
## are at south.

## Select the cities from the east region with less than
## 20 habitants

## Show in what cities from south there are more than 40
## habitants.

## What region has cities with less than 50 habitants?

Challenges for wed, afternoon:

- http://leg.ufpr.br/~fernandomayer/data/
- http://leg.ufpr.br/%7Efernandomayer/data/notas.csv



Structured Query Language - SQL

- https://swcarpentry.github.io/sql-novice-survey/
- http://sqlitebrowser.org/ <---  This is a nice gui for sqlite

I urge you to learn something about `accumulation functions` such as sum, count, avg, and the GROUP BY clause

You can also insert data into the tables of your database using the `INSERT` clause
Finally, you should learn a little bit about relating the multiple tables of your database using the `JOIN` clause.

There's also this tool to graphically design your databases, and there are some examples to use https://editor.ponyorm.com/



Research Data Management

December 13, 2017

- Please complete the questionnaire at   

  https://goo.gl/forms/bX7bgKHxJ1xK2Oyz2

  before the start of this course on Thursday afternoon.

- A detailed agenda and links to material for the RDM module can be found at 
  https://docs.google.com/document/d/1N75mhhHY30fHmlej-HKLSqw-gVZyHe59XiK4m-d5CJs/edit
 
- Google for Education Program:
  Ask the TI team of you institution to subscribe your institutional e-mail for unlimited storage in GoogleDrive
  https://edu.google.com/intl/higher-education/?modal_active=none

- EduDrive (Dropbox-like service for academic community in Brazil): https://edudrive.rnp.br

- DOI Attribution in Brasil (focused on "documents") - Associação Brasileira de Editores Científicos: http://goo.gl/BjduYk

- ORCID: https://orcid.org/

- Author Carpentry lessons - https://authorcarpentry.github.io/

- FAIR data:
  Another (self-)assesment tool: http://oznome.csiro.au/5star/ (including "trust" category) 
  Sample of self-assesment answer: https://oznome.csiro.au/5star?view=5a2a98f044f0d900013d4d45

- LOV (Linked and Open Vocabularies): http://lov.okfn.org/dataset/lov/

- An event next year in Brazil that might be of interest: 
  The Latin America and the Caribbean Scientific Data Management Workshop convened by the World Data System (WDS) 
   http://lacworkshop.icsu-wds.org/

- "ICSU Sustainable Business Model for Research Data Networks" 
https://www.icsu-wds.org/community/working-groups/coordination-and-support-of-international-research-data-networks/coordination-and-support-of-international-research-data-networks

- Literature Suggestion:  Data Management for Researchers. Kristin Briney. Pelagic Press, 2015 (ISBN 978-1-78427-011-7)



Data Reuse Lab (links below from Steve)

LAB LINK
https://docs.google.com/presentation/d/1YweI_BtTY2XQ1HICeoCScQ5ZCz_m7of50MwPKgWZ0qs/edit?usp=sharing
ATTENTION GO-SHIP TEAMS:  There is a new (additional) paper --> https://drive.google.com/file/d/1KqMsXsLZAGCmRSB7J_T4Tlr3v8rCkdlQ/view?usp=sharing

Would you like to select ARGO data for a certain period of time and download it all at once for analysis?  
Here's a tip --> http://www.coriolis.eu.org/Data-Products/Data-Delivery/Data-selection
Also, here's the movie that I showed with audio: --> https://goo.gl/JZZ2DJ

------------
FRIDAY, December 8, 2017

Exercise_ Review the DataOne hydrology DMP and identify what should be kept for the long term (20 mins)
www.dataone.org/sites/all/documents/DMP_Hydrologic_Formatted.pdf 

Presentations/Resources:
Team 2: GO-SHIP R data analysis Github repository: https://www.github.com/abelb0rges/CCHDO_I08S
Team 4: GO-SHIP: https://docs.google.com/presentation/d/1dYjJlnKWXiVIKBHCv4_ZnM-Syk74mRnfkC61_teV9kk/edit?usp=sharing
Team 6: GO-SHIP: https://docs.google.com/presentation/d/1_7G_JdstVkhETm6ppKkpkYRik1-_lyiQVozbeGgxYzE/edit?usp=sharing

ArgoViz (Interactive Earth - Oceanography/Meteorology)
http://data.scripps.earth/argoviz/ 

Knowledge Graphs: 
https://en.wikipedia.org/wiki/Knowledge_Graph (wiki entry)
http://www.sciencemag.org/news/2014/12/geoscientists-aim-magnify-specialized-web-searching (some scienceMag blog entry)
http://www.dataversity.net/building-scientific-knowledge-graph/ (small blog entry 4 science application)



Open Science Session 2 (Friday, 8 Afternoon)

RRI Tools
http://rri-tools.eu


Weekend session on getting involved in Schools

Research Data Alliance - becoming an individual member: https://www.rd-alliance.org/get-involved/individual-membership.html

RDA national groups: https://www.rd-alliance.org/groups/national-groups

Also various disciplinary groups and topics e.g. citation. 

OpenCon: http://www.opencon2017.org/

All course materials used in the school are openly licensed (CC-BY - attribution only) so you can reuse them in your own courses. Please let us know what you do as these success stories help us demonstrate impact and get funding for more schools. Also share back what you develop, specifically translations of software carpentry courses as they are specificallylooking for these at the moment

Repo for translations (Spanish)

https://github.com/malfaro2/CODATA-RDA

Send me an email if you want to be added as a collaborator: marcela.alfarocordoba@ucr.ac.cr
Feel free to copy the repo if you want to do the same in Portuguese 

Data Visualisation 
(William Sherman - shermanw@indiana.edu)

- Visualization Analysis and Design - Tamara Munzer - https://www.amazon.de/Visualization-Analysis-Design-Principles-Techniques/dp/1466508914 

- Wicked problem: https://en.wikipedia.org/wiki/Wicked_problem

- Harvard Inner Life Viz:  https://www.youtube.com/watch?v=FzcTgrxMzZk

- Spurious Correlations: http://www.tylervigen.com/view_correlation?id=359

- Chart Suggestions: https://i1.wp.com/flowingdata.com/wp-content/uploads/2009/01/chart-chart1.jpg?fit=1024%2C767&ssl=1

- Example of a bad graphic, from a presidential candidate in Chile, showed on a live TV debate.https://media.metrolatam.com/2017/11/07/capturadepantalla20171107alas80814am-c2ae668cce940800958cfec42ccbc884-1200x600.jpg

resources:
disk_out_ref.ex2: https://github.com/naucoin/VTKData/blob/master/Data/disk_out_ref.ex2
can.ex2: https://midas3.kitware.com/midas/item/207317



Introduction to Machine Learning

https://rpubs.com/rocknroll/datasp17
http://www-bcf.usc.edu/~gareth/ISL/data.html (book)
http://www-bcf.usc.edu/~gareth/ISL/Advertising.csv (advertising.csv data)

R Markdown Cheat Sheet: https://www.rstudio.com/wp-content/uploads/2015/02/rmarkdown-cheatsheet.pdf (great!)

RPubs:
- https://rpubs.com/preinh/Prestige-CODATA-RDA 
- http://rpubs.com/vitorhirata/rprestige
- http://rpubs.com/avallecam/lmml
- http://rpubs.com/jvmelis/prestige_data_analysis (Camila, Federico, Henrique & Juliano)
- http://rpubs.com/lagrangiana/mlearningcodata17 (Wemi, Renan, Luis & Ignacio)
- http://rpubs.com/lzarba/341212 (Bryan, Anderson, José & Lucía)
- http://rpubs.com/criedo/341304 (Jacqueline, Adriana, Pedro, Cassio)
- https://rpubs.com/Farley_Flausino/handsoncodatalm (Farley Flausino, Jorge Gomez, Debora Druker, Jose Lopez)

Extra Reference:
 Jason's Machine Learning 101
- https://docs.google.com/presentation/d/1kSuQyW5DTnkVaZEjGYCkfOxvzCqGEFzWBy4e9Uedd9k/preview?slide=id.g168a3288f7_0_58
- Might be useful: https://medium.com/ai%C2%B3-theory-practice-business/top-6-errors-novice-machine-learning-engineers-make-e82273d394db


Artificial Neural Networks

https://drive.google.com/file/d/1nuVwwR7aeczbM-vj2UXGXblhY7fqBdxx/view
https://rpubs.com/rocknroll/datasp17-nn

DeepMind AI just taught itself to walk @ https://www.youtube.com/watch?v=gn4nRCC9TwQ
Linear Digression Podcast about Neural Networks (specifically about neural net dropout and reducing overfitting): http://lineardigressions.com/episodes/2017/10/1/neural-net-dropout

Iris Model Improvements Presentations:
- https://drive.google.com/file/d/1lurpX8PF2Ma5uN9sZJXM3MHvEYbMSB_A/view?usp=sharing - Jose Cordova and Anderson Leao
- https://rpubs.com/preinh/iris_introNN_CODATA-RDA
- http://rpubs.com/avallecam/ann
- http://rpubs.com/vitorhs/iris
- http://rpubs.com/jvmelis/iris_NN
- http://rpubs.com/lagrangiana/datasp17-nn-iris (Ignacio, Luis & Renan)

IRIS PCA https://www.math.umd.edu/~petersd/666/html/iris_pca.html 

To make sense of what a layer does: http://scs.ryerson.ca/~aharley/vis/conv/ 3D MNIST Neural Network visualization


Computational Infrastructures

Schedule: https://opensciencegrid.github.io/dosar/Materials/DSP_DT2017/ 
Materials: https://opensciencegrid.github.io/dosar/Materials/DSP_Materials/

To Sign Up for a permanent OSG account go to: http://osgconnect.net/signup
Use DataSaoPaulo as your group while you are exploring the possibilities, when you start doing real research please contact me (rquick@iu.edu) to set up a project for your research. 

DOSAR: Distributed Organization for Scientific and Academic Research http://www.dosar.org/
You are welcome to join our bi-­‐weekly video (Vidyo) meetings. Send request to be added to DOSAR email list to Prof. Greenwood: greenw@phys.latech.edu reference you attended the Research Data Science School in Sao Paulo
If you want long­‐term grid access, you can request membership in the DOSAR VO 



Women in SciTech Authorship

R-ladies:

- https://rladies.org/
- https://github.com/rladies/starter-kit/blob/master/README.md
- https://github.com/rladies/rladies_global_presentations/blob/master/20171021_WSDS2017/RLadies_WSDS_Oct2017.pdf
- Presentation UseR 2017 (video): 
https://channel9.msdn.com/Events/useR-international-R-User-conferences/useR-International-R-User-2017-Conference/R-Ladies-Global-Community

PyLadies ;-):

- http://www.pyladies.com
- http://python.org.br/pyladies 
- SciPy 2017 (channel, 4 everyone):
https://www.youtube.com/playlist?list=PLYx7XA2nY5GfdAFycPLBdUDOUtdQIVoMf



Literature Suggestions

- British Ecological Society’s Guide to Reproducible Code: http://www.britishecologicalsociety.org/wp-content/uploads/2017/12/guide-to-reproducible-code.pdf

-  Methods in Ecology and Evolution Blog (more suggestions included):  https://methodsblog.wordpress.com/2017/12/06/making-your-code-reproducible/ 

- Hands-On Machine Learning with Scikit-Learn and TensorFlow. Aurélien Geron. 2017 (book)




OutOfTopic: (Some Cultural Stuff @ SP):

Av. Paulista Region (Broad Cultural Interest)
- http://centrocultural.sp.gov.br/site/ (CCSP: Sao Paulo Cultural Center)
- https://ims.com.br (IMS: Moreira Salles Institute)
- http://www.biketoursp.com.br/ (Free bike tour - weekends - Limited by subscriptions)
- Baixo Augusta (walk around R. Augusta)

- MASP: https://en.wikipedia.org/wiki/S%C3%A3o_Paulo_Museum_of_Art
- MAM http://mam.org.br/en/

Fradique Coutinho Metro Station (Vila Madalena Region): 
https://goo.gl/maps/UzUkoN9zeF82  (bars, restaurants, pubs... etc..)
 
SESC
- 24 de Maio (in old city center, near Metro Republica/Anhagabau): 
https://www.sescsp.org.br/unidades/36_24+DE+MAIO/#/uaba=programacao#/fdata=id%3D36
- Pompeia (near UNESP):
https://www.sescsp.org.br/unidades/11_POMPEIA/#/uaba=programacao#/fdata=id%3D11
- Pinheiros (near V. Madalena): 
https://www.sescsp.org.br/unidades/10_PINHEIROS/#/uaba=programacao#/fdata=id%3D10

Live (Jazz) Music:
- V Madalena:
http://jazznosfundos.net/home.php
- DownTown Region: 
http://jazzb.net/home.php

- Al Janiah (refugee supportive bar with beer + music): 
https://www.facebook.com/aljaniah01/  
(Bixiga region: https://goo.gl/maps/idmrS6xPXDu)
- Escadaria do Jazz: (Outdoor Live Music @ Bixiga region):
https://www.facebook.com/escadariadojazz/

Ok, beer, coffee:

- Vila Madalena/Pinheiros:
- Coffee lab: http://coffeelab.com.br/o-coffee-lab/ (unique coffee experience)
- SP Tap House: http://www.spth.com.br/ (40 brazilian craft beers - on tap)
- beer4u: http://www.beer4u.com.br/lojas (bottles - great variety good prices, next to the subway)
- EAP: http://www.altodospinheiros.com.br (30+ worldwide craftB on tap and so many bottles, a bit expensive)
- BrewDog: https://www.brewdog.com/bars/worldwide/sao-paulo
- GooseIsland: http://www.gooseislandsp.com
- Praça Benedito Calixto (flea market / pubs & bar nearby, cool music and antiquities at sat. afternoon)
- Av. Paulista region
- Walk through R. Augusta to Praça Roosevelt (pubs, bar & theater nearby)
- Mirante 9 de julho (nice coffee & view https://www.tripadvisor.com.br/Attraction_Review-g303631-d8628181-Reviews-Mirante_9_de_Julho-Sao_Paulo_State_of_Sao_Paulo.html)
- extra:
- https://www.theguardian.com/travel/2014/may/15/top-10-bars-sao-paulo-brazil-world-cup (special star to 'ó do borogodo' w/ samba live)
- http://sprudge.com/the-sprudge-guide-to-sao-paulos-vila-madalena-neighborhood-127584.html (walking tour by Vila Madalena , drinking coffee)
- https://www.eater.com/maps/coffee-cafe-brazil-sao-paulo-caffeine-map


 Souvenirs:
- http://www.taindopraonde.com.br/2017/08/onde-comprar-souvenirs-de-sao-paulo.html
- https://www.yelp.com/search?cflt=souvenirs&find_loc=S%C3%A3o+Paulo+-+SP
- https://www.tripsavvy.com/souvenirs-to-bring-home-from-brazil-1467958 (some ideas)
- http://trip-n-travel.com/listicle/22496/ (list of ideas)
- https://theculturetrip.com/south-america/brazil/articles/best-places-to-buy-souvenirs-in-sao-paulo/ (best places to buy)
- ideas easy to transport: havaianas, bikini, canga (beach stuff)


Airport Rides: 
(this is in case you want to find people leaving at the same time as you, so can share a ride)
(add as many more day/times as you need)

LEAVING FROM THE UNIVERSE FLAT HOTEL AT:
    
Friday Early Afternoon(1pm - 4pm)
Henrique -- about 2pm to Congonhas airport
Abel: I need to be at 3pm at CGH airport

Friday Afternoon (4pm-7pm)

Friday Night (7pm-12): 
Jorge  -- at 10 pm (by bus) to GRU

Saturday early morning (2am-6am)
Ana Leydis --- leaving at 3 am to GRU (departure at 6:30 am)
Andree --- leaving at ~4.30am to GRU (departure at 8.30am)

Saturday morning (6am-12)
Marcela -- leaving at 9am to GRU airport (I'm taking a Taxi/Uber) (departure at 1:00pm)

Saturday afternoon (12-5pm)
Renan -- leaving at 2pm to CGH airport (departure at 5:10pm)
Bryan -- leaving at 12:00 to GRU (departure at 4pm)

Saturday night (5pm-9pm)

Sunday 3pm 
Jose -- have to be at the airport at 3 or a little before

For  those who complain about the Metro in Sao Paulo:
- https://www.youtube.com/watch?v=_QWDY4mo4JQ
      - https://www.youtube.com/watch?v=WigWL1XS8Ro (Yellow line Saxophone)
- https://www.youtube.com/watch?v=ynDTMM2-vXw (More of yellow line sound)
    

#freeTucuman
