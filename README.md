# 정규표현식

https://regexr.com/5mhon <--참고사이트

# /regiex/ ==> Regular expression(정규화된 표현)의 약자

# 언제 사용하는가?
 - 텍스트에서 우리가 원하는 특정한 패턴을 찾을때 (전화번호형태의 패턴, 웹사이트주소형태의 패턴, 이메일형식...의 패턴을 찾을때)
 - 사용자가 입력한 텍스트가 이메일이나 패스워드와 같이 일정한 패턴에 부합하는지 유효성검사를 할때도 사용할 수 있다.
 -  정규식은 문자를 검사하고자 할때 사용하는 식이다.


# 정규식은 / 로 시작하여 "나는 정규표현식"임을 나타낸다.
 - /우리가 찾고자하는 패턴/

 - /regex/i
 - i는 어떤 옵션에 따라서 검색할것인지 플래그를 활용할 수 있다.

# 문법
 1) Group anf ranges
    - |   : 또는
    - ()  : 그룹
    - []  : 문자셋, 괄호안의 어떤 문자든
    - (?:) : 찾지만 기억하지는 않음
    - [^] : 부정 문자셋, 괄호안의 어떤 문자가 아닐때

 2) 제한하기 위해 사용하는
    - ?   : 없거나 있거나(zero or one)
    - * (&#42;)  : 없거나 있거나 많거나(zero or one or more)
    - + (&#43;)   : 하나 또는 많거나(one or more)
    - {n}   : n번 반복
    - {min,}: 최소
    - {min,max}: 최소 그리고 최대
   
 3) 경계에 대한
    -  \b : 단어경계
    -  \B : 단어경계가 아님
    - ^   : 문장의 시작
    - $   : 문장의 끝

 4) 특징을 이용하는 방법
    - \   : 특수문자가 아닌 문자
    - .   : 어떤 글자(줄바꿈 문자 제외)
    - \d  : 숫자
    - \D  : 숫자 아님
    - \w  : 문자(word)
    - \W  : 문자 아님
    - \s  : 공백(space)
    - \S  : 공백이 아닌것




![image](https://github.com/hyunju960429/Regiex/assets/145514544/b79e8e0e-2f19-48a1-9aa5-b4c2e44997aa)


-----------------


    
   
![image](https://github.com/hyunju960429/Regiex/assets/145514544/ab5175af-3bb8-4b42-b075-be6d033d9883)


-----------------------


# T로 시작하고 중간글자가 ex 거나 x 이거나 마지막은 t로 끝나는것을 찾음
![image](https://github.com/hyunju960429/Regiex/assets/145514544/60e81ac1-8b71-42be-9df9-7ff7edda0b4b)

![image](https://github.com/hyunju960429/Regiex/assets/145514544/ef935159-5e42-4141-be6c-06962ed405c5)



----------------------


    

# T로 시작하고 e 또는 x또는 i가 있고 t로 끝남
# [exi] --> 대괄호 안에 있는 글자중 하나라도 만족하는것을 찾아라는 의미 
![image](https://github.com/hyunju960429/Regiex/assets/145514544/e42fc487-23ce-45ab-bacf-20de6f2d6f53)


# 아래 두 이미지는 T로 시작하고 a~x까지의 글자중 하나라도 가지고 있고 t로 끝나는 것을 찾음
     
![image](https://github.com/hyunju960429/Regiex/assets/145514544/ac314ad4-6cf4-4468-b827-fba0f22089d5)

![image](https://github.com/hyunju960429/Regiex/assets/145514544/3058581f-9309-4f07-bb96-a55605f37c54)



-----------------------------------

   
    
    
    
    
# 찾아는 지지만 그룹으로 만들고 싶지 않다면 사용 
      
![image](https://github.com/hyunju960429/Regiex/assets/145514544/508ab56c-17bf-47ba-a854-dbcca875e056)






--------------------------




# a부터 z까지, A부터 Z까지, 0부터 9까지 하나라도 만족하면 모두 찾는다.
      
![image](https://github.com/hyunju960429/Regiex/assets/145514544/23d68f55-fcf3-4f57-925e-215e38a4d782)



      
# a부터 z까지, A부터 Z까지, 0부터 9까지를 제외한 모든것을 찾는다.
![image](https://github.com/hyunju960429/Regiex/assets/145514544/de0368d1-dfeb-41d7-be5c-b75445d8c4c8)



      
---------------------



# ?: 있거나 없거나(많거나X)
![image](https://github.com/hyunju960429/Regiex/assets/145514544/8f94c4b0-fef8-4b66-8ac0-0084074b60e4)





--------------------

# * : 있거나 없거나 많거나
![image](https://github.com/hyunju960429/Regiex/assets/145514544/5c9eb6c2-97b2-4ad8-920e-2165ab97192f)



---------------------

# + : 있거나 많거나
![image](https://github.com/hyunju960429/Regiex/assets/145514544/dd52e6a5-aebb-4a8d-bb33-3affe59d1ac9)



-----------------------


# {n} : n번반복
![image](https://github.com/hyunju960429/Regiex/assets/145514544/0c846b5e-c67c-4ec1-8e5c-69852b18d741)


------------------------

# {min,} : 최소 min 이상
![image](https://github.com/hyunju960429/Regiex/assets/145514544/c39fbe3c-abe0-4bd1-9e3d-6336e8c067ae)


-----------------------

# {min, max} : 촤소 min 이상 최대 max 이하
![image](https://github.com/hyunju960429/Regiex/assets/145514544/2dfa11c6-6901-40f1-b58a-c2a04a0f8c87)


-------------------


# \b : 단어경계 --> /\bYa/ --> Ya인데 단어중에서 Ya로 시작하는것
![image](https://github.com/hyunju960429/Regiex/assets/145514544/530b96bf-d27c-4755-a290-b51b193fc583)


------------------

# \b : 단어경계 --> /Ya\b/ --> Ya인데 단어중에서 Ya로 끝나는것
![image](https://github.com/hyunju960429/Regiex/assets/145514544/7c06ff36-3dd8-4d01-a247-8dba42466150)

-------------------------

# \B : 단어경계가 아님 --> /Ya\B/ --> Ya인데 단어중에서 Ya로 끝나지않는것 모두
![image](https://github.com/hyunju960429/Regiex/assets/145514544/e3694249-150e-4cd3-979b-b8ea66519e47)

------------------------

# ^ : 문장의 시작 --> /^Ya/ --> 문장의 시작이 Ya인것
![image](https://github.com/hyunju960429/Regiex/assets/145514544/c75ee402-ee17-471c-acf3-197fe5e9b5d0)

------------------------

# $ : 문장의 끝 --> /Ya$/ --> 문장의 끝인 Ya
![image](https://github.com/hyunju960429/Regiex/assets/145514544/21bc116d-54b1-4314-8c9f-6336d7e0c8a7)

------------------------

# . : 어떤 글자(줄바꿈 문자 제외) --> /./ --> 모든 문자(줄바꿈제외)
![image](https://github.com/hyunju960429/Regiex/assets/145514544/56a729b2-61ab-45fc-9e0d-06ef5caa9361)

--------------------------

# \ : 특수문자 --> 특수문자 온점(.)을 찾고자 할때
![image](https://github.com/hyunju960429/Regiex/assets/145514544/9360a058-7c90-49b9-8273-9385e9d3d4c8)

-----------------------------



 4) 특징을 이용하는 방법
    - 
    - 
    - \d  : 숫자
    - \D  : 숫자 아님
    - \w  : 문자(word)
    - \W  : 문자 아님
    - \s  : 공백(space)
    - \S  : 공백이 아닌것



