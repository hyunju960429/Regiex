# 정규표현식

https://regexr.com/5mhon <--참고사이트

# /regiex/ ==> Regular expression(정규화된 표현)의 약자

# 언제 사용하는가?
 - 텍스트에서 우리가 원하는 특정한 패턴을 찾을때 (전화번호형태의 패턴, 웹사이트주소형태의 패턴, 이메일형식...의 패턴을 찾을때)
 - 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 일정한 패턴에 부합하는지 유효성검사를 할때도 사용할 수 있다.
 - > 정규식은 문자를 검사하고자 할때 사용하는 식이다.


# 정규식은 / 로 시작하여 "나는 정규표현식"임을 나타낸다.
 - /우리가 찾고자하는 패턴/

 - /regex/i
 - i는 어떤 옵션에 따라서 검색할것인지 플래그를 활용할 수 있다.

# 문법
 1) Group anf ranges
    - |   : 또는

     ![image](https://github.com/hyunju960429/Regiex/assets/145514544/b79e8e0e-2f19-48a1-9aa5-b4c2e44997aa)





    - ()  : 그룹
   
     ![image](https://github.com/hyunju960429/Regiex/assets/145514544/ab5175af-3bb8-4b42-b075-be6d033d9883)





     # T로 시작하고 중간글자가 ex 거나 x 이거나 마지막은 t로 끝나는것을 찾음
     ![image](https://github.com/hyunju960429/Regiex/assets/145514544/60e81ac1-8b71-42be-9df9-7ff7edda0b4b)

     ![image](https://github.com/hyunju960429/Regiex/assets/145514544/ef935159-5e42-4141-be6c-06962ed405c5)






    - []  : 문자셋, 괄호안의 어떤 문자든
   
     ![image](https://github.com/hyunju960429/Regiex/assets/145514544/e42fc487-23ce-45ab-bacf-20de6f2d6f53)





    
    - [^] : 부정 문자셋, 괄호안의 어떤 문자가 아닐때
    - (?:) : 찾지만 기억하지는 않음
      # 찾아는 지지만 그룹으로 만들고 싶지 않다면 사용 
      ![image](https://github.com/hyunju960429/Regiex/assets/145514544/508ab56c-17bf-47ba-a854-dbcca875e056)

