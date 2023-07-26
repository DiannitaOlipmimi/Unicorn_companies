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
- `roi_category` : kategori selisih modal dan nilai asset perusahaan (100% profitable, unprovitable)
- `year category` : kategori selisih tahun perusahaan berdiri dan menjadi unicorn (less than 5 years, more than 5 years)

### 📒 Tujuan:
membuat model regresi yang dapat memprediksi harga penjualan rumah berdasarkan variabel yang ada

### 📒 Langkah Analisis:
✅ *Exploratory Data Analysis* (EDA):
1. Melakukan pengecekan apakah terdapat missing data, duplicate data, dan error data
2. Mengambil tahun pada kolom `date joined` dan mengubahnya menjai kolom `year joined`
3. Menghitung selisih tahun didirikannya perusahaan dengan ditetapkannya menjadi unicorn dengan cara mengurangi kolom `year founded` dengan `year joined`
4. Menghitung ROI atau *Return of Investment* dengan cara:

[]`valuation`-`funding`]/`funding` 

5. Membuat kolom baru yang berisi kategori ROI yang terbagi menjadi perusahaan telah 100% profitable dan unprofitable
6. Membuat kolom baru yang berisi kategori tahun yang terbagi menjadi less than 5 years dan more than 5 years

## 📌**Result**
### 📒 Data Card:

### 📒 Stack area chart:

![Alt text](<Images/stacked area chart.png>)

### 📒 Stacked bar chart:

![Alt text](<Images/funding bar chart.png>)

![Alt text](<Images/valuation bar chart.png>)

### 📒 Stack column chart:

![Alt text](<Images/funding column chart.png>)

![Alt text](<Images/valuation column chart.png>)

### 📒 Stack pie chart:

![Alt text](<Images/roi pie chart.png>)

![Alt text](<Images/years pie chart.png>)

### 📒 Visualisasi:
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