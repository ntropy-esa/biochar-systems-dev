---
name: "Knowledge level 0"
styling:
    sectionClass: "section-sm section-dark"
    containerClass: " "
    rowClass: ""
# in one row, nb of boostrap columns can be defined directly below in HTML

gallery_item:
  - album: "gallery-pyrolysis"
    image: "1_woodpellet.png"
    caption: "Wood pellet 
              <br /> - rather dry, usually below 10%
              <br /> - often a side product from timber production
              <br /> - alternatively, often combusted for heating purposes
              "
  - album: "gallery-pyrolysis"
    image: "2_gardenwaste.jpg"
    caption: "Garden waste              
              <br /> - varying moisture, usually around 50%
              <br /> - material of heterogenous quality, with possible impurities
              <br /> - alternatively, often combusted in waste facilities with energy recovery
              "

  - album: "gallery-pyrolysis"
    image: "3_loggingresidues.png"
    caption: "Logging residues
              <br /> - varying moisture, usually around 50%, with potential partial drying in the forest
              <br /> - often a side product from forestry operations, not harvested or partially harvested
              <br /> - when left in the forest, residues contributes to forest carbon stocks & biodiversity
              "

  - album: "gallery-pyrolysis"
    image: "4_willowchips.jpg"
    caption: "Willow woodchips
              <br /> - varying moisture, usually around 50%
              <br /> - often produced on set aside agricultural land
              <br /> - part of short rotation coppice systems
              "

  - album: "gallery-pyrolysis"
    image: "5_sludge.png"
    caption: "Sewage sludge
              <br /> - varying moisture, usually high moisture content which requires drying before pyrolysis
              <br /> - often seen as a problem, due to potentially high contents of heavy metals, but also an important source of nutrients
              <br /> - alternative uses includes application to agricultural land, incineration, or landfilling
              "
---

<div class="col-md-7 text-left">

## **LCA of biomass pyrolysis**

The environmental impact from operating a pyrolysis plant can be decomposed in the following terms:

- Manufacturing and disposal of the pyrolysis reactor and surrounding equipment (including dryer, post combustion, flue glas cleaning, concrete slab, and maintenance operations)
- The supply and use of industrial products needed for operation of the pyrolysis reactor (electricity, water for quenching, reaction additives, or other consumables)
- Management of side-stream, mostly waste such as ash/fly ash collected in cyclone, and waste water sent to water treatment
- Direct environmental emissions, like dustfrom the stack from the stack/flue gases, but also...)
- Other operations for handling of the pyrolysis products
- Other operations for handling of biomass on site, and feeding
  
These terms rarely extensively modelled... not all contribute or have same relevance for different {{< tooltip_glossary text="environmental impact categories" term_id="" tooltip_text="Environmental impact categories are areas of human concern. Examples are climate change, air pollution, water eutrophication, ozone layer depletion. They are caused by different kind of stressors released by human activities in the environment. Some pollutants can be relevant for one impact category but not for another." >}}

Overall - impact contributions is small in life cycle perspective for high-tech well-used reactors, but can be significant for low-tech reactors due to high emissions (GHG balance). 

### **The type of reactor matters: from low-tech to high-tech**

some images ... low-tech


### **Parametrized life cycle inventory datasets for 3 kind of pyrolysis reactors**

Description of the data set..

Scale to 1 kg of biochar produced... contains... bi

Contains environmental emissions from 2 reactors (low-tech & high-tech)

Need to be linked upstream with: technosphere activities for biomass, electricity, use (from a background database)

How to use it

Limitations of current LCI data... 

{{< button href="../biochar-stability-calculator.xlsx" icon="download" >}} Download dataset as Excel file {{< /button >}}


</div>

<div class="col-md-5 text-right">

### **A gallery of pyrolysis reactors**

{{< gallery album="gallery-pyrolysis" order="asc" resize_options="150x150 webp" classDiv= "text-right" >}}

</div>
