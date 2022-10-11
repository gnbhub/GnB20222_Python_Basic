## ✏ Week 2_Homework
'예제'는 교육자료의 example을 실습해보고, 'Lab'은 lab 문제 자료의 문제를 풀이하세요.

문제는 Google Colaboratory로 풀이하며, 하나의 파일에 문제들을 각 코드 셀에 나누어 풀이해주세요.

작성이 끝난 파일을 본 repo의 week3 폴더에 업로드하세요.


### 1️⃣ 예제 7-3 : 입력된 문자열에서 공백 구분하여 단어로 출력 (in, 문자열 덧셈)


### 2️⃣ 예제 7-12 : 입력한 주민번호에서 생년월일 추출 (인덱싱, 슬라이싱)


### 3️⃣ 예제 7-31 : 이름/비밀번호 체크 프로그램 (.strip(), .replace(), len(), .isalpha(), .isdigit())


### 4️⃣ 예제 7-32 : '-'로 구분된 점수들의 총합 구하기 (.split())


### 5️⃣ Lab 3-1 : 이메일과 전화번호에서 id, 도메인, 가운데 번호 추출하기
```
1. 이메일 주소와 휴대폰 전화번호 입력받기
   - 입력받은 데이터가 유효한지 확인할 것
     -> 이메일과 전화번호는 공백으로 구분 (공백으로 구분되는 문자열이 두 개)
     -> 이메일(앞 문자열) 유효성 : @이 포함되어 있는가?
     -> 휴대폰 번호 유효성 : 구분자에 관계없이 숫자의 개수는 11개
     -> 그렇지 않으면 오류 메세지 출력 후 다시 입력받을 것 (반복문 사용!!)

2. 입력받은 문자열에서 이메일 id, 호스팅, 가운데 번호 추출하여 출력하기
     -> .find(), .rfind(), split() 사용

ex)  입력 : wdh48040@gmail.com01012345678
     출력 : Error! Enter an email address and a phone number seperate by spaces.
     입력 : wdh48040@gmail.com 010.1234.567
     출력 : Error! The phone number should consist of 11 digits.
     입력 : wdh48040@gmail.com 010-1234-5678
     출력 : -> email id : wdh48040
            -> host name : gmail.com
            -> middle part : 1234
