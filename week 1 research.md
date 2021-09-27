✔✔what is a color space? 

색의 특정 조직을 뜻함 > 각 color space는 표현 가능한 범위를 말함 
물리적인 특정 색상은 특정된 생공간에 할당되거나 수학적으로 구조화 될 수 있음 

✔✔why? 

특정 장치에서 다른 장치로 색상을 재현하려 할떄 color space는 그림자/하이라이트(다이나믹 레인지) 색상채도유지 가능여부, 손상정도 파악에 용이 

![KakaoTalk_20210926_231418138](https://user-images.githubusercontent.com/90597861/134844385-e35ec36d-2f89-4f8b-922b-f010ebd24e6f.jpg)

✔✔Histoy 

![KakaoTalk_20210926_235844573](https://user-images.githubusercontent.com/90597861/134844751-21d1c8c1-6f10-4818-9051-9bf677827bec.png)

Munsell color system 
사람이 인식하는 색들을 비슷한 순서대로 붙여서 배열시 원을 이룸 >> color circle 
채도와 명도는 직선방향으로 증감 
>>원통 형태의 3차원 색좌표 표현가능 
색을 공간 좌표에 나타낸 것을 color space or color system 
CIE 1931 표준관찰자 
(색이 균등치 못한 먼셀 색공간으로 비디오 및 각종 산업에서의 개선요구)
많은 사람들을 대상으로 색과 관련된 실험 후 평균치 CIE 1931 RGB, CIE 1931 XYZ. CIE 1976 LAB등 다양한 형태로의 개선 
*CIE외에도 다양한 색공간 존재 (용도와 환경에따라 사용) 

✔✔what is gamut? 

gamut= 색영역 
모든 색공간은 각각이 재현 가능한 색상의 범위가 존재
디스플레이, 카메라, 동영상 포맷과 같은 곧에서 구현가능한 색상의 범위 (성능지표)의 기준 예시) 재현 가능한 색영역에 따라 NTSC72%, sRGB 100%, Adobe RGB 99% 지원 
>>>높은 Gamut? = 표현 가능한 색상의 수가 많아 자연스러운 계조표현 가능 

✔✔what is RGB?

디지털 영상에서 가장 기본이 되는 색공간 
빛의 삼원색 
Red, Green, Blue -Key color 
각 색상이 최대값이 되면 흰색이 되는 감산 혼합 예시) sRGB, Adobe RGB 

✔✔sRGB 

HP, Microsoft 사에서 제안 for computer 
HDTV 시스템에서 사용하는 Rec 709와 동일하 개머트(둘은 감마 차이로 인해 sRGB > Rec 709로 그대로 변환시에 어두워지는 현상, 최근 소프트웨어는 자동보정은 가능) 

1✔✔Apple RGB 

애플사에서 제안 
sRGB가 녹색계열을 온전히 구현하지 못하는 문제를 해결하기 위함 (보다 더 넒은 개머트) 
촬영시 이미지를 모니터로 확인시에 채도가 낮고 녹색이 진한 경우레 촬영된 이미지 파일의 색공간을 제대로 지원하지 못하기 떄문 
> 이 경우 대부분 sRGB 지원 모니터로 Adobe RGB 촬영본을 보는 경우가 대부분 

✔✔YUV,YCbCr/YPbPr what is a chroma sampling? 

Chroma subsampling YCbCr 4:2:0
(크로마:색차+ 서브샘플링: 전체 데이터의 샘플링이 아닌 데이터 일부를 추려서 샘플링) 
>>> Y(LUMA) UV(크로마:색차)로 구성된 YUV 컬러 모델은 Y는 그대로 두고 크로마정보를 서브샘플링하여 전체 영상 데이터를 줄여주는 기술 (Y값도 감마 보정은 이루어짐) 

✔RGB Color Model 
현재 모든 디지털 디스플레이는 어떤 중간 과정을 거치던 최종본은 RGB 컬러 모델로 영상 구현 
>영상을 4:2:0 으로 압축해도 최종본은 RGB로 다시 변환 
컴퓨터 모니터, 디지털 TV, 블루레이, PC, MAC, 디지털 캠코더, Win 10등 대부분 디지털 영상 관련 기기나 소프트 웨어는 8bit RGB시스템을 기본으로 함 
>(만약 10비트 12비트 디스플레이 기기를 구매했더라도 최종컬러는 8비트일 확률이 높다. 10비트로 제작된 영상 소스를 10비트로 처리 가능한 디스플레이 기기에서 봐야하기에)

✔8bit RGB 

![KakaoTalk_20210927_014725615](https://user-images.githubusercontent.com/90597861/134845392-bf72398d-8f52-4e3e-95f1-53ec49683a1c.jpg)

Red,Green,Blue 빛의 3요소 컬러별로 8비트(2의 8승)-256단계의 명암 표현 가능 시스템 
8bit RGB 즉, 24bit 컬러 시스템은 256의 3승으로 천육백만(16,777,216) 컬러 표현 가능 
>RGB(0.0.0)= Black, RGB(255.255.255)= White 
>추가 Win 10에서의 32비트=RGB 8비트 3배 + 알파값 8비트 
>맥OS의 2015년 이후(알캐피탄 이후) RGB 10 지원, 하지만 전체 컬러시스템이 아닌 특정앱(사진, 미리보기등)에서만 지원 

✔YUV,YCbCr Color Model >YCbCr은 YUV의 인코딩 시스템 

위의 RGB모델은 밝고 어두운 값이 포함됨 
반면 YUV는 밝기 정보와 컬러 정보가 부리된 컬러모델 
YUV= Y(루마,휘도) UV(크로마,색차) 

✔why we use YUV?

RGB라는 직관적인 컬러 모델의 존재에도 YUV를 사용하는 2가지 이유 
YUV는 흑백TV에서 컬러TV 변환하는 과정에서 생김 (컨텐츠의 하위 호환성과 더불어 데이터 저장의 효율성 때문에 사용 
>> 여기서 말하는 데이터 저장의 효율성이 크로마 샘플링 
흑백TV시절 명암을 표시하는 휘도인 Y값만 존재, 이후 컬러TV방송 시대 도래 이후 UV값을 더해 컬러영상 
시간이 흘러 아날로그 YUV는 YCrBr이라는 디지털 인코딩 시스템으로 발전 (이와 구분하여 아날로그 인코딩 시스템은 YPbPr로 표기 

![KakaoTalk_20210927_020753663](https://user-images.githubusercontent.com/90597861/134846445-f3cc32a7-d669-48e0-b0d8-5e702da90e08.jpg)

✔where is green? 

위에서 UV에 대해 컬러라는 용어 대신 색차라는 용어를 사용 
색차는 컬러가 아닌 휘도Y값이 더해져야 하는 값 >> 일종의 좌표값이라고 생각해 (Cb= blue-yellow 축상으로부터의 편차, Cr= red-cyan 축상으로 부터의 편차) 

![KakaoTalk_20210927_022952543](https://user-images.githubusercontent.com/90597861/134846646-550297c9-bb1f-4fe3-96c0-f84944e50fcb.jpg)

✔Chroma Subsampling의 원리 

Y값은 인간의 눈에 민감하여 데이터 축소가 힘듬 
대신 CbCr값을 변환해도 인간의 눈은 거의 인식 불가 

4:4:4에서의 각 숫자의 의미 

샘플링 단위는 4열 2행의 총 8개의 픽셀 

![KakaoTalk_20210927_024755900](https://user-images.githubusercontent.com/90597861/134849164-279bf63b-bd65-403d-a5e5-eb2ab76d1264.jpg)

4:4:4에서 
맨앞의 숫자 4는 고정값- 가로 4개의 픽셀이라는 의미 
두번쨰 4는 첫번쨰 행의 숫자, 만약 2가 되면 파란색과 진보라는 무시. 노란색과 연보라만 샘플링 
세번째 4는 두번째 행의 숫자, 같은 원리 
만약 0인 된다면 샘플링하지 않는다는 의미 

예시) 4:2:2

![KakaoTalk_20210927_024756995](https://user-images.githubusercontent.com/90597861/134849498-5f83423c-664c-45dc-8644-4528d69c4c2f.jpg)

4:2:0

![KakaoTalk_20210927_024757083](https://user-images.githubusercontent.com/90597861/134849516-3da1b07f-f8dd-4fb8-8b81-9ef19e90a886.jpg)

YCbCr4:4:4 에서 YCbCr 4:2:0

![KakaoTalk_20210927_024924282](https://user-images.githubusercontent.com/90597861/134849575-d776ffff-3e70-4587-ae9d-4e5e434fba2f.jpg)

8개의 픽셀중 2개만 샘프링시 결과물이 너무 다르지 않은가? 
하지만 루마값이 더해진다면 인간의 눈은 크게 인식하지 못함 

![KakaoTalk_20210927_024755785](https://user-images.githubusercontent.com/90597861/134849720-818bc616-7263-4bda-a691-d97f6eac0f98.jpg)

또한 고해상도로 갈 수록 작은 단위의 변화는 눈을 구분하기 힘들어짐(동영상의 경우 더욱 힘들어짐
따라서 4:4:4는 무압축 데이터, 4:2:2, 4:2:0이 널리 사용됨 
YCbCr 4:2:2 
주로 편집 중간과정서 사용 최종본이 4:2:0이라도 편집과정서의 데이터 손실을 고려해 사용된다 
YCbCr 4:2:0 
원본손실은 있지만 폰트를 제외한 동영상이나 이미지에서의 품질저하를 인지하기 힘듬 
4:2:0은 매우 유용한 샘플링 기술 
기술이 계속 발전하여 저장 용량이 높아지고 전송 대역폭이 커지면 샘플링이 불필요해질까? 
>그 시기는 매우 더디다. 정답은 하위 호환성에 있다 
>새로운 기술은 적용에 있어 현실보다 하위호환성이 떨어진다면 소비자들은 가진 모든 영상 기기를 바꾸어야 하거나 그간의 영상을 보지 못하게 됨 

✔✔CMY(CMYK) 
인쇠매체의 핵심 색공간 
CYAN,MAZENTA,YELLOW+BLACK-KEY COLOR 
색을 섞으면 보다 어두워지는 감산 혼합 
>영상기기보다는 프린터 같은 잉크 또는 토너를 사용하는 인쇄매체를 위한 색공간 
>감산혼합으로 표현 불가능한 흰색은 배경이 되는 매체(종이 등)의 색을 그대로 노출하여 사용 

![KakaoTalk_20210927_034622196](https://user-images.githubusercontent.com/90597861/134850501-d5d8eb37-4249-471c-9ca6-a4bbbe3a74e8.jpg)

✔✔Rec.709/Rec.2020 
Rec.709- HDTV를 위한 해상도, 재생률, 색공간에 대한 규정(=BT.709) 
sRGB와 색공간의 개머트가 동일하지만 다른 감마특성 
>Rec.709가 색공간만을 의마하는것은 아니지만 색공간을 말하는 부분에선 색공간을 의미 
Rec.2020-UHD를 권고안으로 709에 비해 2배이상 넒은 개머트 

> 출처: https://en.wikipedia.org/wiki/Color_space
>       https://dvdprime.com/g2/bbs/board.php?bo_table=dpinfo&wr_id=47998
>       https://terms.naver.com/entry.naver?docId=3340383&cid=58161&categoryId=58161
