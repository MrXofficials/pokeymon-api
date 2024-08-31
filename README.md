

---

# Neumorphic Pokémon App 🎮✨

Welcome to the **Neumorphic Pokémon App**! This fun and interactive web app shows a random Pokémon image and its name every time you click the button, featuring a smooth and playful **Neumorphism UI** design. 🔥✨

### 🚀 Demo Site:
Check out the live demo here 👉 [Neumorphic Pokémon App](https://mrxofficials.github.io/pokeymon-api/)

## Features 💡

- **Random Pokémon**: Get a new random Pokémon with its image and name every time you click the button.
- **Neumorphic UI**: Clean, modern design with soft shadows and a 3D-like effect.
- **Sound Effects**: Enjoy interactive sound effects when clicking and hovering over buttons.
- **Responsive Design**: Looks great on all devices, from mobile to desktop.
- **Simple Animations**: Subtle animations enhance the user experience, making the UI more engaging.

## How It Works ⚙️

This app uses the **PokéAPI** to fetch random Pokémon data.

- **API Endpoint**: `https://pokeapi.co/api/v2/pokemon/`
- **Randomization**: We append a random number (between 1 and 898) to the API URL to get data for a random Pokémon.
- **Data Display**: The Pokémon's name and image are displayed after a successful API call.

### Example API Call:

```js
fetch('https://pokeapi.co/api/v2/pokemon/' + Math.floor(Math.random() * 898))
    .then(response => response.json())
    .then(data => {
        // Display the Pokémon name and image
        document.getElementById('pokemonName').textContent = data.name.toUpperCase();
        document.getElementById('pokemonImage').src = data.sprites.front_default;
    });
```

## Installation 📥

Follow these steps to run the project locally:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/pokeymon-api.git
   ```

2. **Navigate to the project folder**:
   ```bash
   cd pokeymon-api
   ```

3. **Run the app**:
   Open the `index.html` file in your browser.

## Tech Stack 🛠️

- **HTML5**: Markup for structuring the app.
- **CSS3**: Styling with Neumorphism design.
- **JavaScript**: Handling interactivity and API requests.
- **PokéAPI**: Providing Pokémon data.

## Credits 🙏

- **PokéAPI**: Special thanks to [PokéAPI](https://pokeapi.co/) for providing the Pokémon data.
- **Sound Effects**: Sounds by [Fesliyan Studios](https://www.fesliyanstudios.com).

## License 📄

This project is open-source and available under the [MIT License](LICENSE).

---

Enjoy catching random Pokémon in a neumorphic style! If you have any feedback or suggestions, feel free to open an issue. 😊

--- 
