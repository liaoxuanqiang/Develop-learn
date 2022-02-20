# Get started with Python using Windows

## Get started for beginners
### Set up your development environment
#### Install Python
- ```powershell
  winget install Python -s Python #通过winget 安装Python
  Python --version #确认安装版本
  pip --version #确认安装pip（标准包管理器）
  ```
#### Install Visual Studio Code
- ```powershell
  winget install Visual Studio Code
  ```
#### Install Git (optional)
### Hello World tutorial for some Python basics
#### 1.Enter python to run the Python 3 interpreter
- ```powershell
  python
  ```
#### 2.Create a variable
- ```powershell
  variable = 'Hello World!'
  ```
#### 3.Print your variable
- ```powershell
  print(variable)
  ```
#### 4.Find out the length, how many characters are used, of your string variable
- ```powershell
  len(variable)
  ```
#### 5.Convert your string variable to upper-case letters
- ```powershell
  variable.upper()
  ```
#### 6.Count how many times the letter "l" is used in your string variable
- ```powershell
  variable.count("l")
  ```
#### 7.Search for a specific character in your string variable, let's find the exclamation point
- ```powershell
  variable.find("!")
  ```
#### 8.Replace the exclamation point with a question mark
- ```powershell
  variable.replace("!", "?")
  ```
#### 9.To exit Python
- ```powershell
  exit(), quit(), or select Ctrl-Z.
  ```
### Hello World tutorial for using Python with VS Code
#### 1.Open PowerShell and create an empty folder called "hello", navigate into this folder, and open it in VS Code
- ```powershell
  mkdir hello
  cd hello
  code .
  ```
### Create a simple game with Pygame
#### Install pygame
- ```powershell
  python -m pip install -U pygame --user #安装 pygame
  python -m pygame.examples.aliens #通过运行示例游戏来测试安装
  ```
####  Start writing your own game
##### 1.Open PowerShell and create an empty folder called "bounce". Navigate to this folder and create a file named "bounce.py"
- ```powershell
  mkdir bounce
  cd bounce
  new-item bounce.py
  code .
  ```
##### 2.Using VS Code, enter the following Python code
- ```python
  import sys, pygame

  pygame.init()

  size = width, height = 640, 480
  dx = 1
  dy = 1
  x= 163
  y = 120
  black = (0,0,0)
  white = (255,255,255)

  screen = pygame.display.set_mode(size)

  while 1:

    for event in pygame.event.get():
        if event.type == pygame.QUIT: sys.exit()

    x += dx
    y += dy

    if x < 0 or x > width:   
        dx = -dx

    if y < 0 or y > height:
        dy = -dy

    screen.fill(black)

    pygame.draw.circle(screen, white, (x,y), 8)

    pygame.display.flip()
  ```
##### 3.Save it as: bounce.py
4.
## Get started using Python for web development on Windows
### 1.Set up your development environment
#### Install Windows Subsystem for Linux
- ```bash
  lsb_release -dc #查看版本和代码名称
  sudo apt update && sudo apt upgrade #更新发行版
  ```
#### Set up Visual Studio Code
### 2.Create a new project
- ```powershell
  mkdir HelloWorld
  ```
### 3.Install Python, pip, and venv
- ```bash
  python3 --version #确认已安装Python3
  sudo apt update && sudo apt upgrade #更新 Ubuntu 版本
  sudo apt upgrade python3 #更新 Python
  sudo apt install python3-pip #安装 pip
  sudo apt install python3-venv #安装 venv
  ```
### 4.Create a virtual environment
- ```powershell
  python3 -m venv .venv #创建名为 .venv 的虚拟环境
  source .venv/bin/activate #激活虚拟环境,，输入：deactivate命令停用
  ```
