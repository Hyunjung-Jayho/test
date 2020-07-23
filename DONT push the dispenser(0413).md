```markdown

```

<img width="871" alt="MI2RL_logo" src="https://user-images.githubusercontent.com/55417425/77146652-e4a44700-6ace-11ea-9e69-3d38b3f35392.png"><br>



# DONT push the dispenser

* This program is developed to defeat novel corona virus(SARS-CoV-19) and overcome the pandemic of COVID - 19 all together with engineering. This project is a contributed by Medical Imaging and Intelligent Reality Lab in Asan Medical Center(AMC-MI2RL) in Seoul, Korea.
* This device is made with a Arduino Nano CH340,  ultrasonic sen and two pieces of sg90 servo motors.
* [Demo Video(YouTube link)](https://youtu.be/2AqtVSnK7Oo)



## Setting Environment and  Rationale

* Setting

  * 필요 부품(@ 주영쌤!!)

  | 부품명                                    | 필요 갯수             |
  | ----------------------------------------- | --------------------- |
  | CH340 board(compatible with arduino nano) | 1ea                   |
  | servo motor                               | 2ea                   |
  | bread board                               | 1ea                   |
  | 9v battery                                | 4ea                   |
  | 9v battery socket                         | 4ea                   |
  | jumper wire                               | (as mush as possible) |
  | HC_SR04 (ultrasound sensor)               | 1ea                   |
  
  -  Support **USB upload and power supply** as well as  **external power supply(DC 5V~12V)**
- Use 5V-pin for 3.3V ~ 5.5V supply and
    use VIN-pin for 6V ~ 12V
  -  Lower than 100 milliamperes(mA) of current is recommended for 5V 핀으로 출력하여 외부 모듈에 전기를 공급하실 때
  - **Warning** :  Diode can be burnt with higher than 100mA, when using USB port power supply
  
* Rationale 

  * Have you ever worried about the possible contamination of pushing the surface of pump of the dispenser, when using hand sanitizer?
  * For whomever feared about potential exposure to contaminations  through public hand sanitizers

![](https://user-images.githubusercontent.com/42925197/77137204-4903de00-6ab0-11ea-937e-0cba5ad5ad16.png)


  * <u>Alcohol rub is recommended and necessary to reduce the cross contamination  especially for health workers or for the people entering the public space, but the surface of the pump could've been contaminated with (many people) and can possibly increase the risk of infection.</u>
  * 의료종사자들이나, 많은 사람들이 모인 장소를 다녀 온 후 알코올이 들어간 소독제로 손을 소독하는 것은 장려됩니다. 하지만 손소독제 펌프의 표현은 다중의 사용으로 오염되어 있을 수 있고 오히려 감염 위험을 높일 수 있습니다. ( WHO 자료 찾아 읽기, 링크도 넣기.)
  * 이 프로젝트는 이러한 작은 위험이라도 줄여 보고자 하는 목적으로 시작되었습니다.



## 1. NEWS(20.03.19): DONT Push Dispenser ver 0.4

* Following the <u>**spirit/goal/목적/aim the prior(선행하는)**</u> project "DONT/WASH", we developed non-contact type of  liquid dispenser in the purpose of reducing the cross contamination occured at the surface of pump-type hand sanitizers.
* (추가 제안) 자동분사타입의 손세정제의 사용이 가능하지 않을 때 이 장치가 유용할 것입니다. 



## 2. Circuit Construction

* Connect jumper wires  to the adequate port referring the image below.

  ![image](https://user-images.githubusercontent.com/55417425/77146927-8b88e300-6acf-11ea-9d17-d67da54c015c.png)

## 3. Quick Guide

* Setting
  1. Download the "Arduino IDE"([You can find and download it by searching from Google](https://www.arduino.cc/en/main/OldSoftwareReleases)). 
  2. Connect CH340 to PC with USB connector
  3. Connect the devices like the image above
  4. After setting  the 기본 세팅 of Arduino IDE, (이 방법이 어디에 나와 있죠?@ 주영쌤)
  5. Open "DONT_dispenser.ino" and upload the **file** to Arduino with "Ctrl +u"  <u>**( 프로그램을 업로드하라고 되어 있는데 DONT_dispenser.ino 파일인가요? A: 네 맞습니다!)**</u>
  6. Unconnect the USB line with PC and connec the 9V battery to (어디?).
* Run the device
  * If the hand approaches within 12cm from the ultrasould 센서?, the device will automatically pump the sanitizer.
  * [How to wash hand properly?](https://www.youtube.com/watch?v=4O0zkBQTgvI)



## 4. To do

* ```
   * 장치 하우징을 통한 선 최소화 (건전지, 손세정제 교체가 용이하도록)-> 3dp 페이지 링크
   * Agile 손세정제 작동 최적화
   * LED 인디케이터 부착
   * 양산 고려 최적화
   * 따라 만들기 쉽게 설계도 및 제작기법, 제작과정 공개
  ```





## 5. Project Contributers