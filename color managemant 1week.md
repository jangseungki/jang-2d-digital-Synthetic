# 영상은 3가지로 말할 수 있다
> 1. 기록하고자하는 대상이 뭔가? (뭘 찍냐)    <span style="color:red">     <span style="color:blue">
> 2. 기록하는 매체가 뭔가? (무엇으로 찍냐)
> 3. 그것을 무엇으로 재현하는가? (재현 디스플레이가 뭐냐)
> > 이것들은 빛을 통해서 말한다. 그래서 빛의 리얼리즘을 확보하는게 중요하다 (기록하는 매체의 DR의 중요성 하이라이트 클리핑 쉐도우 크러슁,그것은 곧 감정이입)

### 모든 기록하는 매체는 안구를 기반으로 한다 
> 우리가 빛이 많은 공간에서 너무 밝아 대상을 못보는 상황이 생기지는 않으니까 (안구는 빛에 따라 순응)
>> 그것처럼 카메라에선 **ISO**로 조절 (빛의 민감도)
>> 모든 카메라에선 Base Sansitivity가 존재한다 (BS)


ARRI ALEXA 35 ISO에 따른 계조변화

![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/2246b587-ba1a-4d17-9dab-a95428c3b9cd)

VENICE has two base ISO
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/d15df5d5-6910-4faf-a398-aaf35d72b5c8)

# 이런 ISO의 변화는 영상물의 콘트라스트 변화를 가져온다 (조명의 차이가 생김) 
> Tonality: tone&manner (빛과 분위기) 
> Tonality = key+contrast
>> high key,middle key,low key// high contrast, normal contrast, low contrast ( 하이키+로우콘=뷰티,멜로 예시)
>> **즉 메세지를 결정한다**
### 또한 ISO의 변화는 그레인의 차이를 가져온다는 것 (물성의 차이를 가져온다)
> 영화 파이트 클럽의 거친 물성 or 멜로 영화의 부드러운 물성 ~~마띠에르~~ 
> 그레인과 노이즈는 엄연히 다름, 내가 밝은 곧에서 일부로 감도를 올려찍는건 그레인, 암부가 어두워서 억지로 끌어올리는건 노이즈
> ~~내가 마띠에르를 이해하고 알면 그것을 아는 클라이언트를 만난다~~

# 기초개념
## 색은 파장으로 나뉜다 > 단파장(B) 중간(G) 장파장(R)
**안구의 색자극은 RGB(파장)으로 > 신경의 색전달(뇌는 파장으로 색을 인식하는게 아님 즉 간상체와 추상체로 명도와 색을 구분해서 인식,YCbCr은 디지털 비디오가 뇌처럼 인식하는법) > 대뇌의 색인지(HSL)** 모든 색보정의 커리큘럼  
HSL
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/d9bf049d-048a-4462-acbb-95d23c1958c4)
## 우리의 뇌는 명도로 형태를 이해 (색이 아닌) 
**YCbCr** 
> Y는 명도 CbCr은 크로마(색)을 의미 > ~~즉 밝기정보와 색상정보를 따로 인식한다~~ proress422HQ 에서 프로레스는 코덱, 4는 명도 22은 크로마를 의미 (크로마서브 샘플링)
>
> - Luminance (brightness) - Y
- Blue colour difference - Cb
- Red colour difference - Cr

- YCbCr has its origins in television broadcasting. When the world was transitioning from black and white to colour broadcasting, it allowed the use of just one signal for the broadcast of both black and white and colour images. Black and white TV sets could use only the Y (luminance) signals to display black and white images, whereas colour TV sets would also use the Cb and Cr signals to display in colour. Similar encoding methods are the YUV and YPbPr methods.
- 
> ![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/d144a308-3367-4ab6-8762-c4e09f286e59)
> 
1. The camera generates an RGB image from the light received by the image sensor.
2. The RGB image is encoded into a YCbCr signal, which is what is recorded and transmitted to viewing devices.
3. The display device (computer, TV set or monitor) decodes the YCbCr signals and converts them back into RGB for display.
**chroma key 

✔✔YUV,YCbCr/YPbPr what is a chroma sampling? 

To humans, variations in brightness are easier to see than colour differences. Chroma (colour) subsampling is a method that makes use of this to reduce the colour information when converting RGB files to YCbCr signals to enable smaller data files. 4:2:2 and 4:2:0 refer to different methods of chroma subsampling.

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

![FDEFD](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/3646e4da-9638-4d61-86b3-fba815376824)


Red,Green,Blue 빛의 3요소 컬러별로 8비트(2의 8승)-256단계의 명암 표현 가능 시스템 
8bit RGB 즉, 24bit 컬러 시스템은 256의 3승으로 천육백만(16,777,216) 컬러 표현 가능 
>RGB(0.0.0)= Black, RGB(255.255.255)= White 
>추가 Win 10에서의 32비트=RGB 8비트 3배 + 알파값 8비트 
>맥OS의 2015년 이후(알캐피탄 이후) RGB 10 지원, 하지만 전체 컬러시스템이 아닌 특정앱(사진, 미리보기등)에서만 지원 

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

# 브라운관 TV는 HDTV의 표준
> 브라운관 TV의 전자총
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/60a89843-db71-4f33-baff-360f955ede30)
브라운관은 진공상태의 유리벌브 내의 전자총이 전자빔을 쏘고, 내부의 편향코일(DY)이 직진성을 가진 전자빔을 휘게 해 전체 화면에 고루 퍼지게 합니다. 휘어진 전자는 색을 선별하고 위치를 지정해주는 섀도우 마스크를 통과해, 전면유리에 씌어진 형광막에 부딪히면서 R-G-B(적？녹？청)의 빛을 내게 되는 것
전자총자체는 출력값만 결정하기 때문에 Y값처럼 생각하면 된다
> (전자총1 100(출력값), 전자총2 100, 전자총3 100)=WHITE
> (전자총1 100, 전자총2 0, 전자총3 0 )= RED
## 디지털은 2진법 
8bit RGB 

![KakaoTalk_20210927_014725615](https://user-images.githubusercontent.com/90597861/134845392-bf72398d-8f52-4e3e-95f1-53ec49683a1c.jpg)

![FDEFD](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/3646e4da-9638-4d61-86b3-fba815376824)


Red,Green,Blue 빛의 3요소 컬러별로 8비트(2의 8승)-256단계의 명암 표현 가능 시스템 
8bit RGB 즉, 24bit 컬러 시스템은 256의 3승으로 천육백만(16,777,216) 컬러 표현 가능 
>RGB(0.0.0)= Black, RGB(255.255.255)= White 
~~추가 Win 10에서의 32비트=RGB 8비트 3배 + 알파값 8비트~~
>HD= REC.709 (8~10bit)
>UHD= REC.2020 (10~12bit) 2의 10승 =1024 (1024*1024*1024)=10억 컬러
>~~하지만 아직 디스플레이가 10bit 지원율이 낮다~~ 그래서 그 사이에 나온 시네마컬러 표준 **P3**

# SDR (Standard DR)과 HDR 
> HDR의 시초이자 현재의 주역인 Dolby Vision이 처음 소개된 것은 지금으로부터 약 8년 전인 2014년이었다. Dolby社는 이 Dolby Vision을 차세대 영상기술의 핵심으로 제안했고, 사업화에도 상당부분 성공했는데, Dolby Vision은 PQ(Perceptual Quantizer)라고 부르는 HDR을 위해 고안된 새로운 전광 변환 함수(EOTF, Electric-Optical Transfer Function)에 기반하고 있다. CRT(Cathode Ray Tube, 브라운관)를 기반으로 한 기존의 SDR(Standard Dynamic Range)이 약 0.01-100nits 정도의 휘도(Luminance) 범위를 기준으로 하고 있었던 것에 비해, PQ는 0.005-10,000nits의 어마어마하게 넓은 휘도 범위를 눈으로 보여주고 싶어한다.
> HDR은 획기적이었다. 영화와 텔레비전 방송을 통틀어 아마도 가장 의미 있는 전환점(Turning Point)들 중에 하나가 될 수도 있을 것으로 받아들이는 사람들이 많았다. 흑백에서 컬러 방송으로 전환했을 때, 아날로그에서 디지털로 변화했을 때, SD에서 HD를 거쳐 UHD로 진화했던 것에 버금가거나 혹은 그 이상의 진화를 기대할 수 있을 것 같았다.

물론, 우려도 있었다. 항상 그렇듯 새로운 기술이 정착하는 데에는 하드웨어와 소프트웨어의 발전, 그리고 돈과 시간을 필요로 한다. 비록, Dolby社가 빠른 속도로 표준화와 상업화를 추진하는 데 성공하기는 했지만, 아직 많은 시청자들에게 HDR이 현실이 되지는 못했다.

특히, 코로나19 바이러스가 대유행한 지난 2년 반 동안 많은 국가들이 이동 제한과 봉쇄(Lock Down)를 경험했고, 생산과 기술 개발에서도 코로나 백신분야를 제외하고 의미 있는 발전이 드물어 보인다. 방송 기술적 측면에서도 새로운 기술의 적용이나 발전보다는 방송의 유지가 급선무였다. 이동 제한과 재택근무의 한계를 극복하기 위해 IT 기술이 동원되었고, 원격 제작(Remote Production)에 의존해야 했다. 덕분에 UHD와 HDR, 그리고 IP라는 3대 키워드가 코로나 펜데믹 기간에는 크게 주목을 받지 못했다.

이번 글에서는 그동안 HDR의 발자취를 간략히 살펴보고, HDR이 어디까지 왔고, 또 어디로 가고 있는지, 그리고 HDR의 보급에 병목 현상을 일으키고 있는 결정적인 요소는 무엇지에 대해 논의해 보고자 한다.
>  BT.2100HDR에 대한 개념 정립과 표준화는 이미 완성되었다. PQ는 Dolby Vision이 발표되던 2014년에 발빠르게 SMPTE ST-2084로 표준화가 되었고, 같은 해에 ST-2086에 PQ를 위한 정적 메타데이타(Static Metadata)가 표준화되었으며, 이어 2016년에는 ST-2094에 보다 정확한 PQ 영상 재생을 위해 동작 메타데이타(Dynamic Metadata)가 표준화되었다. 그리고 결국 2016년에 국제방송연맹(ITU)이 ITU-R BT.2100을 발표함으로써 PQ는 HDR 방송을 위한 2개의 변환 함수(Transfer Function)의 하나로써 국제적인 표준이 되었다.

기술 특허의 상용화가 전문인 Dolby社의 발 빠른 행보 덕분에 HDR은 표준과 기술뿐 아니라, 상용화된 서비스로 자리잡게 되었다. 이미 2014년부터 여러 OTT업체들의 호응이 있었고, BT.2100 표준이 발표된 2016년에는 Netflix를 비롯한 많은 업체들이 HDR 영상을 서비스하기 시작했다. 또한, BDA(Blu-ray Disc Association)도 10bit PQ를 기반으로 HDR 영상을 Blu-ray Disc에 담기 시작했다.

BT.2100에 표준으로 등록된 또 다른 HDR 변환 함수인 HLG(Hybrid Log Gamma) 역시 이미 2015년에 일본에서 ARRIB STD-B67로 표준화가 진행되었다. HLG는 말 그대로 기존의 Gamma에 Log를 접목시킴으로써 주로 약 0.01-1,000nits(최대 4,000nits) 정도의 휘도(Luminance) 범위를 커버하기 위해 고안되었다. 영국의 BBC와 일본의 NHK가 합작하여 만들어낸 OETF(Opto-Electrical Transfer Function)인데, 예전의 용어로 말하자면(HDR을 위해 고안된), ‘Camera Gamma’라고 할 수 있겠다.

PQ가 Display에서 재현할 수 있는 절대 휘도 레벨(Absolute Luminance Level)을 기준으로 하고 있는 데 비해, HLG는 상대적이고 가변적이다. 즉, Display가 표현할 수 있는 최대 휘도에 따라 System Gamma를 다르게 적용함으로써, 결과적으로 서로 다른 휘도를 가진 Display에서 보더라도 시청자는 거의 유사한 느낌의 Tone으로 영상을 볼 수 있도록 고안한 것이다.
> 정말 손이 많이 가는 PQ
현재 PQ는 주로 Post Production 작업이 가능한 분야, 즉 촬영이 완료된 후에 충분히 시간을 갖고 HDR로 보정 및 마스터링할 수 있는 분야에서 많이 활용되고 있다. 영화나 Blu-ray Disc 제작이 바로 그것이다. 물론, 처음부터 HDR이 고려된 기획과 촬영을 해야 하지만, 다소 아쉬운 부분이 있기는 해도 기존의 Film 영상이나 SDR 영상을 HDR로 다시 마스터링하는 일도 많이 이루어지고 있다. 흑백이 원본인 Film에 컬러를 넣는 작업을 하거나 일반 2D 영상을 3D로 변환시키는 작업을 하는 것에 비유할 수 있을 것이다. OTT업체나 TV 제조사에서는 이러한 SDR-to-HDR 변환이 자동으로 이루어지도록 고안된 장치를 사용하기도 하지만, 아무래도 일일이 손으로 다듬은 HDR에 비해서 품질은 떨어질 수밖에 없다.

> HDR은 말 그대로 영상을 제작하고 송출하는 전체 과정에서 더 높은 Dynamic Range를 재현할 수 있도록 하자는 것이다. 이를 통해, 기존의 방송이나 영화에서 주지 못했던 더 높은 시각적 사실감과 현장감을 전달하는 것을 목표로 한다. 기존보다 더 넓은 Dynamic Range를 갖는다는 것은 더 넓은 범위의 휘도를 표현하자는 것이다. CRT(Cathode Ray Tube, 브라운관)를 기준으로 정의되었던 기존 SDR TV 시스템 기준의 흑색(Reference Black)의 휘도는 0.01nits였는데, HDR에서는 이 보다 훨씬 더 깊은 0.005nits까지 보여줄 수 있어야 하며, 역시 CRT 기준으로 만들어진 기준 백색(Reference White)의 휘도인 100nits(Super White: 160nits)를 훨씬 뛰어 넘어 현실 세계에서 접할 수 있는 수준인 10,000nits의 매우 밝은 빛도 표현할 수 있도록 해야 한다는 것이 Dolby社의 주장이자 희망이었다.
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/53899b10-1eb8-46bd-aa86-c06701a8b85b)
>SDR과 PQ의 비교(10bit Code와 휘도)



여기서 주의할 것은 HDR의 휘도가 1,000nits라거나 최대 10,000nits까지 올라간다고 했을 때, 이것이 기준 Reference White의 휘도를 뜻하는 것은 아니라는 것이다. 기존 SDR의 경우, 99% 이상의 반사율을 가진 백색판(조명으로 비춘 상태)을 촬영했을 때의 밝기를 100%의 Video Level이라 간주하고 100% IRE 등의 용어로 부르곤 했다. 그리고 상용화된 CRT의 밝기가 보통 80-120nits 사이였기 때문에, 흔히 100nits를 Reference White의 휘도 기준으로 사용했었다. 또한, Reference White보다 더 밝은 빛은 다양한 기법을 통해 Super White의 영역에 담아 왔지만, 추가적인 9%(100-109%)의 범위에 하이라이트 디테일을 충분히 살리면서 담는 것은 현실적으로 매우 어려웠다.

참고로 비록 SDR이 CRT를 기준으로 0.01-100nits 정도의 휘도 범위를 가졌다고 했지만, 실제로 방송 영상을 보는 시청자들의 휘도 범위는 모두 다르다. 2000년대 이후에는 LCD가 CRT를 대체하면서 빠른 속도로 시장의 지배적인 Display로 자리잡았는데, LCD의 Reference White 휘도가 보통 150-300nits 사이이다. 결국, 대부분의 소비자들은 0.01-100nits를 기준으로 만들어진 영상을 실제로는 0.5-200nits 정도의 휘도 범위로 보고 있다고 할 수 있다. OLED를 채용한 프리미엄급 TV의 경우에는 0.005-200nits 사이의 훨씬 더 넓은 휘도 범위를 보여줄 수 있지만, 어차피 컨텐츠 자체가 CRT 혹은 CRT와 유사한 수준의 Reference Monitor로 제작되기 때문에, OLED로 본다고 해서 Dynamic Range가 많이 넓어지는 것은 아니다. 단지, OLED 자체가 더 깊은 Black을 표현할 수 있고, 어두운 계조에서도 색 재현력이 우수하기 때문에, 일반적인 LCD에 비해 더욱 강한 명암 대비와 선명한 컬러를 보여준다.

그런데 PQ는 실제 세계에서의 빛의 범위를 최대한 많이 담고자 최대 10,000nits까지 휘도 범위를 설정한 것인데, 이것이 너무 이상적인 수치라서 문제가 있다. 위의 표에서 보는 바와 같이 HDR이라고 해서 무조건 밝은 영상은 아니며, 상당 부분은 기존의 SDR과 호환되도록 설계되었고, 단지 더 어두운 색과 아주 밝은 색의 디테일을 잘 살리자는 것이 HDR의 목적이다. 따라서 0.005-10,000nits라는 엄청난 휘도 범위에도 불구하고 PQ의 Reference White는 위의 표에서 보다시피 58%의 신호 레벨에서 203nits를 기준으로 하고 있다. 물론, 현실에서는 실제 촬영하는 장면에 따라 실내는 약 100-200nits 혹은 야외는 대략 200-400nits를 Reference White로 설정할 것을 권장하고 있다. 어떤 경우든 사용 가능한 Code의 40%-25% 정도를 하이라이트에 할당해야 한다. 이는 하이라이트 디테일을 표현한다는 차원에서는 멋진 일이지만, 애초 Dolby社에서 제안한 12bit PQ가 아닌(기술적으로, 비용적으로) 현실적으로 사용할 수밖에 없는 PQ10(10bit PQ) 시스템에서는 계조 표현력에 있어서 매우 불리하게 작용할 수 있다.


현실적이고 호환성이 좋은 HLG
PQ와 달리, HLG는 0.01-1,000nits 정도의 휘도 범위를 자연스럽게 재현하는 것을 목적으로 하고 있으며, 라이센스도 없고, Metadata와 같은 잡다한 것도 없어서 방송 현장에 적용하는 것이 훨씬 수월하다. 애초에 BBC와 NHK 방송국 연구소에서 고안하고 계속 보완해 나아가고 있는 표준이라, 후반작업을 할 여력이 없는 스포츠나 공연과 같은 방송 현장에서 특히 효과적이다. 또한, SDR과의 호환성도 좋고, 1000nits 정도만 커버하면 되기 때문에, 하이라이트에 지나치게 많은 Code가 할당되지 않고, 약 75% 정도의 Code로 약 200nits까지 커버하는 데 사용할 수 있으므로, 기존의 10bit 시스템을 그대로 사용하더라도 계조 표현력에 큰 문제가 없다는 점이 상대적으로 PQ에 비해 강점이라 하겠다. HLG는 PQ에 비해(10bit 기준으로) 148개 더 많은 Code를 0.001-203nits의 범위에 사용할 수 있으며, Reference White인 203nits 이하에 약 17% 더 많은 Code 사용이 가능하다.
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/c4143fa5-621b-4968-9cd4-1c696bb280d8)
SDR과 HLG의 비교(10bit Code와 휘도)



위에서 설명 드린 바와 같이, HLG는 PQ에 비해서는 10bit 시스템을 사용하는 데 있어 상대적으로 유리하다. 하지만, 그럼에도 불구하고, 12bit 시스템으로 업그레이드해야 하는 이유는 또 있다. HDR 표준인 BT.2100은 PQ와 HLG라는 새로운 EOTF/OETF를 사용한다는 점을 제외하고는 UHD 표준인 BT.2020의 요소들을 거의 그대로 준용하고 있다. BT.2020이 HDTV 표준인 BT.709와 가장 크게 차별화되는 부분이 바로 해상도, 프레임율, 그리고 광색역(Wide Color Gamut)의 적용이다.

BT.709에 비해 훨씬 넓어진 BT.2020의 색역(Color Gamut) 역시 매끄러운 계조 표현을 위해 더 높은 Color Depth를 요구한다. SDR에서 Reference White인 100nits 이하의 계조를 표현하는 데 876개의 Code가 사용되었다. 단순 무식하게 100nits를 876개의 Code로 나누어 보면, 1개의 Code가 바뀔 때마다 약 0.114nits의 휘도가 차이가 난다. 그런데 PQ에서는 Reference White인 203nits 이하의 계조를 표현하는 데 573개의 Code만 사용할 수 있다. 203nits를 573으로 나누어 보면, 1개의 Code당 약 0.354nits의 휘도 차이가 나는 것이다. 즉, PQ로 제작하는 영상은 SDR에 비해 색을 보정할 때, 1/3 정도의 여유 밖에 없기 때문에, 그만큼 여러가지 제약이 따른다.

![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/721d9e72-3a50-4e8c-b02e-7c90e36a6133)

색역(Color Gamut) 비교(BT.709 vs BT.2020)



색역이 넓어졌을 때에도 동일한 효과가 발생한다. BT.2020의 색역은 BT.709에 비해, 약 1.8배 더 넓은 색역을 가진다. CIE xy나 CIE u’v’와 같은 2차원 색공간에서 계산했을 때 이 정도이고, 실제 3차원 색공간에서 계산하면, 더 큰 차이가 날 것이다. BT.2020은 그만큼 풍부한 컬러를 보여주는 것이기 때문에, 이는 무조건 환영받을 일이다.

하지만, 이번에도 문제는 계조 표현력이다. 동일한 10bit Code 896개를 가지고 2배 더 많은 색 범위를 커버해야 하기 때문에, 결과적으로는 BT.2020으로 제작할 때에는 BT.709로 제작할 때에 비해 컬러와 관련된 각종 파라미터들을 건드릴 때, 약 1/2 수준의 여유밖에 없다는 뜻이 된다.

따라서, HDR을 도입하면서 컬러 조작에 대한 여유폭이 최소 1/3~1/2 줄어들고, 또 광색역을 도입하면서 다시 1/2 정도로 여유폭이 줄어든다면, 이 둘을 합쳤을 때, 손댈 수 있는 여유폭은 단순 무식하게 계산해서 대략 1/4 수준으로 떨어진다고 볼 수 있을 것이다. FPGA(Field Programmable Gate Array) 등 각종 반도체부터 시작해서 이를 활용한 하드웨어와 소프트웨어까지 모두 12bit로 업그레이드되려면 얼마나 많은 시간이 흐르고, 비용은 얼마나 더 상승할지 알기 어렵지만, 반드시 12bit로 가야 하는 이유이다. 물론, 그 동안은 예술적인 측면에서 이른 단점들이 어느 정도 커버되긴 할 것이다.
HDR의 뒷다리를 잡는 결정적인 요인은?
사실, HDR의 보급과 정착에 가장 큰 장애가 되고 있는 것은 바로 Display 기술이다. HDR은 기본적으로 더 깊은 Black과 더 높은 피크 휘도(Peak Luminance)를 구현할 수 있는 Display의 등장을 가정하고 있다. 문제는 충분히 저렴해진 LCD의 경우에는 해상도나 크기 측면에서는 기술적인 문제가 전혀 없었지만, Dynamic Range와 Color Gamut 2가지에 한계가 있다. LCD 자체가 가진 구조적인 한계로 인해 휘도를 올리는 데는 문제가 없지만, 동시에 깊은 Black은 전혀 불가능하다. 불가능한 정도가 아니라, Black 휘도도 따라 올라가 오히려 Contrast는 더 악화된다.

컬러의 경우, 광색역을 구현하기 위해 LCD의 Backlight에 Laser 소자를 사용해 보기도 했지만, 현실적으로 너무 비싸고 HDR 구현이 어렵다. 현실적으로는 Blue LED와 Quantum Dot을 결합한 솔루션이 가성비가 좋았지만, BT.2020에서 규정한 너무 넓은 색역의 85% 정도에 그칠 뿐이었다. 결국, LCD를 2장 겹치고 강한 Backlight를 쏴 주어 깊은 Black과 높은 휘도를 동시에 가능하게 해준 Dual Cell이 등장했지만, 아주 잠깐 시장에서 이슈를 일으키고 곧 사라졌다. 이 Dual Cell의 최초 개발사인 Panasonic LCD는 아예 LCD Panel 제조사업을 포기하고 폐업하기에 이르렀다. 이후, 중국의 LCD Panel 제조사 2곳에서 프리미엄 TV용으로 대형 LCD Panel에 Dual Cell 기술을 적용했으나 이 역시 실패하였다.
![image](https://github.com/jangseungki/jang-2d-digital-Synthetic/assets/90597861/860a380e-c62b-451a-87f9-7c10bddf9a52)
Dual Cell LCD Panel 구조도
처음부터 HDR을 위한 이상적인 Display로 주목받았던 Display 기술은 OLED였다. Backlight의 빛을 액정으로 제어하면서 색을 만들어내는 LCD와 달리, OLED는 스스로 빛을 낼 수 있고, 어두운 계조에서의 발색도 우수하며, 특히 깊은 Black을 표현하는 데(낮은 Black 휘도를 내는 데) 있어 타의 추종을 불허한다. CRT보다도 우수하다. 하지만, 생산 기술이 어려워서 방송용 OLED Panel을 세계 최초로 생산해서 한 때 세계 방송용 Monitor 시장을 지배했던 Sony 반도체 사업부도 결국 OLED Panel 제조사업을 포기하게 되었다.
아직 JDI(Japan Display)가 남아 있지만, 충분히 경쟁력 있는 가격으로 중형과 대형 OLED Panel을 개발 및 생산할 수 있는 기술력과 투자력을 가진 회사는 삼성디스플레이와 LG디스플레이뿐이다. 삼성디스플레이와 LG디스플레이 모두 중국 LCD Panel 제조업체들의 거친 추격을 피해 LCD를 포기하고 OLED로 완전 전환을 하던 중에 코로나19 바이러스가 전 세계적으로 유행하게 되면서 다소 속도가 늦춰졌다. 그러나 최근 들어, 두 회사 모두 중형과 대형 OLED Panel에 집중 투자하면서 생산량이 늘고 있고, OLED를 장착한 프리미엄 TV에 대한 수요도 증가하면서 가격도 점차 저렴해지는 선순환이 기대되고 있다. 특히, 서로 다른 기술을 가진 삼성디스플레이와 LG디스플레이가 경쟁하고, 중국업체들이 추격하는 구도라, 코로나 팬데믹 이후에는 더욱 가속도가 붙기를 기대하고 있다.
정리하자면, HDR의 보급에 있어 병목 현상을 일으키고 있는 가장 큰 요소는 Display 기술이라 하겠다. 10bit 시스템을 사용하는 문제는 약간의 화질 희생이나 다른 보완 기법, 혹은 예술적 보완을 통해 어느 정도 안고 갈 수 있는 문제이고, 이미 어느 정도 극복하면서 사용하고 있다. 그러나 그렇다고 Display 기술이 BT.2100에 정의된 수준까지 발전하기만을 손 놓고 기다릴 순 없지 않을까?

1. HDR은 꼭 1,000nits 이상의 피크 휘도를 구현해야 할까?
그렇지 않다고 본다. 앞서 설명한 바와 같이, SDR 시절에는 100nits의 휘도로도 만족하며 살아왔다. 그리고 HDR의 Reference White도 기본적으로는 203nits 수준이다. 그렇다면, 203nits 이상의 하이라이트는 300-400nits 정도만 되어도 이전보다 훨씬 높은 Dynamic Range를 선사해 줄 수 있다. 하이라이트를 너무 많이 담으려 하기 보다는 현실적으로 OLED로 구현 가능한 300-400nits까지만 담아도 OLED의 깊은 Black을 고려하면, 기존 SDR보다 훨씬 강한 명암 대비와 풍부한 컬러를 구현할 수 있다.

Dolby Vision의 무리한 10,000nits 피크 휘도나 심지어 HLG의 1,000nits 조차 굳이 무리하게 따라 갈 필요가 없다. 어쩔 수 없이 현실적으로 10bit의 PQ10을 사용하듯이 피크 휘도 400nits의 ‘HLG 400’을 새로운 표준으로 삼아 상용화를 서두르는 것이 백 번 낫다고 본다.

2. HDR은 꼭 UHD/4K 해상도에서만 구현해야 할까?
역시 그렇지 않다고 본다. BT.2100의 HDR 표준이 대부분 BT.2020의 표준을 준용하고 있지만, 해상도 측면에서는 오히려 Full HD(1920 x 1080)을 포함하고 있다. 해상도로 인한 혜택은 Display의 크기와 시청거리에 따라 얼마든지 무력화될 수 있기 때문에, 결국 화면의 밝기와 명암 대비, 그리고 컬러, 프레임율 등이 차별화의 주인공일 수밖에 없다. 그리고 Full HD에서 HDR을 구현하는 것은 매우 경제적이기도 하다. 기존의 HDTV 방송 인프라를 약간만 보완하면 되기 때문에, UHD보다 빠르게 도입할 수 있기 있다.

마지막으로 최근에 나온 따끈따끈한 정보를 전달해 드리고자 한다. Ultra HD Forum Guidelines의 Version 2.6이 지난 4월말에 발표되었다. 이전 버전에 비해 눈에 띄는 것은 SDR과 HDR, 그리고 PQ와 HLG간의 변환에 유용하게 사용할 수 있는 LUT와 가이드라인이다. 이전 버전에서 발견된 오류들을 해결하였고, 색재현의 정확성이 향상되었다고 한다. 또한, 차세대 오디오에 대한 정보들도 있고, 현장에서의 적용에 참고하기 위한 다양한 정보들이 수록되었다. Ultra HD Forum의 웹사이트를 참고하기 바란다.
