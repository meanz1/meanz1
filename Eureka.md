# Linux 아스키아트
1. 문자  
2. 그림  
3. bashrc/zshrc + alias, man
  
<img width="734" alt="스크린샷 2021-03-24 오전 10 36 38" src="https://user-images.githubusercontent.com/62049151/112241066-e29a3880-8c8c-11eb-9900-b43a49670421.png">
<img width="734" alt="스크린샷 2021-03-24 오전 10 37 26" src="https://user-images.githubusercontent.com/62049151/112241092-efb72780-8c8c-11eb-96ee-6d504c1a9ae3.png">
<img width="734" alt="스크린샷 2021-03-24 오전 10 37 51" src="https://user-images.githubusercontent.com/62049151/112241153-0b223280-8c8d-11eb-805c-eeaec1a156f1.png">  

출처 : (https://daegikim.github.io/articles/2019/08/08/128%EA%B0%9C%EC%9D%98-%EB%AC%B8%EC%9E%90%EB%A1%9C-%EB%A7%8C%EB%93%9C%EB%8A%94-%EC%98%88%EC%88%A0-%EC%95%84%EC%8A%A4%ED%82%A4-%EC%95%84%ED%8A%B8(ascii-art))  

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
  <img width="698" alt="스크린샷 2021-03-24 오전 2 46 29" src="https://user-images.githubusercontent.com/62049151/112193457-3dab3b80-8c4b-11eb-9597-29e857e0211e.png">   
[참고 : cowsay] (https://zcqggntwsd.medium.com/%EC%95%84%EC%8A%A4%ED%82%A4-%EC%95%84%ED%8A%B8%EB%A1%9C-%EC%89%98-%EB%A9%94%EC%8B%9C%EC%A7%80-%EA%BE%B8%EB%AF%B8%EA%B8%B0-ce87aebc6afa)  
<img width="570" alt="스크린샷 2021-03-24 오전 10 32 02" src="https://user-images.githubusercontent.com/62049151/112240714-2cceea00-8c8c-11eb-8269-ef52fe856b0f.png">


  
## 3. bashrc/zshrc + alias, man ..  
목적 : 터미널을 실행시킬 때 welcome message를 아스키아트로 띄우기
<img width="567" alt="스크린샷 2021-03-24 오전 3 03 44" src="https://user-images.githubusercontent.com/62049151/112195765-aa273a00-8c4d-11eb-810c-28f63b39d334.png">  
bashrc/zshrc에서 figlet을 사용할 수 있기 때문에 커맨드에 적었던 것과 똑같이 적어주면 된다.  
그림을 띄우고 싶을 때에는 bashrc/zshrc에서 echo를 통해서 띄워도 되지만 bashrc/zshrc가 지저분해지고, 이스케이프문을 생각해줘야하기 때문에 번거롭다는 단점이 있다.  
사전에 만든 파일을 cat으로 긁어오자 ! (절대 경로로 설정을 해줘야 자기가 어떤 directory에 위치해있던 제대로 출력할 수 있다.)

<img width="567" alt="스크린샷 2021-03-24 오전 2 54 32" src="https://user-images.githubusercontent.com/62049151/112194487-43ede780-8c4c-11eb-80b1-edb0d752a839.png">  

+추가 ] 
### alias  
shell 문법 중 하나인데, 별칭이라는 뜻을 가지고 있으며 실제로도 별칭 역할을 한다.  
```
alias 단축어="실제 실행시킬 명령어"
``` 
<img width="698" alt="스크린샷 2021-03-24 오전 2 53 59" src="https://user-images.githubusercontent.com/62049151/112194681-7861a380-8c4c-11eb-994e-b304933d1259.png">
<img width="567" alt="스크린샷 2021-03-24 오전 3 01 18" src="https://user-images.githubusercontent.com/62049151/112195361-384ef080-8c4d-11eb-94f8-095a7f51eae2.png">  
[참고] (https://powersecurity.tistory.com/17)  

### man  
manual 이라는 뜻의 command 전용 용어이다.  
모르는 것이 있을 때 공식적인 사용 방법을 알려주기에 굉장히 유용하게 사용하고 있다.  
<img width="670" alt="스크린샷 2021-03-24 오전 3 08 10" src="https://user-images.githubusercontent.com/62049151/112196240-2c176300-8c4e-11eb-9ced-88e49d984f67.png">

<img width="670" alt="스크린샷 2021-03-24 오전 3 08 28" src="https://user-images.githubusercontent.com/62049151/112196278-35a0cb00-8c4e-11eb-88cf-2604c002bf46.png">
