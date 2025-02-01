# Vehicle Routing Optimization Web Application

This project is a Flask-based web application designed to optimize vehicle routing and scheduling for deliveries. It allows users to upload shipment data, select time slots, and view optimized trips with detailed metrics. The application provides an interactive interface for visualizing routes and analyzing utilization metrics.

---

## Features

1. **Upload Excel File**:
   - Users can upload an Excel file (`.xlsx`) containing shipment data.
   - The file is processed to extract relevant information for optimization.

2. **Select Time Slot**:
   - Users can choose a preferred time slot for deliveries.
   - Available time slots are displayed in a user-friendly dropdown menu.

3. **Optimized Trips**:
   - The system calculates optimized routes and displays detailed trip information, including:
     - Vehicle type
     - Total shipments
     - Shipments delivered
     - Route
     - MST Distance
     - Trip Time
     - Capacity Utilization
     - Time Utilization
     - Distance Utilization (COV_UTI)

4. **Interactive Map**:
   - Users can view the optimized routes on an interactive map.
   - The map highlights the delivery points and the sequence of stops.

5. **Responsive Design**:
   - The application is fully responsive and works seamlessly on desktops, tablets, and mobile devices.

---

## Technologies Used

### Backend
- **Python**
- **Flask**: Web framework for building the backend.
- **Pandas**: For processing Excel files and data manipulation.
- **Geopy**: For geographical distance calculations.

### Frontend
- **HTML5, CSS3, JavaScript**
- **Bootstrap 5**: For styling and responsive design.
- **Font Awesome**: For icons.
- **Google Maps API**: For interactive map visualization.

---

## Project Structure

```plaintext
vehicle-routing-optimization/
├── app.py                  # Flask application entry points
├── requirements.txt        # Python dependencies
├── static/                 # Static files (CSS, JS, images)
│   └── styles.css          # Custom CSS for styling
├── templates/              # HTML templates
│   ├── upload.html         # Upload Excel file page
│   ├── select_timeslot.html# Select time slot page
│   ├── trips.html          # Display optimized trip
│   └── map.html            # Interactive map page
└── README.md               # Project  documentation
