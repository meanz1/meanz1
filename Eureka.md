# Linux 아스키아트
1. 문자  
2. 그림  
3. bashrc/zshrc + alias, man
  
## 1. 문자  

figlet : 입력한 문자를 큰 문자(Fig character)로 터미널에 출력해 주는 툴  
```
linux : sudo apt install figlet
osx : brew install figlet
```

### 사용법  
```
figlet 원하는 문자
```  
<img width="698" alt="스크린샷 2021-03-24 오전 2 19 58" src="https://user-images.githubusercontent.com/62049151/112189528-71846200-8c47-11eb-9f0a-09c40ad839aa.png">  
  
-c : 가운데 정렬  
-f : 폰트 지정 가능  

[참고 : 폰트 종류] (http://www.figlet.org/fontdb.cgi)  
[참고 : 색, 디자인 커스텀] (https://misc.flogisoft.com/bash/tip_colors_and_formatting) 

+추가) lolcat  
<img width="698" alt="스크린샷 2021-03-24 오전 2 25 49" src="https://user-images.githubusercontent.com/62049151/112190355-42babb80-8c48-11eb-8421-47166792ee38.png">

```
linux : sudo apt install lolcat
osx : brew install lolcat
```  

## 2. 그림  
디렉토리 최상단에 파일 하나를 만들어서(확장자는 없어도 된다. 혹은 shell) 아래 사이트를 참고하여 원하는 그림(아스키 코드로 변환 후) 첨부한다.  
[참고] (https://wepplication.github.io/tools/charMap/#asciiArt)  
[참고] (https://www.ascii-art-generator.org/)
  
  
## 3. bashrc/zshrc + alias, man ..  
목적 : 터미널을 실행시킬 때 welcome message를 아스키아트로 띄우기
