# Ch04
1-4까지

4_1_List
"""
이름 : 박민지
날짜 : 2021/04/06
내용 : 파이썬 자료구조 리스트 실습 교재 p.84
"""

#리스트 생성
list1 = [1, 2, 3, 4, 5] #숫자들이 원소(순서) [0,1,2,3,4]
print('list1 type :', type(list1))
print('list1[0] :', list1[0])
print('list1[2] :', list1[2])
print('list1[3] :', list1[3])

list2 = [5, 3.14, True, 'Apple']
print('list2 type:', type(list2))
print('list2[0]:', list2[0])
print('list2[1]:', list2[1])
print('list2[2]:', list2[2])
print('list2[3]:', list2[3])

list3 = [[1, 2, 3], [4, 5, 6], [7, 8, 9]] #행렬[0] [0,1,2],행렬[1] [0,1,2],헹렬[2] [0,1,2]
print('list3 type :', type(list3))
print('list3[0][2] :', list3[0][2])
print('list3[1][1] :', list3[1][1])
print('list3[2][0] :', list3[2][0])

#리스트 덧셈
animal1 = ['사자', '호랑이', '코끼리']
animal2 = ['곰', '기린']

result = animal1 + animal2
print('result :', result)

#리스트 수정, 추가, 삭제
nums = [1, 2, 3, 4, 5]
nums[1] = 7
print('nums :', nums)

nums[2:4] = [8, 9, 10]
print('nums :', nums)

nums[3:5] = []
print('nums :', nums)

4_2_Tuple
"""
이름 : 박민지
날짜 : 2021/04/06
내용 : 파이썬 자료구조 튜플 실습 교재 p.92
- 튜플 : 고정 리스트(추가,삭제, 수정 불가능)
"""

#튜플 생성
tuple1 = (1, 2, 3, 4, 5)
print('tuple1 type :', type(tuple1))
print('tuple1[0] :', tuple1[0])
print('tuple1[4] :', tuple1[4])
print('tuple1[0] : %d' % tuple1[0])
print('tuple1[4] : %d' % tuple1[4])

tuple2 = ('서울', '대전', '대구', '부산', '광주')
print('tuple2 type :', type(tuple2))
print('tuple2[0] : %s' % tuple2[0])
print('tuple2[4] : %s' % tuple2[4])

#tuple 수정, 추가, 삭제
nums = (1, 2, 3, 4, 5) #튜플은 ()생략 가능 nums = 1,2,3,4,5 가능
#nums[0] = 6
#nums[4] = []
#당연히 수정 추가 삭제 불가능 하기에 오류뜸


4_3_Set
"""
이름 : 박민지
날짜 : 2021/04/06
내용 : 파이썬 자료구조 set(집합) 실습 교재 p.96
"""

#set(집합) 생성
set1 = {1, 2, 3, 4, 5, 3} #집합은 순서 없음
print('set1 type :', type(set1))
print('set1 :', set1)

set2 = set('Hello World') #저장은 'H' 'e' 'l' 'o' 'W' 'r' 'd' ' ' 이렇게 저장됨, 중복허용X
print('set2 type:', type(set2))
print("set2 :", set2)

#집합 출력(리스트 변환)
list1 = list(set1) #set을 list로 변환
print('list1[0] :', list1[0])
print('list1[1] :', list1[1])
print('list1[2] :', list1[2])

list2 = list(set2)
print('list2[0] :', list2[0])
print('list2[1] :', list2[1])
print('list2[2] :', list2[2])


4_4_Dictionary
"""
이름 : 박민지
날짜 : 2021/04/06
내용 : 파이썬 자료구조 Dictionary 실습 교재 p.98
"""

#Dictionary(=key value) 생성
dic1 = {1: '서울', 2: '대전', 3: '대구', 4: '부산', 5: '광주'}
dic2 = {
    'A': 'Apple',
    'B': 'Banana',
    'C': 'Cherry',
}

dic3 = {
    101: [1, 2, 3, 4, 5], #list
    102: (6, 7, 8, 9, 10), #list but tuple
    103: {'한국', '미국', '중국', '일본'}, #set
    104: {'p1': '김유신', 'p2': '김춘추', 'p3': '이순신'} #dic 안에 dic
}

#dic 출력
print('dic1 type:', type(dic1))
print('dic1[1] :', dic1[1])
print('dic1[4] :', dic1[4])
print('dic1[5] :', dic1[5])

print('dic2 type:', type(dic2))
print("dic2['A'] :", dic2['A']) #안의 '를 표시하기 위해 "로 바꿈
print("dic2['B'] :", dic2['B'])
print("dic2['C'] :", dic2['C'])

print('dic3 type:', type(dic3))
print("dic3[101][0] :", dic3[101][0])
print("dic3[101][2] :", dic3[101][2])
print("dic3[102][4] :", dic3[102][4])
print("dic3[103] :", dic3[103])
print("dic3[104]['p1'] :", dic3[104]['p1'])

#dic 응용
dictionaries = [dic1, dic2, dic3] #list로 만듬

print('dictionaries type:', type(dictionaries))
print('dictionaries[0][4] :', dictionaries[0][4])
print('dictionaries[1][A] :', dictionaries[1]['A'])
print("dictionaries[2][104]['p2'] :", dictionaries[2][104]['p2'])

ch01, 1_1_Hello
"""
날짜 : 2021/04/05
이름 : 박민지
내용 : ch01. 파이썬 개발환경 설정 교재 p15
"""

print('Hello World')
print('Hello Python')

#한줄 출력
print('Hello', end=',')
print('Student')
