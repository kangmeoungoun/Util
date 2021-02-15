```java
String a = "select count(%s) from %s x";
String x = String.format(a , "x" , "%s");
System.out.println("x = " + x);
//x = select count(x) from %s x
String member = String.format(x , "member");
System.out.println("member = " + member);
//member = select count(x) from member 

```
