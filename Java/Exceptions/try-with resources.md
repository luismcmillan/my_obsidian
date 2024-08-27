[[Finally]]
```Java
try(Connection conn = DriverManager.getConnection(...)){
	//More SQL Code
} catch(SQLException) {
	//Handle exception
}
```