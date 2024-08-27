- [[JavaScript]]
```JavaScript
//On page script
<script type="text/javascript">  ...
</script>

//Include external JS file
<script src="filename.js"></script>

// Delay - 1 second timeout
setTimeout(function () {
}, 1000);

//Functions
function addNumbers(a, b) {
	return a + b; ;
}
x = addNumbers(1, 2);

//Edit DOM element
document.getElementById("elementID").innerHTML = "Hello World!";

//Output
console.log(a);             // write to the browser console
document.write(a);          // write to the HTML
alert(a);                   // output in an alert box
confirm("Really?");         // yes/no dialog, returns true/false depending on user click
prompt("Your age?","0");    // input dialog. Second argument is the initial value

//Comments
/* Multi line
comment */
// One line
```
