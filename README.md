# 🟢 flutter_function 🟢

**จากโจทย์ที่กำหนดให้** 
1. ให้หาตัวที่น้อยที่สุดใน Array ห้ามใช้ sort
```bash
  listnumber() {
  List<int> Listnum = [80, 44, 12, 43, 55, 44, 90];
  var Value = Listnum[0];
  for (var i = 0; i < Listnum.length; i++) {
    if (Listnum[i] < Value) {
      Value = Listnum[i];
    }
  }
  print("1. ให้หาตัวเลขที่น้อยที่สุดใน Array ห้ามใช้ sort");
  print("Data : $Listnum");
  print("answer : $Value");
}
```
**Output**
```diff
+ answer : 12
```
**2. ให้เรียงลำดับจากจำนวนตัวอักษร โดยให้เรียงจาก น้อยไปมาก**
```bash
liststring() {
  List<String> Listanimal = ['Elephant', 'Dog', 'Cat', 'Alligator', 'Bird'];
  List<String> Value = ['Elephant', 'Dog', 'Cat', 'Alligator', 'Bird'];

  // Sorting string by comparing the length
  Value.sort((a, b) => a.length.compareTo(b.length));

  print("2. ให้เรียงลำดับจากจำนวนตัวอักษร โดยให้เรียงจาก น้อยไปมาก");
  print("Data : $Listanimal");
  print("answer : $Value");
}
```
**Output**
```diff
+ answer : [Dog, Cat, Bird, Elephant, Alligator]
```
**3. ให้หาตำแหน่งตัวที่มากที่สุดใน Array**
```bash
findposition() {
  List<int> data = [1, 44, 5, 89, 100, 1, 44];
  var Value = data[0];
  var position = 0;
  for (var i = 0; i < data.length; i++) {
    if (data[i] > Value) {
      Value = data[i];
      position = i;
    }
  }
  print("3. ให้หาตำแหน่งตัวที่มากที่สุดใน Array");
  print("Data : $data");
  print("answer : $position");
}
```
**Output**
```diff
+ answer : 4
```
**4. ให้แปลงข้อมูลจาก**
```bash
convert() {
  List<List<int>> data = [
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9],
  ];
  List<int> flatList = data.expand((i) => i).toList();
  print("4. ให้แปลงข้อมูลจาก");
  print(data);
  print("เป็น");
  print(flatList);
}
```
**Output**
```diff
+ answer : [1, 2, 3, 4, 5, 6, 7, 8, 9]
```
**5. ให้หาเลขระหว่าง 1 ถึง 50 ว่ามีตัวไหนที่หาร 3 กับ 5 ลงตัว**
```bash
divisible_by_3and5() {
  print("5. ให้หาเลขระหว่าง 1 ถึง 50 ว่ามีตัวไหนที่หาร 3 กับ 5 ลงตัว");
  for (int i = 1; i < 50; i++) {
    if (i % 3 == 0 && i % 5 == 0) print("$i,");
  }
}
```
**Output**
```diff
+ answer : 15,30,45,
```

