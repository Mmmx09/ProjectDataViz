# Scoping Document: E-Waste Data Visualization Project
## 1. Problem Statement
Global E-waste is rapidly becoming a major challenge to environmental sustainability. According to the United Nations, the world generates more than 50 million tons of e-waste every year, but less than 20% of the e-waste is formally recycled. A large number of waste electronic products have not been properly treated, and the toxic substances (such as lead, mercury, cadmium, etc.) contained in them pose a serious threat to the ecological environment and human health.

The purpose of this project is to present the key dimensions of e-waste, such as global distribution, growth trend, per capita production, and recycling efficiency, through data visualization so as to enhance public awareness of the e-waste problem and provide decision-making reference for policymakers and environmental protection organizations.

## 2. Target Audience
This project is designed for the following user groups:
- General Public: To enhance awareness of the e-waste issue through interactive and intuitive charts.
- Policymakers: To offer insights into national performances on e-waste management and inform better regulations.
- Educators and Students: As educational material on global environmental issues and data interpretation.
- Environmental NGOs: To support research, advocacy, and outreach efforts with compelling data visuals.

## 3. Data Sources
The data for this project is sourced from reputable global reports and open datasets, including:
- Global E-waste Monitor (United Nations)
- Primary dataset: 'e-waste dataset final.csv,' which we find in Kaggle, you can go through this link: '(https://www.kaggle.com/datasets/arifmia/e-waste-data)'.

## 4. Design Choices
This visualization platform follows the core principles of clarity, interactivity, and responsiveness:

## 1. Map (Global E-waste Generation and Recycling Rate)
   - A choropleth map is used to display country-level e-waste data. Color gradients convey the magnitude of e-waste generation and recycling rates, providing an intuitive comparison between countries.
   - Interactivity: Users can hover over countries to view specific statistics (e.g., per capita generation, recycling rate), which enhances engagement and supports exploratory data analysis.

2. Line Chart (E-waste Generation Trend)
   - A temporal line chart visualizes the trend in e-waste generation from 2010 to 2023 for selected countries.
   - This format is ideal for tracking changes over time and spotting patterns such as growth spikes or reduction periods.
   - Users can interact with the chart by selecting countries and hovering over data points to see exact values.

3. Parallel Coordinates Plot (Carbon Footprint by Purchase Year)
   - This multivariate chart enables a comparison of carbon footprints across years and cities.
   - The parallel coordinates design is suitable for high-dimensional data, allowing users to trace each city’s performance across multiple years.
   - A region filter and year range slider allow users to drill down into specific segments, providing a customizable exploration experience.

4. Sunburst Chart + Hazard Component Table (Hazardous Material Composition & Impact)
   - The sunburst chart presents hierarchical data of hazardous material types used in appliances.
   - interaction logic: Clicking the outer segments dynamically updates the table beside it, which lists detailed component names, weights, and hazard index values.
   - This chart reinforces the connection between component categories and their toxicological impact.

5. Sankey Diagram (E-waste Transport Routes and Recycling Prices)
   - The Sankey diagram illustrates the flow of e-waste from origin cities through price tiers to destination countries.
   - It’s well-suited for displaying proportional flow data, showing volume distribution and relationships at different stages.
   - Hovering reveals additional metadata, such as recycling company names, methods, and final usage.
