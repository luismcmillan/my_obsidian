```Java
public Employee(){
	super(); //LEGAL
	deptId = 281;
}

public Employee(){
	deptId = 281;
	super(); //ILLEGAL
}

public Employee(){
	deptId = 281;
	super.drive(); //LEGAL
}

public Employee(){
	deptId = 281;
	super.drive(); //LEGAL
}
```