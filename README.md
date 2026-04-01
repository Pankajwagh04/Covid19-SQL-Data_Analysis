# Covid-19 Pandemic: A Comprehensive Data Analysis with SQL & Tableau

![Covid19-](https://github.com/mikeolaniyi/Covid19_Vaccination_Analysis_in_SQL/assets/120651356/ab54c8f4-7465-49b9-8502-c9f758497889)

---

## **Brief Introduction**

The COVID-19 pandemic had a massive global impact, affecting millions of lives. This project aims to analyze the pandemic and extract meaningful insights about its impact across the world.

---

## **The Dataset**

The analysis is based on the World Health Organization (WHO) dataset, focusing on:
- Total cases  
- Death counts  
- Infection rates  
- Vaccination rollouts  
- Impact across continents  

---

## **Key Questions Answered**

- What is the percentage of population vaccinated?  
- What is the number of deaths by continent?  
- Which continents have the highest death count per population?  
- Which countries have the highest infection rate compared to population?  
- What is the total cases & population percentage infected?  
- What is the total cases vs total deaths in Nigeria?  

---

## **Datasets Description**

- **CovidDeaths Table**
  - 26 columns  
  - 81,060 rows  

![image](https://github.com/user-attachments/assets/9a3595c1-af27-4e64-a31c-1ec771ec2521)

---

- **CovidVaccinations Table**
  - 37 columns  
  - 85,171 rows  

![image](https://github.com/user-attachments/assets/f7455feb-625d-4f0b-8a18-3b609017164d)

---

## **Sample SQL Analysis**

```sql
SELECT location, date, total_cases, new_cases, total_deaths, population
FROM CovidDeaths
WHERE continent IS NOT NULL AND total_deaths IS NOT NULL
ORDER BY 1,2;
