# People are becoming more and more away from doing sex

## Background 

Population aging is a one of the biggest issues of the world. Is is well know that one reason of the aging is the increase of average life due to the improvement of the healthcare. Another reason is the decrease of the number of births. 

So why the number of births is decreasing? One explanation may be that contraception has spread due to sex education. However, the data from a long term survey in the US, it turns out that people are becoming more and more away from doing sex. This would be the direct cause of decreasing of the birth. In this post, I explain the trend using the data.


## Data

The data to use is originally from the General Social Survey (https://gssdataexplorer.norc.org/). The survey is conducted from 1989 for every two years, and asking the frequency of doing sex in the last one year to adult people in the US. The questions were asked to 1,372 - 4,510 people for each time, and got 552 - 2,137 effective answers. 

In the question, the respondents answer one of the followings:

- Not at all
- Once or twice
- Once a month
- 2-3 times a month
- Weekly
- 2-3 per week
- 4+ per week
- Dont know
- not applicable 

## What we can know from the data

In the followings. I categorized the data and visualize it so that we can see the trend. 

Following chart is dividing the responedents into people who had sex once a week ore more and people less than that. 
The percentage of having no less than once a week was 46% in 1989 and 36% in 2018, and the chart shows there is a slow but steady trend of decreasing. 


```python
from IPython.display import Image
Image("./chart1.png")
```




![png](output_7_0.png)



Then what is the breakdown of people who did not have sex once a week?
Following chart breaks down the people into two groups, people who did have it once a month or more, and people who did less. 
What this shows is that the segment who did ses less than once a month is increasing. The number is that 29% in 1989 and 36% in 2018. 

The numbers of 2012 is different from other years. I think these are irregular numbers coming from sampling errors etc.


```python
Image("./chart2.png")
```




![png](output_9_0.png)



Let us further divide the less than once a month segument. Following chart divides the segment into people who did it once or more in the last year, and people who did not do. 
Both segments are increasing in the past 30 years, but the segment who did not do sex even for once increase more. 22% in 1989 to 27% in 2018. 

People who do not do sex are increasing. 


```python
Image("./chart3.png")
```




![png](output_11_0.png)



### End Note

This post saw the 30 year trand of freqnecy of doing sex of US adult, and discussed that the frequency is steadily decreasing and especially people who do not do sex at all are increasing. This clearly suggests that this is one of the reason of low birth rate and thus society aging.
This may be the same in other developed countries where the birth rate is decreasing. 

So why is that? Unfortunately this data cannot tell more about in detail. To do so, we need further detailed survey and data. 
For example, we need to understand the changes by age groups, because the changes of age balance in the population might have caused the change. It should be nice to see the changes in the same age group. 
Also, if we see the difference in the different income group, area of residence (ex. urban and rural), we may be able to find some reasons, such as lower income makes having sex difficult or urbanization may be the cause. 

Also, we need to be aware that the data have limited stability. As mentioned earlier, in some year the result shows irregular figures, also as you see below, there are many 'not effecitive ansers' that means they did not answer etc. Non effective answers were omitted from the analysis above, but If people who did not answer were all very freuent or less frequent, the conclusion can be changed. 


```python
Image("./chart4.png")
```




![png](output_14_0.png)



## Interactive Visualization 

Following is the interactive visualization. You can move around and see detailed numbers for each year. 


```python
%%HTML
<div class='tableauPlaceholder' id='viz1581504932390' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Am&#47;AmericanSexFrequency_15814952861410&#47;Story1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='AmericanSexFrequency_15814952861410&#47;Story1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Am&#47;AmericanSexFrequency_15814952861410&#47;Story1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1581504932390');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='1016px';vizElement.style.height='991px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>
```


<div class='tableauPlaceholder' id='viz1581504932390' style='position: relative'><noscript><a href='#'><img alt=' ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Am&#47;AmericanSexFrequency_15814952861410&#47;Story1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='AmericanSexFrequency_15814952861410&#47;Story1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Am&#47;AmericanSexFrequency_15814952861410&#47;Story1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='filter' value='publish=yes' /></object></div>                <script type='text/javascript'>                    var divElement = document.getElementById('viz1581504932390');                    var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='1016px';vizElement.style.height='991px';                    var scriptElement = document.createElement('script');                    scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                </script>



Link to Tabeleau Public: https://public.tableau.com/profile/dslearner#!/vizhome/AmericanSexFrequency_15814952861410/Story1?publish=yes

Data Source: data.world  https://data.world/makeovermonday/2019w29/workspace/file?filename=Americans+Sex+Frequency.xlsx
