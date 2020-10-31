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
입력은 int(input(),진법)으로 변환
- 비트연산(<< >>, ~, &, |, ^)   
- 원하는 숫자 개수 만큼 한 줄에 숫자 입력받기(한 줄에 입력되는 수 만큼 자동 조정됨 x)    
nums = [int(x) for x in input().split()]   
Ex) 1 2 3 4 5인 경우 nums = [1,2,3,4,5] 저장됨   
- print문 줄간격 제거 : print(a, end='')   
- 거듭제곱 : a의 b제곱 = a ** b    

```
