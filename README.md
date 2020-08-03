# NewLaerning
새로 알게 됐거나 헷갈리는 개념들 정리
# LOC vs ILOC
# 주소 : https://lemontia.tistory.com/886

#공통점 df.loc[[행], [열]]
# 행을 필터링할땐 동일하다.
df1.loc[:2]
df1.iloc[:2]

# 열 접근방법에서 차이가 난다.
df1.loc[:2,["label1","label2","label3"]] #열 이름으로 접근
df1.iloc[:2,1:4] #열 번호 인덱싱으로 접근

