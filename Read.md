## 請上傳你們組的答案
### 第一題
```Dart
  var str = '''France
USA
Germany
Benin
China
Mexico
Mongolia''';
  var a = str.split('\n');
  print(a);
```

### 第二題
```
  var str = "How's the Dart book going? :]";
  str = str.replaceAll(':]', '\u{1F61D}');
  print(str);
```

### 第三題
```
  int n = 10;
  var message = StringBuffer();
  for (var i = 0; i < n; i++) {
    message.write('*' * i);
    message.write(' ');
    message.writeln('*' * (n - i - 1));
  }
  print(message);
```

### 第四題
```
  void main(){  => 主程式
    const numbers = [1, 2, 3];    => 常數List
    numbers.forEach((number) => print(3* number));    => 取出List中的元素, 每行分別印出其3倍數值
  }
```

### 第五題
```
是
```

### 第六題
```
  final scores = [89, 77, 46, 93, 82, 67, 32, 88];
  scores.sort();
  var b = scores.reversed;
  // scores.sort((a, b) => b.compareTo(a));
  print(b.where((element) => (element >= 80 && element <= 90)));
```

### 第七題
```
1. 123
```

### 第八題
```
  var evens = [2, 4, 6, 8, 10, 12];
  print(mysum(evens));

int mysum(List<int> ll) {
  return ll.reduce((a, b) => a + b);
}
```
