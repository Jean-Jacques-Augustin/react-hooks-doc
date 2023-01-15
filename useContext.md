# React.UseContext

useContext est un autre hook React qui permet de partager des données entre des composants qui ne sont pas directement liés dans l'arbre de composants. Il fonctionne en combinaison avec le contexte global de React, qui est créé en utilisant la fonction createContext.

### Exemple :
```` js
import React, { createContext, useContext } from 'react';

//Création d'un contexte pour partager la variable de thème
const ThemeContext = createContext('light');

// Composant qui utilise le contexte
function Button() {
const theme = useContext(ThemeContext);

return <button style={{ background: theme }}>I am a button</button>;
}

// Composant qui fourni le contexte
function App() {
const [theme, setTheme] = useState('light');



{{
    get => user, admin => 
}}

return (
<ThemeContext.Provider value={theme}>
<h1>Le thème actuel est {theme}</h1>
<button onClick={() => setTheme('dark')}>Dark Theme</button>
<button onClick={() => setTheme('light')}>Light Theme</button>
<br />
<Button />
</ThemeContext.Provider>
);
}

export default App;
````