---
# try also 'default' to start simple
theme: seriph
layout: first
background: ''
themeConfig:
  primary: '#003576'
drawing:
  enabled: true
slideTitle: Distributed platform for multi-model co-simulations in smart grids
---

## PhDMAN


### Oral Presentation 


### Tutor: Massimo Poncino & Edoardo Patti


### Matteo Orlando-s277013



---
layout: two-cols
---

# Smart Grid

### Main characteristics
- Shift from hierarchical architecture
- Bidirectional flows of data and energy

### Objectives:
- Improve service reliability by increasing automation and monitoring capabilities
- New kind of actors
- Multi-energy approach

### Challenges
- Manage data exchange (IoT)
- Manage Renewable Energy Resources (RES)

::right::

<v-clicks>

<img src="/assets/intro1.png" style="max-height:18vh;margin:auto">
<img src="/assets/intro2.png" style="max-height:18vh;margin:auto">
<img src="/assets/smartgrid.jpg" style="max-height:15vh;margin:auto">

</v-clicks>


---
layout: two-cols
---

# Research topic

**Models for the co-simulation**

In order to reach these objectives to develop models that can seamlessly work together in different combination.
Nowadays there is a lack of tools that enable to do so, the research is mainly focused on studying scenarios that include few models that most of the time are developed ad hoc to work with each other

<div v-click>
<p>
The objective is study an create <b>models</b> for the smart grid scenario which can work in <b>co-simulations</b> infrastructure.
This kind of research is needed to explore the possible scenarios that may appear in the shift towards the smart grid and find the best way to manage it.
</p>
</div>

::right::
<img src="/assets/cosimulation.png" style="margin:auto;max-height:50vh">


---

# Case studies for Smart Grid

**State of the art**

<div class="two-cols">
<div >

<v-clicks>

- Distribution network management (smart building, microgrid..)
- Transmission network management(<b>FDIR</b>,<b>metering</b> ...)
- Distributed energy resource (<b>PV panels</b>, wind turbine..)
- Smart grid communication (protocol, <b>latency</b>...)

</v-clicks>

</div >
<div >
<img src="/assets/cosimulation.png" style="margin:auto;max-height:50vh">
</div >
</div >

<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
</style>

---

# Metering and automation

### State of the art:
- Meters are mainly used for building and distribution network
- Centralized evaluation of the state of the grid
- Low automation

### Objective:
- Smart meter for transmission network
- Automation of outage management (self-healing grid)
- Provide a communication infrastructure

### Challenges:
- Algorithms for grid management can be computational expensive
- Outages needs a lot of time to be solved and human intervention is needed to restore the service

---
---

# 3-phase Smart Metering Architecture

**Proposed solution**

<div class="two-cols">
<div>


<v-clicks>

- 3-phase smart meter prototype with RTS
- Communication infrastructure (REST+MQTT)
- Self-configuration and auto-update of the devices
- On board algorithms (FD,FL, SE)
- External service ( network reconfiguration)
- IoT actuators have been simulated

</v-clicks>

</div>
<div>
<img src="/assets/3sma.png" style="margin:auto;max-height:50vh">
</div>
</div>

<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
</style>


---
layout: two-cols
---

# 3SMA

**Results**

- State estimation capability
- Fast fault detection and location
- Restore of the service in a short amount of time
- Resilience to network congestion

<div class="bottom">

> "A Novel Internet-of-Things Infrastructure to Support Self-Healing Distribution Systems," 2018 International Conference on Smart Energy Systems and Technologies (SEST), 2018, pp. 1-6, doi: 10.1109/SEST.2018.8495717.

> "A Smart Meter Infrastructure for Smart Grid IoT Applications," M. Orlando et al.,in IEEE Internet of Things Journal, vol. 9, no. 14, pp. 12529-12541, 15 July15, 2022, doi: 10.1109/JIOT.2021.3137596.

</div>

::right::
<img src="/assets/3sma1.png" style="margin:auto;max-height:18vh">
<img src="/assets/3sma2.png" style="margin:auto;max-height:12vh">
<img src="/assets/3sma3.png" style="margin:auto;max-height:12vh">

<style>
.bottom{
    margin-bottom:2rem
    }
blockquote{
    font-size:xx-small;
    margin-top:0.5rem
    }
</style>
---
layout: two-cols
---

# 3SMA

**Results**

- State estimation capability
- Fast fault detection and location
- Restore of the service in a short amount of time
- Resilience to network congestion
- Inclusion in co-simulation framework

<div class="bottom">


> "Hybrid SiL and HiL Multi-model Co-simulation Infrastructure for Multi-Energy Systems" Work in Progress
</div>

::right::
<img src="/assets/cosim.png" style="margin:auto;max-height:18vh">

<style>
.bottom{
    margin-bottom:2rem
    }
blockquote{
    font-size:xx-small;
    margin-top:0.5rem
    }
</style>

---

# RES and new actors

### State of the Art:
- Shift from fossil fuel and decreasing cost of PV panels
- Appearance of new actors in the smart grid scenario (prosumers, renewable energy community)
### Objective & novelties:
- Economic analysis of PV systems installation
- Analysis of multiple possible panels configuration
### Challenges:
- Size of the data needed for a fine estimation of the production
- Shading effect of PV panels

---

# Previous works

**Optimal Configuration and Placement of PV Systems in Building Roofs with Cost Analysis** 

<div class="two-cols">
<div>
<div>

- Yearly weather data (i.e. irradiation, temperature) from GIS
- Shading avoidance and/or exploitation
- Improved power generation

</div>
<div class="bottom">

>M. Orlando et al. "Optimal Configuration and Placement of PV Systems in Building Roofs with Cost Analysis," 2020 IEEE COMPSAC

</div>
</div>
<div>

<img src="/assets/res1.png" style="margin:auto;max-height:16vh">
<img src="/assets/improvement.png" style="margin:auto;max-height:17vh">
</div>
</div>

<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
.bottom{
    margin-bottom:2rem
    }
blockquote{
    font-size:xx-small;
    margin-top:0.5rem
    }
strong{
 color:var(--slidev-theme-primary)!important
 }
</style>

---

# Previous works

**Design of District-level Photovoltaic Installations for Optimal Power Production and Economic Benefit.**

<div class="two-cols">
<div>

- Possibility deploy and connect panels across different roofs
- Analysis of the impact of the number of panels  on the power production with costs vs. benefits

<img src="/assets/res2.png" style="margin:auto;max-height:10vh">

>M. Orlando et al. "Design of District-level Photovoltaic Installations for Optimal Power Production and Economic Benefit," 2021 IEEE COMPSAC
</div>
<div>


<img src="/assets/stacked_annotated.png" style="margin:auto;max-height:38vh">
</div>
</div>


<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
.bottom{
    margin-top:4rem
    }
blockquote{
    font-size:xx-small;
margin-bottom:2rem
    }
strong{
 color:var(--slidev-theme-primary)!important
 }
</style>

---

# A framework for economic and environmental benefit through Renewable Energy Community 

Improvement on the previous works

Starting from this works the effort was focused on overcoming 2 main limitation:

- a PV panel could have **only one orientation** (i.e. vertical)
- the economic analysis considered that the owner would **sell all the power produced** by the system

**How to solve them?**

<v-clicks>

- To overcome the first limitation, we enhanced the optimal placement algorithm to take into account the possibility to place panels both vertically and horizontally
- To solve the second limitation considered the possibility that smart grid actors might self-consume a part or even the entirety of the energy produced

</v-clicks>

<style>
strong{
 color:var(--slidev-theme-primary)!important
 }
</style>

---

# A framework for economic and environmental benefit through Renewable Energy Community 

<div class="two-cols">
<div >

Obtained result

- Possibility to evaluate systems with different panel orientation (also mixed)
- By simulating the consumption of a realistic population we can realistically evaluate the benefit of a REC
- $CO_2$ reduction due to usage of renewable energy


>A framework for economic and environmental benefit through Renewable Energy Community" Matteo Orlando et al. IEEE Systems Journal , under review

</div>
<div class="two-cols">

<div >

<img src="/assets/rec1.png" style="margin:auto;max-width:-moz-available">

</div>
<div >
<img src="/assets/rec2.png" style="margin:auto;max-width:-moz-available">
<img src="/assets/rec3.png" style="margin:auto;max-width:-moz-available">

</div>
</div>
</div>

<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
blockquote{
    font-size:xx-small;
margin-bottom: 2rem;
    }
</style>

---

# A framework for economic and environmental benefit through Renewable Energy Community 

<div class="two-cols">
<div >

Obtained result

- Possibility to evaluate systems with different panel orientation (also mixed)
- By simulating the consumption of a realistic population we can realistically evaluate the benefit of a REC
- $CO_2$ reduction due to usage of renewable energy
- Working on parallel execution (@Rasterframes)


</div>

<div >

<img src="/assets/parallel.png" style="margin:auto;max-width:-moz-available">

</div>
</div>

<style>
.two-cols{
grid-template-columns: repeat(2, minmax(0, 1fr));
display:inline-grid
}
blockquote{
    font-size:xx-small;
margin-bottom: 2rem;
    }
</style>

---
layout: two-cols
---

# Ruritage

Rural regeneration through heritage

This project gave me the opportunity to work in a multidisciplinary team that
involves various professionals from different Academias and companies in
Europe. My tasks were related to web programming and API integration

> Tamborrino, R., Dinler, M., Patti, E., Aliberti, A., Orlando, M., De Luca,
> C., ... & Pavlova, I. (2022). Engaging Users in Resource Ecosystem Building
> for Local Heritage-Led Knowledge. Sustainability

> Tamborrino, R., Patti, E., Aliberti, A., Dinler, M., Orlando, M., de Luca,
> C., ... & Pavlova, I. (2022). A resources ecosystem for digital and
> heritage-led holistic knowledge in rural regeneration. Journal of Cultural
> Heritage

::right::

<img src="/assets/ruritage1.png" style="margin:auto;max-width:20vw">
<img src="/assets/ruritage2.png" style="margin:auto;max-width:20vw">

<style>
blockquote{
    font-size:xx-small;
width: 20vw;
margin-top:2rem
    }
</style>

---

# Publication

<div class="publications">

- [J] **A Novel Internet-of-Things Infrastructure to Support Self-Healing Distribution Systems /** Estebsari, Abouzar; Orlando, Matteo; Pons, Enrico; Acquaviva, Andrea; Patti, Edoardo. - ELETTRONICO. - (2018), pp. 1-6. ((Intervento presentato al  convegno International Conference on Smart Energy Systems and Technologies (SEST 2018) tenutosi a Sevilla, Spain nel 10-12 September 2018 [10.1109/SEST.2018.8495717].
- [J] **Engaging Users in Resource Ecosystem Building for Local Heritage-Led Knowledge /** Tamborrino, Rosa Rita Maria; Dinler, M.; Patti, E.; Aliberti, A.; Orlando, M.; De Luca, C.; Tondelli, S.; Amirzada, Z.; Pavlova, I.. - In: SUSTAINABILITY. - ISSN 2071-1050. - ELETTRONICO. - 14:8(2022), p. 4575. [10.3390/su14084575]
- [J] **A Resources Ecosystem for digital and heritage-led holistic knowledge in rural regeneration /** Tamborrino, Rosa Rita Maria; Patti, Edoardo; Aliberti, Alessandro; Dinler, Mesut; Orlando, Matteo; de Luca, Claudia; Tondelli, Simona; Barrientos, Francisco; Martin, John; Cunha, Lu??s F. M.; Stam, Andries; Nales, Aad; Egusquiza, Aitziber; Amirzada, Zahra; Pavlova, Irina. - In: JOURNAL OF CULTURAL HERITAGE. - ISSN 1778-3674. - 57:(2022), pp. 265-275. [10.1016/j.culher.2022.09.012]
- [C] **Optimal Configuration and Placement of PV Systems in Building Roofs with Cost Analysis /** Orlando, Matteo; Bottaccioli, Lorenzo; Patti, Edoardo; Macii, Enrico; Vinco, Sara; Poncino, Massimo. - (2020), pp. 1411-1416. ((Intervento presentato al  convegno 2020 IEEE International Computer Software and Applications Conference (COMPSAC) tenutosi a Madrid, Spain nel 13-17 July 2020 [10.1109/COMPSAC48688.2020.00-58].
- [C] **Design of District-level Photovoltaic Installations for Optimal Power Production and Economic Benefit /** Orlando, Matteo; Bottaccioli, Lorenzo; Vinco, Sara; Macii, Enrico; Poncino, Massimo; Patti, Edoardo. - (2021). ((Intervento presentato al  convegno IEEE International Computer Software and Applications Conference (COMPSAC) tenutosi a Virtual Conference (due to Covid-19) nel July 12-16, 2021 [10.1109/COMPSAC51774.2021.00283].
- [C] **A Smart Meter Infrastructure for Smart Grid IoT Applications /** Orlando, Matteo; Estebsari, Abouzar; Pons, Enrico; Pau, Marco; Quer, Stefano; Poncino, Massimo; Bottaccioli, Lorenzo; Patti, Edoardo. - In: IEEE INTERNET OF THINGS JOURNAL. - ISSN 2327-4662. - STAMPA. - 9:14(2022), pp. 12529-12541. [10.1109/JIOT.2021.3137596]

</div>

<style>
.publications{
  font-size: 0.75rem;
  line-height: 1.5rem;
  margin-top: 1rem;
  margin-bottom: 1rem;
}
</style>

