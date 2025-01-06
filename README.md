# US States Median Income Visualization

This project visualizes the median income of US states using a web-based interactive map. The map is created using the Leaflet.js library and displays income data for each state.

## Project Structure

- `index.html`: The main HTML file that sets up and displays the interactive map.
- `us-states.js`: Contains the GeoJSON data for US states, including their median income.
- `densityscript.js`: Contains additional data and scripts related to the project.
- `style.css`: Contains styles for the project.
- `.vscode/settings.json`: Configuration for the VS Code Live Server extension.

## index.html

The `index.html` file includes the following key components:

1. **HTML Head**:
    - Includes meta tags for character set and viewport settings.
    - Links to the Leaflet.js CSS and JavaScript libraries.
    - Includes custom styles for the map and other elements.

2. **Body**:
    - Contains a `div` with the id `map` where the Leaflet map will be rendered.
    - Includes a script tag to load the `us-states.js` file.

3. **JavaScript**:
    - Initializes the Leaflet map and sets the view to the center of the US.
    - Adds OpenStreetMap tiles to the map.
    - Defines a control to display state information on hover.
    - Defines a function `getColor` to determine the color of each state based on its median income.
    - Defines a function `style` to set the style for each state feature.
    - Defines functions `highlightFeature`, `resetHighlight`, and `zoomToFeature` to handle user interactions with the map.
    - Adds the GeoJSON data from `us-states.js` to the map with the defined styles and interaction handlers.
    - Adds a legend to the map to explain the color coding of the states.

## Usage

To view the project, open the `index.html` file in a web browser. The map will display the US states with colors representing their median income. Hovering over a state will display its name and median income. Clicking on a state will zoom in on that state.

## Dependencies

- [Leaflet.js](https://leafletjs.com/): A JavaScript library for interactive maps.
- [OpenStreetMap](https://www.openstreetmap.org/): Provides the map tiles used in the project.

## License

This project is licensed under the MIT License.
