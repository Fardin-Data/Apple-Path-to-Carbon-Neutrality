# Apple's Path to Carbon Neutrality
![Green Modern Real Estate Agent Linkedin Banner](https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/62bb1b3d-9881-4091-b50e-8d9acbf911df)

## Project Overview
In this project, the exploration focuses on Apple's noteworthy commitment to achieving carbon neutrality by 2030. The project assumes the role of an independent journalist and data visualization enthusiast, involving the analysis of data from Apple's Environmental Progress Reports. The outcome is a data-driven progress report that investigates significant factors impacting CO2 emissions and their development from 2015 to 2023.

## Problem Statement
In 2020, after announcing their corporate operations were officially carbon neutral, Apple pledged to make their products carbon neutral by 2030. To achieve this goal, they set their emissions for 2015 (38.4 million metric tons CO2e) as the baseline and will aim to reduce them by 75% by 2030. The remaining 25% of gross emissions (9.6 million metric tons CO2e) will be removed using carbon offsets, bringing the net emissions to 0.

## Process
`Data Understanding`

Upon importing the data, a thorough exploration was conducted to comprehensively understand the dataset.

`Data Cleaning`

Identification and resolution of null and inappropriate values within the dataset was successfully carried out to ensure appropriate analysis.

`Data Analysis`

The cleaned data underwent analysis using matrix visualizations in Power BI, providing insights into emission progression.

`Measures Creation with Power BI`

To enhance the analysis, custom measures were created using Power BI, allowing for more sophisticated calculations and insights.

<pre><code>
    (
      CALCULATE(
          SUM(greenhouse_gas_emissions[Emissions]),
          FILTER(greenhouse_gas_emissions, greenhouse_gas_emissions[Fiscal Year] = 2015)
      )
      - 
      CALCULATE(
          SUM(greenhouse_gas_emissions[Emissions]),
          FILTER(greenhouse_gas_emissions, greenhouse_gas_emissions[Fiscal Year] = 2022)
      )
  )
  /
  CALCULATE(
      SUM(greenhouse_gas_emissions[Emissions]),
      FILTER(greenhouse_gas_emissions, greenhouse_gas_emissions[Fiscal Year] = 2015)
  )

</code></pre>

`Data Visualization`

Following effective data analysis, a comprehensive report was constructed, considering significant KPIs.

`Insights Gathering`

A thorough analysis revealed numerous crucial insights, which were effectively conveyed.

`Recommendations`

Derived from various insights, a set of recommendations was formulated to achieve the 2030 goal effectively.


## Report Preview
<div align="center">
  <img src="https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/e3453dba-7119-4ad7-b627-17c273e41e85" />
</div>

## Insights

- **Remarkable Emission Reduction Progress:** In just seven years, Apple has achieved an impressive 47.2% reduction in emissions, nearing the 50% mark. With eight more years to reach our 2030 goal, our current 2022 emissions stand at 20.3 million metric tons, aiming to reach 9.6 million metric tons. The pace of emission reduction has been substantial, making it increasingly likely that we will meet our 2030 target. However, we strive to accelerate our efforts for a more assured achievement.


<table>
  <tr>
    <td valign="middle">
      <img src="https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/ac335691-4ad8-4eb7-ab62-319858933b8c" alt="image" width="3000" height="200" />
    </td>
    <td valign="top">
      <strong>Steady Emission Decline Post-2019:</strong><br /><br />
      Since 2019, our carbon footprint from product manufacturing has been on a consistent downward trajectory, with our latest phone boasting the lowest carbon footprint. Overall, our emissions have shown a gradual decline since 2015. Our dedication to carbon removal efforts from 2020 to 2022 has contributed to this reduction.
    </td>
  </tr>
</table>


<table>
  <tr>
    <td valign="top">
      <strong>Product Life Cycle vs. Corporate Emissions:</strong><br /><br />
      Product life cycle emissions significantly outweigh corporate emissions. Nevertheless, both have witnessed exponential reductions. Notably, corporate operations have already achieved carbon neutrality, marking a significant milestone on our sustainability journey.
    </td>
    <td valign="middle">
      <img src= "https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/2d99bb9d-43a0-4fb9-9df2-89125e3da783" alt="image" width="3000" height="200" />
    </td>
  </tr>
</table>


<table>
  <tr>
    <td valign="middle">
      <img src="https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/3688e436-e746-428d-8acf-e36ca286838d" alt="image" width="3000" height="200" />
    </td>
    <td valign="top">
      <strong>Key Emission Contributors:</strong><br /><br />
      The three primary sources of emissions are Manufacturing (including Purchased Goods and Services), Product Use (including the use of sold products), and Product Transportation (both upstream and downstream). Identifying and addressing these sources have been pivotal in our emission reduction efforts.
    </td>
  </tr>
</table>


<table>
  <tr>
    <td valign="top">
      <strong>Positive Correlation with Business Success:</strong><br /><br />
      Counterintuitively, our exponential reduction in carbon emissions has positively impacted our business. Our revenue and market capitalization have been consistently increasing since 2015, reaching their zenith in 2022. This demonstrates that our commitment to sustainability aligns with our financial growth.
    </td>
    <td valign="middle">
      <img src="https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/92fd777e-0f22-493a-b224-2efcd561fbbf" alt="image" width="3000" height="200" />
    </td>
  </tr>
</table>


<table>
  <tr>
    <td valign="middle">
      <img src= "https://github.com/Fardin-Data/Apple-Path-to-Carbon-Neutrality/assets/137788371/9f52981f-c140-4b72-a95b-902b3439b84c" alt="image" width="3000" height="200" />
    </td>
    <td valign="top">
      <strong>Effective Scope 3 Emission Management:</strong><br /><br />
      Among the various sources of emissions, Scope 3 emissions, comprising purchased goods and services, transportation and distribution, business travel, employee commute, product use, and end-of-life factors, have consistently decreased since 2015. Notably, Scope 3 emissions represent the highest contributor to our overall emissions. Our dedicated efforts in reducing these emissions have yielded substantial results, marking a reduction from approximately 40 million metric tons CO2e to 20 million metric tons CO2e in 2022.
    </td>
  </tr>
</table>

## Recommendations:
- **Accelerate Emission Reduction Efforts:** Consider strategies to further accelerate the reduction of emissions. This will help ensure that the 2030 target is met well ahead of schedule, providing a buffer for any unexpected challenges.

- **Sustain Focus on Scope 3 Emissions:** Given that Scope 3 emissions are the highest contributor to overall emissions, continue dedicated efforts in managing and reducing these emissions. Implement supply chain and transportation efficiency measures to further cut down on these emissions.

- **Innovate for Product Carbon Neutrality:** Emphasize the development of products with lower carbon footprints. Continue the trend of lowering the carbon footprint of products throughout their life cycles. Invest in research and innovation to create more eco-friendly designs, materials, and manufacturing processes.

- **Promote Sustainable Product Use:** Educate and incentivize customers to use products in an environmentally responsible manner. This may involve optimizing device settings, prolonging product lifecycles, and recycling old products.

- **Collaborate with Suppliers:** Collaborate closely with suppliers to reduce emissions associated with manufacturing. Encourage and support suppliers in adopting greener practices and sourcing more sustainable materials.

- **Enhance Carbon Offset Strategies:** Continuously evaluate and improve carbon offset initiatives. Explore innovative approaches to carbon offsetting, such as investing in reforestation and renewable energy projects, to make the remaining 25% of emissions removal more efficient and impactful.


## Challenges Faced

During the course of this project, several challenges were encountered:

- **Understanding the Data:** The dataset used in this analysis presented complexities in understanding the data structure and identifying key performance indicators (KPIs). Initially, it was challenging to determine which data points were most relevant for the analysis. However, through thorough exploration and spending time with the data, I was able to gain a deeper understanding and identify important KPIs. This experience significantly improved my analytical abilities and problem-solving skills.

- **Dealing with Null Values:** Null values in the dataset posed a challenge, especially given the relatively small dataset size. Imputing null values proved to be complex, as finding meaningful patterns for replacement was not straightforward. Ultimately, the decision was made to drop null values, as replacing them with arbitrary values would not have been appropriate. This challenge provided insights into the importance of data quality and integrity in the analysis process.

## Learnings

Through the course of this project, I gained valuable knowledge and experience in several key areas:

- **Data Analysis and Visualization:** This project allowed me to enhance my data analysis and visualization skills. I learned how to effectively explore and analyze data, create meaningful visualizations, and communicate insights through data-driven reports.

- **Problem-Solving:** Dealing with complex datasets and challenges in data understanding and quality improved my problem-solving abilities. It taught me to approach problems methodically and explore different solutions.

- **Domain Knowledge:** The project provided me with a deeper understanding of environmental sustainability, carbon emissions, and Apple's commitment to carbon neutrality. This domain knowledge will be invaluable in future projects related to sustainability and corporate responsibility.

- **Data Integrity:** The experience of handling null values reinforced the importance of data integrity and the need for data cleaning and validation processes in any data analysis project.

- **Recommendation Generation:** Formulating recommendations based on data analysis findings enhanced my ability to translate insights into actionable strategies for achieving sustainability goals.

This project was not only about data analysis but also a valuable learning journey that equipped me with new skills and insights to tackle similar challenges in the future.


## Folder/Files Information

- **Data Folder**

  The "Data" folder contains Excel workbooks that provide essential data for the analysis. Here are the files in this folder:

  - `data_dictionary.xlsx`: This workbook contains information about all the tables and the fields in them.
  - `carbon_footprint_by_product.xlsx`: Provides data on carbon footprints for various Apple products.
  - `greenhouse_gas_emissions.xlsx`: Contains data related to greenhouse gas emissions, categorized by year, category, scope, and type.
  - `normalizing_factors.xlsx`: Includes information on normalizing factors, such as revenue, market capitalization, and employee data.

- **Report Folder**

  Inside the "Report" folder, you will find a file named "Progress_Report.pbix." This Power BI file exclusively contains visuals and charts that provide a comprehensive visual summary of the project's findings and data analysis.

  The "Progress_Report.pbix" file is structured as follows:

  - `Report Sheet:` The report sheet is dedicated to visual representations of the project's key findings and data analysis. It includes charts, graphs, and visuals that offer a clear and concise overview of important metrics related to Apple's path to carbon neutrality. These visuals enable stakeholders to quickly grasp the project's insights and make informed decisions.

  - `Insights & Recommendations Sheet:` The second sheet in "Progress_Report.pbix" focuses on insights and recommendations, offering in-depth analysis conclusions and providing recommendations for achieving the 2030 carbon neutrality goal effectively.


## Data Dictionary

- **Greenhouse gas emissions Table**
  
  | Field          | Description                                                |
  | ---------------|------------------------------------------------------------|
  | Fiscal Year    | Apple's fiscal calendar starts on the last Sunday of September and is 364 days long |
  | Category       | Emissions are divided into two categories: corporate emissions and product life cycle emissions |
  | Type           | There are two types of emissions data included: gross emissions (which add to the carbon footprint) and carbon removals (which subtract from the carbon footprint) |
  | Scope          | There are three scopes: direct scope 1 emissions; indirect scope 2 emissions from purchased electricity, steam, heating, and cooling; and indirect scope 3 emissions from purchased goods and services, transportation and distribution, business travel, employee commute, product use, and end of life |
  | Description    | The source of the greenhouse gas emissions |
  | Emissions      | Greenhouse gas emissions (metric tons CO2e) |

- **Carbon footprint by product Table**

  | Field             | Description                                                |
  | ------------------|------------------------------------------------------------|
  | Release Year      | Year the product was released |
  | Product           | Product name |
  | Baseline Storage  | Lowest storage option |
  | Carbon Footprint  | Greenhouse gas emissions from the product life cycle (kg CO2e) |

- **Normalizing factors Table**

  | Field          | Description                                                |
  | ---------------|------------------------------------------------------------|
  | Fiscal Year    | Figures are as of the end of the fiscal year |
  | Revenue        | Net sales (in millions, US$) |
  | Market Capitalization | Value of the company (in billions, US$) |
  | Employees      | Number of full-time equivalent employees |

## Tools Used:

- `Power Query` Employed for data extraction, transformation, and loading (ETL).

- `Power BI` Utilized for creating reports, including data visualization and presentation.

## License
This project is licensed under the MIT License, allowing you to use, modify, and distribute the code and visuals while maintaining the original license terms.

---

For questions or feedback, please contact: fardinkhan.data@gmail.com

Enjoy exploring the project!
