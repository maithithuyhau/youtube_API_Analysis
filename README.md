# Exploratory Data Analysing Using Youtube Video Data from Most Popular Data Science Channels
## I. Aims and objectives
Within this project, I would like to explore the following:
  1. Getting to know Youtube API and how to obtain video data.
    
  2. Analyzing video data and verify different common "myths" about what makes a video do well on Youtube, for example:

  - Does the number of likes and comments matter for a video to get more views?
     
  - Does the video duration matter for views and interaction (likes/ comments)?
    
  - Does title length matter for views?
    
  - How many tags do good performing videos have? What are the common tags among these videos?
    
  - Across all the creators I take into consideration, how often do they upload new videos? On which days in the week?
    
  - Explore the trending topics using NLP techniques
    
  - Which popular topics are being covered in the videos (e.g. using wordcloud for video titles)?
    
  - Which questions are being asked in the comment sections in the videos
    
## II. Steps of the project
1. Obtain video meta data via Youtube API for the top 5 channels in the data science niche (this includes several small steps: create a developer key, request data and transform the responses into a usable data format)
2. Prepocess data and engineer additional features for analysis
3. Exploratory data analysis
4. Conclusions
----------------------------------------------------------------------------------------------
### Exploratory data analysis
### 3.1 Views distribution per channel

With the video statistics for all channel, now we can see how the views are distributed per channel. Some channels might have a lot of views on one of their videos and the rest do not receive many views. Other channels might have more evenly distribution views per video. It can be observed thatTechWorld with Nana, codebasics have quite large variance in their views, suggesting that they have a few viral videos. Alex The Analyst, Thu Vu data analytics have less views overall but the views are more consistent across videos. 
![image](https://github.com/user-attachments/assets/7a66c6bf-3f57-4e9f-a1f5-2608e7a1523c)


#### 3.2 Does the number of likes and comments matter for a video to get more views?

After correcting for the absolute number of views, it turns out that the correlation is much less clear. The comment-view relationship seems to completely disappear: a lot of videos have millions of views and very few comments, while some vides have very few views have better interaction. However, it is understandable that comments take more effort than views and likes, and normally comments would die off when the video gets older.

As for like-view relatioship, we can still see some positive correlation between views and like ratio (though very subtle), which means that the more views a video has, the more people would hit the like button! This seems to support the idea of social proof, which means that people tend to like better the products that are already liked by many other people.
![image](https://github.com/user-attachments/assets/d91da362-ad6a-4fb0-83b0-985dbc383385)

![image](https://github.com/user-attachments/assets/96707338-44e0-4b11-8727-0cbb8494f52b)

#### 3.3 Wordcloud for words in title/comment

It can be seen that most common words are Data, Python, Tutorial, Science,  Projects, Analysis, Programming, Learning, which is very expected.
![image](https://github.com/user-attachments/assets/5f251a4d-a602-4199-bdb2-bee4f5af5571)


You can see that next to the obvious words such as "video", "data", the most frequent words are quite positive, such as "thank", "great", "learning", "well", "Excellent". A lot of comments also request something with the word "please".
![image](https://github.com/user-attachments/assets/eda42e0d-f109-47fd-8073-1ef2da9ca38b)


#### 3.4 Which day in the week are most videos uploaded?

It's interesting to see that more videos are uploaded on Tuesday and Saturday. Fewer videos are uploaded during the weekend. This could be because of the nature of the niche that is more geared towards tutorials and heavy materials, which is not suitable for weekends' consumption. But it could also just means that most creators work on their videos during the weekend or during the week and upload them beginning of the week or Saturday.

![image](https://github.com/user-attachments/assets/1a0f0904-4334-4b9c-83f2-fba5faf9e57b)
-------------------------------------------------------------------------------
### 4. Conclusions
In this Project, I have explored the video data of the five most popular data science/data analyst channels and discovered numerous interesting findings for anyone beginning a YouTube channel in data science or another topic:

- The more likes and comments on a video, the more views it receives. Likes appear to be a better sign of interaction than comments, and the number of likes appears to follow "social proof," implying that the more views the video receives, the more people would like it.
  
- Most videos contain between 5 and 30 tags.
  
- The average title length for the most viewed videos is 30-70 characters. excessively short or excessively long titles appear to reduce viewership.
  
- Videos are typically uploaded on Tuesday and Saturday. Weekends, particularly Sundays, are not popular for releasing new films.

- Comments on videos are generally positive, with a lot of "please" words, indicating possible market holes in material that may be addressed.
