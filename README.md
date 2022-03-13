# Web Scrapping Project: scrapping top repositories of top topics on Github.

- For this web scrapping project, the goal is to scrap Github's [Most popular Page](https://github.com/topics), and obtain the top repositories in each topic(in /data). 
- The site we are going to be scrapping is the topics page of github, it lists all most popular topics on github and provides a description and link to a topic page, which contains the most popular repositories for that topic. 
- Our goal is to obtain information about the top repositories in the most popular topics. 
- We will be using requests, Python, BeautifulSoup, Pandas. 

# Introduction
The site we are going to be scrapping is 'https://github.com/topics'
We will get the top 30 most popular topics on github, obtaining the topic titles, topic descriptions, and the link of the topics. 
Then, for each topic, we will scrap for the top 25 repositories under that topic. The information will be stored in csv files. For each repository, we will obtain the repository username, repository title, repository star reviews, and repository url. 

### Outline:
- Scrap https://github.com/topics
- obtain topic title, topic url, and topic description, and store in dataframe.
- Using the topic url, obtain information about top respositories in each topic page.
    - Parse the repository name, username, url, and star reviews. 
    - Save all topic repo data into csv files with format:
    `repo_name,username,repo_url,stars`
