# APOD (Astronomy Picture of the Day):

One of the most popular websites at NASA is the Astronomy Picture of the Day. This website is one of the most popular websites across all federal agencies. It has the popular appeal of a Justin Bieber video. This endpoint structures the APOD imagery and associated metadata to be repurposed for other applications. In addition, if the concept_tags parameter is set to True, then keywords derived from the image explanation are returned. These keywords could be used as auto-generated hashtags for Twitter or Instagram feeds, but generally help with the discoverability of relevant imagery.

The full documentation for this API can be found in the APOD API GitHub repository.

Example Image: Date - 12/04/2023
Image Name: Plane Crossing Crescent Moon
Image Credit: Juned Patel
![image](https://github.com/ArnavKucheriya/NASA_API/assets/114359370/1dad652f-b6d3-4c51-bacc-9d6c2e4f8ea0)
Image Description: No, the Moon is not a bow, and no, it did not shoot out a plane like an arrow. What is pictured is a chance superposition. The plane's contrail would normally appear white, but the large volume of air toward the rising Sun preferentially knocked away blue light, not only making the sky blue, but giving the reflected trail a bright red hue. Far in the distance, well behind the plane, the crescent Moon also appears slightly reddened. Captured early last month from Bolton, UK, the featured image was taken so soon after sunrise that the plane was sunlit from below, as was its contrail. Within minutes, unfortunately, the impromptu sky show ended. The plane moved out of sight. The Moon kept rising but became harder to see through a brightening sky. And the contrail gradually dispersed.

## HTTP Request
GET https://api.nasa.gov/planetary/apod
concept_tags are now disabled in this service. Also, an optional return parameter copyright is returned if the image is not in the public domain.

## Query Parameters:

| Parameter   | Type         | Default    | Description                                                                                               |
|-------------|--------------|------------|-----------------------------------------------------------------------------------------------------------|
| date        | YYYY-MM-DD   | today      | The date of the APOD image to retrieve                                                                    |
| start_date  | YYYY-MM-DD   | none       | The start of a date range, when requesting date for a range of dates. Cannot be used with date.          |
| end_date    | YYYY-MM-DD   | today      | The end of the date range, when used with start_date.                                                      |
| count       | int          | none       | If this is specified then count randomly chosen images will be returned. Cannot be used with date or start_date and end_date. |
| thumbs      | bool         | False      | Return the URL of video thumbnail. If an APOD is not a video, this parameter is ignored.                   |
| api_key     | string       | DEMO_KEY   | api.nasa.gov key for expanded usage                                                                      |
