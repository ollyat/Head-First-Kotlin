# � ��������

�������� �� �������� ��������� ���� 
� ���������� �� � ������ ������� 
������� printResult. ������ 
�������� ����� �������������� 
������ ���� ���; ������������ 
��� ��������� �� �����������. 
���� ������: ������� ��������, 
��������� ������������� � �����, 
� ��������, ��� �� �������.

```java  
fun printResult(userChoice: String, gameChoice: String) {
    val result: String
    // ���������� ���������
    if (userChoice ... gameChoice) result = "Tie!"
    else if ((userChoice ... "Rock" ... gameChoice ... "Scissors")
            (userChoice ... "Paper" ... gameChoice ... "Rock")
            (userChoice ... "Scissors" ... gameChoice ... "Paper")) result = "You win!"
    else result = "You lose!"
    //������� ���������
    println("You chose $userChoice. I chose $gameChoice. $result")
}
``` 
![](https://github.com/Oljua/Head-First-Kotlin/blob/main/screenshots/TaskNearPool.png)