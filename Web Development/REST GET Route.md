![[NPM Server Foundation]]

```JavaScript
app.get("/random", (req, res) => {
	const randomIndex = ...
	res.json(randomIndex)
})


app.get("/jokes/:id", (req, res) => {
	const id = parseInt(req.params.id);
	const foundJoke = jokes.find((joke) => joke.id === id); // === compares value AND TYPE
	res.json(foundJoke);
});

app.get("/filter", (req, res) => {
	const type = req.query.type;
	const filteredActivities = jokes.filter((joke) => joke.jokeType === type);
	res.json(filteredActivities);
})
```