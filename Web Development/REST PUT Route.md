![[NPM Server Foundation]]

```JavaScript
app.put("/jokes/:id", (req, res) => {
	const id = parseInt(req.params.id);
	const replacementJoke = {
		id: id,
		jokeText: req.body.text,  //Klappt wegen Middleware bodyParser
		jokeType: req.body.type,
	};
	const searchIndex = jokes.findIndex((joke) => joke.id === id);
	jokes[searchIndex] = replacementJoke;
	res.json(replacementJoke)
})
