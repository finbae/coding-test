# coding-test
## programmers

#### 문자열 바꿔서 찾기  
    def solution(myString, pat):  
    myString = list(myString)  
    for i in range(len(myString)):
        if myString[i] == 'A':
            myString[i] = 'B'
            
        elif myString[i] == 'B':
            myString[i] = 'A'
    
    a = ''.join(myString)
    
    if pat in a:
        return 1
    else:
        return 0
        
#### 이어붙인 수
    def solution(num_list):
    answer = []
    answer1 = []
    for i in num_list:
        if i % 2 != 0:
            answer.append(i)
            
    for j in num_list:
        if j % 2 == 0:
            answer1.append(j)
    
    a = ''.join(map(str, answer))
    b = ''.join(map(str, answer1))
    aa = int(a) + int(b)
    
    return aa
