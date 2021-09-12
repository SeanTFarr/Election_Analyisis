# Election_Analysis

## Project Overview
A Colorado Board of Elections employee has requested additional data to perform an audit of a recent local congressional election. The additional data requested was as follows:

1. Calculate the total number of votes cast in the election.
2. Provide a breakdown of the number of votes and the percentage of the total votes for each county.
3. Determine which county had the largest turnout.
4. Determine who the candidates were and then provide a breakdown of the number of votes and the percentage of total votes each candidate received.
5. Determine the winner of the election, provide their vote count, and their percentage of the total votes.


## Resources
- Data source: election_results.csv
- Software: Python 3.9.6, Visual Studio Code 1.60.0

## Election-Audit Results
### The final analysis of the election revealed that:
 There were 369,711 total votes cast in the election.
 This was determined by counting the number of votes as we ran the Python program through the csv file, by first initializing the counter

 <img width="241" alt="Initialiing Total Vote Counter" src="https://user-images.githubusercontent.com/88861780/132977292-820b76ba-4219-472a-965a-1d257f2a71f7.png">

 Then by adding to the count as we looped through the data on the election_results.cvs file.

<img width="324" alt="Add 1 to Total Vote Counter" src="https://user-images.githubusercontent.com/88861780/132977287-3398d0c5-7209-466c-a3a4-5fa20c10bbfe.png">


 ### County Results:
 The county results were determined by utilizing this section of code to run through the elections_results.csv file, pulling the county information, calculating the number of votes per county, and calculation the percentage of the votes for each county.
 
<img width="470" alt="County For Loop" src="https://user-images.githubusercontent.com/88861780/132977294-356cbeae-d35b-4ffe-8f3d-a0163c0749e6.png">

- The county by county breakdown:
  - Jefferson County had 38,855 votes or 10.5% of the precinct.
  - Denver had 306,055 votes or 82.8% of the precinct.
  - Arapahoe had 24,801 votes or 6.7% of the precinct.
- The largest turnout:
  -  Denver County had the largest voter turnout at almost 83% of the precinct.

### Candidate Results:
Similar to the county results, for the candidate results we used this section of code to extract the candidate names, the total votes each one recieved, and calculating the percentage of the total votes cast that each candidate received.

<img width="410" alt="Candidate For Loop" src="https://user-images.githubusercontent.com/88861780/132977295-d92f7a08-e546-48cd-b751-de470dd5d746.png">

- The candidates were: 
  - Charles Casper Stockham 
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 85,213 votes, which is 23.0%  of the total votes.
  - Diana DeGette received 272,892 votes, which is 73.8% of the total votes.
  - Raymon Anthony Doane received 11,606 votes, which is 3.1% of the total votes.
- The winner of the election was:
  - Diana DeGette, who received 272,892 votes, had 73.8% of the total votes cast.

## Election-Audit Summary
With this script, the Colorado Board of Elections can perform additional audits, with proper modifications, of other elections including (but not limited to):

- With a dataset of the entire state they could collect data on all precints. This would need the addition of a "Precincts" dictionary, to give total votes in each precinct across the state, as well as the percentage of the total statewide vote.

- with a dataset that included the cities within the counties and by adding a "City" dictionary to the script, the Board could drill down further into how candidates fared in different regions of the counties, giving a better understanding of the candidates constituents.