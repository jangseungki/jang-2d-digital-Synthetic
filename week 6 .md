*누크에서의 크로마키 노드 

스크린을 배경으로 찍은 소스들로 주로 쓰는 노드 (꼭 스크린에서 찍었다고 쓰는건 아님)
![DFQ](https://user-images.githubusercontent.com/90597861/146696936-93097821-a8d5-4f29-956a-8e66c98a4bff.JPG)

스크린에서 찍지 않았지만 다양한 상황에서 쓰는 노드 

![SQ](https://user-images.githubusercontent.com/90597861/146696953-afd8ded1-b00f-43e2-b30f-b459eff2cf6d.JPG)

각 상황에 맞게 유리한 키어를 쓰면된다. 

*KEY LIGHT 

스포이드를 이용해 키가 되는 색을 선택해서 색상 차를 이용해 키가 되는 색을 빼는 것. 

![keylight_bluescreen](https://user-images.githubusercontent.com/90597861/146697351-e5c051c3-18e0-43f3-830d-cfe011224eb0.png)

합성이 될 소스 

![keylight_bg](https://user-images.githubusercontent.com/90597861/146697362-010a105a-187c-4b5b-9947-98241445e5ec.png)

배경이 되는 소스 

![keylight_side_panel_566x201](https://user-images.githubusercontent.com/90597861/146697410-077a3cfd-9fd0-4641-a2f2-35cababd916c.png)

스크린 컬러는 가장 중요한 매개변수이며 다른 작업을 수행하기 전에 항상 스크린컬러를 선택해야 한다. 
녹색 또는 파란색 커튼의 색상으로 설정해야 한다.사각형을 파란색 픽셀 위로 드래그 하여 이미지에서 직접 화면 색상을 선택. 선택한 픽셀의 평균값이 사용된다.
화면 색상 옆에 있는 색상 견본을 클릭하여 스포이드를 활성화, 뷰어에서 Ctrl/Cmd+Shift+Alt 를 누른 상태에서 직사각형 영역을 파란색 픽셀 위로 클릭하고 드래그한다. 
대부분의 경우 화면 색상을 선택하면 화면 매트가 생성되고 전경이 흐려지므로 이것이 키를 수행하는 데 필요한 전부다.

![keylight_final](https://user-images.githubusercontent.com/90597861/146697556-9781483b-596b-4000-85e2-3694bfde2bd0.png)

합성본.

화면 색상을 설정하면 매트가 생성 된다. Screen Matte 
화면 색상을 설정하면 전경에서도 얼룩이 지워지지만, 얼룩 제거 바이어스 를 사용하여 얼룩 을 더 많이 제거 가능하다.

우리는 결과물의 키가 잘 빠졌는지 확인하기위해 뷰를 달리할 수 있다.

화면 색상을 선택한 후 매트(스크린 매트)를 만들고 전경도 디스필했다면 다양한 뷰로 결과물을 확인할 수 있다. 
배경 위에 전경의 최종 합성을 rgba로 출력하거나 다른 곳에서 합성하기 위해 프리멀트 되었거나 언프리멀트된 상태로 출력가능하다. 
오른쪽 이미지는 왼쪽 이미지에서 스크린 컬러를 선택한 후의 상태 디스플레이를 보여준다. 

![keylight_greenscreen_264x193](https://user-images.githubusercontent.com/90597861/146700329-f1a9b4e5-e43f-4395-849f-56e6be409e31.png)
![keylight_greenscreen1_264x193](https://user-images.githubusercontent.com/90597861/146700342-8cdaba7b-2485-4120-ba7a-e2b08468701a.png)

검은색 픽셀은 최종 합성에서 순수한 배경인 영역
흰색 픽셀은 순수한 전경 영역을 표시

회색 픽셀은 최종 합성에서 전경 픽셀과 배경 픽셀이 혼합된 것. 이러한 회색 픽셀은 배경과 물체의 합성에서 잠재적인 물체를 나타낼 수 있음 (비춰보인다던가)

ClipWhite parameter를 사용해서 이 문제를 해결할 수 있다. 반대로 배경을 분명히 하게 하는 파라미터는 ClipBlack parameter.

배경 픽셀
이미지의 픽셀 채도가 화면 색상과 같거나 더 크면 블루 스크린 배경의 픽셀이 되며 해당 픽셀은 완전히 투명하고 검은색으로 설정된다.

![1_48_377x192](https://user-images.githubusercontent.com/90597861/146701295-5208f64e-bc51-46ba-8d26-4926a86e1ef0.png)

에지 픽셀
픽셀의 채도가 화면 색상보다 작으면 전경 개체의 가장자리가 되며 픽셀에서 화면 색상의 일부를 빼고(스필링) 이미지를 반투명으로 설정

![keylight_edge_pixel_377x188](https://user-images.githubusercontent.com/90597861/146701351-c0c91d27-12f5-4ac5-bedd-13c0c3c6893f.png)

전경 픽셀
픽셀의 기본 구성 요소가 화면 색상의 기본 구성 요소와 동일하지 않으면 전경 픽셀이 있고 알파는 완전히 불투명하게 설정

![keylight_graph_377x192](https://user-images.githubusercontent.com/90597861/146701375-4c0ffdf0-358e-4c1b-a3e3-9495f2f95126.png)

*출처_https://learn.foundry.com/nuke/content/reference_guide/transform_nodes/tracker.html
