# ����� ������������

������ ���� ���� Kotlin �� ���� �������� 
������������ ������ �������� ����. ���������� 
����������� ���� �� ����� ����������� 
� ����������, ����� �� ��������������� 
������ �� ���� ������. ���� �����-�� 
����� �� �������������, �� ��� �� �� 
�� ���������?

���� ���� A
```java  
fun main(args: Array<String>) {
    var x = 1
    while (x < 10) {
        if (x > 3) {
            println("big x")
        }
    }
}
``` 

���� ���� B
```java  
fun main(args: Array<String>) {
    val x = 10
    while (x > 1) {
        x = x - 1
        if (x < 3) println("small x")
    }
}
``` 

���� ���� C
```java  
fun main(args: Array<String>) {
    var x = 10
    while (x > 1) {
        x = x - 1
        print(if (x < 3) "small x")
    }
}
``` 