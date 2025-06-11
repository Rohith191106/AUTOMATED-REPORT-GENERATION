# AUTOMATED-REPORT-GENERATION

COMPANY NAME   :CODETECH IT

NAME:ROHITH.B

INTERN ID:CT04DG566

DURATION:08-06-2025 TO 08-07-2025

MENTOR:NEELA SANTHOSH KUMAR

**CODE:**
import pandas as pd
import matplotlib.pyplot as plt

# Sample dataset
data = {
    'Day': ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
    'Sales': [200, 150, 300, 280, 500, 700, 650]
}

# Create DataFrame
df = pd.DataFrame(data)

# Optional: use a valid style (or skip for default)
plt.style.use('ggplot')  # You can also use 'bmh', 'classic', etc.

# Create the plot
plt.figure(figsize=(10, 6))
plt.plot(df['Day'], df['Sales'], marker='o', linestyle='-', color='blue')
plt.title('Weekly Sales Report', fontsize=16)
plt.xlabel('Day of the Week')
plt.ylabel('Sales')
plt.grid(True)

# Save the chart
plt.savefig("sales_report.pdf")  # Saves in your current working directory
plt.show()

📄**Description of the Code**:

Automated Sales Report Generation using Pandas and Matplotlib

This Python script demonstrates automated data visualization by generating a line chart from sales data and saving it as a PDF report. It uses two key libraries: pandas for data handling and matplotlib for plotting.


---

🔍 Line-by-Line Explanation

1. Import necessary libraries

import pandas as pd
import matplotlib.pyplot as plt

pandas: used for managing and analyzing tabular data.

matplotlib.pyplot: used for creating plots and charts.



---

2. Create a sample dataset

data = {
    'Day': ['Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat', 'Sun'],
    'Sales': [200, 150, 300, 280, 500, 700, 650]
}

A dictionary with days of the week and corresponding sales values is defined.



---

3. Convert the data into a DataFrame

df = pd.DataFrame(data)

This converts the dictionary into a pandas DataFrame for easy data handling and plotting.



---

4. Set the plotting style

plt.style.use('ggplot')

Sets a predefined plotting style for better visual appearance. 'ggplot' gives a grid and soft color palette.



---

5. Create the plot

plt.figure(figsize=(10, 6))
plt.plot(df['Day'], df['Sales'], marker='o', linestyle='-', color='blue')

Initializes a figure of size 10x6 inches.

Plots sales data with blue lines and circular markers.



---

6. Add chart titles and labels

plt.title('Weekly Sales Report', fontsize=16)
plt.xlabel('Day of the Week')
plt.ylabel('Sales')
plt.grid(True)

Adds a title and labels for X and Y axes.

Enables the grid for easier data reading.



---

7. Save and display the chart

plt.savefig("sales_report.pdf")
plt.show()

Saves the plot as a PDF named sales_report.pdf.

Displays the chart in a window.



---

✅ Purpose of the Code

This is a basic automated report generation script.

It visualizes weekly sales performance and outputs it as a PDF chart.

Useful for sales monitoring, performance dashboards, and business reports.

**OUTPUT:**

![Image](https://github.com/user-attachments/assets/0253e473-d4f3-4c37-a274-84185846b468)
