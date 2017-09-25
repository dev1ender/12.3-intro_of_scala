# Assignment 12.3

# Task1 : print the numbers where the corresponding string length is 4

val List1 = List((1,"alpha"),(2,"beta"),(3,"gamnna"),(4,"zeta"),(5,"omega"))
List1.foreach(s=> if(s._2.length == 4) println (s._1))


# Task2 : average of all numbers, where the corresponding string contains alphabet ‘m’
or alphabet ‘z’
val filterList = List1.filter(s=>s._2.contains("m") || s._2.contains("z"))
val mapList1 = filterList.map(s=>s._1)
val sum = mapList1.foldLeft(0)((x,y)=>x+y)
val count = mapList1.length
val avg = sum/count
