![[NPM Server Foundation]]

```JavaScript
app.patch("/jokes/:id", (req, res) => {
	const id = parseInt(req.params.id);
	const existingJoke = jokes.find((joke) => joke.id === id);
	const replacementJoke = {
		id: id,
		jokeText: req.body.text || existingJoke.jokeText,  //Klappt wegen Middleware bodyParser
		jokeType: req.body.type || existingJoke.jokeType,
	};
	const searchIndex = jokes.findIndex((joke) => joke.id === id);
	jokes[searchIndex] = replacementJoke;
	res.json(replacementJoke)
})
