**merge operation 

각 픽셀의 데이터의 산수계산_ 각 픽셀을 더하기 빼기 나누기 곱하기 어떤걸 할거냐?? 
하나하나 따져 보는게 이해하기에 좋다. 

![fgdsfdszf](https://user-images.githubusercontent.com/90597861/143025064-99d73b86-c23b-43a1-8264-14bfe8b8e03b.JPG)

*atop 

![hdfgdfs](https://user-images.githubusercontent.com/90597861/145075553-0b4f2786-3c63-44d0-89ae-f23f9a050e31.JPG)

Ab는 A값에 B의 알파값을 곱하고, A의 알파값과 반대되는 알파값을 가진 B를 더한다? 

그럼 A와 B는 합성이 되고 B의 알파값 또한 남아있겠네? 

*average (A+B)/2

![adsfsdasd](https://user-images.githubusercontent.com/90597861/145077177-dbba56a5-6684-4c42-99fd-706da597a989.JPG)

*color-burn darken B towards A  (Image B gets darker based on the luminance of A)

![;lkioui](https://user-images.githubusercontent.com/90597861/145077822-b876b454-5c84-455b-accd-c5420c9f4d56.JPG)

*color-dodge 	brighten B towards A (mage B gets brighter based on the luminance of A) 

![sdfweq](https://user-images.githubusercontent.com/90597861/145078267-4582766c-0962-4527-870b-6cfb0b477244.JPG)

*difference  abs(A-B) How much the pixels differ.

![asdqwfweqr](https://user-images.githubusercontent.com/90597861/145079481-c6f071d5-a658-4fd7-afa5-74d9dd19470d.JPG)

*over A+B(1-a) 

a는 A의 알파값  풀어보면 

1-a 는 알파값의 전환이 된다. (흑과 백이 바뀌는 상황. 1은 알파값의 1, 즉 흰색 불투명을 의미함) 그 값을 B 플레이트에 곱한다. 그럼 B가 가진 알파값은 (1-a)가 된다. (A의 자리만큼 빈다) 그 상태에서 A를 위에 올려준다. 

![dfsdzfs](https://user-images.githubusercontent.com/90597861/143047341-52d751b0-e462-4276-b702-1028a1aa5680.JPG)
![fsdfasdwq](https://user-images.githubusercontent.com/90597861/143047348-3aada266-c9a5-447e-af93-e7722e1e2ebf.JPG)
![ascdsdzcwdq](https://user-images.githubusercontent.com/90597861/143048335-78df9d76-9226-47c7-b7ef-2ef53735baeb.JPG)

stancil과 plus을 포함한다. 

*exclusion A more photographic form of difference.

![uhjg](https://user-images.githubusercontent.com/90597861/145080485-60caae2e-7629-4d24-b2dc-bea147e936fd.JPG) 

*in Ab  Only shows the areas of image A that overlap with the alpha of B

![qew](https://user-images.githubusercontent.com/90597861/145082359-73597522-d77e-411f-9e1f-6fca19794530.JPG)

*mask Ba 

B에 A의 알파값을 곱하면 B는 A의 알파값만큼만 붙투명하겠네. (in의 반대) 

![qwedqwfcadsf](https://user-images.githubusercontent.com/90597861/145082661-563ad027-11d5-43c4-bd64-597762d31bbf.JPG)

*matte Aa+B(1-a) 

A에 A의 알파값을 곱한다고? 그럼 A는 알파값 1인 부분만 남고 나머지는 불투명. 거기에 B(1-a)를 더하면 뭐야 오버하고 같은거 아님? 아 프리멀트 과정을 해결해 주는구나. 

![hfgdrseqwqw](https://user-images.githubusercontent.com/90597861/143067978-e9d780fa-045d-46dc-9d70-07d0c891295d.JPG)

*out A(1-b) 

B의 알파값의 반대를 A에 적용 
![ereweds](https://user-images.githubusercontent.com/90597861/143075713-433ea402-870d-4a7a-8558-b59e3ff3e90b.JPG)

*Under A(1-b)+B 

out에서 B를 더한다? 

![ERWEWDCS](https://user-images.githubusercontent.com/90597861/143076408-2de5c9f6-fd7f-4890-9c7b-51b88368e606.JPG)

그냥 over를 a,b 소스를 반대로 한거 같은데?? 

*xor A(1-b)+B(1-a) ?

![image](https://user-images.githubusercontent.com/90597861/145083817-6bff9ef1-cee6-46df-aaee-ccaa7d85f6d1.png)

