# ClearSkies: From NASA Data to a 4-Hour Forecast
       
## Our Submission for the NASA TEMPO Air Quality Monitoring Challenge
The Idea (And Why It Works)
We noticed a gap: The air quality reports people see are either too late or too general. Our goal was to build a system, ClearSkies, that proves you can use huge satellite data (NASA TEMPO) and blend it with local ground readings to create a fast, super-local forecast.
It's about getting ahead of the pollution plume to keep vulnerable people safe.
The Live App (Our Deliverable)
This is the functional prototype we built in the short hackathon window. It shows our data fusion and features in action.
https://docs.google.com/spreadsheets/d/1ARKIuq1dIcJgQTbjOMQeKqUPB_NmbB83uMQwRHBRErQ/edit?usp=sharing
[>> CLICK HERE TO SEE THE LIVE CLEARSKIES DASHBOARD <<]
([INSERT YOUR LOOKER STUDIO PUBLIC LINK HERE])
How We Hacked the Data Together
The biggest challenge was pulling data from three complex places and making them talk. We found a way to combine them into one smart forecast:
 * NASA TEMPO Satellite Data (NO2):
   * Source: Satellite NO2
   * Why We Needed It: The Big Picture. We used this to track the movement of pollution across North America—crucial for any prediction! (See TEMPO_Extraction_Notes.txt for how we got the numbers.)
 * Ground Station Measurements:
   * Source: PM(2.5)
   * Why We Needed It: The Real Impact. This is the most dangerous stuff. It gives us the specific health threat at street level.
 * Local Weather Data:
   * Source: Wind Speed
   * Why We Needed It: The Prediction. Wind is the key. We used it to simulate where the pollution will travel over the next few hours.
The Core Logic
We put those three inputs into a simple weighted formula (our prediction model) to prove that the blend works. It shows how the TEMPO satellite data directly improves the accuracy of the final {AQI} forecast.
Our Favorite Features
 * Stop Guessing: Instead of just showing a number, we deliver an Actionable Health Notification (like "High Risk: Stay Indoors"). This turns complex data into immediate, clear advice.
 * Hyper-Local Forecast: The map displays a clear, color-coded grid to show exactly how bad the air quality will be in the next few hours.
 * Built to Scale: Even though this is a no-code prototype, we set it up using simple, separate data and visualization tools. This structure proves the concept is ready to be immediately scaled up using Python and deployed on a real cloud service.
Repository Contents
 * PITCH_DECK.pdf: Our full presentation slides.
 * TEMPO_Extraction_Notes.txt: Our honest account of how we successfully integrated the NASA TEMPO data without getting stuck on complex coding.
