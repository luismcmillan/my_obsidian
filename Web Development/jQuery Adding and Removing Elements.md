```JavaScript
//adding
$("h1").before("<button>New</button>") //<button>New</button> <h1> Hello </h1> 
$("h1").after("<button>New</button>") //<h1> Hello </h1> <button>New</button> 
$("h1").prepend("<button>New</button>") //<h1> <button>New</button> Hello </h1>
$("h1").append("<button>New</button>") //<h1> Hello <button>New</button> </h1>
//removing
$("button").remove();
```