# The emergence of climate awareness

Have a look at our data story :warning::warning:[Let’s rewind climate history](https://ph0tonic.github.io/ada2021/):warning::warning:

## Abstract:

Since 2015 and the Paris Agreements following the COP21, states and citizens are taking the issue of climate change more and more seriously. This has led to strong political movements like the climate strikes initiated by Swedish activist Greta Thunberg. The goal of our project is to rewind the story of climate change through the quotes of multiple newspapers.

We will first be interested in identifying what the quotes reveal about the important events related to climate change. Then we will dig into the actors behind the quotes. We will ask ourseleves if the important newspapers talking about climate change are mostly for a sustainable change or are rather climate sceptics. A focus will be made also on the most important political opinions of the speakers in the quotes. Finally, these analyses will allow us to have a global overview of how and about what Quotebank quotes talk about regarding climate change.

## Research questions:

- How has climate change gained newspapers’ interest through the years ?
- Do the newspapers reflect the public interests regarding climate change ?
- Which figures are the most important about climate change ?
- What are the emotions conveyed by the quotes about climate change ?
- What does it tell us about the newspapers’ point of view on climate change ?

## Proposed additional datasets (if any):

- wiki data
- google trends api

## Methods

We will first process the dataset of newspaper quotes to create a sub-dataset with only quotes that address the topic of climate change.

We intend to use google trends dataset to see if the quotes in the newspapers reflect well what the public interests are. The library pytrends will be used to this end and will let us extract the number of occurrences a word was searched in google and where these words were searched for example.

The dataset wiki data will be used to have information about the speakers, their notoriety or their political orientation. This will allow us to see which type of speaker the newspapers most cite.

We will use a sentiment analysis to examine the emotions conveyed by the quotes. The library VaderSentiment will be used for this analysis. This library can help us extract whether the quotes about climate change are negative or positive.

These analyses will allow us to show the emergence of ecological awareness in the newspapers and in the public, its importance and the vision the newspapers and the public have on climate change.

## Proposed timeline

19.11 : treatments of the data (enriching, filtering, exploring the datasets)

26.11 : analyzing the data (plotting graphs, do some calculations to support the analysis)

03.12 : further analysis and visualization of the data (starting the website that will tell our story)

10.12 : visualization of the data

17.12 : finalization of the report

## Organization within the team:
Marguerite:

- Data processing and filtering
- Topic detection analysis
- Data story writing

Cécile:

- Sentiment analysis
- TF-IDF Analysis of the most important words in the quotes
- Data story writing

Théophile:

- Political analysis of newspapers
- Introduction and questions
- Data story writing

Bastien:

- Data processing and filtering
- Political analysis of speakers
- Data story’s website implementation 

Everyone:

- Conclusion on the topic
- Cleaning up the code
- Finalizing the report

## Repository structure

In this structure you will find multiple jupyter notebooks with the following role :

- `notebook_initial_analysis.ipynb` **Part 0** - which contains all our initial analysis with the data treatment with filtering
- `notebook_newspaper_and_political_analysis.ipynb` **Part 1** - which contains the newspaper analysis of political orientation of newspaper and authors
- `notebook_topic_detection_analysis.ipynb` **Part 2** - which contains an analysis linked with topics and the generation of word clouds for the timeline
- `notebook_term_frequency_analysis.ipynb` **Part 3** - which contains an analysis linked with term frequency analysis
- `notebook_invalid_quotes_analysis.ipynb` **Part Bonus** - which contains an analysis of the `invalid` quotes we identified
