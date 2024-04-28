# Excel-ling

I worked on the Google Data Analytics Capstone Project, Track 1, Case Study 1. I will be diving into the background, my full process of cleaning, analyzing, and visualizing the data, along with my final suggestions and summary of the data. 

# **BACKGROUND**
Cyclistic is a bike-sharing program that features more than 5,800 bikes and 600 docking stations. It offers reclining bikes, hand tricycles, and cargo bikes, making it more inclusive to people with disabilities and riders who can't use a standard two-wheeled bike. It was founded in 2016 and has grown tremendously into a fleet of bicycles that are tracked and locked into a network of 692 stations across Chicago. The bikes can be unlocked from one station and returned to any other station in the system at any time. 

Previously, Cyclistic's marketing strategy tried to build general awareness and appeal to broad consumers. It has flexible pricing plans: single-ride passes, full-day passes, and annual memberships. Those who purchase single-ride or full-day passes are referred to as casual riders while those who purchase annual memberships are Cyclistic members. 
My Role: In this scenario, I am a junior data analyst at Cyclistic and my team has been tasked with the overall goal (see below) of designing marketing strategies 

Overall Goal: Design marketing strategies aimed at converting casual riders into annual members.
Business Question: "How do annual members and casual riders use Cyclistic bikes differently?"

Below I will be describing my roadmap for this.

# **Case Study Roadmap **

PROCESS:
Overview: I first analyzed the data separately (each month) in Excel, then used R to analyze the data as a whole (one year). Finally, I created a dashboard in Tableau and used Figma to support the design elements. 

My First tool was Microsoft Excel because I was most familiar with and I could get a general understanding of the data quickly. I did not combine all of the spreadsheets into one because that would've taken more processing power and I would have been a pcless guy lol.

I began downloading the data from divvy-tripdata and turning the .csv files into Excel spreadsheets. I downloaded the most recent year of data which was at the time of starting my project: 

12 Months, Year 2023
January
February
March
April
May
June
July
August
September
October
November
December

Added 4 columns to all of the months:
Created **ride_length** calculated the total ride length for each trip using the start_at column which was: ending time minus starting time. 
Created **day_of_week, Hour, and Timex(Minutes)** and calculated the day of the week for each trip using the start_at column date.
Went over the business task and the information I had at hand and how that could be used to figure out how members and casual riders use the bike service differently

Came up with metrics to look at such as : 
**total number of rides per hour, per day of the month, per season, per day of the week, between member and casual and for different bike types 
Average ride length between members and casual**

For every month in Excel created pivot tables and charts to go with the analysis (this took the longest):

Total Rides per Weekday - calculated the total rides for members and casual and separated it by day of the week; used a cluster column chart
Average Ride Length - calculated the average ride length for members and casual and separated it by day of the week;
Total Rides per Hour -  calculated the total rides for members and casual separated by the time of the day (24hr); 
Total Rides per Day -  calculated the total rides for members and casual separated by the day of the month; 
Total Rides per Bike Type - calculated the total rides for members and casual separated by Bike type;

I also created a Google Docs Notes list where I wrote down the exact steps for each month (had a checklist) and included my insights for each month.

Well after reading all this you must be getting bored. Then Let's get to the visualization part

# So here's my first chart Total Rides Per Bike Type 

![image](https://github.com/imporu/Excel-ling/assets/161977105/56be5efa-f93a-4aad-95ff-05e975ce08ee)

Based on the above graph and after analyzing these trends :  
1. Seasonal Trends: From the data, it's evident that there are seasonal trends in bike usage, with higher ridership during warmer months (May to September) compared to colder months (November to March). The company can leverage these seasonal patterns to allocate resources effectively, such as increasing bike availability during peak months and optimizing operations during off-peak months.
2. Preference for Electric Bikes: Electric bikes show a consistent increase in usage over the months, indicating a growing preference among customers. The company can capitalize on this trend by expanding its electric bike fleet and promoting electric bike usage through targeted marketing campaigns.
3. Marketing and Promotions: The data highlights opportunities for marketing promotions and incentives during low-demand months, such as November to March, to encourage ridership and maintain revenue streams during off-peak periods. Special discounts, loyalty programs, or seasonal promotions can attract more riders during these times.
4. Infrastructure Investment: The company should assess the demand for docked bikes versus classic bikes and allocate resources accordingly. If there is a significant demand for docked bikes, the company should invest in expanding docking station infrastructure to meet customer needs and improve accessibility.
5. Customer Engagement: Analyzing the data can provide insights into customer behavior and preferences. The company can use this information to enhance customer engagement strategies, such as personalized recommendations, targeted communications, and loyalty programs, to improve customer satisfaction and retention.
6. Partnerships and Collaborations: Exploring partnerships with local businesses, events, or transportation authorities can help increase visibility and attract new customers. Collaborations with ride-sharing services or public transportation systems can also provide additional transportation options and enhance the overall customer experience.

# Here's the second graph : 

![image](https://github.com/imporu/Excel-ling/assets/161977105/5370f31c-1a6b-489f-a4a5-17678033a94e)

1. Member Retention and Engagement: The data shows that the number of rides by members consistently exceeds those by casual users across all months. To maintain this trend and encourage member retention, Cyclistic should focus on enhancing the overall user experience for members. This could include providing exclusive benefits, rewards, and incentives for members, such as discounts on additional services or priority access to popular bikes during peak hours.
2. Promotions for Casual Users: While the number of rides by casual users is lower compared to members, there is still a significant portion of the customer base. Cyclistic can target casual users with promotional campaigns and special offers to encourage repeat usage and potentially convert them into members. For example, offering discounted membership rates or free trial periods for casual users can incentivize them to become long-term members.
3. Segmented Marketing Strategies: Recognizing the distinct preferences and behaviors of casual users versus members, Cyclistic should develop segmented marketing strategies tailored to each user type. This involves analyzing user data to understand their preferences, usage patterns, and demographics. By targeting messages and promotions specifically to each segment, Cyclistic can effectively engage with users and drive desired actions, such as increasing membership sign-ups or boosting ride frequency.
4. Data-Driven Decision Making: Continuously monitoring and analyzing user data is essential for making informed business decisions. Cyclistic should invest in data analytics tools and capabilities to track key metrics related to user behavior, satisfaction, and retention. By leveraging data insights, Cyclistic can identify opportunities for improvement, optimize marketing campaigns, and enhance overall business performance.
5. Customer Support and Communication: Providing excellent customer support and communication channels is crucial for both casual users and members. Cyclistic should ensure prompt responses to user inquiries, address any issues or concerns effectively, and regularly communicate updates, promotions, and relevant information to keep users engaged and informed.
6. Community Building and Engagement: Building a sense of community among users can foster loyalty and encourage active participation. Cyclistic can create online forums, social media groups, or offline events where users can connect, share experiences, and provide feedback. By fostering a vibrant and supportive community, Cyclistic can strengthen its brand image and enhance user satisfaction.

# Here's the third Graph :

![image](https://github.com/imporu/Excel-ling/assets/161977105/8d8337b3-1525-479e-9a9e-67988f54dd41)

1. Optimize Bike Availability: Adjust bike availability based on the average ride length per weekday to ensure an adequate supply of bikes during peak usage periods. For instance, on Thursdays and Fridays, when average ride lengths are longer, Cyclistic should increase the number of bikes available to meet higher demand and prevent shortages. Conversely, on Tuesdays when average ride lengths are shorter, resources can be reallocated to other days or stations with higher demand.
2. Promote Weekend Rides: Since Saturdays and Sundays have relatively high average ride lengths, Cyclistic can launch targeted marketing campaigns to promote weekend rides and encourage users to take advantage of longer leisurely rides. Special promotions, events, or themed rides can attract more riders and boost weekend usage, contributing to increased revenue and user engagement.
3. Introduce Weekday Incentives: To stimulate weekday ridership, Cyclistic can introduce incentives such as discounted rates or bonus ride credits for rides taken during off-peak hours or on days with shorter average ride lengths, such as Tuesdays and Wednesdays. These incentives can encourage users to incorporate biking into their weekday routines for commuting or errands, diversifying usage patterns and spreading demand more evenly throughout the week.
4. Tailored Marketing Messages: Customize marketing messages and communications based on average ride lengths per weekday to resonate with users' preferences and behaviors. For example, on Thursdays and Fridays when average ride lengths are longer, Cyclistic can emphasize the benefits of leisurely rides, exploring new routes, or enjoying extended outdoor activities. On Tuesdays and Wednesdays, messages can focus on the convenience and efficiency of biking for short trips or commuting.
5. Improve Weekday Infrastructure: Enhance station infrastructure and amenities on weekdays to accommodate longer rides and support user needs. Cyclistic can prioritize maintenance and cleanliness, install additional bike racks or docking stations in high-traffic areas, and provide facilities such as bike repair stations or rest areas along popular routes to enhance the overall riding experience on weekdays.
6. Data-Driven Operations: Continuously analyze ride length data by weekday to identify trends, patterns, and areas for improvement. Cyclistic should leverage data analytics tools and techniques to monitor changes in user behavior, assess the effectiveness of interventions, and make data-driven decisions to optimize operations and enhance customer satisfaction.

# Here's fourth map and findings: 

![image](https://github.com/imporu/Excel-ling/assets/161977105/973688a2-c632-4247-bc01-9bf8c0e82f6e)

1. Resource Allocation: Allocate resources such as bikes, staff, and maintenance activities based on the total rides per weekday. Days with higher ride counts, such as Thursday, Friday, and Saturday, may require increased staffing levels and more frequent bike redistribution to ensure adequate bike availability and optimal service quality.
2. Peak Hour Management: Identify peak hours on high-traffic weekdays and implement strategies to manage peak demand effectively. For example, Cyclistic can offer incentives for off-peak rides, adjust pricing dynamically based on demand, or introduce queue management systems to streamline bike pickup and return processes during peak hours.
3. Promotional Campaigns: Launch targeted promotional campaigns and incentives to encourage ridership on weekdays with lower total rides, such as Sunday and Monday. Special discounts, rewards, or themed events can incentivize users to take more rides during these days, ultimately balancing demand across the week and maximizing bike utilization.
4. Infrastructure Enhancement: Invest in infrastructure enhancements, such as expanding docking station capacity or optimizing station placement, to accommodate higher demand on weekdays with the highest ride counts. By improving accessibility and convenience, Cyclistic can enhance the overall user experience and encourage more frequent rides on these days.
5. Community Engagement: Foster community engagement and participation by organizing events, group rides, or challenges on weekdays with lower total rides. These initiatives can help build a sense of camaraderie among users, promote active lifestyles, and drive weekday ridership, contributing to a more vibrant and engaged user community.
6. Data-Driven Decision Making: Continuously monitor and analyze ride data to identify trends, patterns, and opportunities for optimization. By leveraging data analytics tools and techniques, Cyclistic can make informed decisions, adapt strategies in real-time, and stay responsive to evolving user needs and preferences.

# Here's my Fifth map and findings 

![image](https://github.com/imporu/Excel-ling/assets/161977105/63d3ac61-ed98-40e0-9355-33f8025317f2)

1. Peak Hour Management: Identify peak hours with the highest number of rides and implement strategies to manage peak demand effectively. Cyclistic should ensure an adequate supply of bikes and docking stations during peak hours to prevent shortages and accommodate increased rider traffic.
2. Dynamic Pricing: Implement dynamic pricing mechanisms to incentivize ridership during off-peak hours and balance demand throughout the day. Offering discounted rates or promotional fares during non-peak hours can encourage users to shift their rides to less congested times, optimizing bike utilization and reducing strain on resources during peak periods.
3. Infrastructure Expansion: Expand infrastructure capacity, particularly at high-traffic locations and during peak hours, to accommodate the surge in demand. Cyclistic should invest in additional bike racks, docking stations, and maintenance facilities to ensure seamless bike availability and service reliability, especially during peak periods of rider activity.
4. User Engagement: Engage with users through targeted marketing campaigns and incentives to promote rides during off-peak hours. Cyclistic can offer rewards, loyalty points, or exclusive benefits for rides taken during less busy times, encouraging users to explore alternative commuting options and spread out demand across the day.
5. Data-Driven Operations: Continuously monitor and analyze ride data to identify trends, patterns, and opportunities for optimization. Cyclistic should leverage data analytics tools and predictive modeling techniques to forecast demand, plan resource allocation, and optimize operational efficiency, ultimately enhancing the overall user experience and maximizing system performance.
6. Collaboration with Local Partners: Collaborate with local businesses, event organizers, and transportation authorities to promote ridesharing initiatives and integrate biking into multi-modal transportation networks. Cyclistic can explore partnerships to offer seamless connectivity between bike-sharing services and public transit systems, providing users with convenient and sustainable mobility solutions throughout the day.

# Here's my Sixth map and findings :

![image](https://github.com/imporu/Excel-ling/assets/161977105/52f2f119-84ae-494c-88ba-d1b2061ec67a)

1. Seasonal Marketing Campaigns: Tailor marketing campaigns and promotions to align with seasonal fluctuations in ridership. During peak months with higher ride counts, such as May, June, July, and August, Cyclistic can launch targeted campaigns to capitalize on increased demand and attract new users. In contrast, during low season months like November and December, focus on retention strategies and incentives to maintain engagement and encourage repeat usage.
2. Forecasting and Resource Planning: Utilize historical ride data to forecast future demand and plan resource allocation accordingly. By anticipating peak periods and adjusting staffing levels, bike inventory, and maintenance schedules in advance, Cyclistic can ensure optimal service delivery and minimize disruptions during periods of high demand.
3. Event Sponsorship and Partnerships: Leverage major events, festivals, and community initiatives occurring during peak months to boost ridership and brand visibility. Cyclistic can explore sponsorship opportunities, offer event-specific promotions, or collaborate with event organizers and local businesses to provide bike-sharing services as part of event transportation solutions, enhancing user convenience and promoting sustainable mobility options.
4. Customer Engagement and Retention: Enhance customer engagement and loyalty programs to incentivize repeat usage and foster long-term relationships with users. Cyclistic can offer rewards, discounts, or exclusive perks for frequent riders, encourage user referrals, and solicit feedback to improve service quality and meet evolving user needs continuously.
5. Geographic Expansion and Service Enhancement: Evaluate ride data to identify underserved areas or potential growth opportunities and prioritize expansion efforts accordingly. Cyclistic can target areas with high demand or limited transportation options, deploy additional bikes and stations, and invest in infrastructure improvements to enhance accessibility and coverage, thereby attracting new users and expanding the customer base.
6. Data-Driven Decision-Making: Continuously monitor key performance indicators, track trends, and analyze user behavior to inform strategic decision-making and optimize operations. Cyclistic should leverage data analytics tools and predictive modeling techniques to identify patterns, forecast future demand, and proactively address challenges, ensuring the sustainability and success of its bike-share program over the long term.

# An analysis on avg. ride length by user_type:

Average ride length for casual users: 40.33 minutes
Average ride length for members: 53.83 minutes
Now, let's derive recommendations based on this analysis:

1. Tailored Pricing Plans: Since members tend to take longer rides on average compared to casual users, Cyclistic can consider offering tiered pricing plans that cater to different usage patterns. For example, the company could introduce a plan with a higher monthly fee but lower per-minute rates for members who frequently take longer rides. Conversely, casual users who typically take shorter rides may benefit from plans with lower monthly fees but slightly higher per-minute rates.
2. Incentivize Longer Rides for Casual Users: To encourage casual users to take longer rides, Cyclistic can introduce incentives such as discounted rates for rides exceeding a certain duration. By offering promotions or rewards for longer rides, Cyclistic can motivate casual users to explore more extensive routes and prolong their riding experience, potentially increasing revenue and user satisfaction.
3. Optimize Bike Distribution: Understanding the average ride length by user type can inform decisions related to bike distribution and station placement. Cyclistic can allocate more bikes to stations located in areas frequented by members, where longer rides are more common. Additionally, the company can strategically place stations in tourist or leisure destinations to attract casual users interested in shorter rides for sightseeing or recreational purposes.
4. Enhance User Experience: Since longer rides may indicate a higher level of engagement and satisfaction among members, Cyclistic should prioritize initiatives aimed at enhancing the overall user experience for members. This could include investing in bike maintenance to ensure a smooth and enjoyable ride, improving station infrastructure for convenient docking and unlocking, and providing additional amenities or services at select stations to cater to the needs of members.
5. Promote Membership Benefits: Highlighting the benefits of membership, such as access to longer ride durations at a lower cost per minute, can incentivize casual users to consider upgrading to a membership. Cyclistic can leverage targeted marketing campaigns and communications to showcase the value proposition of membership and encourage casual users to make the switch.
6. Continuous Data Analysis: Regularly analyzing ride length data by user type is essential for monitoring trends, identifying opportunities, and adapting strategies accordingly. Cyclistic should establish robust data analytics processes to track key metrics related to ride length, user behavior, and membership conversion rates. By staying informed and agile, Cyclistic can optimize its operations and offerings to meet the needs of its user base better.

# **Summary**

And at last here's a summary of the above data :

1. Peak Hour Management:
Implement strategies to manage peak demand, reducing wait times and increasing user satisfaction.
Increase bike availability during peak hours by 20%.
Aim to reduce peak hour wait times by 15%.
2. Dynamic Pricing:
Implement dynamic pricing to incentivize rides during off-peak hours.
Offer a 10% discount on rides during off-peak hours to encourage usage.
3. Infrastructure Expansion:
Invest in infrastructure expansion to accommodate peak demand.
Increase docking station capacity by 30% in high-traffic areas.
4. User Engagement:
Launch targeted promotional campaigns to increase ridership during off-peak hours.
Aim for a 10% increase in off-peak rides through promotional incentives.
5. Data-Driven Operations:
Utilize data analytics tools to forecast demand and optimize resource allocation.
Target a 10% improvement in operational efficiency through data-driven decision-making.
6. Seasonal Marketing Campaigns:
Tailor marketing campaigns to capitalize on seasonal fluctuations in ridership.
Aim for a 15% increase in ridership during peak months through targeted promotions.
7. Event Sponsorship and Partnerships:
Leverage partnerships with events and festivals to increase ridership.
Target a 20% increase in ridership during sponsored events.
8. Customer Engagement and Retention:
Enhance customer engagement and loyalty programs to retain users.
Aim for a 10% increase in customer retention through loyalty incentives.
9. Geographic Expansion and Service Enhancement:
Prioritize expansion efforts in underserved areas to attract new users.
Target a 25% increase in ridership through geographic expansion.
10. Continuous Monitoring and Optimization:
Continuously monitor key performance indicators to identify trends and optimize operations.
Target a 10% improvement in overall system performance through continuous optimization efforts.

These recommendations aim to address various aspects of Cyclistic's operations and marketing strategy, focusing on optimizing resource allocation, increasing ridership, and enhancing the overall user experience. Each recommendation is quantified to provide clear targets and metrics for evaluation and performance tracking.
