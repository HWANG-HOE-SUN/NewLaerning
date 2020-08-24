# NewLaerning
새로 알게 됐거나 헷갈리는 개념들 정리
# LOC vs ILOC
주소 : https://lemontia.tistory.com/886

#공통점 df.loc[[행], [열]]
#행을 필터링할땐 동일하다.
df1.loc[:2]
df1.iloc[:2]

#열 접근방법에서 차이가 난다.

df1.loc[:2,["label1","label2","label3"]] #열 이름으로 접근

df1.iloc[:2,1:4] #열 번호 인덱싱으로 접근


# args vs Kwargs (핸즈온에선 kargs라고도 많이씀)

args(non keyworded arguments)
#개수제한없이 튜플형태의 인자를 받아온다.

예제코드]
def func(*args):

   print(args)
   
   print(type(args))
   
func(1,2,3)

-> 1,2,3
<class 'tuple'>

kwargs(keyworded arguments)
#개수제한없이 딕셔너리형태의 인자를 받아온다.

예제코드]

def func2(**kwargs):

   print(kwargs)
   
   print(type(kwargs))
   
func2(a=1,b=2)

->{ 'a':1, 'b':2 }
<class 'dict'>


