# Analysis of unofficial 2021 ballot measure results in New York City
This repository contains data, analytic code, and findings on New York City's votes for the five statewide ballot measures.

## Data
This analysis uses a spreadsheet containing scraped unofficial 2021 election data from the New York City Board of Elections. The dataset is too large to be uploaded to Github, but can be downloaded here: https://docs.google.com/spreadsheets/d/1Ireuox4h_NZdnqkqCgadv0kFhhy5I2MKu_vJeLBiHK8/edit?usp=sharing.

The spreadsheets contain the following columns relevant to this analysis

* `Office`— This refers to the office that the votes correspond to. For this analysis, each of the ballot proposals are listed under this column.
* `Candidate`— This refers to the candidate running for office. For this analysis, this column will tell us whether a proposal received yes or no votes
* `Votes`— This column holds the total votes per election district.

## Methodology
This notebook is split into three parts:

### Part 1: Identify and clean the column names
* Filter the `office` column to isolate all the ballot proposals
* Create a new column for each ballot proposal
* Simplify the names of each proposal for readability

### Part 2: Calculate the total votes
* Find the sum of each yes and no vote for each proposal
* Create a `yes` and `no` column with the vote share sum
* Find the sum of yes and no votes to see how many people voted for each proposal
* Simplify the proposal name further for readability
* Plot the total_votes_per_proposal to see which proposals had the most voter engagement

### Part 3: Calculate the vote share for each proposal
* Creates a yes_pct and no_pct column
* Calculates the percentage of yes and no votes per proposal
* Round each percentage to the nearest tenth decimal

# Outputs
The results of "Part 2" are saved as "2021_ballot_vote_share_assignment_1.csv".

# Running the analysis yourself
To run the analysis, you will need

* Python 3
* The python libraries specified in requirements.txt

# Licensing
All code in this repository is available under the MIT License. The data file in the output/ directory is available under the Creative Commons Attribution 4.0 International (CC BY 4.0) license. All files in the data/ directory are released into the public domain.

# Feedback / Questions?
Contact Marina Samuel at marinasamuel114@gmail.com.

 
