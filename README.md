# 404-55-SUSTAIN-AI-THON

NeighbourNet is a web application designed to connect users with local service providers such as electricians, plumbers, educators, water suppliers, and also integrating charity services. The platform leverages geolocation data to find providers within a radius of the user’s preference, ensuring fast and efficient access to essential services all in one place.
________________________________________
Workflow Diagram

![Screenshot 2025-01-20 220127](https://github.com/user-attachments/assets/a0df620d-103c-4b4d-ba0f-74d7f2662d37)

![image](https://github.com/user-attachments/assets/35b86074-9691-4d01-8a09-4704eef34f55)

User Access -> Frontend (HTML/CSS/React.js) -> Backend API (Express.js) -> Providers Data (JSON) -> Filter by Distance -> Return Results to Frontend
1.	User Access: Users open the web application in their browser.
2.	Frontend: Users click the “Get Nearby Providers” button, and the browser retrieves their geolocation data.
3.	Backend API: The frontend sends a request to the backend API with the user's latitude and longitude.
4.	Providers Data: The backend fetches data from a static providers.json file.
5.	Filter by Distance: The backend calculates the distance between the user and each provider using the geolib library, filtering providers within a preferred radius.
6.	Return Results: The backend returns the filtered providers to the frontend for display.
________________________________________
Concept Map
Core Components:

•	Frontend: 

HTML5, CSS3, and React.js for user interaction and geolocation.

Displays results dynamically in a user-friendly list.

•	Backend: 

Node.js and Express.js for server-side processing.

Geolib for distance calculations.

dotenv for environment variable management.

•	Data: 

Static providers.json file containing sample provider data for this prototype.
________________________________________
Tech Stack
1.	Frontend: HTML5, CSS3, React.js

2.	Backend: Node.js, Express.js, Geolib, dotenv

3.	Data Storage: JSON File (static data storage for prototype)
________________________________________
Novelty

NeighbourNet offers a lightweight, scalable solution for connecting users with local service providers without relying on external APIs, reducing costs and dependencies. By utilizing geolocation and a simple JSON-based database, this project provides an affordable and efficient alternative for small communities or organizations. This is a unified solution for all day to day needs.
________________________________________
Solution

NeighbourNet addresses the challenge of quickly finding service providers in a user’s vicinity by:
1.	Simplifying Access: Users can easily locate nearby services with a single click.
2.	Customizability: Service providers and their details can be updated directly in the providers.json file.
3.	Scalability: The application can integrate with external APIs (e.g., Google Maps) in the future for real-time data and extended functionality.
________________________________________
Additional Features

1.	Error Handling: 
o	Handles missing or invalid geolocation data.
o	Provides user-friendly alerts for issues.
2.	Modular Code: 
o	Easily extendable with additional services or data sources.
3.	Environment Variables: 
o	Uses .env for configurable settings like server port and future API keys.
________________________________________
Setup Instructions

Prerequisites
•	Node.js installed on your machine.
Steps
1.	Clone the repository: 
2.	git clone https://github.com/username/neighbournet.git
3.	Navigate to the backend folder and install dependencies: 
4.	cd neighbournet/backend
5.	npm install
6.	Create a .env file in the backend folder: 
7.	PORT=5000
8.	Start the backend server: 
9.	npx nodemon server.js
10.	Open the index.html file in your browser to interact with the frontend.
________________________________________
Future Enhancements
1.	Integration with External APIs:
 	Add real-time provider data using Google Maps API or similar services.
2.	Enhanced Search Filters: 
Allow filtering by service type or rating.
3.	Database Integration: 
Replace the static JSON file with a database like MongoDB or Firebase for dynamic data management.
4.	Mobile App: 
Create a mobile-friendly version using React Native or Flutter.
________________________________________

