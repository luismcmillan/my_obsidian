[[Maps]]
```Java
Map map = new HashMap();
MyDate birthday = new MyDate(1,1,1996);
MyDate anniv = new MyDate(1,1,1996);
MyDate taxday = new MyDate(1,1,1996);
map.put("anniversary", anniv);
map.put("birthday", bithday);
map.put("taxday", taxDay);
MaDate d = (MyDate)map.get("birthday");
map.remove("taxday");

map.keySet() //return key objects in a map
map.values() //return value objects in a map
```