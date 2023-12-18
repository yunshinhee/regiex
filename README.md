# 정규표현식
# /regiex/ ==> Regular expression 의 약자

#언제 사용하는가?
  - 텍스트에서 우리가 원하는 특정한 패턴을 찾을 때 (전화번호형태의 패턴, 엡사이트 주소형태의 패턴, 이메일형식의 패턴을 찾을 때 등등)
  - 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 특정한 패턴에 부합하는지 유효성 검사를 할때도 사용할 수 있다.
  - 정규식은 문자를 검사하고자 할때 사용하는 식이다.

    # 정규식은 /로 시작하여 "나는 정규표현식"임을 나타낸다
    - /우리가 찾고자하는 패턴/
    - /regex/i
    - i는 어떤 옵션에 따라 검색할건지 플래그를 활용할 수 있다.

   # 문법
   1) Groups and ranges
      - | : 또는
      - ![image](https://github.com/yunshinhee/regiex/assets/145514638/4e80315b-28f3-4ac1-b607-14cad6cebebf)
      - () : 그룹
      -![image](https://github.com/yunshinhee/regiex/assets/145514638/2631a3cb-3167-434b-8188-a921a7d57c77)


      - [] : 문자셋, 괄호안의 어떤 문자든
      - [^] : 부정 문자셋, 괄호안의 어떤 문자가 아닐 때 [^a] -> a가 아닐때
      - (?) : 찾지만 기억하지는 않음
     
      - Fr로 시작하고 중간 글자가 e 가 되고  nch로 끝나는것을 찾음
      - ![image](https://github.com/yunshinhee/regiex/assets/145514638/80053e4f-aaf9-4e54-ac46-f7cba39d6fcd)

