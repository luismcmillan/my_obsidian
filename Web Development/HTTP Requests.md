- [[Express]]
```JavaScript
app.get("/",(req, res) => { //localhost:3000/
	res.send("<h1>Home Page</h1>")
})

app.get("/about",(req, res) => { //localhost:3000/
	res.send("<h1>About Me</h1>")
})

app.post("/user/angela",(req, res) => { //localhost:3000/
	res.sendStatus(200);
})

app.put("/user/angela",(req, res) => { //localhost:3000/
	res.sendStatus(200);
})

app.patch("/user/angela",(req, res) => { //localhost:3000/
	res.sendStatus(200);
})

app.delete("/user/angela",(req, res) => { //localhost:3000/
	res.sendStatus(200);
})
```