# HEART: Health Events & Activity Reporting Tool

<img width="832" height="562" alt="HEART" src="https://github.com/user-attachments/assets/12d05ff5-9406-4f03-93c4-2407ae40e392" />

HEART - a free-to-use tool parsing Apple Health and Fitness application data from Full File System (FFS) Extractions in a forensic manner!

# Version 1.0 Features:

- Easy to install and use application

- HTML report generation to review Classic Health Artifacts, User Attribution Artifacts, and other Health Artifacts (as supported through input data)

- 29 currently supported artifacts

- Glossary derived from database information

- Tables are easy to view and filter thanks to Tabulator

- CSV / PDF Report generation, based off artifact selection

- HTML Light and Dark Mode

# HEART, the Application:

Application use is as easy as browsing for your input FFS Extraction, browsing to your output location, and selecting "Process"! Processing time will vary based on database size. 

HEART output files include the HEART HTML Report and a folder containing Apple Health and Fitness Application databases. 

Once processing is complete, selecting "Close" will both exit the application and launch the HTML report. Data is processed to minimize the size of the HTML report as much as possible. Overall HTML report sizes are variable based on input database values and artifacts supported. Initial HTML report loading times will vary as well - based on size of the report.

# Classic Health Artifacts:

- Heart Rate
- Steps Taken
- Distance Traveled
- Calories Burned
- Flights Climbed

# User Attribution:

- Height 
- Weight

# Health Artifacts:

- Activity
- Resting Heart Rate
- Walking Heart Rate Average
- Heart Rate Notifications (Low / High)
- Six-Minute Walk
- Time in Daylight
- All Sleep Data
- Sleep Data by Sleep Period
- Watch Worn Data
- Sleeping Wrist Temp - Vitals
- Sleeping Wrist Temp - Weekly
- Respiratory Rate
- Respiratory Rate - Daily
- Respiratory Rate - Weekly
- Connected Device Information - Device History
- Consolidated Connected Device History
- Environmental Sound
- Noise Notifications
- Headphone Audio Levels
- Workouts
- Workouts Location Data
- Workouts Additional Metadata
- Glossary

# Acknowledgments:
- This software includes the CustomTkinter library, which is licensed under the MIT License. Copyright (c) 2023 Tom Schimansky. The full license text can be found [here](https://github.com/TomSchimansky/CustomTkinter)
- This software includes the Tabulator library, which is licensed under the MIT License. Copyright (c) 2015-2025 Oli Folkerd. The full license text can be found [here](https://github.com/olifolkerd/tabulator/blob/master/LICENSE)
- This software uses the [Pillow library](https://pypi.org/project/pillow/) (PIL fork), licensed under the Historical Permission Notice and Disclaimer (HPND). 

# Gratitude and Thanks:
We would like to extend our gratitude, and provide reference to, others within our great DFIR Community who have furthered the support of Apple Health and Fitness artifacts, scripts, and more:

- Sarah Edwards and [APOLLO](https://github.com/mac4n6/APOLLO)

- Ian Whiffin and Health Data Types available at [DoubleBlak](https://www.doubleblak.com/blogPost.php?k=Health)

- Alexis Brignoni and all who assisted in Health Data within [iLEAPP](https://github.com/abrignoni/iLEAPP)
