
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

# 선정한 프로젝트

hunspell-ko는 오픈소스 데스크톱에 사용되는 한국어 맞춤법 사전으로, 윈도우 환경에서 돌아가는 것과는 비교된다.

--------------------------------------------

# 프로젝트 조사

hunspell의 활용 범위: 리브레오피스나 오픈오피스, 파이어폭스, 오페라, 아파치 등 해외에서 제작된 프로그램에 한글을 지원하기 위해 사용되고 있음

활용 방법:
1. hunspell 작동 방법을 코드를 통해 파악 / hunspell을 현재 사용되지 않고 있는 다른 프로그램에 이식 (pull-request를 통한 답변을 받지 못함 + 여력이 되지 않아 실패)
2. hunspell의 맞춤법 검사 - 기준은 윈도우에서 가장 많이 사용하는 한글 오피스 + 표준국어대사전을 통한 검사 시작 (선택!)

How?
우분투의 리브레오피스의 언어 설정이 한글로 가능하다면, 그것은 hunspell-ko를 기반으로 한 것임. 따라서 리브레오피스에 낱말이나 문장을 적어 맞춤법 검사를 시행하고, 이를 한글 오피스나 표준국어대사전을 통해 검사를 하면 됨.
-> 찾아낸 오류들을 pull-request를 하여 hunspell-ko의 맞춤법 정확성을 높이는데 기여할 목적


---------------------------------------------

# 활동

1. 예외 경우
2. 합성어(한글+한글 or 한문+한문 or 한문+한글)
3. 한문어
4. 외래어 (+ 고유어)
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
