---
layout: page
title: "The Global Grid: Mapping Our Energy Future"
permalink: /projects/final-project/
---

# The Global Grid: Mapping Our Energy Future
**Author:** Michael Chiflikyan

### **Project Resources**
* **Primary Dataset:** [WRI Global Power Plant Database (v1.3.0)](https://datasets.wri.org/dataset/globalpowerplantdatabase)
* **Analysis Notebook:** [View the Full Python Analysis on GitHub](https://github.com/MichaelChiflikyanBSIS/MichaelChiflikyanBSIS.github.io/blob/main/FinalProject3.ipynb)
---

### **The Invisible Network Powering Our Lives**
Our modern world relies on a massive network of nearly 30,000 power plants that feed into the global electricity grid. From massive nuclear facilities to sprawling solar farms, this network is the heartbeat of modern civilization. This project explores a comprehensive directory from the World Resources Institute to see exactly how our world is powered today.

### **Energy Access Shapes Everyday Life**
Electricity is deeply integrated into modern society; access to reliable power determines nearly every aspect of social development. Hospitals, schools, and businesses cannot operate without dependable infrastructure. In many parts of the world, unreliable grids still lead to shortages that slow economic growth, making energy infrastructure a key humanitarian and economic issue.

### **Why Geography Matters in Energy Production**
One of the most fascinating patterns in the dataset is how geography influences power plant types. Nations with large rivers invest heavily in hydroelectric power, while desert regions with high sunlight exposure are adopting solar farms. The result is a global energy map that reflects both technological development and the physical geography of our planet.

### **A Map of Human Progress and Challenges**
By tracking geographic locations, fuel types, and generation capacity, we can see how different nations have prioritized energy security. Historically, coal and gas have dominated because they provided the high-capacity power needed for industrialization. However, the data now shows a rapid diversification toward solar, wind, and hydro power.

### **Industrial Growth and Fossil Fuel Dependence**
For much of the twentieth century, industrial growth was directly tied to fossil fuel expansion. These plants were designed for reliability and scale, often producing enormous amounts of electricity for urban populations. However, this expansion came with environmental consequences, including rising emissions and air pollution.

### **Renewable Energy Is Expanding Rapidly**
Although fossil fuels still represent a major share of generation, renewable technologies are expanding at an unprecedented pace. Declining costs have accelerated the deployment of green infrastructure. Unlike traditional thermal plants, renewable systems tend to be distributed across many smaller installations, leading to the high density of solar and wind facilities seen in recent decades.

### **The Great Energy Transition**
The "commissioning year" in this dataset allows us to see the lifecycle of energy technology as it evolves. We can observe a clear trend where older, massive fossil fuel plants are increasingly being joined by smaller and more numerous renewable installations. This transition represents a global shift toward a more sustainable future.

---

### **Interactive Exploration: Capacity vs. Time**

This chart allows you to see the "evolutionary" timeline of our global energy grid. Every circle represents a single power plant. The higher the circle is on the chart, the more electricity that plant is capable of producing. 

<div id="vis" style="width: 100%;"></div>
<script src="https://cdn.jsdelivr.net/npm/vega@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-lite@5"></script>
<script src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>
<script>
  vegaEmbed('#vis', '{{ "/assets/js/main_viz.json" | relative_url }}');
</script>

*Tip: Click a fuel type in the legend to filter the view. You can also zoom into specific decades to see the density of new plant openings.*

---

### **The Bigger Picture: Scaling and Impact**

#### **1. Global Capacity by Fuel Type**
![Average Capacity by Fuel Type]({{ "/assets/pngs/fuel_capacity.png" | relative_url }})
*Figure 1: This chart compares the average generating capacity across different energy sectors. While renewable plants are now more numerous, traditional thermal and nuclear plants lead in raw power output per facility. Source: Created by Michael Chiflikyan using WRI Data.*

#### **2. Environmental Context: Total Global Output**
![Total Global Capacity]({{ "/assets/pngs/emissions_context.png" | relative_url }})
*Figure 2: This chart shows the total power generation capacity currently installed worldwide for each fuel type. While our interactive map shows thousands of new green dots (Solar and Wind), this chart reveals that traditional fuels like Coal and Gas still account for the largest share of the world's total power output.*

---

### **Technical Methodology**
The analysis was performed using Python, utilizing the Pandas library for data cleaning and Altair for the interactive visualizations. The data was filtered to highlight impactful trends for a general audience.

---

### **Citations and Data Sources**
* **Primary Data:** Global Power Plant Database. 2021. Washington, DC: World Resources Institute. [https://datasets.wri.org/dataset/globalpowerplantdatabase](https://datasets.wri.org/dataset/globalpowerplantdatabase)
