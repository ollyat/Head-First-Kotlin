<div>
  <p><h1>�������� Kotlin �� ����� Head First Kotlin<img src="screenshots/name_book.jpeg" width="150" align="right"> </h1>������ ����������� ������������ ����� ������������ ������� �� ����� �������� ����� ���������������� Kotlin �� ����� Head First Kotlin.</p>
</div>


����������:
---
- [x] [����� 1. ������ ����. �� ����� �������](#�����_1._������_����._��_�����_�������)   
- [������:](chapter-1)
  - [����������� � ���������](chapter-1/MyFirstApp)
  - [����� ������������](chapter-1/MySecondApp)
- [x] [����� 2. ������� ���� � ����������. �� ����� ����������](#�����_2._�������_����_�_����������._��_�����_����������) 
- [������:](chapter-2)
  - [Phrase-O-Matic](chapter-2/PhraseOMatic)
  - [����� ������������](chapter-2/CompilerApp2)
  - [����������� � ���������](chapter-2/MagnetsApp2)
- [x] [����� 3. �������. �� ��������� main](#�����_3._�������._��_���������_main)
- [������:](chapter-3)   
  - [����������� � ���������](chapter-3/MagnetsApp3)
  - [����� ������������](chapter-3/CompilerApp3)
  - [� ��������](chapter-3/NearPool)
  - [����  ������-�������-������](chapter-3/RockPaperScissors)
- [x] [����� 4. ������ � �������. ������� �����](#�����_4._������_�_�������._�������_�����)
- [������:](chapter-4)
  - [���������� Songs](chapter-4/Songs) 
  - [����������� � ���������](chapter-4/MagnetsApp4)
  - [����� ������������](chapter-4/CompilerApp4)
  - [���������� Dogs](chapter-4/Dongs)
  - [� ��������](chapter-4/NearPoolApp4) 
- [ ] ��������� � �����������. ������������ 
- [ ] ����������� ������ � ����������. �������� � ������������ 
- [ ] ������ ������. ������ � ������� 
- [ ] Null � ����������. � ������� � ����������� 
- [ ] ���������. ������� ������� ����� 
- [ ] ���������. �� ������ ���� ���� ���� ����� 
- [ ] ������-��������� � ������� ������� �������. ��������� ���� ��� ������ 
- [ ] ���������� ������� ������� �������. ����������� ����������� 
- [ ] ���������� I. �����������. ������������ ������ 
- [ ] ���������� II. ������������. ��� ��� ��������� 
- [ ] ���������� III. �������. ���-10 ���, ������� �� �� �����������

## �������� �������
### <a name="�����_1._������_����._��_�����_�������"></a> ����� 1. ������ ����. �� ����� �������

- �������� ����� var ���������� ����������, �������� ������� ����� **����������**;
- �������� ����� val ���������� ����������, �������� ������� �������� **����������**;
- println ��������� ����� ������ ����� ������, � print ���������� ����� � ��� �� ������. 

#### <a name="�������_����_�_����������._��_�����_����������"></a> ������� ���� � ����������. �� ����� ����������

��� | ������������ | ���� | �������� �������� |
----|------|-------------------|-------------------|
������������� | Byte | 8 ����� | �128 �� 127 |
������������� | Short | 16 ����� | �32768 �� 32767 |
������������� | Int | 32 ���� | �2147483648 �� 2147483647 |
������������� | Long | 64 ���� | �huge �� (huge - 1) |
� ��������� ������ |  Float | 32 ���� | -3.4*1038 �� 3.4*1038 |
� ��������� ������ |  Double | 64 ���� | �5.0*10-324 �� �1.7*10308 |
���������� | Boolean | - | true ���  false |
������� � ������ | Char | 16 ����� | 1 ������ |
������� � ������ | String | - | ������� ��������, ������������ � ������� |

- ���������� ���������� � ����� ��������� ����, �������� ���: var smallNum: Short;
- � ���������� �������� ������ �� ������;
- �������������� ���������� �� ������ ���� � ������, ���������� ��������� �������: var z: Long = **x.toLong()**;
- ������� ��������� �������� arrayOf(). �������� var myArray = arrayOf(1, 2, 3). ��� ��������� ������� ������� ������������ �������: myArray.size;
- Math.random() ���������� ��������� ����� � ��������� �� 0 �� (�����) 1;
- ����� ����������� ���� ������� var myArray: Array<Byte> = arrayOf(1, 2, 3);
- ��� �������� val ����� ��������� ���������� � �������.

### <a name="�����_2._�������._��_���������_main"></a> ����� 2. �������. �� ��������� main

- �������� ������� �������� ��������� �������:
```java  
fun foo(int1: Int, int2: Int) {
 println("Parameter is $param")
}
``` 
- ����� ������� �������� ��������� �������:
```java  
fun main(args: Array<String>) {
 foo()
}
``` 
- ������� �� ������������� ��������� �������� ��������� �������:
```java  
fun max(a: Int, b: Int): Int = if (a > b) a else b
``` 
 - ���������� ������������� ���� **Unit** ��������, ��� ������� �� ���������� ��������, � ���� ������ ����������  �������� ������������ ����;

- ���� �������� ��������� �������:
```java  
for (x in 1..10) {
 //����� ����������� ���
}
``` 
- �������� **until** ��������� ������� ����� �� �����, ���, �������������� ���� ���� ������� ����� �� 1 �� 99. �������� .. ������� ����� �� 1 �� 100
```java  
for (x in 1 until 100) println(x)
``` 
- �������� **downTo** ������� ����� � �������� �������:
```java  
for (x in 15 downTo 1) println(x)
``` 
- �������� **step** ������ ������ ����:
 ```java  
for (x in 1..100 step 2) println(x)
``` 
- ������� ��������� ������� �� ��������:
```java  
for (index in optionsParam.indices) {
    println("Index $index has item ${optionsParam[index]}")
}
``` 
- ���� ������������ ��� �������� �������. ������ �������� ������������� ���������� index, � ��� ������� � ���������� item;
```java 
for ((index, item) in optionsParam.withIndex()) {
    println("Index $index has item $item")
}
```
- ��������� �Ȓ � ���� (&& � ||)
-  Kotlin ���������� ������� toLowerCase , 
toUpperCase � capitalize ��� �������� ������, ��������������� � ������� ��������, �������� �������� ��� � ��������� 
� ��������� ��������� �����. ��������, ��������� ������� 
���������� ������� capitalize ��� �������������� ������ 
����� ������ � ������ userInput:
```java 
 userInput = userInput.capitalize()
```
#### <a name="������_�_�������._�������_�����"></a> ������ � �������. ������� �����
- ����������� ������ �������� ��������� �������:
```java
�lass Dog (val name: String, var weight: Int, val breed: String) {
    fun bark() {
               println(if (weight < 20) "Yip!" else "Woof!")
               }
}
```
- �������, ������������ 
������ ������, ���������� �������� ������. 
����� ������ ������������ ������ ������.
- ������� �������� �������� ��������� �������:
```java
var dogs = arrayOf(Dog("Fido", 70, "Mixed"), Dog("Ripper", 10, "Poodle"))
```
- ���������� ������� � ������������� ������� �� ���� 
�������� ������:
1. ���������� ����������
```java
var myDog = Dog("Fido", 70, "Mixed")
```
2. �������� �������
3. ���������� ������� � ���������� ����������� ������������ 
������.
- ����������� ����������� ��� �������� 
���������� �������. 
�� ������������ ��� 
����������� ������� 
� �� �������������.
- ������������� ������������
��� �������� ������ Dog �� �������� ����������� � ������� ������ 
� ����������� � ��� ��� � � ��������� ������:
```java
class Dog(val name: String, var weight: Int, val breed: String) {
 ...
}
```
- ������ ������ ����������
����������� ������, � ��� 
�������� � �����������
�����������
- ������ ������������� �������
��������, �� ������ �������� � ����� Dog �������� activities � 
���������������� ��� ��������, ������� �� ��������� �������� �������� �Walks�. ���, ������� ��� ������, �������� ���:
```java
class Dog(val name: String, var weight: Int, val breed: String) {
    var activities = arrayOf("Walks")
 ...
}
```
- � ����� ���������, ��� �� ������ �������� �������� ��������� 
������������ ����� ���, ��� ����������� ��� ��������. ��������, 
�������� breed ������ ��������, ����������� ������������, 
������ ������������� ������ ������, ��������������� � �������� ��������. ��� ����� ������� toUpperCase ������� ������ 
������, ��������������� � �������� ��������, ������� ����� 
������������� �������� breed:
```java
class Dog(val name: String, var weight: Int, breed_param: String) {
    var activities = arrayOf("Walks")
    val breed = breed_param.toUpperCase()
 ...
}
```
- *����� �������������*   
���� �������� ������ ������������������ ���-�� ����� �������, ��� ������� ���������, ��� ���� ��� �������� ������� ������� ������ ����������� �������������� 
���, ����� ������������ ���� ��� ��������� ������ �������������. ����� ������������� ����������� ��� ������������� ������� ����� �� ����� ������ ������������ 
� ���������� ��������� init. ��������� ���� ������������� ������� ��������� 
������ ���, ����� ���������������� ������ Dog:
```java
class Dog(val name: String, var weight: Int, breed_param: String) {
    var activities = arrayOf("Walks")
    val breed = breed_param.toUpperCase()
    init {
       println("Dog $name has been created.")
 }
 ...
}
```
- get-�����
```java
class Dog(val name: String, var weight: Int, breed_param: String) {
    var activities = arrayOf("Walks")
    val breed = breed_param.toUpperCase()
    val weightInKgs: Double
    get() = weight / 2.2
```
- set-�����
```java
class Dog(val name: String, weight_param: Int, breed_param: String) {
    var activities = arrayOf("Walks")
    val breed = breed_param.toUpperCase()
    var weight = weight_param
    set(value) {
        if (value > 0) field = value
}
```

### <a name="�����_4_���������_�_�����������._������������"></a> ����� 4 ��������� � �����������. ������������

- ������������ ������������� ������������ ����;
- �����, ���������� ����� ���, ���������� ������������, � ������, ����������� �� ����, ���������� �����������.