# Video Game Data Analysis
<h3>Table of Content</h3>
<ul>
  <li>Project Description</li>
  <li>Dataset Description</li>
  <li>Executive Summary</li>
  <li>Data Cleaning</li>
  <li>Deep Dives</li>
  <li>Recommandations</li>
</ul>
<h3>Project Description</h3>
<p> This is a data analysis on a table of video games sold in North America, Europe, Japan, and other regions. The goal is to determine what drove the sales of video games. How the culture of different regions would influence the sales of games. Finally, I will recommand what game shops owners should do to get the right genres, titles and consoles to have a fantastic selling experience.</p>
<h3>Dataset Description</h3>
<p>
 This dataset is a single table dataset about video game sales. The cleaned table includes 17570 rows and 16 columns. It includes 12039 unique video game titles, 39 unique consoles, 20 genres, 673 publishers and 2663 developers with sales from North America, Europe, Japan, and other regions as well as the total sales. This table recorded video game sales from 1977-01-01 to 2020-12-31.
</p>

![table](https://github.com/user-attachments/assets/ea1fd3dd-bd75-40b8-bc38-338ff0d0b0b6)


<h3>Executive Summary</h3>
<p>
  Total sales ranges from 1977 with 2.5 million dollars from North America, Europe, Japan, and other regions and started accelerate in 1992 with exponential growth since then. It later reached a peak annual sale of 538.11 million dollars in 2008, and then it went down and drop to 3.45 million annual sales in 2020. The total sales had amounted to 6.6 billion dollars over the period. The decline was caused by lack of data rather than the decline of gaming industry. The top 2 consoles were PS series and Xbox series with total sales of 1046.86 million dollars and 859.93 million dollars respectively, and counts for 71% of total market. Top video games are always available in this two consoles. The most popular genres are Sports, Actions and Shooters with total sales of 1187.51, 1125.89 million and 995.5 million dollars, 50% of total sales. The most popular franchises are Grand Theft Auto, Call of Duty, FIFA. Genres and titles that are sold well are those related the most to a region's culture. The most profitable publishers are Activation, EA, EA sports, Ubisoft, THQ with total sales of 722.77, 644.13,485.66, and 462.57 million dollars respectively. Top publishers and developers have enough power to determine even dictate the direction of a region's gaming culture if not globally.</p>

![Sales_shares1](https://github.com/user-attachments/assets/8c471e12-1a52-49da-82b6-01a8200c6fc7)


<h3>Data Cleaning</h3>
<ol>
  <li>Removed rows with null values in such columns as na_sales, other_sales, pal_sales, and jp_sales simultaneously. </li>
  <li>Replaced null values with 0s for the columns of total_sales, na_sales, other_sales, pal_sales, and jp_sales. Then remove rows of with 0s in all sales columns.</li>
  <li>Create a new column called “Year” derived from release_date columns.</li>
  <li>The number of total rows had dropped from 64091 to 17570. It was a big reduction, but the sum of total sales from the new data frame didn’t reduce at all comparing to the old data frame. So, it’s not going to affect our analysis. </li>
  <li>Regrouped console into console families with three categories. PS series, Xbox series, and other series.</li>
</ol>
<h3>Deep Dives</h3>
<ol>
  <li>Regional Sales trend. From 1977 to 2020, video game sales started at 2.5 million dollars in 1977, and didn’t explode 1993 for all regions, which coincide with the release of the most popular console of all time PlayStation series. Sales in all regions peaked in the year of 2008 with 290 million in NA, 146.42 in Europe, 30 in Japan, and 71 in other regions. Then it has coming down since due to lack of data rather than the decline of the industry. </li>
  
![Sales_Trend](https://github.com/user-attachments/assets/d3f3e0e8-4843-41fc-b57d-8c5ab3126381)


  
  <li>Sale shares Trend. In terms of market shares for the entire period, North America has made the biggest sales of 3345.52 million dollars (51% of the total share), European market 1916.83 million dollars (29%), Japanese and other markets at 652 million (10%) and 687 million dollars (10%). Thus, the total sale across all regions in this period is 6605 million dollars. In terms of percentage sale shares through the period, until 1984, America had over 80% market shares, then it was overtaken by Japan until 1997. Starting 1997, America started topping video game sales and dominated.</li>

![Sales_shares2](https://github.com/user-attachments/assets/c6fb9521-773f-43d7-b09f-0f6c6c1a7463)

  
  <li>Console family sales. In terms of console series, PS was introduced in 1994, which enabled the exponential growth of the gaming market as a whole. Xbox was introduced in early 2000s. All in all, PS has a market share of 49%, Xbox 21%, and the rest 31%. For top 10 best sold consoles for all regions, it always includes PS, Xbox and Nintendo families. PS series outperformed Xbox in every region especially in its home turf, Japan. Both consoles continue to own a lion share of market combined.</li>

![console_family_sales2](https://github.com/user-attachments/assets/693bfb05-a402-4d84-a1cc-f5e0f80c2f4b)


![console_family_sales](https://github.com/user-attachments/assets/c6e18d9a-948d-4258-b7ab-e7b4c97e93c6)
  
  <li>Genre Sales. There are 20 genres in total from this dataset. The top 3 genres in term of sales are action, shooter, and sports across all regions except in Japan, the list includes role-play, sports and actions. The top 3 genres take up around 50% market shares of all time across regions. Japan had very different top genres as its top three were role play, sports and actions. It looks like Japan is not very big on American gun cultures.</li>

![genre_sales](https://github.com/user-attachments/assets/5a395138-0bd9-475c-b2ef-a597bc3ea108)


  
  <li>Titles sales. It has a lot to do with the region’s cultures. For example, in North America, the top 10 titles were dominated by 7 call of duty, which are in the genre of shooter, which has a lot to do with America’s gun cultures. In Europe, 6 out of top 10 titles were dominated by FIFAs from the sports genre. Thanks to their love of soccer. In Japan, the top 10 titles are all Japanese home-grown games produced by Japanese developer and published by Japanese companies. Also, most of those top 10 are only available in Nintendo, which are Japanese consoles. For other regions, it’s top 10 very similar to American’s top10. It means American cultures are very influential in those regions. Basically, titles are very unique to its own cultures tend to be popular in its own region but under perform in other regions. For example, FIFA and call of duty are popular in its own region but under performs in Japan. We can see, Japanese are very protective of their town cultures. </li>

![title_sales1](https://github.com/user-attachments/assets/642b9876-5325-4eb0-88ac-71f800cb62b6)

![title_sales2](https://github.com/user-attachments/assets/721fed4c-6298-41da-a672-de27db1b4e2e)


  
  <li>Publisher sales. There are 673 publishers. The top 10 publishers take up around 60% of market shares across all regions. Except in Japan, the top publishers are Activation, EA, EA sports, Ubisoft, THQ and Sega. In Japan, however, the top publishers are all Japanese companies. Top developers are subsidiaries of top publishers. </li>
</ol>

![publisher](https://github.com/user-attachments/assets/8a509644-f242-41f1-b9a6-06500ef24e85)

<h3>Recommandations</h3>
<p>
 Bestselling titles and bestselling genres are very dear to regions’ own cultures and tend to under perform in others. However, it could over perform if the culture is influential in other regions. For game retail stores, they should sell and promote titles and the genres, which are center to the region’s cultures. Soccer is very popular in Europe; that’s why FIFA was doing well in Europe. Basketball and football are popular in the states, but the video games are not, those games should be promoted and pushed to get better sales in the regions, both games are not in top 10 currently.  FIFA is doing well in Europe but not Japan, and people in Japan love soccer as well, so it would be a good idea to promote FIFA games to Japanese market and to try win a spot in top 10 titles. FIFA could also be promoted to Chinese market since Chinese people are crazy about soccer as well, and Chinese market is large. In addition, American’s popular video games should also be promoted in China since America cultures are still influential in China.  Also, any game stores should prioritize PS, Xbox, and Nintendo gaming consoles since most games are only available in the three consoles. For example, most Japanese games are only available in Japanese consoles. If developers want to take a bite of Japanese gaming market, it’s better off to collaborate with Japanese local companies since Japanese are very protective of their cultures.  
</p>

