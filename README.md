<h1>Crop Production Analysis (2005-2015)</h1>
<h3>Project Overview: -</h3>
<p>In this project, I utilized a combination of Power BI and Python libraries to conduct a comprehensive and detailed analysis of crop production data from 2005 to 2015. Python was primarily used for data cleaning, including handling null values and removing outliers, after which the cleaned data was imported into Power BI for further analysis and visualization.</p>
<p>Within the Power BI dashboard, I compared crop production data at both the state and district levels. I also explored how crop production varied across different seasons, allowing for a deeper understanding of regional and seasonal patterns in agricultural output.
To gain clearer insights, I employed various metrics such as Total Production, Total Area under Cultivation, and Production per Area. These metrics helped identify trends and patterns in crop production over the decade. They also provided a basis for understanding the top-performing states and crops, the relationship between cultivation area and production output, and other crucial correlations.</p>
<p>Throughout the project, several interesting facts and insights emerged, such as the identification of the states with the highest production, the seasonal impacts on crop yields, and how certain crops performed better in specific regions. These insights not only highlight key agricultural trends but also offer a detailed look at the factors influencing crop production in India during this time period
</p>
<h3>Data Source: -</h3>
<p>For this project, I utilized an Excel file downloaded from Kaggle.</p>
<p><b>Crop Production data:</b> The dataset consists of over 200,000 records of agriculture-related data spanning from 1997 to 2015. It contains information on the total production (in metric tons) of various crops across multiple states in India. Additionally, it provides details on the amount of land under cultivation (in acres) for different crops in various regions. The dataset also includes season-wise and district-wise breakdowns, offering a comprehensive view of agricultural activities across different states.</p>
<h3>Tool Used: -</h3>
<ul>
  <li>Power BI desktop</li>
  <li>Power BI query editor</li>
  <li>Jupyter notebook</li>
  <li>Python with Pandas, NumPy libraries</li>
</ul>
<h3>Data Cleaning and Transformation: -</h3>
<p>The dataset spans a significant time period, from 1997 to 2015, which introduces some data irregularities such as null values and outliers. I used Python for data cleaning, including handling null values and removing outliers.</p>
<p>To identify outliers, I applied the Z-score method, which is calculated using the formula:</p>
<p>Z-score = |data value – mean|/standard deviation</p>
<p>I applied this formula to the Area column and marked records with a Z-score greater than 3 as outliers, which I then removed from the dataset.</p>
<p>For handling null values, only the Production column had missing data. To improve accuracy, I created a new column, Production per Area, by dividing the production value by the area while keeping the null values in place. Instead of removing the null values, I grouped the data by State, District, Crop, and Season, and replaced the nulls with the mean of the respective group.</p>
<p>Finally, I divided the dataset into four parts based on different time periods and exported them as CSV files. For further analysis, I focused on the period from 2005 to 2015 and imported that subset into Power BI Desktop.</p>
<h3>Metrics Used: -</h3>
<ul>
  <li>Total Production</li>
  <li>Total Area</li>
  <li>Percent growth in production and agricultural land</li>
  <li>Production per area</li>
  <li>Total Crops</li>
</ul>
<h3>Key Findings: -</h3>
<ul>
  <li>The states with the highest overall agricultural production are Kerala, Tamil Nadu, and Andhra Pradesh. Kerala significantly dominates due to its large advantage in      coconut production, which has the largest share among all crops. Kerala is the biggest coconut producer.</li>
  <li>In terms of production per area, the top states are Punjab, Puducherry, Kerala, Andaman & Nicobar Islands, and Andhra Pradesh.</li>
  <li>States with the largest agricultural land areas are Uttar Pradesh, Madhya Pradesh, Maharashtra, Karnataka, Bihar, and Rajasthan.</li>
  <li>Coconut and sugarcane are the most produced crops, accounting for 80-90% of total production.</li>
  <li>Kerala, Andhra Pradesh, and Tamil Nadu are the leading states in coconut production.</li>
  <li>Uttar Pradesh, Maharashtra, Tamil Nadu, and Karnataka are the dominant producers of sugarcane.</li>
</ul>
<h4>Season-wise insights: -</h4>
<ol>
  <li>Autumn: -</li>
  <ul type="disc">
    <li>Northern and eastern states like Bihar, Odisha, West Bengal, and Assam hold a large share in production.</li>
    <li>Major crops for this season include maize, rice, jute, paddy, and ragi.</li>
  </ul>
  <li>Kharif: -</li>
  <ul type="disc">
    <li>Uttar Pradesh and Maharashtra are the main producers, with Karnataka, Madhya Pradesh, and Gujarat also contributing significantly in terms of agricultural land.</li>
    <li>Key crops of this season are sugarcane, sweet potato, ginger, rice, and maize.</li>
  </ul>
  <li>Rabi: -</li>
  <ul type="disc">
    <li>Uttar Pradesh leads in total production during this season, followed by West Bengal, Madhya Pradesh, and Bihar.</li>
    <li>Main crops of this season include potato, onion, papaya, tapioca, cabbage, and pineapple.</li>
  </ul>
  <li>Summer: -</li>
  <ul type="disc">
    <li>West Bengal leads in total production during the summer season, with Assam and Karnataka also contributing significantly.</li>
    <li>Major crops include banana, sugarcane, brinjal, and potato.</li>
  </ul>
  <li>Winter: -</li>
  <ul type="disc">
    <li>Odisha, Assam, Bihar, and West Bengal hold the largest share in total production.</li>
    <li>Prime crops of this season are sugarcane, potato, wheat, paddy, and rice.</li>
  </ul>
</ol>
<h4>Some Important Findings: -</h4>
<ul>
  <li>Apart from the Kharif season, total production in all other seasons has seen positive growth over the decade.</li>
  <li>Crops that have experienced significant production growth over the decade, along with their leading contributing states, include:
    <ol type="1">
      <li>Oilseeds, Mango, Brinjal, Papaya, Cowpea – Andhra Pradesh</li>
      <li>Cowpea, Dry Ginger, Black Pepper, Arecanut – Karnataka</li>
      <li>Pulses – Uttar Pradesh and Madhya Pradesh</li>
      <li>Ginger – Assam and Nagaland</li>
      <li>Lentil – Uttarakhand</li>
    </ol>
  </li>
  <li>States that have shown remarkable percentage growth in production over the decade include:
    <ol type="1">
      <li>Tamil Nadu (8872%)</li>
      <li>Andhra Pradesh (133.94%)</li>
      <li>Assam (140%)</li>
      <li>Maharashtra (73%)</li>
      <li>Bihar (96%)</li>
      <li>Madhya Pradesh (61%)</li>
      <li>Chhattisgarh (182%)</li>
    </ol>
  </li>
  <li>Although coconut and sugarcane are the top two crops in production, their production growth has been modest at 8.25% and 1.75%, respectively.</li>
  <li>Several crops with significant total production have seen negative growth, primarily due to a significant reduction in agricultural land. Examples include banana, tapioca, cabbage, sweet potato, and garlic.</li>
  <li>Interestingly, there are crops with negative production growth but positive growth in production per area.</li>
</ul>
<h3>Learning Outcomes: -</h3>
<p>Aside from creating dashboards and visuals, one of the most valuable lessons I learned in this project was the importance of data cleaning. To derive accurate and consistent insights that won’t mislead viewers, it's essential to work with clean data that has minimal irregularities. This project gave me a great opportunity to apply data cleaning techniques, ensuring the data was free of errors or outliers that could distort the analysis. I used Python libraries extensively for these operations, which reinforced my understanding of how crucial data preparation is to the overall success of any data analysis project.</p>
