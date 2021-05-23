# Election_Analysis

## Project Overview
A Colorado Board of Elections employee gave the following tasks to complete the election audit of a recent local congressional election:
1. Calculate the total number of votes cast.
2. Get a complete list of candidates who received votes.
3. Calculate the total number of votes each candidate received.
4. Calculate the percentage of votes each candidate won.
5. Determine the winner of the election based on popular vote.

## Resources
- Data Source: election_results.csv
- Software: Python 3.7.6, Visual Studio Code, GitBash

## Election-Audit Results
- There were 369,711 votes cast in the election.
- County Votes break down as follows:
    - Jefferson contributed 38,855 votes, 10.5% of the total vote.
    - Denver contributed 306,055 votes, 82.8% of the total vote.
    - Arapahoe contributed 24,801 votes, 6.7% of the total vote.
- The county with the highest voter turn out was **Denver**.
- Candidate Votes break down as follows:
    - Charles Casper Stockham earned 85,213 votes, 23.0% of the total vote.
    - Diana DeGette earned 272,892 votes, 73.8% of the total vote.
    - Raymon Anthony Doane earned 11,606 votes, 3.1% of the total vote.
 - The winner of the election was **Diana DeGette**, with 272,892 votes and 73.8% of the total vote.

## Challenge Overview
 - In an earlier version of the code, the List variables titled candidate_options and county_names contained the String variables candidate_name and county_name, respectively. This caused confusion in the debugging process. To improve clarity, candidate_name was renamed to current_candidate_name and county_name was renamed to current_county_name.
- (https://user-images.githubusercontent.com/83254435/119278009-55ba1f80-bbe8-11eb-9d2c-eae6f240e090.png)

# Election-Audit Summary
- The current version of the code reads election_results.csv and converts it into a list of pre-established dictionaries. It then loops through each row of data to tally the total number of votes and populate a list of candidate options and county names. It tallies each instance of a candidate's name as a vote for that candidate, and tallies each instance of a county's name as a vote cast from that county. Then it performs an analysis of the totals obtained, and prints the results into a .txt file. 
- If tracked in the data source file, one could create additional lists to be populated and tallied within the programmed for loop. Suggested lists could include demographics related to voter turnout such as political parties, voting methods, or polling places.
- (https://user-images.githubusercontent.com/83254435/119278355-55228880-bbea-11eb-88e3-e0a79729c7d7.png)
- To scale the code to a Presidential Election, a dictionary that contains State Names and Electoral Votes could be created. The final analysis would use conditional statements to assign the designated number of Electoral Votes to the candidate who wins the Popular Vote in each given State.
