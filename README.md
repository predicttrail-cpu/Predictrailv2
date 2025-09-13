# Predictrail v2 - Trail Running Pace & Nutrition Planner

`Predictrail v2` is a web-based tool designed for trail runners to create detailed race plans. By uploading a GPX file of a race course and providing some personal performance metrics, users can get a sophisticated prediction of their race, including segment-by-segment pace, time, and a personalized nutrition strategy.

## Features

- **GPX File Analysis**: Upload your race's GPX file to see the course on an interactive map.
- **Interactive Course Map**: Powered by Leaflet, the map allows you to visualize the entire route.
- **Custom Segments**: Add aid stations or custom markers directly on the map to split the race into manageable segments.
- **Personalized Athlete Profile**: Input your weight, gender, and reference race performances to tailor the predictions to your fitness level.
- **Advanced Pace Model**: The tool uses a model that accounts for distance, elevation gain/loss, course technicality, and athlete fatigue to predict your pace for each segment.
- **Nutrition Planning**: Automatically calculates the required calorie and carbohydrate intake for each leg of the race based on your profile and the effort required.
- **Detailed Race Plan**: The output is a clear, table-based race plan showing:
  - Segment details (distance, elevation).
  - Predicted time and pace for each segment.
  - Cumulative time.
  - Estimated calorie and carbohydrate needs.
- **Responsive Design**: The interface is built with Tailwind CSS, making it accessible on both desktop and mobile devices.

## How to Use

1.  Open the `index.html` file in your web browser.
2.  **Enter Your Details**: Fill in your weight and select your gender.
3.  **Add Reference Performances**: Input at least one recent race or training run (e.g., a 10k time). This helps the model understand your current fitness level.
4.  **Load Your Course**: Upload the GPX file for the race you want to plan. The course will appear on the map.
5.  **(Optional) Add Aid Stations**: Click directly on the track on the map to add aid stations or other important points. These will be used to create custom segments in your race plan.
6.  **Configure the Model**: Adjust settings like the course's overall technicality and the expected fatigue factor for more fine-tuned predictions.
7.  **Generate Your Plan**: Click the "Générer le Plan de Course" button.
8.  **Review Your Plan**: Your detailed race plan will appear at the bottom of the page.

## Technical Stack

- **Frontend**: HTML5, JavaScript (ES6+)
- **Styling**: [Tailwind CSS](https://tailwindcss.com/)
- **Mapping**: [Leaflet.js](https://leafletjs.com/)
- **GPX Parsing**: [togeojson.js](https://github.com/tmcw/togeojson)