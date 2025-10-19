Facebook Ads Performance Analytics Power BI Project
Welcome to my latest Power BI analytics project and GitHub contribution! This dashboard provides a deep, data-driven look into Facebook Ads performance using real-world campaign data. My goal was to create a tool that not only displays metrics but also uncovers cost efficiency, demographic impact, and conversion trends, all powered by custom DAX measures and a strong focus on data storytelling.

Table of Contents
Introduction

Project Description

Installation

Usage

Custom DAX Measures

Screenshots

License

Introduction
Project Title: Facebook Ads Performance Analysis Created By: Rakesh Aamalepatil Tools Used: Power BI, DAX, Excel Focus Areas: Digital marketing metrics, audience segmentation, cost optimization

Project Description
This Power BI dashboard offers a comprehensive analysis of Facebook ad campaigns across key performance indicators: CPA (Cost Per Acquisition), CPC (Cost Per Click), CPM (Cost Per Mille), CTR (Click-Through Rate), and conversion rates. It is designed to be an essential tool for marketers and analysts to:

Identify top-performing ads.

Optimize spending by analyzing age and gender demographics.

Decode overall campaign effectiveness.

Key Features
Top 5 Ad Rankings by CPA, CPC, CPM, and conversion cost

Demographic Breakdown by age and gender

Trend Analysis across the August campaign dates

Custom DAX Measures for segmentation, cost efficiency, and performance scoring

Interactive Filters for campaign ID, gender, and time slices

Installation
To explore or modify this Power BI project, follow these steps:

Clone the repository:

Bash

git clone https://github.com/Sachin-Analyst/FUTURE_DS_02.git
Install Power BI Desktop: Download and install Power BI Desktop.

Open the Facebook Ads Performance Dashboard:

Navigate to the Dashboards folder and open the .pbix file.

Review the charts and measures to understand the analysis.

To create a dashboard from scratch (optional):

Navigate to the Raw Data folder in the FUTURE_DS_02 repo and download the .xlsx file.

Review the data in Excel and save it to your local computer.

Open Power BI Desktop > Blank Report > Get data > Excel > Connect > Then choose the file on your local machine.

Usage
What You Can Explore
The dashboard provides multiple avenues for insight generation, including:

Conversion trends by gender across August

Age-wise conversion rates and ad spending

Cost-per-click and cost-per-acquisition efficiency

Campaign-level performance insights

Slicer-based filtering for custom views

Screenshots
Screenshot: Main Dashboard Overview

Screenshot: Top Performing

These are the DAX formulas created and applied.

1.CPA = DIVIDE(SUM(data[spent]), SUM(data[total_conversion]))

 [ CPA stands for Cost Per Acquisition, We find CPA to measure the efficiency of a marketing campaign ]

2.CPAC = DIVIDE(SUM(data[spent]), SUM(data[approved_conversion]))

[ CPAC, which stands for Cost Per Approved Conversion, is a crucial metric for evaluating the efficiency and profitability of advertising campaigns. ]

3.CPC = DIVIDE(SUM(data[spent]),SUM(data[clicks]))

[ CPC stands for Cost Per Click You calculate CPC to determine the cost-effectiveness of your advertising, as it shows how much you pay for each click on your ad. ]

4.CPM = DIVIDE(SUM(data[spent]), SUM(data[impressions])) *1000

[ CPM, or Cost Per Mille, is a fundamental metric used in advertising to measure the cost of one thousand ad impressions. 
Businesses use it to gauge the cost-effectiveness of an ad campaign and to compare the costs of different advertising channels. ]

5.CR = DIVIDE(SUM(data[total_conversion]),SUM(data[clicks]))

[ CR stands for Conversion Rate .
It tells you what percentage of people who clicked on your ad or visited your site completed a desired action, like making a purchase or signing up for a newsletter. ]

6.CTR = DIVIDE(SUM(data[clicks]), SUM(data[impressions]))

[ CTR stands for Click through rate ,You calculate CTR to measure the effectiveness of an ad or content. 
It helps you understand how often people who see an ad or content actually click on it, which is an indicator of its appeal and relevance]

Explore the DAX Measures folder for detailed breakdowns and the business logic behind each formula.

License
This project is licensed under the MIT License. See the LICENSE file for details.
