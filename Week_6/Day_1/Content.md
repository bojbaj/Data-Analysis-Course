# Day 1 Content: Advanced Interactive Visualizations with Plotly and Dash

## Overview
Interactive dashboards are powerful tools for data exploration and presentation. Today, you will learn how to create advanced interactive visualizations using **Plotly** and **Dash**, a Python framework for building web-based dashboards. By the end of the day, you will be able to create dynamic dashboards with multiple components, such as dropdowns, sliders, and graphs, and deploy them for real-time data exploration.

---

## 1. Introduction to Dash
Dash is a Python framework for building web-based dashboards. It integrates seamlessly with Plotly, allowing you to create interactive visualizations that can be embedded in web applications. Dash is ideal for creating dashboards that allow users to explore data in real-time.

### Key Features of Dash:
- **Interactivity**: Dropdowns, sliders, and other interactive components.
- **Integration with Plotly**: Use Plotly charts in Dash applications.
- **Deployment**: Deploy dashboards as standalone web applications.

### Why Use Dash?
- It allows you to create professional-quality dashboards with minimal code.
- It supports real-time data updates and user interactions.
- It integrates well with other Python libraries like Pandas and NumPy.

---

## 2. Creating Basic Dashboards with Dash
### 2.1 Layout Components
Dash provides a variety of layout components, such as dropdowns, sliders, and buttons, that can be used to create interactive dashboards.

### 2.2 Plotly Graphs in Dash
You can embed Plotly graphs in Dash applications to create interactive visualizations. Dash allows you to update graphs in real-time based on user input.

### 2.3 Callbacks
Callbacks are functions that update the dashboard based on user input. For example, you can use a callback to update a graph when the user selects a value from a dropdown.

---

## 3. Deploying Dashboards
Dash applications can be deployed as standalone web applications using platforms like **Heroku** or **AWS**. You can also share dashboards as HTML files or embed them in websites.

---

## 4. Practice Exercises
Today, you will work with three datasets to apply what you've learned. Each dataset is designed for specific practices:

### Dataset 1: Sales Data (`Dataset1.csv`)
- **Description**: Contains sales data with columns like `Region`, `Sales`, `Profit`, and `Quantity`.
- **Practices**: Practice 1, Practice 2.

### Dataset 2: Customer Feedback Data (`Dataset2.csv`)
- **Description**: Contains customer feedback scores and demographic information.
- **Practices**: Practice 3, Practice 4.

### Dataset 3: Product Performance Data (`Dataset3.csv`)
- **Description**: Contains product performance metrics like `Price`, `Sales`, and `Customer Rating`.
- **Practices**: Practice 5, Practice 6.

---

## 5. Practice Tasks
### Practice 1: Creating a Basic Dashboard
- **Dataset**: `Dataset1.csv`
- **Task**: Create a basic dashboard with a dropdown to select a region and display `Sales` and `Profit` for the selected region.
- **Deliverable**: "Practice1_Dashboard.html"

### Practice 2: Adding Interactive Components
- **Dataset**: `Dataset1.csv`
- **Task**: Add a slider to filter `Sales` by quantity and update the graph in real-time.
- **Deliverable**: "Practice2_Dashboard.html"

### Practice 3: Creating a Feedback Dashboard
- **Dataset**: `Dataset2.csv`
- **Task**: Create a dashboard with a dropdown to select an age group and display `Feedback Score` trends over time.
- **Deliverable**: "Practice3_Dashboard.html"

### Practice 4: Customizing a Dashboard
- **Dataset**: `Dataset2.csv`
- **Task**: Add multiple interactive components (e.g., dropdowns, sliders) to filter and visualize `Feedback Score` by region and age group.
- **Deliverable**: "Practice4_Dashboard.html"

### Practice 5: Creating a Product Performance Dashboard
- **Dataset**: `Dataset3.csv`
- **Task**: Create a dashboard with a dropdown to select a product and display `Price`, `Sales`, and `Customer Rating`.
- **Deliverable**: "Practice5_Dashboard.html"

### Practice 6: Deploying a Dashboard
- **Dataset**: `Dataset3.csv`
- **Task**: Create a comprehensive dashboard with multiple interactive components and deploy it as an HTML file.
- **Deliverable**: "Practice6_Dashboard.html"

---

## 6. Advanced Reading
For further learning:
- [Dash Documentation](https://dash.plotly.com/)
- [Interactive Dashboards with Dash](https://towardsdatascience.com/interactive-dashboards-with-dash)