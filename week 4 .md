**merge operation 

각 픽셀의 데이터의 산수계산_ 각 픽셀을 더하기 빼기 나누기 곱하기 어떤걸 할거냐?? 
하나하나 따져 보는게 이해하기에 좋다. 

![fgdsfdszf](https://user-images.githubusercontent.com/90597861/143025064-99d73b86-c23b-43a1-8264-14bfe8b8e03b.JPG)

*over A+B(1-a) 

a는 A의 알파값  풀어보면 

1-a 는 알파값의 전환이 된다. (흑과 백이 바뀌는 상황. 1은 알파값의 1, 즉 흰색 불투명을 의미함) 그 값을 B 플레이트에 곱한다. 그럼 B가 가진 알파값은 (1-a)가 된다. (A의 자리만큼 빈다) 그 상태에서 A를 위에 올려준다. 

![dfsdzfs](https://user-images.githubusercontent.com/90597861/143047341-52d751b0-e462-4276-b702-1028a1aa5680.JPG)
![fsdfasdwq](https://user-images.githubusercontent.com/90597861/143047348-3aada266-c9a5-447e-af93-e7722e1e2ebf.JPG)
![ascdsdzcwdq](https://user-images.githubusercontent.com/90597861/143048335-78df9d76-9226-47c7-b7ef-2ef53735baeb.JPG)
stancil과 plus을 포함한다. 

*atop_ Ab+B(1-a) ??

Ab는 A값에 B의 알파값을 곱하고, A의 알파값과 반대되는 알파값을 가진 B를 더한다? 

그럼 A와 B는 합성이 되고 B의 알파값 또한 남아있겠네? 

*mask Ba 
B에 A의 알파값을 곱하면 B는 A의 알파값만큼만 붙투명하겠네.

*matte Aa+B(1-a) 

A에 A의 알파값을 곱한다고? 그럼 A는 알파값 1인 부분만 남고 나머지는 불투명. 거기에 B(1-a)를 더하면 뭐야 오버하고 같은거 아님? 아 프리멀트 과정을 해결해 주는구나. 

![hfgdrseqwqw](https://user-images.githubusercontent.com/90597861/143067978-e9d780fa-045d-46dc-9d70-07d0c891295d.JPG)


