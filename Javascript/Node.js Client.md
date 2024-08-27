[[Express]]
[[JavaScript]]
```Javascript
fetch('http://localhost:3000/') 
.then(response => { if (!response.ok) 
	{ 
		throw new Error('Netzwerkantwort war nicht ok'); 
	} 
		return response.json(); 
	}).then(data => { console.log('Erhaltene Daten:', data); // Verarbeiten Sie die Daten weiter })
	.catch(error => { 
		console.error('Es gab ein Problem mit Ihrer Fetch-Operation:', error); });
```