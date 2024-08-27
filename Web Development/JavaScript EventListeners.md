- [[DOM Document Object Model]]
- [[JavaScript]]
```JavaScript
document.querySelector("button").addEventListener("click", handleClick);

function handleClick() {
	alert("I got clicked")
}

document.querySelector("button").addEventListener("click", function () {
	alert("I got clicked")
});

```