# EPIC
The EPIC API provides information on the daily imagery collected by DSCOVR's Earth Polychromatic Imaging Camera (EPIC) instrument. Uniquely positioned at the Earth-Sun Lagrange point, EPIC provides full disc imagery of the Earth and captures unique perspectives of certain astronomical events such as lunar transits using a 2048x2048 pixel CCD (Charge Coupled Device) detector coupled to a 30-cm aperture Cassegrain telescope.

Image metadata and key information are provided by the JSON API and can be requested by date and for the most recent available date. A listing of all available dates can also be retrieved via the API for more granular control.

Development of the EPIC API began in 2015, and is supported by the web development team for the Laboratory for Atmospheres in the Earth Sciences Division of the Goddard Space Flight Center. More information regarding the API and retrieval of the imagery for download can be found on the EPIC website.

## Retrievable Metadata
The following information is available for every image in the collection:

- Image [name]
- Date
- Caption
- centroid_coordinates
- dscovr_j2000_position
- lunar_j2000_position
- sun_j2000_position
- attitude_quaternions

Example Image: <br>

<br>

Querying by Date:
| Parameter              | Type         | Default                   | Description                                                                                       |
|------------------------|--------------|---------------------------|---------------------------------------------------------------------------------------------------|
| natural                | string       | Most Recent Natural Color | Metadata on the most recent date of natural color imagery.                                         |
| natural/date           | YYYY-MM-DD   | Most Recent Available      | Metadata for natural color imagery available for a given date.                                     |
| natural/all            | string       | Dates for Natural Color    | A listing of all dates with available natural color imagery.                                       |
| natural/available      | string       | Dates for Natural Color    | Alternate listing of all dates with available natural color imagery.                                |
| enhanced               | string       | Most Recent Enhanced Color| Metadata on the most recent date of enhanced color imagery.                                         |
| enhanced/date          | YYYY-MM-DD   | Most Recent Available      | Metadata for enhanced color imagery for a given date.                                               |
| enhanced/all           | string       | Dates for Enhanced Imagery  | A listing of all dates with available enhanced color imagery.                                       |
| enhanced/available     | string       | Dates for Enhanced Imagery  | Alternate listing of all dates with available enhanced color imagery.                                |
| api_key                | string       | DEMO_KEY                  | API key from api.nasa.gov for expanded usage.                                                      |
