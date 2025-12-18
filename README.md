**PROJECT OVERVIEW**

This project analyzes visitor flows across Hong Kong using Power BI.
The dashboard highlights key metrics such as arrivals vs departures, visitor type breakdowns, control point comparisons, and geographic patterns to support insights into tourism trends and mobility management.


**DATASET**

Source: data.gov.hk 

Dataset: Visitor records by date, control point, and visitor type

Fields Used: Date/ Control Point/ Location / Arrival / Departure/ Hong Kong Residents/ Mainland Visitors/ Other Visitors

**PROCESS**

Data Import

- Imported raw dataset into Power BI.
- Renamed columns for clarity (HKResidents, MainlandVisitors, OtherVisitors).

  
Data Cleaning

- Trimmed and standardized text fields (Control Point, Location, District).
- Ensured consistent date formatting.


Data Modeling
- Built schema with relationships between Date, Control Point, and Visitor Type.
- Created calculated columns and measures for arrivals and departures.

DAX Measures

Total Visitor = 'dataset'[Hong Kong Residents] + 'dataset'[Mainland Visitors] + 'dataset'[Other Visitors]

Arrival Total = CALCULATE( SUM('dataset'[Total Visitor]), 'dataset'[Arrival / Departure] = "Arrival")


Visualization

Section 1
- Cards: Year 2024 Arrival Total / Departure Total
- Donut Chart: Visitor type share
- Bar Chart: Total visitors by month
- Waterfall Chart: Visitors by arrival/departure and month
- Line Chart: HK residents by year and arrival/departure

Section 2
- Bar Chart: Visitors by control point
- Table: Control point, district, total visitor
- Map: Bubble map of visitors by location

Section 3
- Line Chart: Visitor trend by year and arrival/departure
- Tree Map: Visitors by district and arrival/departure

  
**SKILLS DEMONSTRATED**
- Data cleaning and transformation
- Data modeling with relationships
- DAX measures for KPIs
- Geographic mapping
- Interactive dashboard design
- Storytelling with data


i. Dashboard for Overview
<img width="1311" height="728" alt="image" src="https://github.com/user-attachments/assets/400f4d9b-5a01-4a76-9cfe-e392000e7d9a" />

ii. Dashboard for Control Point
<img width="1445" height="803" alt="image" src="https://github.com/user-attachments/assets/64ec2507-20f1-49d2-9379-a3342582a2f7" />

iii.Dashboard for Visitor Type
<img width="1446" height="810" alt="image" src="https://github.com/user-attachments/assets/b5e5437d-b3dd-474b-8f47-835ecad36dc8" />

iv. Create relationship
<img width="1303" height="841" alt="image" src="https://github.com/user-attachments/assets/ef86bb1f-5b6f-48d0-adc9-a5d4d2516a15" />
