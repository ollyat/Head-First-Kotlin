# ����� ������������

���� ��������� ��� ������ ������� Kotlin. 
���������� ����������� ���� 
�� ����� ����������� � ����������, ����� 
�� ��������������� ������ �� ���� ������. ���� �����-�� ����� �� �������������, 
�� ��� �� �� �� ���������?

���� ���� A
```java  
fun doSomething(msg: String, i: Int): Unit {
    if (i > 0) {
        var x = 0
        while (x < i) {
            println(msg)
            x += 1
        }
    }
}
``` 

���� ���� B
```java  
fun timesThree(x: Int): Int {
 x = x * 3
 return x
}
``` 

���� ���� C
```java  
fun maxValue(args: Array<Int>) {
    var max = args[0]
    var x = 1
    while (x < args.size) {
        var item = args[x]
        max = if (max >= item) max else item
        x = x + 1
    }
    return max
}
``` 