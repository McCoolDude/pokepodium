Pokemon Ranking App
This is a simple web application that allows users to select up to 10 of their favorite Pokemon, assign them points (totaling exactly 10 points across all selected Pokemon), and visualize their rankings in an interactive bar chart. The chart displays each Pokemon's sprite above its bar, with a unique sorting order: the highest-ranked Pokemon is centered, the second highest is to its left, and all subsequent Pokemon are sorted in descending order of points (then alphabetically) to the right. Users can also download their generated chart as an image.

Features
Searchable Pokemon Selection: Choose from a comprehensive list of all available Pokemon via an autocomplete search input for each of the 10 ranking slots.

Dynamic Sprite Display: As you select a Pokemon, its official sprite automatically appears next to its name.

Flexible Ranking Slots: Use as many or as few of the 10 slots as you like, as long as at least one Pokemon is selected.

Point Assignment: Assign a score from 0 to 10 to each selected Pokemon using a dropdown.

Total Points Validation: The application ensures that exactly 10 points are assigned across all selected Pokemon before generating the chart.

Dynamic Bar Chart Generation: A bar chart visually represents your rankings, with bar heights corresponding to points assigned.

Unique Chart Layout: The highest-ranked Pokemon is centered, followed by the second highest to its left, and the rest sorted descendingly (then alphabetically) to the right.

Pokemon Sprite on Chart: Each bar displays the respective Pokemon's sprite above it.

Download Chart as Image: Easily save your personalized ranking chart as a PNG image.

Responsive Design: The layout adjusts for optimal viewing on various screen sizes.

Dark Theme: The application features a dark background with white text for a modern look.

How to Use
Select Pokemon: In each of the 10 available slots, type the name of a Pokemon into the search input. Suggestions will appear as you type. Select a Pokemon by clicking on the suggestion or by typing the full name and pressing Enter/Tab.

Assign Points: Use the dropdown next to each selected Pokemon to assign points from 0 to 10.

Monitor Points: Keep an eye on the "Points Remaining" indicator. You must assign exactly 10 points across all the Pokemon you have selected.

Create Chart: Once you've assigned all 10 points and selected your Pokemon (ensuring no duplicates), click the "Create My Ranking Chart" button.

View and Download: Your custom bar chart will appear below the input section. You can then click the "Download Chart as Image" button to save it.

Technologies Used
HTML5: For the basic structure of the web page.

CSS3 (Tailwind CSS): For styling and responsive design. Tailwind CSS is loaded via a CDN.

JavaScript (ES6+): For all application logic, including data fetching, UI generation, validation, chart drawing, and image download.

PokeAPI: A free RESTful API that provides access to Pokemon data (names and sprites).

API Reference
The application uses the PokeAPI to fetch Pokemon data.

https://pokeapi.co/api/v2/pokemon?limit=10000: Used to fetch a comprehensive list of Pokemon names and their detail URLs.

https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/{id}.png: Used to construct the direct sprite URLs for efficiency and to avoid canvas tainting issues during image download.

Running Locally
To run this project on your local machine:

Save the Code: Save the provided HTML code into a file named index.html in a new folder (e.g., pokemon-ranking-app).

Open in Browser: Simply open the index.html file in your web browser. Most modern browsers will execute the embedded JavaScript and CSS directly.

Alternatively, for a more robust local development setup, you can use a simple HTTP server (e.g., Python's built-in server):

Navigate to Directory: Open your terminal or command prompt and navigate to the pokemon-ranking-app folder.

cd path/to/your/pokemon-ranking-app

Start HTTP Server:

python -m http.server 8000
# Or for Python 3:
# python3 -m http.server 8000

Access App: Open your web browser and go to http://localhost:8000.
