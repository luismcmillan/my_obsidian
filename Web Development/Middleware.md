[[Express]]
```JavaScript
import express from "express";
import morgan from "morgen";

const app = express();
const port = 3000;

function logger(req, res, next){ 
	console.log("Request Method: ", req.method);
	console.log("Request URL: ", req.url);
	next(); // WICHTIG!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
}

app.use(morgan("tiny")); //use external Middleware
app.use(logger); //own Middleware

app.get("/",(req, res) => { //localhost:3000/
	res.send("<h1>Home Page</h1>")
})
```
