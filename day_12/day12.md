필수 1
-----

1. 파이썬의 list 자료형과 tuple 자료형의 차이를 서술해주세요.

* list와 tuple 모두 순서가 있고 중복이 가능하지만 / list와는 다르게 tuple은 수정과 삭제가 불가능하다.
  좀 더 중요한 자료들을 다룰 때 사용한다(tuple)

2. 프로그래밍을 할 때 tuple 자료형으로 관리해야 할 데이터의 예시를 들어주세요. (세 번째 ‘리스트 튜플 (3)’ 강의 참고)

* 중요데이터. 고객 계좌 번호 등의 변경되면 실행이 오작동 되거나 심각한 오류가 생기는 것 등

3. 아래 문구에서 알맞은 선택지를 선택해주세요.
list 자료형과 tuple 자료형은 순서를 (가지고 / 가지지 않고) 중복을 (허용한다 / 허용하지 않는다.)

* list 자료형과 tuple 자료형은 순서를 가지고 중복을 허용한다.

4. list 자료형의 extend 함수와 append 함수의 차이를 서술해주세요. ( 설명하기 어렵다고 판단되시면 코드로 예시를 들어주셔도 좋습니다. )

* append와 extend 둘 다 새로 추가하는 것은 맞지만 append는 list 자체를 추가하고 extend는 새로운 원소로서 하나의 리스트로 추가한다.

extend method
`a = [1, 2, 3, 4, 5]
b = ['a', 'b']
a.extend(b)
print(a)
-> [1, 2, 3, 4, 5, 'a', 'b']`

append method
`a = [1, 2, 3, 4, 5]
b = ['a', 'b']
a.append(b)
print(a)
-> [1, 2, 3, 4, 5, ['a', 'b']]`

필수 2
-----

다음은 변수에 list를 할당한 코드입니다. 해당 코드를 기준으로 아래의 요구사항을 충족한 코드를 작성해주세요.
li = [5, 2, 3, 1, 4]

1. li에서 1이라는 값을 출력하는 print문을 작성해주세요. ( 인덱싱 활용 )

* print(li[3])

2. li의 요소 2개를 더해서 5가 출력되게 하는 print문을 작성해주세요.

* print(li[1]+li[2])

3. li의 1번 인덱스부터 3번 인덱스까지 슬라이싱하여 출력하는 print문을 작성해주세요. (결과값: [2, 3, 1])

* print(li[1:4])

4. 변수 li를 이용해서 [5, 2, 3, 1, 4, 5, 2, 3, 1, 4]를 출력하는 print문을 작성해주세요.

* print(li*2)

5. li 리스트의 끝에 6이라는 요소를 추가해주는 코드를 작성해주세요.

* li.append(6)

6. li 리스트를 오름차순으로 정렬시켜주는 코드를 작성해주세요.

* li2 = reversed(li)
print(list(li2))

* li.sort()

7. li 리스트에서 3이라는 값을 찾아 지워주는 코드를 작성해주세요.

* li.remove(3)

8. li 리스트에서 2번 인덱스 자리에 6이라는 숫자를 추가해주는 코드를 작성해주세요. (결과: [5, 2, 6, 3, 1, 4])

* li.insert(2, 6)

필수 3
----- 

다음은 변수에 tuple을 할당한 코드입니다. 해당 코드를 기준으로 아래의 요구사항을 충족한 코드를 작성해주세요.
tu = (5, 2, 1, 2,  (4, 3, 6))

1. tu 안에 있는 4라는 값(요소)를 출력하는 print문을 작성해주세요.

* print(tu[4][0])

2. 1 이라는 값이 tu에서 어느 인덱스에 위치하는지를 출력해주는 print문을 작성해주세요.

* print(tu.index(1))

3. 2 라는 값이 tu 에서 몇 개 있는지를 출력해주는 print 문을 작성해주세요.

* print(tu.count(2))

4. 10 이라는 값이 tu 안에 있는지를 출력해주는 print문을 작성해주세요. ( 결과값은 False입니다. )

* print(10 in tu)

필수 4
-----

다음은 변수에 list 자료형인 값을 할당한 코드입니다. 해당 코드를 기준으로 아래의 요구사항을 충족한 코드를 작성해주세요.
li = [5, 2, 1, 2,  [4, [3, 7, 2], 6]]

1. li안에서 7을 출력하는 코드를 입력해 주세요.

* print(li[4][1][1])

다음은 변수에 list 자료형인 값을 할당한 코드입니다. 해당 코드를 기준으로 아래의 요구사항을 충족한 코드를 작성해주세요.
li = [7,5,3,2,0,9,1,4,8,6]

2. li를 내림차순으로 정렬하는 코드를 짜 주세요.

* li.sort(reverse=True)
  print(li)

필수 5
-----

지금까지 과제로 작성한 모든 코드를 직접 입력해보며 실습해보세요.
아래 웹사이트에서 파이썬 코드를 입력하면 우측에 그림(기호)로 표현해주어 데이터가 어떻게 입력되는지 쉽게 알 수 있습니다.
http://www.pythontutor.com/live.html#mode=edit
실습 후 아래에 Generate permanent link 를 누른후 우측에 만들어진 URL(주소) 를 Github Gist 에 넣어주세요.

http://www.pythontutor.com/live.html#code=li%20%3D%20%5B5,%202,%203,%201,%204%5D%0Aprint%28li%5B3%5D%29%0Aprint%28li%5B1%5D%2Bli%5B2%5D%29%0Aprint%28li%5B1%3A4%5D%29%0Aprint%28li*2%29%0Ali.append%286%29%0Aprint%28li%29%0Ali.sort%28%29%0Aprint%28li%29%0Ali.remove%283%29%0Aprint%28li%29%0Ali.insert%282,6%29%0Aprint%28li%29%0A%0Atu%20%3D%20%285,%202,%201,%202,%20%284,%203,%206%29%29%0Aprint%28tu%5B4%5D%5B0%5D%29%0Aprint%28tu.index%281%29%29%0Aprint%28tu.count%282%29%29%0Aprint%2810%20in%20tu%29%0A%0Ali%20%3D%20%5B5,%202,%201,%202,%20%5B4,%20%5B3,%207,%202%5D,%206%5D%5D%0Aprint%28li%5B4%5D%5B1%5D%5B1%5D%29%0A%0Ali%20%3D%20%5B7,5,3,2,0,9,1,4,8,6%5D%0Ali.sort%28reverse%3DTrue%29%0Aprint%28li%29%0A&cumulative=false&curInstr=23&heapPrimitives=nevernest&mode=display&origin=opt-live.js&py=3&rawInputLstJSON=%5B%5D&textReferences=false

심화 1
-----

1. 아래의 print문은 에러를 발생시킵니다. 아래의 코드가 ‘10Hello’라는 값으로 출력되도록 하는 print문을 작성해주세요.
a = [10, 100, 'hello']
print(a[0] + a[2]) # error!

* print(str(a[0]) + a[2])

2. li = [1, 3, 5, 4, 2]라는 리스트를 [5, 4, 3, 2, 1]로 만들어 출력시키는 코드를 작성해주세요.

* li.sort(reverse=True)
  print(li)

3. 튜플 자료형 tu = (1, 2, 3)을 이용해서 (1, 2, 3, 4)가 출력되도록 하는 print문을 작성해주세요.

* tu = tu + (4,) 
  print(tu)

심화 2
-----

파이썬에는 문자열을 일정 규칙에 따라 list 자료형으로 만들어주는 split 함수와 https://wikidocs.net/13#split
list 자료형을 문자열로 만들어주는 join 함수가 있습니다. https://wikidocs.net/13#join
이 두 함수와 아래의 문자열 변수 make_email을 활용해서 이메일 형식의 문자열(fastcampus@gmail.com)을 출력하는 코드를 작성해주세요.
         
주의: make_email에 split 함수를 사용한다고 해서 make_email의 값이 변하지는 않습니다. 문자열을 List 자료형으로 변환한 그 값을 변수에 할당하는 등의 방법을 사용해서 코드를 작성해주세요.
ex) hello = 'a:b:c:d'
hello.split(':')
print(hello) # 'a:b:c:d'

`
make_email = 'fastcampus, gmail.com' 
  make_email.split() 
  -> ['fastcampus,', 'gmail.com']

  make_email.split('fastcampus : gmail.com')
  -> ['fastcampus, gmail.com']

  "@".join(['fastcampus', 'gmail.com'])
  -> 'fastcampus@gmail.com'
  `


심화 3
-----

리스트를 정렬하는 방법에는 sorted()와 .sort()의 두 가지 방법이 있습니다.

두 방식의 방법상의 차이점과 리턴값을 기반으로 두 방식이 어떻게 다른지 서술해 주세요.
	
2. li를 내림차순으로 정렬하는 코드를 짜 주세요.

.sort : method  원본을 결과값으로 바꾼다.  method는 클래스의 함수를 의미한다.
sorted() : 함수 원본을 그대로 두고 결과값을 바꾼다.

`li = [1, 3, 5, 9, 8, 10, 2, 4, 7, 0, 6]`

` print(sorted(li, reverse=True))
 -> [10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0] `

 `print(li.sort(reverse=True)) 
 -> None          `



심화 4
-----

Q1> 아래 date 리스트에서 각 날짜 년, 월, 일 중 ‘일’ 만 빼서 day 리스트에 넣어보세요.
date = [‘2019-06-16’, ‘2019-06-17’, ‘2019-06-18’]
정답 예시: day = [‘16’, ‘17’, ‘18’]

* day = [date[0][-2:], date[1][-2:], date[2][-2:]]
  print(day)

Q2> 아래 unordered 리스트를 오름차순으로 정리해보세요.
* 새로운 리스트를 만들지 말고 해결해보세요.
* .sort를 쓰지말고 해결해보세요.
unordered = [5, 4, 1, 2, 3]
정답 예시: unordered = [1, 2, 3, 4, 5]

* print(sorted(unordered))
	
심화 5
-----

다음과 같은 리스트가 주어졌을 때 가장 큰 숫자 3개와 가장 작은 숫자 3개를 슬라이싱을 이용해 출력하는 코드를 작성해주세요.
number = [3, 5, 6, 10, -3, -10, -123, 45, 78, 90, 1, -11, -23, 23]
실행 예: 
largest: [45, 78, 90]
smallest: [-11, -23, -123]

* number.sort()
 print(number)
 -> [-123, -23, -11, -10, -3, 1, 3, 5, 6, 10, 23, 45, 78, 90]
 
  largest = sorted(number)[-3:] 
  -> [45, 78, 90]
 
  smallest 
  sorted(number)[:3]
 


	
읽어보기
------

오늘 많은 새로운 함수를 써보셨습니다. 이게 다가 아니고 앞으로도 수많은 기능과 함수 등등을 마주치실텐데요. 어떻게 알아보고 적용하는 게 최선일까요? 그리고 찾아본 모든 것들을 다 외우면 될까요?

이에 대한 저의 생각을 정리해봤습니다. 앞으로 파이썬이나 다른 언어 등을 공부하실 때 도움이 되었으면 좋겠습니다.
오늘 고생하셨습니다!!

https://gist.github.com/shoark7/eeb85a521f004c1f63bef7ebea9c9b74




