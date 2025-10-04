# ClearSkies: From NASA Data to a 4-Hour Air Quality Forecast
### Our Submission for the NASA TEMPO Air Quality Monitoring Challenge

We developed ClearSkies, a functional prototype that addresses a critical need: fast, hyper-local air quality forecasts. Current reports are often too general or delayed. Our solution leverages satellite and ground data to predict air pollution movement up to four hours in advance, providing crucial, immediate warnings for public health.

## The ClearSkies Dashboard
The core of our submission is this live, interactive dashboard, which demonstrates our data fusion and predictive model in action.

[>> CLICK HERE TO SEE THE LIVE CLEARSKIES DASHBOARD (Looker Studio) <<]
https://lookerstudio.google.com/reporting/e57e0415-8126-4aa4-ad48-e934dc0178fb

Data Source (Google Sheet):
https://docs.google.com/spreadsheets/d/1ARKIuq1dIcJgQTbjOMQeKqUPB_NmbB83uMQwRHBRErQ/edit?usp=sharing

## Our Data Fusion Logic

The central challenge was synthesizing data from three complex, disparate sources into a single, reliable forecast. Our methodology successfully combines these inputs:
    -> NASA TEMPO Satellite Data (Nitrogen Dioxide - NO 2 ): Provides the macro-level "Big Picture"                       necessary to track the movement of pollution plumes across broad regions.
             
   ->Local Ground Station Readings (Particulate Matter - PM 2.5 ): Measures the real impact at street                   level, identifying the most immediate health threat.
              
   -> Local Weather Data (Wind Speed and Direction): Serves as the predictive variable, allowing us to                   simulate where pollution will travel over the next four hours.

Core Logic: We integrated these inputs using a weighted formula to create a robust Air Quality Index (AQI) prediction model, demonstrating how satellite data directly enhances the accuracy and timeliness of the final forecast.

## Key Features of ClearSkies

-> Actionable Health Notifications: We transform complex AQI numbers into immediate, clear advice (e.g., "High Risk: Stay Indoors"), enabling prompt public response.

-> Hyper-Local Forecast: The color-coded map provides a detailed grid visualization, pinpointing exactly where and when air quality is expected to deteriorate in the next few hours.

-> Scalable Architecture: Built as a no-code prototype, the system uses separate, modular tools, proving the concept is immediately ready for production-level scaling using cloud services and machine learning for enhanced accuracy.

## Repository Contents

-> PITCH_DECK.pdf: Our full presentation slides detailing the project's problem, solution, and future roadmap.

-> TEMPO_Extraction_Notes.txt: Documentation outlining our process for successfully integrating the raw NASA TEMPO data stream into our forecasting model.


