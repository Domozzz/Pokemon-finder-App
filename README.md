# Pokemon-finder-App
This code is a React component that uses the PokeAPI to search for Pokemon by name. It imports the useState and useEffect hooks from React, as well as TailSpin from react-loader-spinner. It also imports the App.css file. The component has two state variables, name and data, and two boolean variables, err and isLoading. 

The getPokemon() function is an asynchronous function that sets isLoading to true, then attempts to fetch data from the PokeAPI using the name state variable as a parameter. If successful, it sets err to false and sets data to the returned JSON object. If unsuccessful, it sets data to false and err to true. 

The useEffect hook calls getPokemon() when the component mounts and logs data in the console. The handleSubmit() function calls getPokemon() when a form submit event occurs. 

The return statement renders a div with a form for entering a Pokemon name and either an error message or loading spinner if no data was found or is being fetched respectively, or an image of the Pokemon along with its name and weight if successful.

