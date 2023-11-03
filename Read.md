


> [!第1題]
>將多行字符串，如下面的文本，拆分成單行的列表  
>提示：在換行字符處進行拆分。

```dart

void main() {
 String nation = '''
 France
 USA
 Germany
 Benin
 China
 Mexico
 Mongolia
 ''';
```


```dart
 List<String> lines = nation.split('\n');
 print(lines);
}
```

>[!Ans]
>[ France, USA, Germany, Benin, China, Mexico, Mongolia, ]
>


>[!第2題]
>
>在線上找一個表情符號來替換以下文本中的 :]

```
void main() {
  String message = "How's the Dart book going? \u{1F602}";
  print(message);
}
```


>[!Ans]
>How's the Dart book going? 😂
>


>[!第3題]
>
>使用字符串緩衝區(StringBuffer())來構建以下字符串：

```
void main() {
  List<int> l1 = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9];
  var buffer = StringBuffer();
  for (var i in l1) {
    buffer.write('*' * i);
    buffer.write(' ');
    buffer.write('*' * (9 - i));
    buffer.writeln();
  }
  var result = buffer.toString();
  print(result);  
}
```


>[!Ans]
> *********
>* ********
>** *******
>*** ******
>**** *****
>***** ****
>****** ***
>******* **



