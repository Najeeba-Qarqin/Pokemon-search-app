# Pokemon-Search-App 🚀

## Project Description 📝

> Pokemon Search App build in HTML, CSS and javaScript it can search for pokemons from their ID or name, and free code camp certifcation project.

- Search for pokemons from their ID and name and fetch information from free code camp to the DOM.
- From this project i learned how to use javaScript in projects and javaScript and how to fetch real data.
- The style and accessibility of this project make's it stand out.

### HTML:
```html

    <div class="output">
      <div class="name-and-id">
        <span id="pokemon-name"></span>
        <span id="pokemon-id"></span>
      </div>
      <div class="size">
        <span id="weight"></span>
        <span id="height"></span>
      </div>
      <div id="sprite-container" class="sprite-container"></div>
      <div id="types"></div>
    </div>

```
### CSS:
```css

.bottom-container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 100%;
  height: 90vh;
}

table {
  width: 90%;
  margin: 30px;
}

table td,
th {
  border: 3px solid lightgray;
  padding: 6px;
  text-align: center;
  border-radius: 10px;
  width: 50%;
  background-color: orange;
}

```
### JS:
```javascript

const fetchData = async () => {
  try {
    const pokemonNameOrId = searchInput.value.toLowerCase();
    const res = await fetch(`https://pokeapi-proxy.freecodecamp.rocks/api/pokemon/${pokemonNameOrId}`);
    const data = await res.json();
    getPokemonData(data);
  } catch (err) {
    alert('Pokémon not found');
  }
};

```

## Demo 📸

![Demo](/demo.png)

## Technologies Used 🛠️

- HTML
- CSS
- JavaScript

## Features ⭐

- Building Pokemon Search App.

## Author 👩‍💻


- LinkedIn: [najeeba-qarqin](https://www.linkedin.com/in/najeeba-qarqin-5419502ab?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)
- Email: [najeebaqarqin](najeebaqarqin@gmail.com)
- GitHub: [Najeeba_Qarqin](https://github.com/Najeeba-Qarqin)
