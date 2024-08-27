- [[SQL]]
```Java
public static Connection connectToDb(String dbHost, String dbPort, String dbName, String dbUser, String dbPasswd) throws SQLException{
	Connection conn = null;
	conn = DriverManager.getConnection("jdbc:postgresql://"+dbHost+":"+dbPort+"/"+ dbName, dbUser, dbPasswd);
	System.out.println("Connection to "+dbName+" is "+conn.isValid(1));
	/** possible URL-Strings:
	* dbUrl = "jdbc:postgresql:postgres" Server running on localhost at port 5432
	* dbUrl = "jdbc:postgresql://" + dbHost + "/" + dbname; -> Default port 5432
	* dbUrl = "jdbc:postgresql://" + dbHost + ":" + dbPort + "/" + dbname;
	*
	*/
	return conn;
}

public static ArrayList<String> sms_length_logging(Connection conn, ArrayList<String> content) throws SQLException {
	PreparedStatement prpStmt = conn.prepareStatement("select *...");
	ResultSet rs = prpStmt.executeQuery();
	while(rs.next()) {
		content.add(rs.getString("name")+','+rs.getString("blablabla"));
	}
	prpStmt.close();
	rs.close();
	return null;
}

private static void executeCall(Connection conn) throws SQLException {

CallableStatement stmt = conn.prepareCall("INSERT INTO javaeetodo.tag (tag_description) VALUES(?)");

stmt.setString(1, "Test");

stmt.execute();

stmt.close();

}
```
