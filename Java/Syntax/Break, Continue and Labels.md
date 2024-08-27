[[Java Syntax]]
```Java


int x = 0;
while (true){
	if(i == 10){
		break;
	}
}

for(int i = 0; i < 100; i++){
	if(k % 7 == 0){
		continue;
	}
	System.out.println(i+ "is not dividible by 7");
}

outer_label:
while(true) {
	int z = 0;
	while(true){
		if(z >= 10){
			break outer_label;
		} else {
			System.out.println(z++);
		}
	}
}


```