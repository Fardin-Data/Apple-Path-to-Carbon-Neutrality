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




