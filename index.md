
### Team Name: 021B
### Jaeyeong Yoo, Hanyoung Lee, Wonyo Cho


project name: 한글 맞춤법 검사






--------------------------------------------
# 목차

1. 선정한 프로젝트
2. 프로젝트 조사
3. 활동
4. 히스토리


--------------------------------------------

# 1. 선정한 프로젝트

오픈소스 데스크톱에 널리 사용되는 hunspell 맞춤법 검사 프로그램에서 동작하는 (현재 유일한) 한국어 맞춤법 사전입니다.
현재 여러 리눅스 배포판과 오픈소스 애플리케이션에서 동작합니다.
-단어 단위 맞춤법 검사
-불규칙 활용을 포함한 용언 활용 등 교착어인 한국어의 특징에 맞게 구현
-hunspell 맞춤법 검사를 사용하는 프로그램이라면 수정 없이도 한국어 맞춤법 검사가 동작
-오픈소스 배포 가능한 단어 데이터 사용

이 곳에는 소스 코드가 들어 있습니다. 맞춤법 검사 기능을 사용하려면 OS별 패키지를 설치하시거나, 여러 가지 애플리케이션별 확장 기능을 이용하십시오. 또는 빌드한 사전 파일을 사용할 수도 있습니다.
사전 파일은 ko.aff 파일과 ko.dic 파일 2개로 이루어져 있고 hunspell 사전이 저장되는 위치에 복사해 사용할 수도 있습니다.
리눅스 배포판에 들어 있는 브라우저나 오피스 프로그램은 보통 내장된 hunspell을 사용하도록 빌드되어 있습니다. 그러니 배포판에 포함된 패키지를 설치하면 프로그램별 확장 기능을 따로 설치하지 않아도 됩니다.
-데비안: hunspell-ko 패키지 설치, 6.0 (squeeze) 이후 패키지 정보
-우분투: hunspell-ko 패키지 설치, 9.10 (karmic) 이후 패키지 정보
-페도라: hunspell-ko 패키지 설치, fc12 이후 패키지 정보
-Mac OS X 10.5: BaramSpellChecker
-Mac OS X 10.6 이상: /Library/Spelling 또는 홈폴더/Library/Spelling 아래 aff/dic 파일 복사
-Mozilla/Firefox 부가 기능
-LibreOffice 및 OpenOffice.org 부가 기능

ko.dic 파일에는 표제어 데이터가 들어 있고 ko.aff (affix) 파일에는 단어의 활용 정보가 들어갑니다. aff 파일과 dic 파일은 hunspell의 전신인 myspell에서도 이용하는 형식이지만 한국어 데이터는 hunspell에만 들어 있는 기능이 필요하기 때문에 hunspell에서만 동작합니다.
--------------------------------------------

# 2. 프로젝트 조사

hunspell의 활용 범위: 리브레오피스나 오픈오피스, 파이어폭스, 오페라, 아파치 등 해외에서 제작된 프로그램에 한글을 지원하기 위해 사용되고 있음

### 활용 방법

1. hunspell 작동 방법을 코드를 통해 파악 / hunspell을 현재 사용되지 않고 있는 다른 프로그램에 이식 (pull-request를 통한 답변을 받지 못함 + 여력이 되지 않아 실패)
2. hunspell의 맞춤법 검사 - 기준은 윈도우에서 가장 많이 사용하는 한글 오피스 + 표준국어대사전을 통한 검사 시작 (선택!)

### How?

우분투의 리브레오피스의 언어 설정이 한글로 가능하다면, 그것은 hunspell-ko를 기반으로 한 것임. 따라서 리브레오피스에 낱말이나 문장을 적어 맞춤법 검사를 시행하고, 이를 한글 오피스나 표준국어대사전을 통해 검사를 하면 됨.
-> 찾아낸 오류들을 pull-request를 하여 hunspell-ko의 맞춤법 정확성을 높이는데 기여할 목적


---------------------------------------------

# 활동


1. 예외 경우
2. 합성어(한글+한글 or 한문+한문 or 한문+한글)
3. 한문어
에 대해서 맞춤법 오류가 뜨는 경우



--------------------------------------------------------------
# 히스토리

## 05.16

### 이번에 한 일

clone and download ZIP file.
we download the Python compiler because the project is based on Python.
we see the code – the commends are written in Korean. It makes us more comfortable the understand.

*코드는 윈도우 환경에서 안 돌아가는 듯 하다.
*코드를 돌리지 못했고 어떻게 해야할 지 모르겠다. 돌아가지 않는 원인을 찾고 코드를 돌려야한다.



### 앞으로 할 것

1. 프로그램 실행
2. 에러 찾아보기
3. 프로그램에 도움이 될만한 새로운 컨텐츠 생각해보기
4. 피드백 주기
5. 위의 단계 반복


### 각자 한 일

Basically all members implement the program.
-> 프로그램 실행이 안돼서 단어 추가를 건의하는 방향으로 수정.

Cho wonyi – Implement the program in Ubuntu. Write issue and Wiki. Write README.

Yoo jaeyeung – Wiki, write the daily action 

Lee hanyoung – Manage all the project




## 05.30

1.  리눅스 환경에서 파이선 파일을 다운받아 실행을 시켜보려 했으나, 돌아가지 않았고 조교님께 여쭤본 후 파일 자체가 이상하다고 여겨 pull request를 보냈다.
2. 단어 추가를 건의하는 방향으로  계획을 수정했다.




## 06.06

 여전히 프로그램 실행이 안되고 깃헙을 확인하지 않아서 커멘드가 안온게 아니라 그냥 pull request를 받아주지 않는 것임을 확인.
 
 

## 06.11~12

'hunspell'은 이미 다방면에 적용되어 있는 프로그램 (ex: 리브레 오피스) 따라서 이 프로그램이 찾아내지 못하는 문법적 오류를 리브레오피스에서 찾아낸다.  -> hunspell을 열람해서 맞춤법을 확인한다는 목표에 부합

리브레오피스를 통해 hunspell에 적용되어 있지 않는 까다로운 한국어 맞춤법을 찾아서 제작자에게 보내준다.
