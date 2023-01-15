# React.useState

React Hooks est une fonctionnalité introduite par Facebook dans React 16.8 qui permet aux développeurs de gérer l'état et les effets de bord de leurs composants React sans utiliser de classes.


### Exmeple

```` js
import React, { useState } from 'react';

function Counter() {
const [count, setCount] = useState(0);

return (
<>
<p>Le compteur est actuellement à {count}</p>
<button onClick={() => setCount(count + 1)}>Incrémenter</button>
<button onClick={() => setCount(count - 1)}>Décrémenter</button>
</>
);
}

export default Counter;
````