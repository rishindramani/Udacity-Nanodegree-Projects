# Ford GoBike Trip Data Visualization for 2018
## by Rishindra Mani Katiyar


## Dataset
>The dataset was originally made up of 1863721 rows and 14 columns. After cleaning,dropping null rows and adding new columns, the dataset now consist of 1851950 rows and 18 columns. The variables are as follows:

>* Trip Duration (seconds)
>* Start Time and Date
>* End Time and Date
>* Start Station ID
>* Start Station Name
>* Start Station Latitude
>* Start Station Longitude
>* End Station ID
>* End Station Name
>* End Station Latitude
>* End Station Longitude
>* Bike ID
>* User Type (Subscriber or Customer – “Subscriber” = Member or “Customer” = Casual)
>* Bike share for all trip
  
I added the following columns:

>* Start_month
>* Start_weekday
>* Start_hour
>* Duration_min



## Summary of Findings

>In the exploratory analysis,I found out that most trips were taken between 8am and 9am in the morning and between 5pm and 6pm in the evening during weekdays and users mostly make use of the bikes during Summer which makes sense because weather conditions have a significant effect on the bicycle Sharing system.Trips tend to be shorter on Monday through Friday compared to weekends.The highest trip taken in days of the week was on Tuesday and the highest trip taken in the month of the year was in October.Generally, average trip takes up to 14 minutes but the average trip depends on if the user is a Subscriber or Customer.



>I also found out that there are a lot more subscribers users than customers.Subscribers makes use of the bike sharing system heavily on weekdays thereby making the number of trips peaked around 8-9am in the morning and 17-18pm in the evening.There were more trips on weekdaydays (Mon-Fri) compared to weekends because subcribers use the bike sharing system more on weekdays than weekends while customers use the bike sharing system more on weekends than weekdays.Customers tend to ride for fun or for leisure in the afternoon or early evenings during weekends as most of them are either tourist or visitors while Subscribers use the bike sharing system as a means of transport to work thus most trips were on work days (Mon-Fri) and especially during rush hours (when going to work in the morning and getting off work in the afternoon).


## Key Insights for Presentation
>using nbconvert to export the notebook and set up a server for the slides.
> >jupyter nbconvert slide_deck_template.ipynb --to slides --post serve --template output_toggle

>For the presentation, I focus on the influence of user type, time duration, weekday and month on bike sytem data. I started by introducing start week variable and then use countplot to see how bike sharing system is used during the week.

>Afterwards, I introduced the independent categorical variable(user type)to plot dependent variable. To start,I use the countplot to plot bike user type by month using user type variable as hue.I also use boxplot to plot start week and time duration, using user type as hue. then I used heatmap to plot weekdays and user start hour across user type.

