# Linking Freight Flows & Regional Economics

### Table of Contents
	•Tableau Dashboard
	•Motivation
	•Questions
	•Normalizing the Data
	•Problems and Hurdles
	•Technologies Used
	•Data Sources
	•Conclusion

## Tableau Dashboard

Link: []

## Motivation

The movement of freight across the U.S. is tightly connected to regional economic performance. 
By linking the Freight Analysis Framework (FAF5), Commodity Flow Survey (CFS), and BEA Regional Economic Accounts, this project aims to show how commodities flow between regions, what modes of transportation dominate, and how these flows tie into GDP and employment. 
This combination helps policymakers, analysts, and businesses understand both logistics and economic impact.

### Questions
	1.Which commodities and modes dominate freight value and tonnage by state or metro?
	2.How do origin–destination freight corridors align with state GDP and employment trends?
	3.Do states with higher freight intensity (value of freight relative to GDP) show unique commodity or mode profiles?
	4.Are there trends where certain transportation types and commodity freight paths have more GDP growth?

## Normalizing the Data

FAF and CFS share SCTG commodity codes and mode categories, allowing them to be cross-validated. BEA adds GDP, employment, and income at the state level. 
Data cleaning involved aligning commodity codes, standardizing geography using FIPS, and normalizing units (tons, value, ton-miles). 
Interim datasets were created in CSV format for consistency across Python and Power BI.

### Problems and Hurdles
	•Aligning FAF regions with state-level BEA data required building a crosswalk.
	•Large file sizes in FAF OD tables made processing and joins slow.
	•Commodity reclassification and missing values in CFS required careful handling.

### Technologies Used
	1.Python / Pandas / Camelot / seaborn / matplotlib
	2.Tableau – for dashboards and storytelling.

## Data Sources
	•Freight Analysis Framework (FAF5) – OD flows by commodity, mode, tons, value. 
	•Commodity Flow Survey (CFS 2022) – validates flows, adds shipment-level details.
	•BEA Regional Economic Accounts – GDP, employment, and income by state and metro.

## Conclusion

This project demonstrates how freight flows are not just about tons and value—they’re directly tied to economic structure and growth. 
States with higher manufacturing activity show stronger flows in machinery, electronics, and chemicals, while corridor analysis highlights links between freight growth and GDP gains in export-oriented sectors. 
The integration of FAF, CFS, and BEA provides a richer, policy-relevant perspective on U.S. logistics and regional economies.
