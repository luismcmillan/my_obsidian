```JavaScript
import express from "express";
import bodyParser from "body-parser";

const app = express();
const port = 3000;
const masterkey = "lksfs-fnvök-dsnvöa-dlmvd-aälvm"
app.use(bodyParser.urlencoded({ extended: true})); //Middleware

app.listen(port, () => {
	console.log('Server running on port +${port}.');
});
```