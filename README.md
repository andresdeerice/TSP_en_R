Este tipo de problemas conocidos como TSP (travelling salesman problem), buscamos minimizar el recorrido del viajante, siendo que este debe pasar por todas las ciudades y volver a la primera.

El recorrido eficiente puede encontrase mediante fuerza burta, es decir, probar todas los caminos posibles y elegir el más corto. Sin embargo, este método es altamente costoso en tiempo y recursos computacionales, por lo que se prefiere utilizar aproximaciones, tales como son los métodos heurísticos. Estos no proporcionan la solución óptima pero si una lo suficientemente buena.
. Nearest Neighbor Algorithm (NNA): este algortimo comienza el recorrido en una ciudad origen y va a la siguiente más cercana, sin visitar, hasta volver a la ciudad origen.
. Recursive Nearest Neighbor Algorithm (RNNA): este método es una variante del anterior, con la diferencia de que inicia el recorrido por todos los puntos origen e itera NNA, terminando seleccionando el recorrdio más corto.
. Cheapest-Link Algorithm (CLA): este consiste en ordenar las distancias entre las ciudades de menor a mayor. Se empieza por el recorrido más corto, y así sucesivamente pero con las condiciones de que 1- ) este no debe cerrar el circuito sin haber cubierto todos los puntos y 2-) cada punto no puede tener más de dos arcos. Este proceso se repite hasta que se complete la ruta.

Los paquetes de R necesarios para este ejercicio son: 'TSP', 'maps' y 'geosphere'.
