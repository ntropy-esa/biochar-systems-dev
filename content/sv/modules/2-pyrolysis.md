---
title: "2 - Pyrolysis"
description: "this is meta description"
draft: false
image : "images/portfolio/work2.jpg"
bg_image: "images/feature-bg.jpg"
menu:
  main:
    parent: "Systems analysis"
    name: "2. Pyrolysis"
    weight: 3

category: "Module"
information:
  - label : "Client"
    info : "Jannie Kelonsky"
  - label : "What We Did"
    info : "Website Redesign"
  - label : "Tools Used"
    info : "Photoshop,Illustrator"
  - label : "Completed on"
    info : "17th March 2014"
  - label : "Skills"
    info : "HTML5 / PHP / CSS3"
  - label : "Client"
    info : "Jannie Kelonsky"

# Page-specific JavaScript & CSS #ESA
js : ["bw2widgets/d3.v3.min", "bw2widgets/widget_demo", "bw2widgets/widget_plot_types", "js/mermaid.min"]
css : ["bw2widgets/widget"]

---

## Behance Website Redesign

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quas officiis cumque, harum dicta necessitatibus
reprehenderit, delectus molestiae, impedit alias adipisci distinctio voluptas. Tempora modi amet voluptate
at provident soluta consequatur.

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolores quibusdam sed, neque recusandae, est
odit. A facere tempore soluta laborum.

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Incidunt, rem eaque facilis. Sit, voluptas?
Error soluta odio, harum tenetur, alias in iure ipsam blanditiis illo, ratione, magnam a minima incidunt!
Suscipit facilis, ut maxime libero necessitatibus, rerum aut voluptates aliquam maiores iusto qui
temporibus nesciunt, incidunt in quasi. Veniam aliquid ea aperiam, obcaecati voluptate ab, temporibus
fugiat at, inventore molestiae quibusdam, modi numquam debitis libero aut eum. Architecto sit quia quidem
odit, quasi eveniet reprehenderit rerum dolorem voluptate sed aspernatur numquam enim, adipisci iste optio
ea libero laboriosam praesentium aperiam nobis vero tempore consequuntur sapiente eos at. Suscipit quis
voluptatibus temporibus dolore consectetur ex excepturi adipisci sunt. Maxime aperiam eos illum minima
aliquid voluptate autem qui at impedit recusandae earum possimus, alias, maiores sint, sed quia quis aut
cupiditate voluptatem reiciendis. Facilis nobis assumenda totam officiis dicta autem dolorem quidem
similique, delectus rerum laborum veritatis, cum magnam dignissimos necessitatibus possimus error, eius
omnis veniam culpa, porro officia adipisci exercitationem minus hic. Ipsum veritatis repudiandae nulla quo
dicta voluptates tenetur mollitia perferendis sequi, magnam doloremque odit similique, sit, voluptas unde
iste molestias. Accusantium, corporis quibusdam quod in animi earum alias autem ipsum. Eaque rem numquam
delectus veniam commodi doloribus consequatur deleniti?

Lorem ipsum dolor sit amet, consectetur adipisicing elit. Dolores neque vero quasi quisquam atque in,
libero ab sunt eius! Nesciunt laboriosam alias corporis sit accusantium voluptate sapiente debitis quos
mollitia saepe maxime ipsum facilis dolore voluptas inventore veniam deleniti, eligendi harum aperiam iusto
culpa? Delectus dolorum facere quasi iure explicabo?


## Insert a bw2widget via in its own section
Random markdown text before the widget
{{< bw2widget widgetName="X1"  widgetTitle="Biochar production from willow">}} 
Random markdown text after the widget

## What follows the shortcode
Some other random text 

## Another shortcode: youtube video
{{< youtube id="PfIGIUWJnkw" title="2nd Green Carbon webinar" autoplay="false" class="col-lg" >}}

## Another shortcode: reference to another page
This is a link to the [Overview]({{< ref "modules/_index.md" >}})

## Another shortcode: highlight python code
{{< highlight python "linenos=table" >}}
import brightway2 as bw2
bw2.projects.set_current("MyProject")
## Check https://gohugo.io/content-management/syntax-highlighting/ for other styling
{{< /highlight >}}

## A figure: image with caption
{{< figure src="../esmeralda.jpg" title="Fig. Esmeralda" width="20%">}}

## Flowcharts
<script>mermaid.initialize({ startOnLoad: true, securityLevel: 'loose'});</script>
{{< mermaid align="left" >}}
graph LR;
    A(Biomass production) -->|biomass| B(Pyrolysis)
    B -->|oil and tars| C(Co-product use)
    B -->|biochar| D(Biochar product manufacturing)
    E(Supply of other materials) -->|other materials| D
    D -->|biochar product| F(Biochar product use)
    F -->|biochar product waste| G(Biochar product end-of-life)
{{< /mermaid >}}
https://mermaid-js.github.io/mermaid/#/
https://mermaid-js.github.io/mermaid/#/flowchart?id=styling-and-classes
https://github.com/kubernetes/website/blob/main/layouts/shortcodes/mermaid.html


    C -->|One| D[ {{< ref "modules/_index.md" >}} ]
    C -->|Two| E[<a href=""> Result two </a> ]

https://it.knightnet.org.uk/kb/hugo/embed-diagram/


## Tooltip with glossary
https://kubernetes.io/docs/contribute/style/hugo-shortcodes/#glossary
https://github.com/kubernetes/website/tree/main/layouts/shortcodes

Par exemple, le snippet suivant est rendu à {{< tooltip_glossary text="cluster" term_id="cluster" >}} avec une infobulle :

## Table interactive
Check out
https://biochar-international.org/biochar-classification-tool-interface/
