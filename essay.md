# Dashboards for Biology: Stop Treating Your Plots Like PowerPoint

### Introduction

Biologists have used static figures to show data for many years. We create graphs, put them in PowerPoint, and present them. But this old way has problems. Our data is getting bigger and more complex. Static plots cannot show everything we need to see. The answer is interactive dashboards. These let us explore data in real time and make better decisions.

### Problems with Static Plots

When we use static figures, we follow these steps: ask a question, collect data, make a plot, and share our interpretation. This works for final papers. But it creates problems during research.

**We can only show a few things at once**: A regular scatter plot shows two or three variables. But modern experiments create data for hundreds or thousands of features at the same time. We must choose which variables to plot. This means we might miss important patterns.

**We cannot explore easily**: Once we make a figure, we need to create new plots to test new ideas. This takes time and might stop us from looking at data in different ways.

**Hard to communicate**: Static figures need long captions to explain everything. Readers cannot look at the data themselves or test their own ideas.

### Interactive Dashboards: A Better Way

Interactive dashboards change how we use data visualization. Instead of just showing conclusions, dashboards let people explore data. This is very useful in biology. Our datasets often have unexpected patterns. Different people need to see the data in different ways.

#### Why Dashboards Help Biologists

**Filter and sort data easily**: Researchers can filter data by different conditions. For example, in single-cell RNA sequencing, users can filter cells by cluster, gene expression, or patient information. All plots update right away.

**Look at data at different scales**: Biology works at many levels—from molecules to cells to tissues to whole organisms. Interactive dashboards let us move between these levels easily. A user might start with a big picture view, then click to see details about individual genes.

**Test ideas quickly**: Instead of making new plots for each question, researchers can change parameters in real time. This makes the process of forming and testing ideas much faster.

**Better reproducibility**: Good dashboards show analytical decisions clearly. When parameters are in a user interface instead of hidden in code, the analysis becomes easier to understand and repeat.

#R has powerful tools for making interactive biology dashboards. Tools like Shiny and Quarto allow researchers to create these dashboards without needing web development expertise. Shiny builds web-based applications where users can interact with data through buttons, sliders, and filters. Quarto creates interactive documents that combine analysis code with visualizations that users can manipulate directly in their browser.

### Case Studies: Dashboards in Action

#### Clinical Trials and Drug Studies
Consider a clinical trial monitoring patient responses to cancer treatment across different therapy groups. A static bar graph might show average response rates, but it locks in which patient groups are compared, what timepoint is displayed, and which biomarkers are shown. An interactive dashboard could let a researcher:
i. Filter patients by age, disease stage, or baseline biomarker levels.
ii. Switch between viewing response rates, side effect profiles, or quality of life scores.
iii. Examine how individual patients responded throughout the treatment period.
The dataset reveals more insights, not because of better graphics, but because researchers can ask different questions of the same data. The FDA's Sentinel Initiative demonstrates this approach by using dashboards to track drug safety patterns across millions of patient records.


### How to Start

For biologists who want to move from static plots to interactive dashboards:

**Start small**: Begin with one analysis that you do repeatedly. Build a simple dashboard that automates parameter selection and makes visualizations. Even basic interactivity (filtering, zooming, tooltips) helps immediately.

**Improve based on use**: Give dashboards to actual users (lab members, collaborators, yourself) and watch how they use the tool. Which features get used most? Where do users get confused? Make changes based on real usage.

**Make it robust**: Dashboards often get used longer than expected. Invest time in error handling, input validation, and documentation. Future you will appreciate clear comments and good failure handling.

**Share and work together**: The R community has many resources for dashboard development. Share your dashboards (even imperfect ones) to get feedback and help others learn. Many successful tools started as personal projects shared openly.

### Conclusion

Moving from static figures to interactive dashboards is more than a technical change. It is a shift in how we think about data visualization in biological research. Instead of seeing plots as endpoints that show conclusions, dashboards treat visualization as a process that enables exploration, discovery, and decision-making.

As biological datasets continue to grow, the ability to create interactive dashboards will become essential for researchers. The tools are ready to use. Learning resources are available. The impact on research efficiency and quality is large. The question is not whether to use interactive visualization, but how quickly we can stop treating our plots like PowerPoint.

### References

Allaire, J.J., Teague, C., Scheidegger, C., Xie, Y., & Dervieux, C. (2024). Quarto: R Interface to 'Quarto' Markdown Publishing System. https://quarto.org

Chang, W., Cheng, J., Allaire, J., Sievert, C., Schloerke, B., Xie, Y., Allen, J., McPherson, J., Dipert, A., & Borges, B. (2021). shiny: Web Application Framework for R. R package version 1.7.1. https://CRAN.R-project.org/package=shiny

Perkel, J. M. (2018). Data visualization tools drive interactivity and reproducibility in science. Nature, 554(7690), 133–134. https://doi.org/10.1038/d41586-018-01322-9

Sievert, C. (2020). Interactive Web-Based Data Visualization with R, plotly, and shiny. Chapman and Hall/CRC. https://plotly-r.com

Weissgerber, T. L., Milic, N. M., Winham, S. J., & Garovic, V. D. (2016). Beyond bar and line graphs: Time for a new data presentation paradigm. PLoS Biology, 14(4), e1002484. https://doi.org/10.1371/journal.pbio.1002484