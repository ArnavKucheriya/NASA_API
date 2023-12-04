# NASA API
Welcome to the NASA API portal. The objective of this site is to make NASA data, including imagery, eminently accessible to application developers. This catalog focuses on broadly useful and user friendly APIs and does not hold every NASA API.

Access NASA API: https://api.nasa.gov/

# Authentication
You do not need to authenticate in order to explore the NASA data. However, if you will be intensively using the APIs to, say, support a mobile application, then you should sign up for a NASA developer key.

## Web Service Rate Limits
Limits are placed on the number of API requests you may make using your API key. Rate limits may vary by service, but the defaults are:

Hourly Limit: 1,000 requests per hour
For each API key, these limits are applied across all api.nasa.gov API requests. Exceeding these limits will lead to your API key being temporarily blocked from making further requests. The block will automatically be lifted by waiting an hour. If you need higher rate limits, contact us.

## DEMO_KEY Rate Limits
In documentation examples, the special DEMO_KEY api key is used. This API key can be used for initially exploring APIs prior to signing up, but it has much lower rate limits, so you’re encouraged to signup for your own API key if you plan to use the API (signup is quick and easy). The rate limits for the DEMO_KEY are:

Hourly Limit: 30 requests per IP address per hour
Daily Limit: 50 requests per IP address per day
How Do I See My Current Usage?
Your can check your current rate limit and usage details by inspecting the X-RateLimit-Limit and X-RateLimit-Remaining HTTP headers that are returned on every API response. For example, if an API has the default hourly limit of 1,000 request, after making 2 requests, you will receive this HTTP header in the response of the second request:

X-RateLimit-Remaining: 998

The hourly counters for your API key reset on a rolling basis.

Example: If you made 500 requests at 10:15AM and 500 requests at 10:25AM, your API key would become temporarily blocked. This temporary block of your API key would cease at 11:15AM, at which point you could make 500 requests. At 11:25AM, you could then make another 500 requests.

Anyone can register for an api.nasa.gov key, which can be used to access data across federal agencies.
<<<<<<< HEAD

## APIs:
- APOD (Astronomy Picture of the Day)
- Asteroid NeoWs (Near Earth Object Web Service)
- DONKI (Space Weather Database of Notifications, Knowledge, Information)
- Earth (Significant Public Investment in Earth Observation Data)
- EONET (The Earth Observatory Natural Event Tracker)
- EPIC (Earth Polychromatic Imaging Camera)
- Exoplanet (Programmatic Access to NASA's Exoplanet Archive Database)
- GeneLab (Programmitic Interface for GeneLab's Public Data Repository Website)
- Insight (Mars Weather Service API)
- Mars Rover Photo (Image Data gathered by NASA's Curiosity)
- NASA Image and Video Library (API to access NASA's Media Library)
- TechTransfer (Patents, Software, and Tech Transfer Reports)
- Satellite Situation Centre (System to Cast Geocentric Spacecraft Location Information into Framework)
- SSD/CNEOS (Solar System Dynamics and Centre for Near-Earth Object Studies)
- Techport (API to make NASA Technology Project Data in ML Format)
- TLE API (Two Line Element Data for Earth-Orbiting Objects at Point and Time)
- Vesta/Moon/Mars Trek WMTS (A Web Map Tile Service for the Vesta, Moon, and Mars Trek Imagery Projects)
=======
>>>>>>> aee2a6f2a236a50c416a954589ab11b1d4fed991
