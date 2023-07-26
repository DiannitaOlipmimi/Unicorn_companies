# Unicorn_companies
### **Visualisasi Unicorn Companies**
Private companies with a valuation over $1 billion as of March 2022, including each company's current valuation, funding, country of origin, industry, select investors, and the years they were founded and became unicorns.


## 📌Table of contents
- [Study Case](https://github.com/DiannitaOlipmimi/regresi_linier#study-case)
- [Result](https://github.com/DiannitaOlipmimi/regresi_dan_asumsinya#step-by-step-analysis)
- [Dataset](https://github.com/DiannitaOlipmimi/regresi_dan_asumsinya#step-by-step-analysis)
- [Links](https://github.com/DiannitaOlipmimi/regresi_dan_asumsinya#step-by-step-analysis)

## 📌**Study Case**
### 📒 Data dan Variabel:
data yang didapatkan merupakan data yang memiliki informasi harga-harga penjualan rumah pada tahun-tahun sebelumnya. data ini memiliki data numerik dan data kategorikal dengan variabel-variabelnya,
- `Company` : nama perusahaan yang telah terdaftar menjadi unicorn
- `Valuation` : nilai asset perusahaan
- `Date Joined` : tanggal perusahaan terdaftar menjadi unicorn
- `Industry` : industri perusahaan
- `City` : kota asal perusahaan
- `Country` : negara asal perusahaan
- `Continent` : benua asal perusahaan
- `Year Founded` : tahun didirikannya perusahaan
- `Funding` : jumlah modal perusahaan
- `Select Investors` : investor yang menanamkan modal kepada perusahaan
- `Year Joined` : tahun perusahaan menjadi unicorn
- `roi` : return of Investment (profitabilitas) perusahaan
- `range` : selisih modal dan nilai asset perusahaan 
- `roi_category` : kategori selisih modal dan nilai asset perusahaan [100% profitable, unprovitable]
- `year category` : kategori selisih tahun perusahaan berdiri dan menjadi unicorn [less than 5 years, more than 5 years]

### 📒 Tujuan:
membuat model regresi yang dapat memprediksi harga penjualan rumah berdasarkan variabel yang ada

### 📒 Langkah Analisis:
✅ *Exploratory Data Analysis* (EDA):
1. Melakukan pengecekan apakah terdapat missing data, duplicate data, dan error data
2. Mengubah data kategorik menjadi ata numerik apabila diperlukan
3. Melakukan deskriptif statistik pada data (melihat rata-rata, median, dan nilai lainnya)
4. Memvisualisasikan data untuk melihat pola data
5. Melihat adanya outlier menggunakan boxplot
6. Mencari hubungan antar variabel menggunakan scatter plot

Analysis Steps:

Data Loading and Initial Exploration:

Load the Unicorn Companies dataset into the analysis environment.
Check the dimensions of the dataset (number of rows and columns).
Examine the first few rows to get a sense of the data structure and variables.
Data Cleaning and Preprocessing:

Handle missing values and outliers, if any, to ensure data integrity.
Convert data types as needed for visualization (e.g., converting the valuation from text to numeric format).
Overview Visualization:

Create a bar chart or pie chart to visualize the distribution of unicorn companies across different industries or countries.
Show the top industries and countries with the highest number of unicorn companies.
Valuation Distribution:

Plot a histogram or box plot to visualize the distribution of company valuations.
Analyze the spread of valuations and identify any potential outliers or extreme values.
Time Trend Analysis:

Create a line chart or area chart to visualize the trend of unicorn companies founded over the years.
Analyze the growth of unicorn startups and identify any spikes or declines in their formation.
Funding Analysis:

Generate a bar chart or stacked bar chart to visualize the number of funding rounds for unicorn companies.
Compare the funding rounds' frequencies across different industries or countries.
Correlation Analysis:

Create a heatmap to visualize the correlation between valuation and other numeric features (e.g., funding rounds, year of founding).
Identify any significant correlations that may influence a company's valuation.
Geographic Visualization:

Use a geographic map or choropleth map to visualize the distribution of unicorn companies across different countries.
Adjust the map colors based on valuation to highlight the countries with the highest-valued startups.
Bubble Chart for Industry Insights:

Generate a bubble chart to represent the relationship between valuation, funding rounds, and industry.
Size the bubbles based on valuation and color them by industry to visualize patterns.
Interactive Dashboard:

Combine multiple visualizations into an interactive dashboard using tools like Tableau or Plotly.
Allow stakeholders to explore the data dynamically, filtering by industry, country, or valuation.
Insights and Recommendations:

Summarize key findings and insights from the visualizations.
Identify emerging trends, potential growth opportunities, and challenges faced by unicorn companies.
Provide recommendations for investors, entrepreneurs, and policymakers based on the data-driven analysis.
By visualizing the Unicorn Companies dataset, stakeholders can gain valuable insights into the unicorn startup landscape, helping them make informed decisions and strategies related to investments, market opportunities, and industry-specific trends.

## 📌**Result**
![Alt text](Images/dashboard.png)


## 📌**Dataset**
### **Unicorn Companies**
|Company              |Valuation      |Date Joined|Industry                       |City          |Country      |Continent    |Year Founded|Funding        |Select Investors                                                      |Year Joined|roi     |range|roi_category   |year category   |
|---------------------|---------------|-----------|-------------------------------|--------------|-------------|-------------|------------|---------------|----------------------------------------------------------------------|-----------|--------|-----|---------------|----------------|
|Yidian Zixun         |$1,000,000,000.|17-Oct-17  |Mobile & telecommunications    |Beijing       |China        |Asia         |2021        |$151,000,000.  |Phoenix New Media, Tianjin Haihe Industry Fund                        |2017       |562.25% |-4   |100% profitable|less than 5 year|
|Flink Food           |$3,000,000,000.|1-Dec-21   |E-commerce & direct-to-consumer|Berlin        |Germany      |Europe       |2021        |$1,000,000,000.|Mubadala Capital, Bond, Prosus Ventures                               |2021       |200.00% |0    |100% profitable|less than 5 year|
|Playco               |$1,000,000,000.|21-Sep-20  |Other                          |Tokyo         |Japan        |Asia         |2020        |$140,000,000.  |Sozo Ventures, Caffeinated Capital, Sequoia Capital                   |2020       |614.29% |0    |100% profitable|less than 5 year|
|Mensa Brands         |$1,000,000,000.|16-Nov-21  |Other                          |Bengaluru     |India        |Asia         |2021        |$218,000,000.  |Accel, Falcon Edge Capital, Norwest Venture Partners                  |2021       |358.72% |0    |100% profitable|less than 5 year|
|ClickHouse           |$2,000,000,000.|28-Oct-21  |Data management & analytics    |Portola Valley|United States|North America|2021        |$300,000,000.  |Lightspeed Venture Partners, Almaz Capital Partners, Altimeter Capital|2021       |566.67% |0    |100% profitable|less than 5 year|

## 📌**Links**
https://www.mavenanalytics.io/data-playground?accessType=open&order=fields.numberOfRecords

https://www.investopedia.com/articles/basics/10/guide-to-calculating-roi.asp#:~:text=Return%20on%20investment%20(ROI)%20is%20an%20approximate%20measure%20of%20an,finally%2C%20multiplying%20it%20by%20100.