# HEART: Health Events & Activity Reporting Tool

<img width="985" height="837" alt="V 2 0_1" src="https://github.com/user-attachments/assets/1255c74e-1d0b-4c90-9770-efa13e69b8a4" />

HEART by Metadata Forensics - a free-to-use tool parsing Apple Health and Fitness application data in a forensic manner!

# Newest Features:

- **Version 2.0** adds support for **Artifact Selection** and **Timestamp Display**.
    - **Artifact Selection**: Choose which artifacts to process. Analyze a single artifact, a selected subset, or all currently supported artifacts.
    - **Timestamp Display**: Display timestamps in **UTC (default)** or convert them to the **device's local time**. This reduces the number of timestamp columns by half, resulting in smaller, more readable HTML reports.

- Version 1.4.2.0 adds Environmental Sound - Detailed, Headphone Audio Levels - Detailed, and Nutrition artifacts, along with updates to the Glossary as well.

Previously, Environmental Sound and Headphone Audio Levels were typically aggregated into 30-minute intervals. In additional to those present artifacts, the new detailed artifacts provide much finer temporal resolution - parsing data at a much more granular level and isolated dB spikes down to individual one-second intervals in some cases.

- Version 1.4.1.0 adds Health Details, Cardio Recovery, Heart Rate Variability, Mindful Minutes, State of Mind, and Breathing Disturbances artifacts, along with updates to the Glossary as well.

- Version 1.4.0.0 adds cache_encryptedC.db support for Steps, Walking + Running Distance, and Floors Ascended / Floors Descended. NikeFuel support added. _Minor updates to additional artifacts also added._

- Version 1.3.1.0 adds quality-of-life updates.

- All about the Speed! Version 1.1.0.0 added support for Walking Speed, Running Speed, Stair Speed Up, and Stair Speed Down (Version 1.1.0.1, 1.1.0.2, 1.2.0.0, and 1.3.0.1 minor updates)

- Added Device Local Time conversions! Because most Apple Health and Fitness application artifacts are attributed to the specific device that measured and recorded the event, the associated time zone is preserved as well. This enables a unique Device Local Time conversion based on the device’s time zone at the time of the event, rather than applying a single overall time zone conversion.

- Increased support! Now supporting Full File System Extractions, TAR files, some DAR files, Advanced Logical (Encypted) Extractions, and iTunes Encypted Backups!

# HEART by Metadata Forensics Features:

- Easy to install and use application

- HTML report generation to review Classic Health Artifacts, User Attribution Artifacts, and other Health Artifacts (as supported through input data)

- 48 currently supported artifacts

- Glossary derived from database information

- Tables are easy to view and filter thanks to Tabulator

- CSV / PDF Report generation, based off artifact selection

- HTML Light and Dark Mode

# HEART by Metadata Forensics, the Application:

Application use is straightforward: browse for your input file, choose an output location, select the artifacts to process, verify the timestamp display, and click **Process**. Processing time will vary depending on the size of the database.

HEART by Metadata Forensics generates an HTML report along with a folder containing the processed Apple Health and Fitness application databases.

When processing is complete, you can immediately open the output folder, launch the HTML report, or click **Close & Exit** to exit the application.

Data is optimized during processing to keep the HTML report as compact as possible. Report size will vary based on the amount of data and supported artifacts contained in the input database. Initial report loading times will also vary with report size. Once the HEART icon appears in the report window, the report has finished loading and is ready for navigation.

# Classic Health Artifacts:

- Heart Rate
- Steps
- Walking + Running Distance
- Calories Burned
- Flights Climbed

# User Attribution:

- Health Details
- Height 
- Weight

# Health Artifacts:

- cache_encryptedC - Steps
- cache_encryptedC - Distance
- cache_encryptedC - Floors Asc Desc
- Activity
- NikeFuel
- Cardio Fitness
- Cardio Recovery
- Heart Rate Variability
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
- Nutrition
- Mindful Minutes
- State of Mind
- Watch Worn Data
- Wrist Temperature
- Sleeping Wrist Temp - Vitals
- Sleeping Wrist Temp - Weekly
- Respiratory Rate
- Respiratory Rate - Daily
- Respiratory Rate - Weekly
- Breathing Disturbances
- Connected Device History
- Consolidated Connected Device History
- Device Information - Current Device
- Environmental Sound
- Environmental Sound - Detailed
- Noise Notifications
- Headphone Audio Levels
- Headphone Audio Levels - Detailed
- Workouts
- Workouts Location Data
- Workouts Additional Metadata
- Glossary

_* A redesigned Blood Oxygen feature was introduced on August 14, 2025, for Apple Watch Series 9, Series 10, and Apple Watch Ultra 2. OS requirements are Apple iPhone iOS 18.6.1 or higher and Apple Watch watchOS 11.6.1 or higher. iOS 26 and watchOS 26 continue to support this feature._

# Leveraging Tabulator:



https://github.com/user-attachments/assets/67a616a2-1e66-45ed-8153-3508469db8ed



Reviewing out data with Tabulator, we can search and filter in real time with our records count adjusting on the fly. Searching within multiple columns filters the data even further. 

Wish the columns were in a different order? Change them! The changes reflect in exported reports as well.

# cache_encryptedC.db Support: 

Steps, Walking + Running Distance, and Floors Ascended / Floors Descended  parsed through the cache_encryptedC.db, _/private/var/root/Library/Caches/locationd/_, provides a much more granular look at some of the same data from the healthdb_secure.sqlite. While the data retention period is much shorter, this data breakdown is much more temporally precise. Read more about this data and our research [here](http://metadataperspective.com/2026/05/19/empirical-assessment-of-apple-health-activity-data-accuracy-granularity-and-database-artifacts/).

<img width="898" height="423" alt="Floors Asc Desc" src="https://github.com/user-attachments/assets/f56ad108-027a-4e8d-9780-7ff94c6770ed" />

# Quality-of-Life Updates:

<img width="993" height="848" alt="V 2 0_2" src="https://github.com/user-attachments/assets/9f1d85b7-b8f4-4fff-84c0-3e55326ce8da" />

The _Processing Complete_ window provides options to open the output folder, view the report, or close and exit HEART by Metadata Forensics.

The selected output folder now includes an automatically generated, process-unique subfolder named:

`HEART_Output_YYYY_MM_DD_HH_MM_SS`

This subfolder contains the Database directory and the HEART.html report.

# Usage

The latest installer can be downloaded from the **Releases** section of this repository. When launching the tool for the first time, Microsoft Defender SmartScreen may display a warning. If prompted, select **More info**, then **Run anyway** to start the application.


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

A little help from our friends:

- Special thanks to Kevin Pagano ([@stark4n6](https://github.com/stark4n6)) for suggesting the improvements introduced in version 1.3.1.0. Grateful for the feedback that helps make the tool more user-friendly and continues to improve its functionality.
