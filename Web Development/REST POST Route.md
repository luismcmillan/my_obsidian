![[NPM Server Foundation]]

```JavaScript
app.post("/jokes", (req, res) => {
	const newJoke = {
		id: jokes.length + 1,
		jokeText: req.body.text,  //Klappt wegen Middleware bodyParser
		jokeType: req.body.type,
	};
	jokes.push(newJoke);
	console.log(jokes.slice(-1))
	res.json(newJoke)
})
```