# Kickstarting with Excel

## Overview of Project

In this project, we decided to look at the correlation between outcomes based on launch date and outcomes based on their fundraising goals.

### Purpose

The purpose of this analysis was to help Louise better understand correlation with how her fundraising campaign went compared to other campaigns. The first data that we pulled out is on the "Outcomes Based on Launch Date" worksheet. You can see where we looked at the success of campaigns across a 12-month period. We split out the data using a pivot table. From there we could see whether the campaign was canceled, failed, still live, or successful. We were then able to display the data in a line chart to look for any trends. The next data that we pulled was to look at the relationship between the outcomes based on their fundraising goal amount. To do this we created a simple table using rows and columns. The first part was to count the number of successful, failed, and canceled campaigns and list them based on their fundraising amount. The next step was to add up the total number of campaigns, regardless of amount, based on their fundraising goal amount. From there we were able to calculate a percentage based on whether the campaign was successful, failed, or was canceled.

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

To look at the "Outcomes Based on Launch Date", we created a Pivot Table with our data from the Kickstarter tab. We ended up filtering our Pivot Table using first the "Parent Category" and then the "Year". Our columns were based on the different types of outcomes (successful, failed, and canceled). We wanted to look at the data over the course of the year, so we used the "date created" column for our rows. Then for our values we used the "count of the outcomes" data column. We were finally able to visualize the data using a Line Pivot Chart.

![Theater Outcomes vs Launch Screenshot](https://user-images.githubusercontent.com/110848660/189773082-b71ad6ea-3ab9-4bfa-b269-cf6d194770e8.png)
![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/110848660/189771567-9d3f9db5-9544-47a3-9a9d-3e00aec4bdea.png)

### Analysis of Outcomes Based on Goals

To look at the "Outcomes Based on Goals", we created a table by labeling the necessary columns and then entering various rows labels for the goal amounts. We were able to come up with the number of successful, failed, and canceled campaigns by using the =countifs() function. We had to reference the "Kickstarter" worksheet to find up to three different criteria for getting the data we needed. Then we had to utilize the =sum() function to add up the total number of projects broken out by the goal amount. From there we were able to calculate the percentage of successful, failed, and canceled campaigns. We were finally able to visualize the data by using a line chart.

![Outcomes Based on Goal Screenshot](https://user-images.githubusercontent.com/110848660/189772960-38af69c5-df43-4fe6-aed3-74c737cd9514.png)
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/110848660/189771576-2577b6b9-5799-44b8-9f66-a424a63baac5.png)

### Challenges and Difficulties Encountered

*One of the challenges in the exercise was dealing with the unix time format. It is a hard format to read without changing it into a more readable format which we were able to do in Excel. This allowed us to have a better idea of when the campaigns were created.

*Another challenge was using the =countifs() functions in Excel while dealing with looking at data across different columns. Many of the formulas were looking at data with three different types of criteria which lead to a lot of parameters in the formular bar.

*The last challenge that I ran into was making sure that I was using the correct sign while looking for greater than or less than. I wasted some initial time and was dealing with some bad data in my chart before checking back over all of my formulas and finding my mistake. I also originally left out the equals sign which caused my numbers to be incorrect. It was a good lesson to make sure I check that more closely in the future.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

The first conclusion that I was able to draw from the data is that the highest number of successful campaigns occurred in May, June, and July. November and December appeared to have the lowest number of successful campaigns. 

The second conclusion that I had was that there was not as big of a swing with the failed campaigns like there were with the successful ones. There is a clear difference in the way the successful line looks compared to the failed line. The "Failed" line is consistent throughout the year before a dip in September and followed by a spike in October. October was also the only month without a canceled campaign on record.

- What can you conclude about the Outcomes based on Goals?

I can conclude from looking at the "Outcomes based on Goals" worksheet that most campaigns were for less than $5,000. We can also see that almost half of the entire kickstarter campaigns were in the “$1,000 to $5,000 dollar” range. The "Less than 1000" and "1000 to 4999" ranges had the most number of campaigns so it's not surprising to see them also have the two highest successful percentage rates. There was also a pretty big drop in the number of total projects once you get past the fundraising goal of $10,000. There was some success as we got into the higher fundraising goal ranges, but it was not very consistent. One other interesting thing that I noticed was that there were not any canceled fundraising campaigns in this subcategory.

- What are some limitations of this dataset?

One of the limitations of the dataset is that we had all of the countries combined. There is data from 21 different countries in this workbook so that should be considered when looking at the data. Some of these countries may not have the same number of donors or the ability of those donors to donate as high of amounts as in some other countries. If Louise is interested in doing another compaign, I'd recommend looking at kickstarter campaigns in whatever country she is looking to do the play in to get a better idea of what has had success there.

Another limitation of the dataset is that we looked at combined data over multiple years. There are possible economic events that could've happened in one or more countries during a particular year that could've swung the data in one direction. For example, if we wanted to look at a trend today over the last 5 years, we would need to account for the economic effects of Covid-19 and not treat every year the same.

The final limitation that came to mind was that there was no time element captured in our charts for the length of a campaign. We can't see if shorter campaigns fared better or worse than campaigns that ran longer. Having some data showing that time element may help Louise decide if it's worth running a long campaign or not in case she is having trouble reaching her goal. We were able to see an ideal time for launching the campaign but didn't really look into if there was correlation between a short campaign vs. a long one.

- What are some other possible tables and/or graphs that we could create?

I think one of the most beneficial things would be to create the same data and look at it with the data filtered out by country. That would give us a better understanding of how similar campaigns faired in a particular country. For example, one country may value theater more while another country may value film & video more.

Another possible thing to create would be to make tables based on the year. That way we could see if there were big swings in the number successful campaigns one year compared to the next year. Having a very successful month one year may not translate to the next year and combining them all together may skew the data.
