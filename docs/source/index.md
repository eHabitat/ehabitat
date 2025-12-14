---
html_theme.sidebar_secondary.remove:
sd_hide_title: true
---

<!-- CSS overrides on the homepage only -->
<style>
/* Adjusting the content width on homepage */
.bd-main .bd-content .bd-article-container {
  max-width: 70rem; /* Increase homepage width from 60rem to 70rem */
}

/* Add extra padding to sections */
article.bd-article section {
  padding: 3rem 0 7rem;
}

/* Override all h1 headers except for the hidden ones */
h1:not(.sd-d-none) {
  font-weight: bold;
  font-size: 48px;
  text-align: center;
  margin-bottom: 4rem;
}

/* Override all h3 headers except those in the hero section */
#hero h3 {
  font-weight: normal; /* Change h3 in hero to normal weight */
}

h3 {
  font-weight: bold;
}

/* Hero layout */
#hero {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;
  margin-bottom: 4rem;
}

#hero-left {
    max-width: 476px;
    width: 100%;
    margin: auto 0;
}

@media (max-width: 768px) {
  #hero {
    grid-template-columns: 1fr;
  }
}


</style>


(homepage)=
# eHabitat: Exploratory analysis of Energy models



```{raw} html
<div id="hero">
  <!-- Left section for title, description, and buttons -->
  <div id="hero-left">
    <h2 style="font-size: 50px; font-weight: bold; margin: 2rem auto 0;">eHabitat</h2>
    <h3 style="font-weight: normal; margin-top: 0;">
      An Interactive Framework for Energy Monitoring & Climate Awareness
    </h3>
    <p>
      eHabitat is designed to enhance the understanding of energy consumption patterns and climate-related impacts through real-time, generative time series analysis.
      <br>
      Built on PyTorch, eHabitat can be easily installed via pip.
    </p>

    <div class="homepage-button-container">
      <div class="homepage-button-container-row">
        <a href="./getting_started/index.html" class="homepage-button primary-button">Get Started</a>
        <a href="./archive/index.html" class="homepage-button secondary-button">Archive</a>
      </div>

      <div class="homepage-button-container-row">
        <a href="./archive/" class="homepage-button-link">
          See Archive Reference
          <svg class="svg-icon" viewBox="0 0 20 20">
            <path fill="none" d="M1.729,9.212h14.656l-4.184-4.184..." />
          </svg>
        </a>
      </div>
    </div>
  </div>

  <div id="hero-right">
    <img src="_static/images/ehabitat_logo.svg" alt="eHabitat Logo" />
  </div>
</div>


### eHabitat ```Archive```

<table id="customers">
  <thead>
    <tr>
      <th>Dataset</th>
      <th>Frequency</th>
      <th>Duration</th>
      <th>Type</th>
      <th>Location</th>
      <th>Measurements</th>
      <th>Download <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" class="bi bi-download" viewBox="0 0 16 16"> <path d="M.5 9.9a.5.5 0 0 1 .5.5v2.5a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1v-2.5a.5.5 0 0 1 1 0v2.5a2 2 0 0 1-2 2H2a2 2 0 0 1-2-2v-2.5a.5.5 0 0 1 .5-.5z"></path> <path d="M7.646 11.854a.5.5 0 0 0 .708 0l3-3a.5.5 0 0 0-.708-.708L8.5 10.293V1.5a.5.5 0 0 0-1 0v8.793L5.354 8.146a.5.5 0 1 0-.708.708l3 3z"></path> </svg> </th>
      <th>Source</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>eHabitat-ESS(Ours)</td>
      <td>1Hz</td>
      <td>6 months</td>
      <td>Residential</td>
      <td>France</td>
      <td>I, V, P, Q, S</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://eHabitattimeseries.github.io/eHabitat-timeseries/ess_datasets/index.html" target="_blank"> [1]</a> </td>
    </tr>
    <tr>
      <td>IDEAL</td>
      <td>1Hz</td>
      <td>18 months</td>
      <td>Residential</td>
      <td>UK</td>
      <td>P, S</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://datashare.ed.ac.uk/handle/10283/3647" target="_blank"> [2]</a> </td>
    </tr>
    <tr>
      <td>Enertalk</td>
      <td>15 Hz</td>
      <td>3 days</td>
      <td>Residential</td>
      <td>South Korea</td>
      <td>P, Q</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://www.nature.com/articles/s41597-019-0212-5" target="_blank"> [3]</a> </td>
    </tr>
    <tr>
      <td>LIT</td>
      <td>15 kHz</td>
      <td>30 sec</td>
      <td>Residential</td>
      <td>Brazil</td>
      <td>P, S</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://pessoal.dainf.ct.utfpr.edu.br/douglasrenaux/LIT_Dataset/" target="_blank"> [4]</a> </td>
    </tr>
    <tr>
      <td>AMPds</td>
      <td>0.1 mHz</td>
      <td>2 years</td>
      <td>Residential</td>
      <td>Canada</td>
      <td>P, S, I</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="http://ampds.org/" target="_blank"> [5]</a> </td>
    </tr>
    <tr>
      <td>COOLL</td>
      <td>100 kHz</td>
      <td>6 sec</td>
      <td>Individual appliance</td>
      <td>France</td>
      <td>I, V</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://coolldataset.github.io/" target="_blank"> [6]</a> </td>
    </tr>
    <tr>
      <td>WHITED</td>
      <td>44 kHz</td>
      <td>5 sec</td>
      <td>Individual appliance</td>
      <td>Multiple</td>
      <td>I</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://www.cs.cit.tum.de/dis/resources/whited/" target="_blank"> [7]</a> </td>
    </tr>
    <tr>
      <td>REFIT</td>
      <td>1 Hz</td>
      <td>4+ years</td>
      <td>Residential</td>
      <td>UK</td>
      <td>P</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://pureportal.strath.ac.uk/en/datasets/refit-electrical-load-measurements-cleaned" target="_blank"> [8]</a> </td>
    </tr>
    <tr>
      <td>Dataport</td>
      <td>1 Hz</td>
      <td>4+ years</td>
      <td>Residential</td>
      <td>US</td>
      <td>P, S</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://ieee-dataport.org/" target="_blank"> [9]</a> </td>
    </tr>
    <tr>
      <td>UK-DALE</td>
      <td>16 kHz</td>
      <td>2 years</td>
      <td>Residential</td>
      <td>UK</td>
      <td>I, V, P, Q, S</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://www.nature.com/articles/sdata20157" target="_blank"> [10]</a> </td>
    </tr>
    <tr>
      <td>DRED</td>
      <td>1 Hz</td>
      <td>6 months</td>
      <td>Residential</td>
      <td>Netherlands</td>
      <td>P</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://www.st.ewi.tudelft.nl/~akshay/dred/" target="_blank"> [11]</a> </td>
    </tr>
    <tr>
      <td>PLAID</td>
      <td>30 kHz</td>
      <td>5 sec</td>
      <td>Individual appliance</td>
      <td>US</td>
      <td>I, V</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://energy.duke.edu/content/plug-load-appliance-identification-dataset-plaid" target="_blank"> [12]</a> </td>
    </tr>
     <tr>
      <td>ECO</td>
      <td>1227 kHz</td>
      <td>6 sec</td>
      <td>Residential</td>
      <td>Switzerland</td>
      <td>I, V, P, pf</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://sites.google.com/view/activities-prediction-202b/project-homepage/eco-dataset" target="_blank"> [13]</a> </td>
    </tr>
     <tr>
      <td>iAWE</td>
      <td>1 Hz</td>
      <td>73 days</td>
      <td>Residential</td>
      <td>India</td>
      <td>I, V, P, Q, S, pf</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://iawe.github.io/" target="_blank"> [14]</a> </td>
    </tr>
     <tr>
      <td>Tracebase</td>
      <td>1 Hz</td>
      <td>1 day</td>
      <td>Individual appliance</td>
      <td>Germany</td>
      <td>P</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://github.com/areinhardt/tracebase" target="_blank"> [15]</a> </td>
    </tr>
     <tr>
      <td>REDD</td>
      <td>16.5 kHz</td>
      <td>19 days</td>
      <td>Residential</td>
      <td>US</td>
      <td>I, V, P</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://tokhub.github.io/dbecd/links/redd.html" target="_blank"> [16]</a> </td>
    </tr>
     <tr>
      <td>BLUED</td>
      <td>12 kHz</td>
      <td>1 week</td>
      <td>Residential</td>
      <td>US</td>
      <td>I, V</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td><a href="https://tokhub.github.io/dbecd/links/Blued.html" target="_blank"> [17]</a> </td>
    </tr>
     <tr>
      <td>Electricity AP</td>
      <td>16 mHz</td>
      <td>4 months</td>
      <td>Residential</td>
      <td>Belgium</td>
      <td>P</td>
      <td><a href="https://github.com/oublalkhalid/eHabitat/raw/main/_static/eHabitat-001145324.hdf5">HDF5 file</a></td>
      <td> <a href="https://opennetzero.org/dataset/electricity-maps" target="_blank"> [18]</a> </td>
    </tr>
  </tbody>
</table>


## Sponsors and Institutional Partners
<p style="font-weight: bold; margin-top: 0;"> With gratitude to <a href="https://www.ip-paris.fr/">Institute Polytechnique de Paris</a>, <a href="https://www.ox.ac.uk/">Oxford Institute of Mathematics</a>, OneTech TotalEnergies for generously supporting the development and maintenance of eHabitat.</p>
  
This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png