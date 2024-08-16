# Exploring YouTube Music Channels: Insights Through Data Analysis

### Medium - Article(https://medium.com/@niraliparikh17/exploring-youtube-music-channels-insights-through-data-analysis-8a64e20449f0)

## Project Overview

This project explores data from popular YouTube music channels to uncover patterns and factors contributing to their success. By analyzing metrics such as subscriber counts, view counts, likes, comments, tags, and upload times, we aim to identify key elements influencing a channel's popularity and video performance.

### Key Insights

- **Subscriber vs. View Trends:** A stacked column chart reveals that Trap Nation leads with around 30 million subscribers, while Sony Music Entertainment has the fewest subscribers among the analyzed channels. Interestingly, higher subscriber counts do not always correlate with more views, suggesting that subscriber numbers alone may not determine a channel’s success.

- **Likes and Comments Correlation:** Scatter plots indicate a strong correlation between views and both likes and comments, with likes showing a more significant relationship. As view counts increase, so do likes and comments. However, when normalized to likes and comments per 1000 views, the correlation weakens, especially for comments. This may be due to the greater effort required for comments compared to likes and a decrease in interaction as videos age.

- **Title Length:** The scatter plot of title length versus views shows no strong relationship. Most-viewed videos have titles between 10 and 100 characters, but title length does not significantly impact view count.

- **Tags Count:** Analysis using scatter plots shows that videos with 5 to 30 tags are most common. Although there's no clear relationship between the number of tags and view count, videos with too few or too many tags tend to receive fewer views, suggesting an optimal range for tag count.

- **Upload Patterns:** The line and stacked column chart reveals a higher frequency of uploads on Tuesdays and Fridays, with fewer uploads on weekends. This pattern might reflect increased viewer engagement on these days.

## Dataset

Data was collected from nine popular YouTube music channels using the YouTube API. Key metrics include subscriber count, view count, and video-specific details. The dataset includes additional columns such as `tagsCount`, `likeRatio`, `commentRatio`, `titleLength`, `Day`, `Likes per 1000 Views`, and `Comments per 1000 Views`.

### Channels Analyzed

1. **Atlantic Records** 
2. **Warner Music India**
3. **TheSoundYouNeed** 
4. **Sony Music Entertainment**
5. **NPR Music** 
6. **YouTube Music** 
7. **Trap Nation** 
8. **Coke Studio Pakistan** 
9. **HollywoodRecordsVEVO** 

## Data Collection Process

1. **Data Extraction:** Data was collected using Python's `pytube` library and the YouTube API. The `googleapiclient.discovery` module was used to build the API client.
2. **Statistics Retrieval:** Channel statistics such as subscriber count, view count, and video count were extracted.
3. **Video Data:** Retrieved details including title, description, tags, views, likes, comments, and upload date.
4. **Data Enrichment:** Additional columns for tags count, like ratio, comment ratio, and title length were added.
5. **Data Visualization:** The enriched CSV file was imported into Power BI for visualization and analysis.

## Visualizations

- **Subscribers by Channel Name:** Stacked Column Chart
- **Views by Channel Name:** Stacked Column Chart
- **Views vs. Subscribers Trends:** Line and Stacked Column Chart
- **Likes and Comments Correlation:** Scatter Charts 
- **Title Length vs. Views:** Scatter Chart
- **Tags Count vs. Views:** Scatter Chart
- **Upload Frequency by Day:** Stacked Column Chart

## Instructions for Use

1. **API Setup:** Obtain a YouTube API key and list of channel IDs.
2. **Data Extraction:** Run the provided Python code to collect channel and video data.
3. **Data Processing:** Save the data into a CSV file and upload it into Power BI.
4. **Visualization:** Use Power BI to create visualizations and analyze the data.

## Dependencies

- Python
- `pytube` library
- YouTube API
- `pandas` library
- `numpy` library
- `matplotlib` 
- `matplotlib.ticker` 
- `googleapiclient.discovery` for API client
- Power BI for data visualization

## Future Enhancements

- Expand the analysis to include more channels and different genres.
- Explore the impact of video content and genre on viewership.
- Implement machine learning models to predict video success based on tags, title length, and upload time.
