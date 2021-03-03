## Youtube trending videos analysis

### Trending on Youtube
Trending helps viewers what is happening on YouTube and in the world. Trending aims to surface videos that a wide range of viewers would find interesting. Some trends are predictable, like a new song from a popular artist or a new movie trailler.
The lsit of trending videos is updated roughly every 15 minutes.

![image of youtube](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/trend_youtube.jpg)

### Here we can see that  the given videos  were trended in 2017-18 mostly.

![image of count trend](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/count_trend.png)

### Here we can see how views,likes, dislikes are assocciated to each other

![image of corr_heatmap](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/corr_heatmap.png)

The takeaway from here is that views has association with likes, dislikes and comment count. Which is intuitive for most people. The most strongest assocoaion between views and likes. 

### Here we can see correlation between variables

![image of views_likes_scatter](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/corr_multivar.png)

We can see that views and likes variables have strong positive correlation.The more views the more likes. Same applies to dislikes, comment count. Also, we can observe outliers.

### Here we can see numbers of times the video  were trended in each category

![image num of trend by category](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/num_of_trendingvid.png)

That is right the videos from Entertainment category were in trend more times than other video.

### Here we can see what content is about in Entertainment category 
![image of words_cloud](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/word_count.png)

### Here we can see the video that had been viewed 252 million times for just less than a month
![image of gambino gif](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/gambino.gif)

### Lets take a look how quickly video generated the views (i.e. temparature) 
![image of gambino rised up](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/gambino_risedup.png)

Interestingly, what enabled such a tremendous growth? I assumed that video went viral.

### Here we can see overal dynamic in views in the same period of time

![image of total views plot](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/total_views_plot.png)

### Here top 10 videos from YouTube trend in 2017-18
![image of top 10 content](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/top10_wereintrend.png)


## Conlusion

* We defined that content from Entertainment category were in YouTube Trend most times 
* We defined top 10 videos that were in Trend most times amongst all categories
* We define strong association between views, likes, dislikes
* We define positive correlation between views, likes, dislikes
* We define video that was viewed 252 million time  for less than  a month

Lastly, lets see views & likes count by category. But this time, beacause we know about outliers like Gambino and others, we should apply median to check central tendency

```data.groupby('category_name').agg('median').sort_values(by='views',ascending=False)```

### Here we can see views & likes by category
![image of likes&views](https://github.com/evgenygrobov/EDA-case-study/blob/main/images/likes_views_category.png)

Clearly, Gaming and Music category lead the group with more views. Keep in mind, if you want to start doing business on YouTube, that not all videos went viral! 





