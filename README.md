# Web-Word-Visualization

## Development Period
- 2016.07 ~ 2016.12

## Development Language & Tools
- Language : Java, Node.js, Javascript
- Tools : Eclipse, Atom, Cent OS,MongoDB, D3

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

## Problem Solving
- The first problem was that the system turned off. This was caused by a lack of exception handling in Crawling. Because of the nature of the crawler that follows URLs, it is sometimes because you have accessed pages that only contain photos or videos. To solve this problem, I used the method of employing the exception handling of the actual Web Crawler.
- The second problem was that could not analyze recently published words. Because Komoran used for morphological analysis analyzed morphemes based on the old Wikipedia dictionary. Words that want to know the distribution by graph appeared in the article, but it was very serious that it was not visualized in my system. To solve the problem, I went into Github and read the document and analyzed the code. I also actively exchanged emails with developers and found solutions. I fixed the problem by manually adding words to the userDB file that Komoran refers to and marking it as a single noun.

## Technique
- Using Jsoup develop crawler
- Using D3 visualize distribution by graph
- Using Node.js develop web server to show graph and title(+URL)
