필수 1
-----


1. 파이썬 데이터타입에는 어떤 것들이 있는지 강의에 나온 8가지를 작성해주세요.

* Boolean, String, Numbers, List, Set, dictionaries, tuples, bytes 

2. print("fastcampus"[0:4])는 어떻게 출력되는지 작성해주세요.

* 앞 lens의 길이가 4번째까지인 fast가 출력된다.

3. 아래 파이썬에서 사용되는 연산자들이 있습니다. 해당 연산자들이 어떤 연산을 하는지 작성해주세요.
	+	-	*	/	//	%	**	+=	*=

* + : 더하기, - : 빼기, * : 곱하기, / : 나누기, // : 몫, % : 나머지, ** : 제곱, 
  += : 왼쪽 변수에 오른쪽 값을 더하고 결과를 왼쪽변수에 할당, a += b : a = a+b, *= : 왼쪽 변수에 오른쪽 값을 곱하고 결과를 왼쪽 변수에 할당
  
필수 2
-----

1. v_float이라는 변수에 9.0이라는 값을 할당했습니다. 이 v_float 변수의 값을 정수(int)로 바꾸는 코드를 작성해주세요.

* v_flaot = 9.0
  print(int(v_flaot))

2. 이스케이프 문자를 활용해서 ‘I like "apples"’ 를 출력하는 print문을 작성해주세요.

* print('I like \"apples\"') = I like "apples"
escape_str1 = "I like \"apples\""
print(escape_str1)
= I like "apples"

3. "fastcampus" 라는 문자를 슬라이싱하여 "fast" 로 출력되게 하는 print문을 작성해주세요.

* print("fastcampus"[0:4])

4. -7의 절대값을 출력하는 print문을 작성해주세요.
	
* print(abs(-7))

필수 3
-----

1. "Nice Day"라는 문자열의 길이를 출력하는 print문을 작성해주세요.

* print(len("niceday"))

2. ‘\\ ^_^ \\’  이라는 문자열을 이스케이프 문자를 사용하지 않고 출력하도록 하는 print문을 작성해주세요.

* print(str(r"‘\\ ^_^ \\’"))

3. 연산자를 사용하여 ‘*’을 100개 출력하는 print문을 작성해주세요.

* str_o1 = '*'
print(str_o1 * 100)

4. print 함수를 한 번 사용하여, 문자열을 아래처럼 출력하는 코드를 작성해주세요.
나는
고양이를
좋아한다.

* multi_str1 = \
    """
    나는
    고양이를
    좋아한다.
    """
print(multi_str1)

심화 1
-----

1. divmod 함수를 이용하여 100을 8로 나눈 몫을 변수 m, 나머지를 변수 n에 할당하는 코드를 작성해주세요.

* n, m = divmod(100, 8)
print(n, m)

2. 문자열 슬라이싱을 통해 "python"이라는 문자열을 거꾸로 뒤집는 print문을 작성해주세요.

* print(list(reversed('python')))


3. 문자열 슬라이싱을 통해 "hello world"라는 문자열의 짝수번째 문자만 출력되도록 print문을 작성해주세요.
(프로그래밍에서 인덱스는 0부터 시작합니다. 1번째 인덱스부터 계산해주세요.  결과값: 'el ol')
	
*  a = 'hello world'
print(a[1::2])
-> el ol

심화 2
-----

1. "hello python"이라는 문자열의 첫글자를 대문자로 바꿔 출력이 되도록 print문을 작성해주세요.

* print("Capitalize:", "hello python".capitalize())

2. "nice man"이라는 문자열을 "cool man"으로 바꾸어(대체되어) 출력이 되도록하는 print문을 작성해주세요.

* a = "nice man"
print("replace:",a.replace("nice", "good"))

3. 주민번호가 담긴 person이라는 변수에서 이 사람이 태어난 달과 날을 출력하는 print문을 작성해보세요. 
person = ‘881220-1234567’  # 주의 : 이 줄을 그대로 복사붙여넣기 하면 따옴표 ‘ ‘ 가 제대로 인식되지 않을 수 있습니다.
( 881220-1234567 이라고 하면 1220이 출력되면 됩니다. )

* person = '881220-1234567'
print(person[2:6:])

심화 3
-----

다음 링크는 문자열과 관련된 함수를 정리한 내용들을 담고 있습니다. 문자의 수를 세는 count 함수부터 strip 함수까지 쭉 읽어본 뒤 다음 슬라이드의 문제를 풀어보시기 바랍니다 :)
https://wikidocs.net/13#_19
count, find, index, join, upper, lower, lstrip, rstrip, strip

*

심화 4 
-----

" python is a good language   "라는 문자열이 있습니다. 이를 good이라는 변수에 담은 뒤 아래와 같은 조건을 만족하는 print문을 작성해주세요.
( 이전 슬라이드의 내용을 참고하여 문제를 풀어주세요. )

1. a의 개수가 몇개인지 출력하는 print문을 작성해주세요.

* good = " python is a good language "
print(good.count('a'))

2. 위 문자열의 양쪽 공백을 없애 출력하는 print문을 작성해주세요.

* print(good.strip())

3. 위 문자열을 모두 대문자로 바꾼 문자열을 출력하는 print문을 작성해주세요.

* print(good.upper())

4. 문자 d가 어느 위치에 있는지를 출력하는 print문을 작성해주세요.

* print(good.find('d'))
