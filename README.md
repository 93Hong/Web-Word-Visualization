# Web-Word-Visualization

## Description
- A system that analyzes words by crawling news articles from websites and social networks.
- Visualize distribution by morphological analysing crawled data.
- Web server execute crawler every 30 minutes. Then web server update graph
- Graph show data for 10 day.

## Process
- Article crawling -> morphological analysis -> store to the database
- -> search delete insert word -> visualization (graph & title)

## Function
- Word : search, delete, insert
- Visualization : word distribution graph
- URL : location of the original article

## Tools & Technique
- Using Jsoup develop crawler
- Using D3 visualize distribution by graph
- Using Node.js develop web server to show graph and title(+URL)
