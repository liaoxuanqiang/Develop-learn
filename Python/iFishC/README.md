# iFishC tutorial
## 1.变量和字符串
### 变量
#### 变量的定义
- ```py
  x = 3
  print(x)
  ```
#### 变量名的设置规则
- ```py
  loveyou1314 = 1314 #变量名以字母、数字、下划线设置
  520baby = 520 #变量名不能以数字开头
  幸运数 = 588 #变量名可以是中文字符
  print(幸运数)
  ```
#### 字符串类型变量名
- ```py
  name = '小甲鱼'
  print(name)
  name = "老乌龟"
  print(name)
  ```
#### 变量的赋值
- ```py
  x = 3
  y = 5
  y = x
  print(y)

  x = y = 3
  x
  y

  x = 3
  y = 5
  z = x
  x = y
  y = z
  print(x,y)

  x = 3
  y = 5
  x, y = y, x
  print(x, y)
  ```
### 字符串
#### 单双引号字符串
- ```py
  print('I Love China.') #Single quotes
  print("I Love FishC.") #Double quotes
  
  print('Let's go!') #语法错误
  print("Let's go!")
  ```
#### 转义字符
- ```py
  print('"Life is short, you need Python."')
  print('\"Life is short, Let\'s learn Python.\"')
  print("\"Life is short, Let\'s learn Python.\"")

  print("I Love Python.\nI Love FishC.")
  ```
#### 原始字符串
- ```py
  print("D:\three\two\one\now") #语法错误
  print("D:\\three\\two\\one\\now")
  print(r"D:\three\two\one\now") #raw strings 原始字符串

  ```
#### 跨行字符串
- ```py
  poetry = 
  """
  面朝大海，春暖花开
  从明天起，做一个幸福的人
  喂马、劈柴，周游世界
  从明天起，关心粮食和蔬菜
  我有一所房子，面朝大海，春暖花开
  从明天起，和每一个亲人通信
  告诉他们我的幸福
  那幸福的闪电告诉我的
  我将告诉每一个人
  给每一条河每一座山取一个温暖的名字
  陌生人，我也为你祝福
  愿你有一个灿烂的前程
  愿你有情人终成眷属
  愿你在尘世获得幸福
  我只愿面朝大海，春暖花开
  """
  #triple quoted
  print(poetry)
  ```

#### 字符串的加法和乘法
- ```py
  520 + 1314
  '520' + '1314' #字符串拼接

  print("我每天爱你三千遍！\n" * 3000) #重复打印字符串
  ```
## 2.数字类型
### 整数
- ```py
  1234567890 / 987654321 #进行除法运算
  6 / 3
  ```
### 浮点数
- ```py
  0.1 + 0.2

  i = 0
  while i < 1:
      i = i + 0.1
      print(i)

  0.3 == 0.1 + 0.2
  0.3 < 0.1 + 0.2

  import decimal
  a = decimal.Decimal('0.1')
  b = decimal.Decimal('0.2')
  print(a + b)

  c = decimal.Decimal('0.3')
  a + b == c

  0.00005

  ```
### 复数
- ``` py
  1 + 2j

  x = 1 + 2j
  x.real
  x.imag
  ```
### 数字运算
- ```py
  3 / 2
  3 // 2
  -3 / 2

  3 % 2
  6 % 2
  x == (x // y) * y + (x % y )
  divmod(3, 2)
  divmod(-3, 2)

  x = -520
  abs(x)
  y = -3.14
  abs(y)
  z = 1 + 2j
  abs(z) #求复数的模

  int('520')
  int(3.14)
  int(9.99)

  float('3.14')
  float(520)
  float('+1E6')

  complex("1+2j")
  complex("1 +2j") #错误语法，字符串不能有空格

  pow(2, 3)
  2 ** 3
  pow(2, -3)
  2 ** -3
  pow(2, 3, 5)
  2 ** 3 % 5

  ```
## 3.布尔类型
- ```py
  bool(250)
  bool("假")
  bool("False")
  bool(False)
  bool("")
  bool(" ")
  bool(520)
  bool(0)
  bool(0.0)
  bool(0j)
  ```
### 定义为False的对象
#### None和False
### 值为零的数字类型
#### 0