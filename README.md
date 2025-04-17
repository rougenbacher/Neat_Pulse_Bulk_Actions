# Neat Pulse - Bulk Action Tool

<!-- Back to top link. -->
<a id="readme-top"></a>


<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/othneildrew/Best-README-Template">
    <img src="images/neat-color.png" alt="Logo" width="402" height="116">
  </a>

  <h3 align="center">Neat Pulse :: Bulk Action Tool</h3>

  <p align="center">
    An awesome tool to bulk create rooms or update room locations in <a href="https://neat.no/pulse">Neat Pulse</a>
    <br />
    <a href="https://neatpulsebulkactions.replit.app/"><strong>Go to the tool!</strong></a>
    <br />
    <br />
    <a href="https://neatframe.zoom.us/clips/share/WigZ6lvnSROc7eUMkGdtdg">View Demo</a>
    &middot;
    <a href="https://github.com/rougenbacher/Neat_Pulse_Room_Create/issues/new?template=bug_report---.md">Report Bug</a>
    &middot;
    <a href="https://github.com/rougenbacher/Neat_Pulse_Room_Create/issues/new?template=feature_request---.md">Request Feature</a>
  </p>
</div>





<!-- ABOUT THE PROJECT -->
## About The Project
<br>

> [!IMPORTANT]
> Warning: While I work at Neat, this tool is not officially supported, endorsed, or maintained by Neat. It is an independent project created to assist Neat customers. <b>Use at your own risk.</b> Neat assumes no responsibility for any issues arising from its use. Thoroughly test in a non-production environment before making any critical or large-scale changes.
<br>
<img src="images/PulseTool.png" alt="ProductImage" width="720" height="auto">

Managing large-scale deployments of Neat devices should be seamless and efficient. This online tool was developed to simplify the process of bulk room creation and updating locations in bulk in Neat Pulse. By leveraging available APIs, this tool streamlines room provisioning and updating rooms, reducing the time and effort required for large deployments—all through a simple, user-friendly interface.

Here’s Why
* <b>Simplifies Bulk Room Creation</b> - Eliminates the 20-room manual creation limit by enabling CSV uploads.
* <b>Reduces Manual Location Changes</b> - Eliminates the need to go room by room to update locations for rooms that have been bulk uploaded.
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
  <li>An API Key with Read and Write Access</li>
  <li>Your Organization ID</li>
  <li>Region(s) and location(s) created in your Pulse tenant.</li>
  <li>List of room names that you would like to create.</li>
</ul>


<!-- USAGE EXAMPLES -->
## Bulk Room Creation
<ol>
  <li><strong>Set Up Locations</strong>
    <ul>
      <li>Create necessary Regions/Locations in Neat Pulse. Rooms without a location will be assigned to "Unassigned" and must be updated manually or with location update feature of tool.</li>
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
      <li><b>For large number of rooms, it will look as though nothing is happening but the app takes some time to make the changes so be patient and dont' close or reload the page.</b>
<br></li>
      <li>Click *Choose file* to select your populated CSV. Note: Rooms without a location will be assigned to "Unassigned" and must be updated manually.</li>
      <li>Click *Create Rooms*. This will create new rooms in the appropriate locations. Once completed you will see the status of each room along with its enrollment code.  You can write these down or just click *Download CSV* to get an updated CSV populated with enrollment codes.</li>
    </ul>
  </li>
  <li><strong>Delete API Key</strong>
    <ul>
      <li>As this API key wont be used for a continuing integration, it is best practice to delete your API Key in Neat Pulse. Do this by going to *Settings > API Keys*.  Then click the pencil at the right of the API key being used and click *Delete API Key* from the pop-up dialog box.</li>
    </ul>
  </li>
</ol>

## Bulk Location Update
<ol>
  <li><strong>Set Up Locations</strong>
    <ul>
      <li>Create necessary Regions/Locations in Neat Pulse. You will need these locations in order to assign them to rooms in your tenant.</li>
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
      <li>Navigate to the <a href="https://neatpulsebulkactions.replit.app/update-locations">Bulk Location Update Tool</a></li>
      <li>Enter your API Key and press *Set API Key*</li>
      <li>Enter your Organization ID and press *Set Org ID*</li>
    </ul>
  </li>
  <li><strong>Get Location IDs</strong>
    <ul>
      <li>Press the *Get Locations* button to get location IDs. Make sure to note these as they'll be needed in the next step.</li>
    </ul>
  </li>
  <li><strong>Get Rooms</strong>
    <ul>
      <li>Press the *Get Rooms* button to get a list of all rooms in your organization with their current locations.  Click the *Download Updated CSV* button to get a CSV with all rooms and  their current locations</li>
    </ul>
  </li>
  <li><strong>Update CSV</strong>
    <ul>
      <li>Update CSV by removing rooms that don't require a location update and update the location ID for rooms that you want to update the location for.  *Note: You only need to update the location ID.  You can leave the Location field as unassigned.*</li>
    </ul>
  </li>
  <li><strong>Update Locations</strong>
    <ul>
      <li>Click *Choose file* to select your updated CSV.</li>
      <li>Click *Update Locations*. This will update the locations of the rooms in the CSV. Once completed you will see the status of each room's location update.</li>
    </ul>
  </li>
  <li><strong>Delete API Key</strong>
    <ul>
      <li>As this API key wont be used for a continuing integration, it is best practice to delete your API Key in Neat Pulse. Do this by going to *Settings > API Keys*.  Then click the pencil at the right of the API key being used and click *Delete API Key* from the pop-up dialog box.</li>
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

Project Link: [https://github.com/rougenbacher/Neat_Pulse_Bulk_Actions](https://github.com/rougenbacher/Neat_Pulse_Bulk_Actions)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

