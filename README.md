# 🏴󠁧󠁢󠁳󠁣󠁴󠁿 Edinburgh Food Finder

An interactive web-based map application designed to help travelers discover diverse culinary experiences in Edinburgh.

## 🌟 Project Motivation
During a past trip to Edinburgh, I was overwhelmed by the sheer number of dining options. To solve the "decision paralysis" many tourists face, I developed this tool to categorize and visualize the city's restaurants by cuisine, allowing users to find exactly what they are craving with ease.

## 🛠️ Tech Stack
- **Engine:** [Mapbox GL JS](https://www.mapbox.com/mapbox-gljs)
- **Data Source:** [OpenStreetMap](https://www.openstreetmap.org/) (via Overpass Turbo)
- **Formatting:** GeoJSON
- **Frontend:** HTML5, CSS3, JavaScript (ES6)

## 🎯 Main Features
- **Dynamic Cuisine Filter:** Toggle between 10+ categories (Indian, Cantonese, Italian, etc.) using a real-time filtering engine.
- **Two-Tier Info System:** - **Hover:** Quick name/cuisine preview.
  - **Click:** Smooth `flyTo` animation and a side panel with contact info, opening hours, and website links.
- **Google Maps Integration:** Direct one-click navigation link for every venue.
- **Geofencing:** Map restricted to the Edinburgh city center for a focused user experience.

## 📊 Data Processing
The raw OSM data was normalized to handle inconsistent tagging (e.g., `cuisine` vs `Cuisine`). I implemented a coalesce logic in JavaScript to ensure data integrity and formatted multiple address tags into human-readable strings.

## 🚀 Future Improvements
- Integration with Live APIs (Yelp/Google Places) for real-time ratings.
- User geolocation for "Near Me" restaurant discovery.
- Advanced spatial heatmaps to show culinary density.
