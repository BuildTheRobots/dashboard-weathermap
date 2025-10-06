# Live Weather Map Dashboard

This project is a single-page, dynamic weather map dashboard designed for a Network Operations Center (NOC) or for weather enthusiasts. It provides a flexible and customizable interface for monitoring multiple weather maps simultaneously.

## Features

*   **Dual Map Carousels:** Display two independent columns of weather maps, each with its own configurable carousel.
*   **Customizable Map Selection:** Choose from a wide variety of weather map layers, including rain, wind, temperature, cloud cover, and more.
*   **Configurable Rotation Interval:** Set the rotation speed for each carousel independently.
*   **Per-Map Hold Time:** Override the default interval for specific maps to keep them on screen for a longer or shorter duration.
*   **Live UK Weather Warnings:** A dedicated panel displays the latest weather warnings from the Met Office.
*   **Tropospheric Ducting Forecast:** Includes a view of the latest tropospheric ducting forecast map.
*   **Persistent Settings:** All your settings are saved locally in your browser, so your dashboard is always configured the way you left it.
*   **Clean, Modern UI:** Built with Tailwind CSS for a clean and responsive user interface.

## Technology

*   **HTML/CSS/JavaScript:** The application is built with standard web technologies.
*   **Tailwind CSS:** Used for styling the user interface.
*   **Ventusky:** Weather map iframes are embedded from Ventusky.
*   **Met Office:** Weather warning data is sourced from the Met Office's public RSS feed.
*   **DX Info Centre:** The Tropospheric Ducting map is sourced from dxinfocentre.com.

## Deployment

This is a single HTML file application that can be hosted on any static web hosting service, including GitHub Pages.

## External Resources & Acknowledgements

This dashboard relies on several excellent external services to provide its data.

### Ventusky

The core weather map visuals are provided by [**Ventusky**](https://www.ventusky.com/). We are grateful that they offer a highly usable, completely free, no-signup-required service for embedding their maps.

*Note: As the maps are embedded via an `<iframe>`, we cannot easily customize the Points of Interest (POIs) or fully control the frame's content. Future development may explore other alternatives if more advanced features are required.*

### Met Office

The UK Weather Warnings are sourced from the **Met Office**. The preferred API-based data feed is currently unavailable to new applicants as the service is being retired. As a fallback, this dashboard uses the public RSS feed. To bypass browser CORS (Cross-Origin Resource Sharing) restrictions when fetching the RSS feed, the data is routed through the free, public `allorigins.win` proxy.

### Tropospheric Ducting Forecast

The tropospheric ducting forecast map is provided by William Hepburn's **DX Info Centre**. A huge thank you for this, as it appears to be the only publicly available service offering this specific forecast map.

*Disclaimer: The method used to display this map (cropping a larger image) is a bit cheeky and may be against their terms of service. As this dashboard is for personal, non-commercial use to monitor conditions that cause me headaches, it is included here until a more officially supported alternative can be found.*

## Vibe to the max

### Google Gemini

There is an awful lot of vibe involved in the writing of this project. I hated writing HTML in the 90's, complicating matters with ECMA and css has not increased my enjoyment since. Not to underplay the amount of back and forth required to get to this point, but hot-damn, late 2025 LLMs are one hell of a drug. 

*"And I, for one, welcome our new AI overlords. I'd like to remind them as a trusted network operator, I can be helpful in rounding up packets to quantise in their underground inference caves."*