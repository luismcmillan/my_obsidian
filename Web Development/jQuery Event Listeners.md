[[JavaScript EventListeners]]
```JavaScript
$("h1").click(function(){
	$("h1").css("color", "purple")
});


//bei mehreren Buttons ohne jQuery
for(var i = 0; i<5;i++){
	document.querySelectorAll("button")[i].addEventListener("click", function(){
		document.querySelector("h1").style.color = "purple"
	});
}
//Mit jQuery
$("button").click(function() {
	$("h1").css("color", "purple");
});


$("h1").on("mouseover", function() {
	$("h1").css("color", "purple")
})
```