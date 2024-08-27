[[JavaScript]]
[[CDN]]
```HTML
<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
```

```HTML
<!DOCTYPE html>
<html>
	<head>
		<title>Page Title</title>
		<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.3.1/jquery.min.js"></script>
	</head>
														#Inline
	<body onload="alert('Hello')"> 
	
		<h1>My First Heading</h1>
		<p>My first paragraph.</p>
														#Internal
		<script type="text/javascript"> 
			alert("Hello");
		</script>
														#External 
		<script src"index.js" charset="utf-8"></script>
	
	</body>
</html>
```

![[jQuery ready]]


![[jQuery Selecting Elements]]

![[jQuery Manipulating Styles]]

![[jQuery Manipulating Text]]

![[jQuery Manipulating  Attributes]]

![[jQuery Event Listeners]]

![[jQuery Adding and Removing Elements]]
```Javascript
document.querySelector("h1")
//vs
jQuery("h1")
//vs
$("h1")
```