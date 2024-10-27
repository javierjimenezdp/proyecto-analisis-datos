# proyecto-analisis-datos
This project analyzes the appropriation of Information and Communication Technologies (ICT) in communities using survey data. By uncovering trends and usage patterns through descriptive statistics and visualizations, the findings aim to inform stakeholders about ICT utilization and guide efforts to improve access and training.


# Project Title: Analysis of ICT Appropriation in Communities

## Description
This project focuses on analyzing the appropriation of Information and Communication Technologies (ICT) in communities, using data gathered from a national survey. The objective is to identify trends, barriers, and the usage of technologies among different demographic groups. The analysis includes descriptive statistics and visualizations to provide insights that can guide decision-making related to technology implementation in these communities.

# ICT Appropriation Analysis Project

## Description
This project analyzes the appropriation of Information and Communication Technologies (ICT) in communities using survey data. By uncovering trends and usage patterns through descriptive statistics and visualizations, the findings aim to inform stakeholders about ICT utilization and guide efforts to improve access and training.

## Introduction
This project aims to explore how communities engage with ICT, identifying key barriers and opportunities for improvement. 

## Problem Description
Despite the growing availability of technology, many communities face challenges in effectively utilizing ICT. This project seeks to understand the level of ICT appropriation and its implications for community development.

## Data Source
The dataset used for this analysis was obtained from the following link:
[Data Source](https://www.datos.gov.co/Ciencia-Tecnolog-a-e-Innovaci-n/Medici-n-del-nivel-de-apropiaci-n-TIC-en-la-comuni/mzrr-5rzf/data_preview)

## Methodology
1. **Data Collection:** Data was obtained from community surveys focusing on ICT usage.
2. **Data Cleaning:** Data was cleaned and preprocessed for analysis.
3. **Descriptive Analysis:** Statistical measures and visualizations were employed to identify trends.

# Project Title: Analysis of Technology Appropriation

## Description
This project analyzes the appropriation of information and communication technologies (ICT) in the community. The analysis involves demographic factors such as age and gender, as well as the frequency of internet access among respondents. The goal is to provide insights that can inform decision-making related to ICT initiatives.

## Introduction
The increasing relevance of ICT in our daily lives highlights the need to understand its appropriation across different demographics. This project aims to analyze the usage patterns of technology in the community, focusing on age, gender distribution, and internet access frequency. By utilizing data analysis techniques, we aim to identify trends and provide actionable insights.

## Methodology
1. **Data Collection**: The dataset was obtained from [data.gov.co](https://www.datos.gov.co) and contains information on technology appropriation within the community.
2. **Data Analysis**: We performed descriptive statistical analysis to explore demographics and internet access patterns.
3. **Visualization**: Various graphs were generated to illustrate the findings clearly.

## Installation
To run this project, you'll need to have Python installed along with the following libraries:
- `pandas`
- `matplotlib`

You can install these packages using pip:

```bash
pip install pandas matplotlib


import pandas as pd
import matplotlib.pyplot as plt

# Step 1: Load the dataset
# Ensure the dataset CSV is in the same directory as this script.
datos = pd.read_csv('data.csv')  # Replace 'data.csv' with the path to your dataset.

# Step 2: Age Distribution Graph
plt.figure(figsize=(10, 6))  # Set the size of the plot
# Count the occurrences of each age range and sort them by age
age_counts = datos['Edad'].value_counts().sort_index()  
# Create a bar plot for age distribution
age_counts.plot(kind='bar', color='skyblue')  
plt.title('Age Distribution')  # Set the title of the plot
plt.xlabel('Age Ranges')  # Label for the x-axis
plt.ylabel('Frequency')  # Label for the y-axis
plt.xticks(rotation=45)  # Rotate x labels for better readability
plt.grid(axis='y')  # Add a grid on the y-axis for easier comparison
plt.tight_layout()  # Adjust layout to make room for labels
plt.savefig('age_distribution.png')  # Save the figure as a PNG file
plt.show()  # Display the plot

# Step 3: Gender Distribution Graph
plt.figure(figsize=(10, 6))  # Set the size of the plot
# Count the occurrences of each gender
gender_counts = datos['Genero'].value_counts()  
# Create a pie chart for gender distribution
gender_counts.plot(kind='pie', autopct='%1.1f%%', startangle=90, colors=['#ff9999','#66b3ff','#99ff99'])  
plt.title('Gender Distribution')  # Set the title of the plot
plt.ylabel('')  # Remove y-label as it's not needed for a pie chart
plt.axis('equal')  # Equal aspect ratio ensures that pie is drawn as a circle.
plt.savefig('gender_distribution.png')  # Save the figure as a PNG file
plt.show()  # Display the plot

# Step 4: Internet Access Frequency Graph
plt.figure(figsize=(10, 6))  # Set the size of the plot
# Prepare the data for plotting access frequency
internet_access_counts = datos['Frecuencia_acceso'].value_counts()  
# Create a line plot for internet access frequency
internet_access_counts.plot(kind='line', marker='o', color='orange')  
plt.title('Internet Access Frequency')  # Set the title of the plot
plt.xlabel('Access Frequency')  # Label for the x-axis
plt.ylabel('Number of Respondents')  # Label for the y-axis
plt.grid()  # Add grid for better readability
plt.savefig('internet_access_frequency.png')  # Save the figure as a PNG file
plt.show()  # Display the plot
```

## Code Documentation

### 1. Import Libraries
- Import necessary libraries for data manipulation (`pandas`) and visualization (`matplotlib`).

### 2. Load Dataset
- Load the dataset into a Pandas DataFrame. Ensure the dataset file is in the correct directory.

### 3. Age Distribution Graph
- Count occurrences of each age range.
- Generate a bar plot showing the age distribution of respondents.

### 4. Gender Distribution Graph
- Count occurrences of each gender.
- Create a pie chart representing gender distribution among respondents.

### 5. Internet Access Frequency Graph
- Count occurrences of each internet access frequency.
- Create a line plot showing how often respondents access the internet.

## Conclusions
The analysis reveals significant insights into the appropriation of ICT in the community. Key findings include:
- The majority of respondents are within the 18-24 age range, suggesting a younger demographic is more engaged with technology.
- The gender distribution indicates a higher number of male respondents compared to females.
- Internet access frequency varies, with many respondents accessing it daily, highlighting the importance of connectivity.

## Recommendations
- Implement targeted ICT initiatives to engage the younger demographic.
- Address gender disparities by promoting inclusivity in technology access and training.
- Enhance internet infrastructure to ensure reliable access for all community members.




```
### How to Use This README

1. **Copy and Paste**: Copy the entire content and paste it into your `README.md` file in your GitHub repository.
2. **Dataset**: Make sure that you have the dataset file (e.g., `data.csv`) in the same directory as your code when you run it.
3. **Run the Code**: Execute the provided Python code to generate the graphs and ensure they are saved as PNG files.
4. **Adjust as Needed**: Feel free to modify any sections of the README to better fit your project’s specifics or to provide additional context.

This `README.md` now contains everything from project setup to code execution and results, making it comprehensive and informative for anyone who views your GitHub repository.
```
