```   
1주차 요약   
- input()은 str형태, int(input())으로 형변환 필요.   
- 파이썬은 and or 사용, if elif else 구조로 구성됨.   
- 입력 여러개 받기 : map 사용   
- 문자 안에 따옴표 : \',\"   
- 문자 길이 : len('문자')   
- 소수점 자리수 및 반올림 : print('%.6f' % round(a,2))   
- .format : {:04d}, {:.2f}위와 동일함   
- 파이썬의 int범위, float범위   
- 몫 : //, 나머지 : %, divmod(a,b)는 몫과 나머지 같이 반환   
- 삼항 연산자 : 결과 if 조건 else (다른결과 if 조건 else 다른결과)   
- 아스키코드 : ord(문자), chr(숫자)   
- 진법변환 : format(숫자, ‘b’/'o'/'x')  ,  format(숫자, ’#b’/'#o'/'#x') 접두어   
a = int(input(),2) -> 2진수 입력을 10진수로 변환       
n=10, format(n,'b') -> 10진수 입력을 2진수로 변환    
입력은 int(input(),진법)으로 변환
- 비트연산(<< >>, ~, &, |, ^)   
- 원하는 숫자 개수 만큼 한 줄에 숫자 입력받기(한 줄에 입력되는 수 만큼 자동 조정됨, 배열형태)    
nums = [int(x) for x in input().split()]   
Ex) 1 2 3 4 5인 경우 nums = [1,2,3,4,5] 저장됨   
- print문 줄간격 제거 : print(a, end='')   
- 거듭제곱 : a의 b제곱 = a ** b   
- 루트 : x ** 0.5   
- 리스트 역방향 접근 : for i in num_list[::-1], 리스트 최대최소 : max,min(리스트)   
```   
   
```
2주차 요약   
- 여러 줄(N개) 입력을 리스트로 만들기 : Nums = [input() for _ in range(N)]
- 문자열 + 연산   
- 튜플 자료형 : () , 다익스트라 최단경로 구할 때 우선순위 큐에 들어가는 값은 튜플로 선언해야 한다.(변경되선 안됨)   
- 사전 자료형 : data = dict(), data["사과"] = 'Apple' , 해시테이블(Hash Table), 검색 및 수정에 있어 O(1) 시간에 처리   
ex) key_list = data.keys(), value_list = data.values() : 키 리스트, value 리스트 반환   
for key in key_list :   
   print(data[key])   
- 집합 자료형 : {}, list에 중복 제거할 때 사용, 순서가 없다. data=set([1,2,3,2])  => {1,3}      
교집합 : a&b(a와 b 모두 속한 값), 합집합 : a|b(a또는 b에 속해있는 값), 차집합 : a-b(a에만 속해있는 값)   
집합 연산 후 결과를 list() 형태로 형변환해야 index 접근 가능함!   
원소 추가(여러개) : add(), updata([]), 원소 제거 : remove()  , 시간복잡도 : O(1)    
- 함수 : def 함수명(매개변수): (반복적인 코드 효율적 처리)
- global 사용법   
- 입력 속도 Up   
1) 1줄에 입력받기(띄어쓰기 기준 - int형)(1차원 배열)import sys   
Data = [int(x) for x in sys.stdin.readline().split()]     
ex)  1 2 3 4 5 => [1,2,3,4,5]   
2) 1줄에 입력받기(띄어쓰기 기준 - 문자열)(1차원 배열)import sys   
Data = sys.stdin.readline().split()   
ex)  a b c d e => ['a','b','c','d','e']     
3) 1줄에 입력받기(띄어쓰기 없는 경우 - 문자열,숫자)(2차원 배열)import sys
Data = sys.stdin.readline().split()   
Data[0] = 'abcde', Data[0][0] -> 'a'    
4) K개의 줄에 입력받기(띄어쓰기 없는 경우 - int형)(1차원 배열)import sys    
Data = [int(sys.stdin.readline()) for i in range(n)]      
ex) 1: 123, 2: 333, 3: 12 -> [123,524,231]   
5) K개의 줄에 입력받기(띄어쓰기 없는 경우 - 문자열)(1차원 배열)import sys    
Data = [sys.stdin.readline() for i in range(n)]      
ex) 1: abc, 2: z, 3: qw -> ['abc','z','qw']      
5) K개의 줄에 입력받기(띄어쓰기 기준 - 문자열,숫자)(3차원 배열) import sys   
names = [sys.stdin.readline().split() for _ in range(n)]      
names[0], names[0][0] -> 첫줄 입력(1차원 배열), names[0][0][0] -> 첫줄 입력 처음 문자 1개     
ex) 1 : 11 12, 2 : ab cd, 3 : abcd 123 -> [['11', '12'], ['ab', 'cd'], ['abcd', '123']]   
6) a,b 같은 형태로 입력받는 경우 import sys    
a,b = map(int, sys.stdin.readline().split())     
- 문자열.(upper(), lower(), isupper(), replace('바꿀문자','새문자'), zfill(개수), find('문자), count('문자')    
- {:2d} : 2자리 숫자, 비어있으면 0채우기   
- range(시작,끝,-1) : 시작부터 1씩감소       
- while 1 : index = name.find('target',index+1) ,, 특정 문자 index 모두 찾기   
- 형변환(int to str) : str(), repr()  | 형변환(str to int) : int()    
- 3개의 수 최소 공배수?? 방법1)
day=1;   
while(day%a!=0 or day%b!=0 or day%c!=0) :   day++;   
- 2차원배열 초기화(nxn)   
arr = [[0]*n for _ in range(n)]   
```    
