# Weather Explorer

A responsive weather app built with HTML, CSS, and vanilla JavaScript. Prepared with AI assistance as a learning project.

## Run locally

Download the repository, open a terminal in its folder, and run:

```sh
python -m http.server 8000
```

Then open http://localhost:8000. On Windows, use `py -m http.server 8000` if `python` is unavailable.

## Features

- Search cities and choose among matching locations
- Current temperature, feels-like temperature, humidity, and wind
- Five-day high/low forecast
- Loading, no-results, and network-error messages
- Cancels outdated requests
- Responsive design and accessible status updates

## How it works

`app.js` searches the Open-Meteo geocoding API, then uses the selected coordinates to fetch weather. It creates page elements with `textContent`, avoiding HTML injection from search results. `AbortController` cancels outdated requests.

## Data and limits

Weather model data supplied by [Open-Meteo](https://open-meteo.com/), with [API documentation](https://open-meteo.com/en/docs) and [geocoding documentation](https://open-meteo.com/en/docs/geocoding-api). No API key is required for the non-commercial endpoint. Internet access is required. Current conditions are model estimates; this app is not an emergency-alert service. Review the provider's terms before commercial use.

## Practice ideas

Add Celsius/Fahrenheit switching, saved favourite cities, or an hourly chart. Understand and adapt the code before describing it in a job interview.
