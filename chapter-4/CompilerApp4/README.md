# ����� ������������

������ ���� ���� Kotlin �� ���� �������� ������������ ������ �������� ����. ���������� ����������� 
���� �� ����� ����������� � ����������, ����� �� 
��������������� ������ �� ���� ������. ���� 
�����-�� ����� �� �������������, �� ��� �� 
�� �� ���������?

���� ���� A
```java  
class TapeDeck {
    var hasRecorder = false

    fun playTape() {
        println("Tape playing")
    }

    fun recordTape() {
        if (hasRecorder) {
            println("Tape recording")
        }
    }
}

fun main() {
    t.hasRecorder = true
    t.playTape()
    t.recordTape()
}
``` 

���� ���� B
```java  
class DVDPlayer(var hasRecorder: Boolean) {
    fun recordDVD() {
        if (hasRecorder) println("DVD recording")
    }
}

fun main() {
    val d = DVDPlayer(true)
    d.playDVD()
    d.recordDVD()
}
```