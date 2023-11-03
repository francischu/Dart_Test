## 第1題
將多行字符串，如下面的文本，拆分成單行的列表
提示：在換行字符處進行拆分。
```
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

 List<String> lines = nation.split('\n');
 print(lines);
}
```


## 第2題
在線上找一個表情符號來替換以下文本中的 :]
```
void main() {
  String message = "How's the Dart book going? \u{1F60A}";
  print(message);
}
```
參考:https://www.unicode.org/emoji/charts/full-emoji-list.html


## 第3題
使用字符串緩衝區(StringBuffer())來構建以下字符串：
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

```
StringBuffer Buffer = StringBuffer("**********");
  String str = Buffer.toString();
  for (int i = 0; i <= 10; i++) {
    int index = i;
    String insert = ' ';
    String test = str.substring(0, index) + insert + str.substring(index);
    print(test);
  }
```

## 第4題
請解釋以下程式碼：
```
void main() {
 const numbers = [1, 2, 3];
 numbers.forEach((number) => print(3 * number));
}
```
答:建立一個List,拜訪每一個List元素,並輸出3\*元素
結果為:
3
6
9
## 第5題
請判斷下列程式碼輸出是否跟第4題相同
```
void main(){
 const numbers = [1, 2, 3];
 final triple = (int x) => print(3 * x);
 numbers.forEach(triple);
}
```
答: 輸出結果一樣

## 第6題
給定以下考試分數：  
- final scores = [89, 77, 46, 93, 82, 67, 32, 88];  
- 使用 sort 將分數從高到低排序。  
- 使用 where 查找所有B級分數，即所有分數在 80 到 90 之間的分數。
```
void main() {
 final scores = [89, 77, 46, 93, 82, 67, 32, 88];
 scores.sort((a, b) => b - a);
 print("排序后的分数：$scores");
 final bGrades = scores.where((score) => score >= 80 && score <= 90).toList();
 print("B级分数：$bGrades");
}
```

## 第7題
請查看程式碼並回答以下問題
 final looped = <\int>\[];
問:looped可以放入哪些值？
 1. 123 
 2. "123"
 3. (123)
 4. [123]
答: 1

## 第8題
請寫一個函數讓`evens`中的全部元素相加
(不得侷限在目前僅有的數字範圍及長度)
```
void main() {
 List<int> evens = [2, 4, 6, 8, 10, 12];
 int sum = 0;
 for (var i in evens) {
   sum += i;
 }
 print(sum);
}
```

