# J124-Final
## By Sofia Schnurer

dataset: https://docs.google.com/spreadsheets/d/1uBeZoFyMGG1coBuBjTrJCk-j13NVXJF6V0TOm8bHr4E/edit#gid=898543253, https://github.com/BuzzFeedNews/2016-10-facebook-fact-check

## Data Analysis Questions: 

### 1. What was the most widely shared post from these outlets and was the post from a right-leaning or left-leaning outlet?
![question 1](https://github.com/sofia-sch24/J124-Final/blob/38b657e356eb6115e4d488d6f774240a59e3e500/question%201.png)

How I found the answer: Sort the column "share count" from Z ---> A. This should give you the largest share count at the top. 

The most widely shared post in this dataset is by Occupy Democrats with a share count of 1,088,995. Notably, this post contains no factual content meaning this is misinformation. As classified by Buzzfeed, Occupy Democrats is a left-leaning site and the information posted was in the form of a video. 

### 2. Of the posts that were comprised of photos, was the content mostly true or was there no factual content?
![question 2](https://github.com/sofia-sch24/J124-Final/blob/354224851dce37137bd0c0de1953599ec0d7fcdb/question%202.png)

How I found the answer: Create a FILTER on the sheet of "Post Type" and "Rating" only. The formula I used was =FILTER(G2:H2283,G2:G2283 ="photo")

Upon creating this filter, it was very easy to notice that "no factual content" was designated to the majority of photos. Therefore, based on the content in this dataset, the posts that were photos had a majority rating of "no factual content"

### 3. Of the 3 categories (left, mainstream, and right), which one contained the most "mostly false" and "no factual content" in their ratings?
![question 3](https://github.com/sofia-sch24/J124-Final/blob/e774a377651c849f29ec23442b525055770d7362/question%203.png)

How I found the answer: Go to "insert" and create a pivot table. Select "category" for row, "rating" for column, and COUNTA "rating" for value. The pivot table will categorize the number of posts based on "rating" and "category". 

By using this pivot table, I found that left-leaning sites in this dataset had the most ratings "no factual content". However, by combining the ratings of "mostly false" and "no factual content", right-leaning sites overwhelmingly produced the most misleading posts with 178 of 666 posts. 

### 4. Of the various sites, what is their category makeup? Additionally, which sites received the highest share count?
![question 4](https://github.com/sofia-sch24/J124-Final/blob/16cd3e56b60a4b3f5f0eafe816b785bdc1f4c1c2/question%204.png)

How I found the answer: Go to "insert" and create a pivot table. Select "page" for row, "category" for column, and  SUM "share count" for value. The pivot table will categorize the summary of share counts based on page and category. 

### 5. In the days leading up to the 2016 election, what was the makeup of mostly true to less factual content? Was there more "no factual content" ratings in the last few days the content in this dataset was published?
![question 5](https://github.com/sofia-sch24/J124-Final/blob/9db8c4b39ffdcf308ba7e1e1db0c0c75f12250a5/question%205.png)

How I found the answer: Go to "insert" and create a pivot table. Select "Date Published" for row, "rating" for column, and COUNTA "rating" for value. The pivot table will categorize the posts based on rating and date published. 

## Data Visualization

![data viz 1](https://github.com/sofia-sch24/J124-Final/blob/54c9e9b3a75f4f50171ed7fce0e37dfa664f184c/data%20viz%201.png)


## Story Pitch and Sources

It is essential with the prevalence of social media to understand and identify disinformation and extreme content. Many experts are now advising users to excerise increased caution with content on the internet and social media in general. Facebook has shaped the 2016 election and the past 6 years through their inability to curb misinformation. In so many ways, having content without restrictions feeds into Facebook's strategy for more users and more time spent on the platform. As a OSINT researcher at the Berkeley Law Human Rights Center, I've used open source investigations to identify and verify human rights violations. In my findings, I do come across disinformation and understand the methods to verify sources but this knowledge is not widely accessible. Seeing how prevalent misinformation is across social media made me intrigued to do some data analysis on it. 

As anyone would know, misinformation is very dangerous as some content can further racism, xenophobia, sexism, homophopbia, anti-semitism, and islamophobia. Misinformation also contributes to climate change denial, anti-vaccinations, and increased partisanship. 

What intrigues me is understanding how Facebook has changed its policies and whether these policies have been effective in countering misinformation. I hope to speask with experts and facebook users on how they feel policies have changed and whether they've seen increased effectiveness in countering misinformation. I hope to write a story discussing the changes Facebook has made as a response to the Cambridge Analytica scandal and overall disinformation surrounding the 2016 election and whether these policies have been effective in countering misinformation. I hope to add testimony from leading researchers in the communications and misinformation field regarding Facebook's policies changes and the concerns these researchers have over the lack of awareness surrounding misinformation. I hope to also interview Craig Silverman, the co-author of the Buzzfeed report I based my data analysis off, to hear his observations after writing that massive report and whether he notices differences in the emergence of misinforming posts from the outlets the report studied (ex. CNN Politics, Freedom Daily, Occupy Democrats). 

## Sources

1. Professor Stephanie Edgerly- stephanie.edgerly@northwestern.edu, (847) 467-2528
Edgerly is an Associate Professor at Northwestern University studying disinformation and its effects on media. Her work focuses on how social media alters the way an audience chooses to consume news and how this impacts their political engagement. I would ask her questions regarding how the 2016 election has shaped Americans' trust in social media and if she beleives misinformation has worsened on the platform. 

2. Professor Kenneth Joseph- kjoseph@buffalo.edu, 716-645-0682
Joseph is an Assistant Professor of Computer Science and Engineering at the University of Buffalo. His expertise focuses on misinformation and politics as well as societal impacts of social media and online platforms. I would ask his questions regarding whether Facebook's new policies has effectively contributed to removing more misleading posts and steps users can take to tell if posts on Facebook are misleading, besides reviewing the source. 

3. Craig Silverman, craig.silverman@buzzfeed.com
Silverman is the founding editor of the report published by Buzzfeed and the dataset I based my work off of. Although the report is dated back to the 2016 election, I would like to ask him and contributing reporters on his team the most surpising work they found during this report. I would also ask if they have noticed marked changes in the proliferation of misinformation on Facebook today in comparison to 2016 (the year the report was written). 

### Additional Data Sources: 

1. Q2 2022 Widely Viewed Content Report by Meta, https://transparency.fb.com/data/widely-viewed-content-report/

2. "In Ukraine, Facebook fact-checkers fight a war on two fronts" by The Washington Post, https://www.washingtonpost.com/technology/2022/04/12/facebook-fact-checkers-misinformation-ukraine-war/
