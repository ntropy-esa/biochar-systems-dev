---
name: "Knowledge level 0"
styling:
    sectionClass: "section-sm section-dark"
    containerClass: " "
    rowClass: ""
# in one row, nb of boostrap columns can be defined directly below in HTML

---

## **... lead to a diversity of product distribution and qualities**

<div class="col-md-4 text-left">
In the case of pyrolysis, 

- Typical product distribution, .... in mass units .... in energy units...
- qualities... of the char

Properties of hydrothermal & torrefaction char... why is it peculiar 

Properties of gasification char... why is it peculiar

### **Mass and energy balance models for pyrolysis**
Predicting the exact composition and the qualities of ... is not easy may require advanced chemistry models (e.g. Aspen, ...) or even actual experimentation and analysis of the products.

However, in the litterature, existing models for simpler models exists. Here, we present two of these. 
</div>

<div class="col-md-8 text-left">
{{< tabs name="MEB_pyrolysis">}}
  {{% tab name="Model 1"%}}
  This model applies to the simple, yet most common, case where pyrolysis oil & gas are directly combusted after pyrolysis to generate heat. It was developped and used in the case studies of this paper.

  **Description**:
  
  what is in the scope, what is excluded from it..: biomass drying, heat recovery, turbine
  Disclaimer: it's to the user to make sure that combination of (mutually dependent) parameters make sense (e.g. if biochar yield is 10% or 30% probably also affects its carbon contents)

  **Model inputs**:
  - q
  
  **Model outputs**: 
  - q


  **Sankey Widget**
  
  To do 

  {{< button href="../biochar-stability-calculator.xlsx" icon="download" >}} Download as Excel {{< /button >}}
  {{< button href="../biochar-stability-calculator.py" icon="download" >}} Download as Python script {{< /button >}}

  {{% /tab %}}


  {{% tab name="Model 2"%}}
  This second model is derived from the research article by [Woolf and colleagues (2014)](https://pubs.acs.org/doi/10.1021/es500474q). The authors described it as "an  accurate-yet-simple empirical model for predicting yields, product compositions, and energy balances from biomass slow pyrolysis".

  **Description**:

  what is in the scope, what is excluded from it..

  **Model inputs**:
  - q
  
  **Model outputs**: 
  - q



  **Sankey Widget**
  
  To do 
  {{< button href="../biochar-stability-calculator.xlsx" icon="download" >}} Download as Excel {{< /button >}}
  {{< button href="../biochar-stability-calculator.py" icon="download" >}} Download as Python script {{< /button >}}

  {{% /tab %}}

  {{% tab name="Model 3"%}}
  Again, [Woolf and colleagues (2021)](https://pubs.acs.org/doi/10.1021/acs.est.1c02425), released some empirical equations to determine the biochar yield of a process, based on the biomass ash content, the biomass lignin content, and the pyrolysis temperature.

  **Description**:

  what is in the scope, what is excluded from it..

  **Model inputs**:
  - q
  
  **Model outputs**: 
  - q

  **Plotly 2D graph with 3rd param as slider**
  
  To do: 
  {{< button href="../biochar-stability-calculator.xlsx" icon="download" >}} Download as Excel {{< /button >}}
  {{< button href="../biochar-stability-calculator.py" icon="download" >}} Download as Python script {{< /button >}}

  {{% /tab %}}
{{< /tabs >}}

</div>
