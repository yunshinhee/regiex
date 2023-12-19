# 정규표현식
# /regiex/ ==> Regular expression 의 약자

# 언제 사용하는가?
  - 텍스트에서 우리가 원하는 특정한 패턴을 찾을 때 (전화번호형태의 패턴, 엡사이트 주소형태의 패턴, 이메일형식의 패턴을 찾을 때 등등)
  - 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 특정한 패턴에 부합하는지 유효성 검사를 할때도 사용할 수 있다.
  - 정규식은 문자를 검사하고자 할때 사용하는 식이다.
# 정규식은 /로 시작하여 "나는 정규표현식"임을 나타낸다
- /우리가 찾고자하는 패턴/
- /regex/i
- i는 어떤 옵션에 따라 검색할건지 플래그를 활용할 수 있다.
# 문법
   1) Groups and ranges
      - 🚩 | : 또는
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/4e80315b-28f3-4ac1-b607-14cad6cebebf)
      - 🚩 () : 그룹
      - 1번째 그룹 you또는 to를 찾고 2번째 그룹에서는 the를 찾음
      ![image](https://github.com/yunshinhee/regiex/assets/145514638/2631a3cb-3167-434b-8188-a921a7d57c77)
      - Fr로 시작하고 중간 글자가 e 가 되고  nch로 끝나는것을 찾음
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/80053e4f-aaf9-4e54-ac46-f7cba39d6fcd)

      - 🚩 [] : 문자셋, 괄호안의 어떤 문자든
      - [ead] 대괄호 안에 있는 글자중 하나라도 만족하는 것을 찾음
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/f6d3e33d-1306-4490-85b1-b523b88193bb)
      - gr로 시작하고 중간글자가 a또는 e또는 d가 있고 y로 끝나는 것을 찾음
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/438e31b3-6278-4b10-a448-ead0deecdf2c)
      - =========================💡위의 두 이미지는 같다

      - gr로 시작하고 중간글자가 a~g가 되고 y로 끝나는 것을 찾음 
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/20f1a820-f6f0-44e9-b00a-c6089478f61d)
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/ef8ee9c3-c96d-4f94-b2c9-528b390f4a5f)
      - =========================💡위의 두 이미지는 같다

      - 🚩 [^] : 부정 문자셋, 괄호안의 어떤 문자가 아닐 때 [^a] -> a가 아닐때
      - a 부터 z 까지, A부터 Z까지 , 0부터 9까지가 아닌것을 찾음 (띄어쓰기 포함)
      ![image](https://github.com/yunshinhee/regiex/assets/145514638/f5ea4e5a-b4ed-4fa1-99d0-d2a4c1dcf983)

      - 🚩 (?) : 찾지만 기억하지는 않음
      -  찾아는 지지만 그룹으로 만들고 싶지 않다면 사용
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/05dfe757-e717-4a3b-8487-c8cc135eee49)
       
      - 💡 a 부터 z 까지, A부터 Z까지 , 0부터 9까지를 찾음  (특수기호 제외)
       ![image](https://github.com/yunshinhee/regiex/assets/145514638/0dad4b6d-e63a-4095-91ee-829b99ae4882)
     
   2) 제한하기 위해 사용하는
      -  ? : 없거나 있거나(zero or one)
      - ＊ : 없거나 있거나 많거나(zero or more)
      -  + : 하나 또는 많거나(one or more)
      -  {n} : n번 반복
      -  {min,} : 최소
      -  {min,max} : 최소 그리고 최대
   3) 경계에 대한
      - \b : 단어경계 
      - \B : 단어경계가 아님  
      - ^ : 문장의 시작  
      - $ : 문장의 끝
   4) 특징을 이용하는 방법
      - \ : 특수문자가 아닌 문자를 찾을 때
      - . : 어떤/모든 글자 (줄바꿈/엔터키 문자 제외)
      - \d : 숫자(digit)
      - \D : 숫자가 아님(digit)
      - \w : 문자(Word)
      - \W : 문자가 아님(Word)
      - \s : 공백(space)
      - \S : 공백이 아님(space)


     

      



