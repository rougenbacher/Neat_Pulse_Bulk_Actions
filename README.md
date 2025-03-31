# Neat Pulse - Bulk Room Creation

<!-- Back to top link. -->
<a id="readme-top"></a>


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/neat-color.png" alt="Logo" width="402" height="116">
  </a>

  <h3 align="center">Neat Pulse :: Bulk Room Creation Tool</h3>

  <p align="center">
    An awesome tool to bulk create rooms in <a href="https://neat.no/pulse">Neat Pulse</a>
    <br />
    <a href="https://neatpulseroomcreate.replit.app/"><strong>Go to the tool!</strong></a>
    <br />
    <br />
    <a href="https://github.com/othneildrew/Best-README-Template">View Demo</a>
    &middot;
    <a href="https://github.com/rougenbacher/Neat_Pulse_Room_Create/issues/new?template=bug_report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/rougenbacher/Neat_Pulse_Room_Create/issues/new?template=feature_request---.md">Request Feature</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
<br>
<img src="images/pulsetool.png" alt="ProductImage" width="720" height="auto">

Managing large-scale deployments of Neat devices should be seamless and efficient. This online tool was developed to simplify the process of bulk room creation in Neat Pulse, allowing Neat customers to upload a CSV file and generate multiple rooms at once. By leveraging available APIs, the tool streamlines room provisioning, reducing the time and effort required for large deployments—all through a simple, user-friendly interface.

Here’s Why
* <b>Simplifies Bulk Room Creation</b> - Eliminates the 20-room manual creation limit by enabling CSV uploads.
* <b>No API Knowledge Required</b> - Many enterprise customers lack the expertise to use APIs directly, so this tool provides an intuitive interface.
* <b>Faster Deployments</b> - Reduces the time and effort needed for setting up large-scale Neat Pulse environments.
* <b>Enrollment Codes in CSV Format</b> - Generates enrollment codes in the same CSV format used for room creation, making it easy to distribute and track.

Read on to get started! 

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

Follw the below steps to get started bulk enrolling devices into Neat Pulse. 

### Prerequisites

You will need the following in order to use this tool:
<ul>
  <li>An active Neat Pulse account.</li>
  <li>Pulse Plus or Pro licenses for all devices to enable API access</li>
  <li>An API Key with Read abd Write Access</li>
  <li>Your Organization ID</li>
  <li>Region(s) and location(s) created in your Pulse tenant.</li>
  <li>List of room names that you would like to create.</li>
</ul>


<!-- USAGE EXAMPLES -->
## Usage
<ol>
  <li><strong>Set Up Locations</strong>
    <ul>
      <li>Create necessary Regions/Locations in Neat Pulse. Rooms without a location will be assigned to "Unassigned" and must be updated manually.</li>
    </ul>
  </li>
  <li><strong>Get Org ID and API Key</strong>
    <ul>
      <li>In your Pulse tenat, navigate to the *Settings* tab on the left. From there copy the *Organization ID*.</li>
      <li>While still in *Settings*, click *Create API Key*. Give a descriptive name and ensure you select both *Read* and *Write* for the scope.</li>
    </ul>
  </li>
  <li><strong>Set Organization ID and API Key</strong>
    <ul>
      <li>Navigate to the <a href="https://neatpulseroomcreate.replit.app/">Bulk Room Creation Tool</a></li>
      <li>Enter your API Key and press *Set API Key*</li>
      <li>Enter your Organization ID and press *Set Org ID*</li>
    </ul>
  </li>
  <li><strong>Get Location IDs</strong>
    <ul>
      <li>Press the *Get Locations* button to get location IDs. Make sure to note these as they'll be needed in the next step.</li>
    </ul>
  </li>
  <li><strong>Download and Fill Out CSV</strong>
    <ul>
      <li>Click *Downlad CSV Template* to download a pre-populated CSV.</li>
      <li>Fill out CSV with Room Names and Location ID gathered in the previous step. Leave the *enrollment_code* column empty.</li>
    </ul>
  </li>
  <li><strong>Create Rooms</strong>
    <ul>
      <li>Click *Choose file* to select you populated CSV. Note: Rooms without a location will be assigned to "Unassigned" and must be updated manually.</li>
      <li>Click *Create Rooms*. This will create new rooms in thr appropriate locations. Once completed you will see the status of each room along with its enrollment code.  You can write these down or just click *Download CSV* to get an updated CSV populated with enrollment codes.</li>
    </ul>
  </li>
  <li><strong>Delete API Key</strong>
    <ul>
      <li>As this API key wont be used for a continuing integration, it is best practice to delete your API Key in Neat Pulse. Do this by going to *Settings > API Keys* and clicking the pencil at the right of the API key being used and click *Delete API Key* from the pop-up dialog box.</li>
    </ul>
  </li>
</ol>

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

- [ ] Add standalone Zoom Room creation
- [ ] Add ability to create Pulse Rooms and Zoom Rooms with one CSV
- [ ] Add standalone Teams Room creation (pending MSFT limitstions)
- [ ] Add ability to create Pulse Rooms and Teams Rooms with one CSV

See the [open issues](https://github.com/rougenbacher/Neat-Pulse---Bulk-Room-Create/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- CONTACT -->
## Contact

Chris Rouge - [LinkedIn](http://linkedin.com/in/chrisrouge) - rougechris@protonmail.com

Project Link: [https://github.com/rougenbacher/Pulse-Bulk-Create](https://github.com/rougenbacher/Pulse-Bulk-Create)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

