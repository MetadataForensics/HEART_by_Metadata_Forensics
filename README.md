# HEART: Health Events & Activity Reporting Tool

<img width="832" height="542" alt="V 1 3 0 0" src="https://github.com/user-attachments/assets/9d9324a2-e047-416d-9122-aef92144ac4e" />

HEART by Metadata Forensics - a free-to-use tool parsing Apple Health and Fitness application data in a forensic manner!

# Newest Features:

- Added Local Device Time conversions! Because most Apple Health and Fitness application artifacts are attributed to the specific device that measured and recorded the event, the associated time zone is preserved as well. This enables a unique Local Device Time conversion based on the device’s time zone at the time of the event, rather than applying a single overall time zone conversion. <br>
  _Note: If the data source is a binary object, device attribution is not preserved; therefore, no associated time zone can be determined._

- Increased support! Now supporting Full File System Extractions, TAR files, some DAR files, Advanced Logical (Encypted) Extractions, and iTunes Encypted Backups!

- All about the Speed! Version 1.1.0.0 added support for Walking Speed, Running Speed, Stair Speed Up, and Stair Speed Down (Version 1.1.0.1, 1.1.0.2, and 1.2.0.0 minor updates)

# HEART by Metadata Forensics Features:

- Easy to install and use application

- HTML report generation to review Classic Health Artifacts, User Attribution Artifacts, and other Health Artifacts (as supported through input data)

- 37 currently supported artifacts

- Glossary derived from database information

- Tables are easy to view and filter thanks to Tabulator

- CSV / PDF Report generation, based off artifact selection

- HTML Light and Dark Mode

# HEART by Metadata Forensics, the Application:

Application use is as easy as browsing for your input file, browsing to your output location, and selecting "Process"! Processing time will vary based on database size. 

HEART by Metadata Forensics output files include the HEART HTML Report and a folder containing Apple Health and Fitness Application databases. 

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
- Cardio Fitness
- Walking Speed
- Running Speed
- Stair Speed Up
- Stair Speed Down
- Blood Oxygen*
- Resting Heart Rate
- Walking Heart Rate Average
- Heart Rate Notifications (Low / High)
- Six-Minute Walk
- Time in Daylight
- All Sleep Data
- Sleep Data by Sleep Period
- Watch Worn Data
- Wrist Temperature
- Sleeping Wrist Temp - Vitals
- Sleeping Wrist Temp - Weekly
- Respiratory Rate
- Respiratory Rate - Daily
- Respiratory Rate - Weekly
- Connected Device Information - Device History
- Consolidated Connected Device History
- Device Information - Current Device (New)
- Environmental Sound
- Noise Notifications
- Headphone Audio Levels
- Workouts
- Workouts Location Data
- Workouts Additional Metadata
- Glossary

_* A redesigned Blood Oxygen feature was introduced on August 14, 2025, for Apple Watch Series 9, Series 10, and Apple Watch Ultra 2. OS requirements are Apple iPhone iOS 18.6.1 or higher and Apple Watch watchOS 11.6.1 or higher. iOS 26 and watchOS 26 continue to support this feature._

# Leveraging Tabulator:



https://github.com/user-attachments/assets/67a616a2-1e66-45ed-8153-3508469db8ed



Reviewing out data with Tabulator, we can search and filter in real time with our records count adjusting on the fly. Searching within multiple columns filters the data even further. 

Wish the columns were in a different order? Change them! The changes reflect in exported reports as well.

# Usage

You may also be required to take additional steps when running the tool the first time, through Microsoft Defender SmartScreen. In the Microsoft Defender SmartScreen select "More info" and "Run anyway" to launch the application the first time. 


# Acknowledgments:
- This software uses the CustomTkinter library, which is licensed under the MIT License. Copyright (c) 2023 Tom Schimansky. The full license text can be found [here](https://github.com/TomSchimansky/CustomTkinter)
- This software uses the Tabulator library, which is licensed under the MIT License. Copyright (c) 2015-2025 Oli Folkerd. The full license text can be found [here](https://github.com/olifolkerd/tabulator/blob/master/LICENSE)
- This software uses the [Pillow library](https://pypi.org/project/pillow/) (PIL fork), licensed under the Historical Permission Notice and Disclaimer (HPND).
- This software uses the [iphone_backup_decrypt](https://pypi.org/project/iphone-backup-decrypt/) library, licensed under the MIT License. 

# Gratitude and Thanks:
We would like to extend our gratitude, and provide reference to, others within our great DFIR Community who have furthered the support of Apple Health and Fitness artifacts, scripts, and more:

- Sarah Edwards and [APOLLO](https://github.com/mac4n6/APOLLO)

- Ian Whiffin and Health Data Types available at [DoubleBlak](https://www.doubleblak.com/blogPost.php?k=Health)

- Alexis Brignoni and all who assisted in Health Data within [iLEAPP](https://github.com/abrignoni/iLEAPP)
