---
name: "Knowledge level 0"
styling:
    sectionClass: "section-sm section-dark"
    containerClass: " "
    rowClass: ""
# in one row, nb of boostrap columns can be defined directly below in HTML

---

<div class="col-md-10 text-left">

## **... lead to a diversity of product distribution and qualities**
</div>
<div class="col-md-2">
</div>

<div class="col-md-4 text-left">

- Typical product distribution, .... in mass units .... in energy units...

Weber K, Quicker P (2018) Properties of biochar. Fuel 217:240–261. https://doi.org/10.1016/j.fuel.2017.12.054

UC David Biochar Database n.d. http://biochar.ucdavid.edu (accessed September
30, 2015).

Ippolito JA, Cui L, Kammann C, et al (2020) Feedstock choice, pyrolysis temperature and type influence biochar characteristics: a comprehensive meta-data analysis review. Biochar 2:421–438. https://doi.org/10.1007/s42773-020-00067-x

### **Mass and energy balance models for pyrolysis**
Predicting the exact composition and the qualities of ... is not easy may require advanced chemistry models (e.g. Aspen, ...) or even actual experimentation and analysis of the products.

However, in the litterature, existing models for simpler models exists. Here, we present two of these. 
</div>

<div class="col-md-8 text-left">
{{< tabs name="MEB_pyrolysis">}}
  {{% tab name="Model 1"%}}
  This model applies to the simple, yet most common, case where pyrolysis oil & gas are directly combusted after pyrolysis to generate heat. It was developped and used in the case studies of this research project.

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
  This second model is derived from the research article by [Woolf and colleagues (2014)](https://pubs.acs.org/doi/10.1021/es500474q). The authors described it as "an  accurate-yet-simple empirical model for predicting yields, product compositions, and energy balances from biomass slow pyrolysis" helping to "quantify the trade-offs between energy and biochar yields in bioenergy–biochar systems".

  **Description**:

- Model limited to pyrolysis, in particular slow-pyrolysis. It excludes gasification, where some oxygen or steam is allowed in the reactor.
- Multiple pathways to produce biochar and biofuel (either gas or liquid fuel) are considered (see Table 1 in the article). To clarify, it includes biomass processing, pyrolysis, and upgrading of the pyrolysis oil and gas through several pathways. Gas pathways: water-gas shift reaction to produce hydrogen; catalytic methanation of pyrolysis gas. Liquid fuel pathways: catalytic methanol synthesis, Ljungdahl-Wood pathway, Fischer-Tropsch synthesis. 
- It assumes that all energy inputs needed by the process (heat and electricity) come from the pyrolysis products or from extra biomass. To clarify, this assumes no external inputs of e.g. natural gas or grid electricity.
- 

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
  [Woolf and colleagues (2021)](https://pubs.acs.org/doi/10.1021/acs.est.1c02425) released empirical equations to determine the **biochar yield** and the **biochar carbon content** of a given pyrolysis process based on the biomass ash content, the biomass lignin content, and the pyrolysis temperature.

  **Description**:

  The model is based on meta-analysis of data found in the literature. Two meta-analyses are cited:
  - [Neves et al., 2011](https://doi.org/10.1016/j.pecs.2011.01.001), with 128 measurements from 26 papers (R<sup>2</sup> = 0.65), for biochar carbon content
  - [Woolf et al., 2014](https://pubs.acs.org/doi/10.1021/es500474q), with 146 measurements from 18 papers (R<sup>2</sup> = 0.65), for biochar yield

  The model assumes that the ash content in the biomass is conserved during pyrolysis, and remains in the biochar.

<sub></sub>
<sup></sup>
  **Model inputs**:
  - T &rarr; the pyrolysis temperature, in degree Celcius
  - F<sub>a,bm</sub> &rarr;  the ash contrent of the biomass, on a dry basis
  - L &rarr; the lignin content of the biomass, on a dry basis
  
  **Model outputs**: 
  - Y<sub>BC</sub> &rarr; the dry-ash-free yield of biochar from pyrolysis
  - F<sub>C</sub> &rarr; the organic carbon mass fraction on a dry mass basis

  **Equations**:

  <span style="text-align:center">

 <!--
    *Y<sub>BC</sub>* = 0.1261 + 0.5391 e<sup>-0.004*T*</sup> + 0.002733*L*

    *F<sub>C</sub>* = (1- (F<sub>a,bm</sub>) / (F<sub>a,bm</sub> + Y<sub>BC</sub>) ) * (0.93 - 0.92 e<sup>-0.0042*T*</sup> >
 -->

  $$ Y_{BC} = 0.1261 + 0.5391 e^{-0.004T} + 0.002733L $$

  $ F_C = (1 - \frac{F_{a,bm}}{F_{a,bm} + Y_{BC}} ) * (0.93 - 0.92 e^{-0.0042T}) $

  </span>

  <!--
  **Plotly 2D graph with 3rd param as slider**
   -->

  {{< button href="2-pyrolyisis-woolf2021-biochar-carbon-yield.xlsx" icon="download" >}} Download as Excel {{< /button >}}

  {{% /tab %}}
{{< /tabs >}}

</div>
