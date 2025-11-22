🌍 Global Mortality Dashboard — Power BI Project

This project explores global mortality patterns using an interactive Power BI dashboard. The goal is to understand how many people die, what they die from, where deaths are highest, and how these patterns have changed over time.

The dashboard provides a comprehensive overview of global health challenges and supports data-driven decision-making for researchers, policymakers, and public health analysts

📌 Project Overview

The dataset contains:

Causes of Death

Country

Country Code

Number of Deaths

Year

With these fields, the dashboard answers key public health questions such as:

Which cause of death kills the most people globally?

Which countries experience the highest mortality?

How do deaths change across different years?
What diseases affect specific countries the most?


📊 Key Insights from the Dashboard
🔢 1. Total Global Deaths

Millions of deaths were recorded across the entire period, reflecting the significant global mortality burden.

💔 2. Leading Cause of Death

Cardiovascular diseases emerge as the highest cause of death worldwide, far exceeding other causes.

📈 3. Death Trends Over Time

The trend analysis shows a steady rise in deaths over many years, which may be linked to population growth, aging, and lifestyle factors.

🌏 4. Country with the Highest Death Count
Countries with larger populations (e.g., China, India) contribute the highest total death numbers.

🗺️ 5. Causes of Death by Country

Different countries struggle with different major causes — some face infectious diseases, while others face non-communicable diseases.

🧠 DAX Measures Used
Total Deaths = SUM('Global Mortality'[Number of deaths])

Top Cause Deaths = 
CALCULATE(
    [Total Deaths],
    TOPN(1, 'Global Mortality', [Total Deaths], DESC)
)

Total Deaths by Year = 
CALCULATE(
    [Total Deaths],
    ALLEXCEPT('Global Mortality', 'Global Mortality'[Year])
)



🛠️ Tools & Technologies

Power BI

Power Query

DAX (Data Analysis Expressions)

Excel

Data Modeling (Star Schema)

🗂️ Dashboard Features

KPI Cards:
✔ Total Deaths
✔ Top Cause of Death
✔ Top Country by Deaths

Visuals:
📈 Death Trends Over Time
📊 Top Causes of Death
🥧 Deaths by Country
🧱 Causes of Death by Country (Stacked Bar)

Slicers:
🔽 Select Year
🔽 Select Country
🔽 Select Cause of Death

🎯 Purpose of the Project

This project was designed to:

Analyze mortality trends globally

Identify top disease burdens across regions

Support health research and policy formation

Showcase Power BI skills for data storytelling

🙋‍♀️ About the Author

Omolola Olorunnishola
Biochemistry × Data Science × Artificial Intelligence x Data Analysis

Passionate about using data insights to solve real-world health problems.
