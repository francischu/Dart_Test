#  將多行字符串，如下面的文本，拆分成`單行`的`列表`
提示：在換行字符處進行拆分。
``` dart
void main(){
    // 定義一個字符串，其中包含各國家名稱，每個名稱由換行符分隔

    String countriesString = """
    France
    USA
    Germany
    Benin
    China
    Mexico
    Mongolia
    """;

    // 使用.split()方法按換行符將字符串分割成列表
    List<String> countriesList = countriesString.split('\n').where((item) => item.isNotEmpty).toList();

    // 印出列表，確認轉換是否正確
    print(countriesList);
}
```

# 在線上找一個表情符號來替換以下文本中的 `:]`
``` dart
void main(){
	String text = "How's the Dart book going? :]";
	String updatedText = text.replaceAll(':]', '😊');
	print(updatedText);
}
```

# 使用字符串緩衝區(StringBuffer())來構建以下字符串
``` dart
void main(){
    // 創建一個StringBuffer實例
    StringBuffer buffer = StringBuffer();
    // 使用for迴圈來構建圖案
    for (int i = 0; i < 10; i++) {
      // 添加前導空格
      for (int j = 0; j < 10; j++) {
        if (i == j)
          buffer.write(' ');
        else
          buffer.write('*');
      }
      // 每行結尾添加換行符
      buffer.writeln();
    }
    // 印出構建好的圖案
    print(buffer.toString());
}
```
# 請解釋以下程式碼
``` dart
void main(){
  const numbers = [1, 2, 3];
  numbers.forEach((number) => print(3* number));
   /*
    這一行代碼使用了forEach方法，這是List類提供的一個方法，用於對列表中的每個元素執行給定的函數。
    forEach方法接收一個函數作為參數。在這個例子中，使用了箭頭函數(number) => print(3 * number)，
    它對列表中的每個元素（在這裡被命名為number）進行操作。

    箭頭函數的本體是print(3 * number)，這表示它會計算number乘以3的結果，然後將該結果打印到控制台上。
    */
}
```

# 請判斷下列程式碼輸出是否跟第上題相同
``` dart
void main(){
  const numbers = [1, 2, 3];
  final triple = (int x) => print(3 * x);
  numbers.forEach(triple);
}
```
## <結果是相同的>

# 考試分數分級
``` dart
void main(){
	final scores = [89, 77, 46, 93, 82, 67, 32, 88];
    // 使用sort方法和比較函數從高到低排序分數
    scores.sort((a, b) => b.compareTo(a));
    print('Sorted scores from high to low: $scores');
    // 使用where方法找出所有B級分數（80到90之間，不包括90）
    var bGrades = scores.where((score) => score >= 80 && score < 90).toList();
    print('B grade scores (80 to 89): $bGrades');
}
```
# 查看程式碼並回答
```
inal looped = <int>[];
```

問：looped可以放入哪些值？
 1. 123
 2. "123"
 3. (123)
 4. [123]
## 只有 2. 不行
``` dart
void main(){
    final looped = <int>[];

    looped.add(123);

    // looped.add("123");  // 错

    looped.add((123));

    // looped.add([123]);  // 错

    looped.addAll([123]);

    print(looped);
}
```

# 請寫一個函數讓`evens`中的全部元素相加
```
evens = [2, 4, 6, 8, 10, 12];
```
``` dart
void main()
{
	List<int> num = [1,2,3,5,5,6,6,8,8,1,10,22,13,18,353];
    num.forEach((element) => print(element));
    print('elements sum is: ${addAllElements(num)}');
}

