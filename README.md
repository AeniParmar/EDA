---

# **Zomato Dataset Exploratory Data Analysis (EDA)**  

## **Project Overview**  
This project performs an exploratory data analysis (EDA) of the Zomato dataset to derive insights into restaurant ratings, country-wise data distribution, and other key trends. Additionally, it integrates country information using a supplementary dataset and visualizes findings to enhance understanding.  

---

## **Dataset Information**  

### **Datasets Used**:  
1. **zomato.csv**: Contains details of various restaurants, including ratings, location, and delivery options.  
2. **Country-Code.xlsx**: Maps country codes to their respective country names.  

### **Key Features in the Datasets**:  
- **Aggregate Rating**: Overall restaurant rating.  
- **Rating Color**: Visual representation of ratings.  
- **Country Code**: Identifier for restaurant locations.  
- **Has Online Delivery**: Indicates if online delivery is available.  
- **City**: City where the restaurant is located.  

---

## **Steps in Analysis**  

### **1. Data Loading and Initial Exploration**  
- Load the datasets using Pandas.  
- Display the first few rows of the data using `.head()`.  
- Inspect data types, check for missing values, and generate statistical summaries using `.info()`, `.describe()`, and `.isnull().sum()`.  
- Visualize missing data with a heatmap.  

### **2. Data Merging**  
- Merge `zomato.csv` with `Country-Code.xlsx` on the `Country Code` column using a left join.  

### **3. Data Visualizations**  

#### a. **Country-Wise Restaurant Distribution**  
- Create a pie chart for the top three countries with the highest number of restaurants.  

#### b. **Rating Analysis**  
- Group data by `Aggregate Rating`, `Rating Color`, and `Rating Text`.  
- Generate bar plots to analyze the number of ratings in each category.  
- Create a count plot for `Rating Color`.  

#### c. **Analysis of Zero Ratings**  
- Identify countries with restaurants having zero ratings.  

#### d. **Currency Usage by Country**  
- Group data by `Country` and `Currency` to map currencies used in each country.  

#### e. **Online Delivery Availability**  
- Analyze countries offering online delivery using value counts.  

#### f. **City-Wise Restaurant Distribution**  
- Create a pie chart for the distribution of restaurants across the top five cities.  

---

## **Observations**  

### **Rating Distribution**  
- Most ratings fall between **2.5 and 3.4**, indicating an average category.  
- A significant number of restaurants are **"Not Rated"**.  

### **Country Analysis**  
- **India** has the highest number of restaurants with zero ratings.  

### **Currency Analysis**  
- Each country uses its specific currency for transactions.  

### **Online Delivery**  
- Online delivery services are primarily available in **India** and the **UAE**.  

---

## **Libraries Used**  
- **Pandas**: For data manipulation and analysis.  
- **NumPy**: For numerical computations.  
- **Matplotlib**: For static visualizations.  
- **Seaborn**: For enhanced statistical data visualization.  

---

## **How to Run the Code**  

1. **Dataset Setup**  
   - Ensure both datasets (`zomato.csv` and `Country-Code.xlsx`) are in the same directory as the code file.  

2. **Install Dependencies**  
   - Install necessary libraries using the following command:  
     ```bash  
     pip install pandas numpy matplotlib seaborn  
     ```  

3. **Execution**  
   - Run the code in a Jupyter Notebook or any Python IDE.  

---

## **Future Scope**  
1. Extend the analysis to include **restaurant cuisines**.  
2. Perform **time-series analysis** if temporal data is available.  
3. Create an **interactive dashboard** for exploring the data more effectively.  

--- 
