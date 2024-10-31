# Data Scraping Explanation
- ### Data was collected using a Python script with GitHub API authentication for efficient access. I first used the API’s search method to filter and retrieve an initial set of user data, then accessed each user’s ***repos_url*** to gather project-specific repository details, extracting only the necessary attributes.
<br>

# Interesting and Surprising Fact
- ### One surprising finding was that repositories with active documentation (***has_wiki=True***) tended to receive significantly higher star counts, suggesting that clear documentation may contribute to project popularity.
<br>

# Actionable Recommendation for Developers
- ### To boost project visibility and engagement on GitHub, developers should prioritize adding and maintaining a ***comprehensive Wiki*** or ***project documentation***, as this can positively impact star count and attract more contributors.
<br><br>

# Questions Answers
### 1. Who are the top 5 users in Beijing with the highest number of followers? List their login in order, comma-separated. <sub></sub>
#### Ans: michaelliao, daimajia, xiaolai, draveness, hongyangAndroid

### 2. Who are the 5 earliest registered GitHub users in Beijing? List their login in ascending order of created_at, comma-separated. <sub></sub>
#### Ans: robin, nwind, reeze, kejun, ZhangHanDong

### 3. What are the 3 most popular license among these users? Ignore missing licenses. List the license_name in order, comma-separated. <sub></sub>
#### Ans: mit, apache-2.0, gpl-3.0

### 4. Which company do the majority of these developers work at? <sub>(Company (***cleaned up as explained above***))</sub>
#### Ans: BYTEDANCE

### 5. Which programming language is most popular among these users? <sub></sub>
#### Ans: JavaScript

### 6. Which programming language is the second most popular among users who joined after 2020? <sub></sub>
#### Ans: Jupyter Notebook

### 7. Which language has the highest average number of stars per repository? <sub></sub>
#### Ans: Jinja

### 8. Let's define leader_strength as followers / (1 + following). Who are the top 5 in terms of leader_strength? List their login in order, comma-separated. <sub></sub>
#### Ans: michaelliao, ityouknow, liuhuanyong, thunlp, shenghy

### 9. What is the correlation between the number of followers and the number of public repositories among users in Beijing? <sub>Regression slope of followers on repos (to 3 decimal places, e.g. 0.123 or -0.123)</sub>
#### Ans: 0.032

### 10. Does creating more repos help users get more followers? Using regression, estimate how many additional followers a user gets per additional public repository. <sub>Regression slope of followers on repos (to 3 decimal places, e.g. 0.123 or -0.123)</sub>
#### Ans: 0.656

### 11. Do people typically enable projects and wikis together? What is the correlation between a repo having projects enabled and having wiki enabled?  <sub>Correlation between projects and wiki enabled (to 3 decimal places, e.g. 0.123 or -0.123)</sub>
#### Ans: 0.279

### 12. Do hireable users follow more people than those who are not hireable? <sub>Average of following per user for hireable=true minus the average following for the rest (to 3 decimal places, e.g. 12.345 or -12.345)</sub>
#### Ans: 149.651

### 13. Some developers write long bios. Does that help them get more followers? What's the impact of the length of their bio (in Unicode words, split by whitespace) with followers? (Ignore people without bios) <sub>Regression slope of followers on bio word count (to 3 decimal places, e.g. 12.345 or -12.345)</sub>
#### Ans: -10.176

### 14. Who created the most repositories on weekends (UTC)? List the top 5 users' login in order, comma-separated <sub>Users login</sub>
#### Ans: zhufengnodejs, i5ting, mozillazg, hailiang-wang, HuangCongQing

### 15. Do people who are hireable share their email addresses more often? <sub>[fraction of users with email when hireable=true] minus [fraction of users with email for the rest] (to 3 decimal places, e.g. 0.123 or -0.123)</sub>
#### Ans: -0.280

### 16. Let's assume that the last word in a user's name is their surname (ignore missing names, trim and split by whitespace.) What's the most common surname? (If there's a tie, list them all, comma-separated, alphabetically) <sub>Most common surname(s)</sub>
#### Ans: Zhang

###
###
###