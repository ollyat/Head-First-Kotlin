# ����� ������������

������ ���� ���� �� ���� �������� ������������ 
������ �������� ����. ���������� ����������� ���� 
�� ����� ����������� � ����������, ����� 
�� ��������������� ������ �� ���� ������. ���� �����-�� ����� �� �������������, 
�� ��� �� �� �� ���������?

���� ���� A
```java  
fun main(args: Array<String>) {
    val hobbits = arrayOf("Frodo", "Sam", "Merry", "Pippin")
    var x = 0;
    while (x < 5) {
        println("${hobbits[x]} is a good Hobbit name")
        x = x + 1
    }
}
``` 

���� ���� B
```java  
fun main(args: Array<String>) {
    val firemen = arrayOf("Pugh", "Pugh", "Barney McGrew", "Cuthbert", "Dibble", "Grub")
    var firemanNo = 0;
    while (firemanNo < 6) {
        println("Fireman number $firemanNo is $firemen[firemanNo]")
        firemanNo = firemanNo + 1
    }
}
```