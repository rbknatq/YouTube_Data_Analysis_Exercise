# YouTube Data Analysis Exercise
Using the YouTube API to collect some data from five channels and analysing it, to hopefully understand their performance.

### This project was inspired by the article ["An Analysis of the Top Tech YouTube Channels with Python"](https://towardsdatascience.com/an-analysis-of-the-top-tech-youtube-channels-with-python-ad42c0291723) from Guillaume Weingertner in [Towards Data Science.](https://towardsdatascience.com/)

To use the YouTube API you need to request an API key in the Google Developers Console on the "Credentials" tab. Then you need to enable the YouTube API service. This is nicely explained by Weingertner in his article. You can also go to the [Google documentation](https://developers.google.com/youtube/v3/getting-started?source=post_page-----ad42c0291723--------------------------------) to get more detailed information.

To get the channel IDs you just need to go to the main page of the channel you are interested in, right click with your mouse and go to the "View page source" tab. There you can use the search function to go to the link that includes the "channel_id".

## Getting the Data:
On the "YouTube API Data gathering" file here in the repository you can see the step by step of gathering the data, making some preliminary cleaning and saving the data into .csv files. 

## Analysing the Data:
On the second Jupyter Notebook called "YouTube Analysis - five cooking channels" is the data analysis as such. There you will find some data transformation, some calculations and some visualizations. We had two .csv files to begin with "overview_data" and "videos_data".

### Takeaways from the Overview data:
* In general, the more views a channel gets, it seems they will have the most amount of subscribers. 
* Jauja Cocina mexicana has the highest amount of views and subscribers, even if her channel has the lowest viewer/subscriber ratio and the least amount of videos.
* Even though La Cocina de Loli Dominguez has almost the same viewer/subscriber ratio than Vicky Receta Fácil, Vicky has the second highest subscriber count, thanks to the fact that she has more views. 
* Temperos e Sabores has the highest viewer/subscriber ratio, but again, since she has the second lowest views, she also has the second lowest subscriber count of the group.
* It would be interesting to get more data to go deeper into how to get views for the channel, since that seems to be one of the (if not THE) key to the success of the channel.

### Takeaways from the Videos data:
* The two most common words all five channels use, both in titles and tags, are: "Fácil"(easy) and "Receta"(recipe). However, they use it much more often in the tags. Fácil(easy) is used in 99% of the video tags and Receta(recipe) is used around 90% of the time. In the title the words are used about 35-40% of the time.
* Besides those words, some other words repeat both in the title and tags. For example: Paso(step) from "paso a paso" or "step by step". That one is however much more frequently used in titles and it is number 20 in frequency in the tags.
* Horno (oven) is the 6th more common word in titles and the 7th more common word on tags.
* The words used give us an idea of what makes the channel interesting for viewers and what information are they looking for. 

* The duration of the videos does not seem to have an influence in the amount of views the video (or channel) gets. All five channels seem to be in a downward trend in views since 2021 approximately. in 2016 'Jauja Cocina Mexicana' published the videos that have given her  the most views in her channel. 'Vicky Receta Facil' published in 2015 the most succesful video or videos of her channel. All channels seemed to have an increase in views in around 2020, and this was most likely due to the pandemic and quarantine measures. 'Ana recetasfaciles' has succesful videos that she published in 2016, 2018 and 2020. She is also has an upward trend in the amount of videos she is releasing, this can be due to the use of YouTube Shorts, which are shorter videos that can be faster to produce. This may be confirmed by the graph of the duration of videos, where we see that 'Ana recetasfaciles' has been making shorter videos in average. 

* 'Jauja Cocina Mexicana' has little variation in the duration of her videos, and even though 'Temperos e Sabores' has a bit more peaks and valleys than 'Jauja', her videos tend to last more or less the same over the years. 'Vicky Receta Facil' had shorter videos in the early years of her channel. She made her longest videos around 2015 and 2018 and seems to have been making slightly shorter videos since.

## Conclusions

* This analysis was based on an arbitrary choice of channels. They do have some things in common: all five channels create content mainly in spanish, are hosted by a woman who started the channel at home on her own and not with a team of producers or similar. They all create sweet and savory recipes and all have over 2.5 million subscribers. 

* Content is king. Meaning, the data on this very small sample of channels shows that regardless of the year a video (or channel) was created, the duration of their videos, the conversion rate from view to subscriber or the amount of videos released... the higher the views, the higher the likes, subscriber count and comments. This would translate, in theory, in higher income for the channel, but the data gatehered in this case did not contain information on income or demographics. 

* Making content that attract views is the key. There are many strategies that people follow, but that is out of the scope of this analysis. What we could see from the data, is that some clues may be in the words used to title, describe and tag the videos, so a deeper analysis into the description of the videos and maybe the tags and titles per channel would be interesting.

* Increasing the number and types of channels may present interesting comparative results. Meaning, including more channels that have producers behind it, or focus only on sweet recipes, or have other formats of presenting the videos. 

* This was, in any case, a nice and fun project to practice the understanding of APIs, cleaning, analysing and visualizing data with python.

* I also created some of the graphics on my [Tableau Public profile](https://public.tableau.com/app/profile/rebeca.natera/viz/YouTubeAnalyticsProject-fiveHispanicCookingChannels/YouTubeAnalyticsProject), because it helps to practice with that tool as well and also the visualizations are a more interactive.
