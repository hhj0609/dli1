JetsonNano AI basic
=============
<b> 1. Jetson Nano  세팅 준비물</b>
<br>
<br>
<TT> Sd 카드</TT>
<small><br>
<TT> CSI 웹캠</TT>
<small><br>
<TT> USB Data 케이블 </TT>
<small><br>
<TT> 쿨링팬 </TT>
<small><br>
<TT> 지지대</TT>
<small><br>
<TT> WIFI Dongle</TT>
  <small><br>
<TT> 무선 마우스<span>&#183;</span>키패드</TT>
    
<b> ubuntu <span>&#183;</span> 쿨링팬 설치 </b>

-------------  
JetsonNano Setting
-------------

<TT> 2GB JetsonNano Se</TT> 
    
![Jetson-nano-labeled-01](https://user-images.githubusercontent.com/108248472/196337513-8e8b4551-7b4d-4e56-a5e2-358ecbe0cda6.png)    

<TT> JetsonNano Setting </TT>   
    
![jetson nano setting](https://user-images.githubusercontent.com/108248472/196337173-8193eacc-75de-4b20-9beb-3b6b07280179.jpg)

<b>terminal Open</b>
```
sudo apt-get upgrade
sudo apt install python3-pip #스크린 캡처 기능 설치
sudo pip3 list
sudo -H pip3 install -U jetson-stats
pip3 list| grep jetson
reboot!! #컴퓨터를 재부팅 합니다
jtop #젯슨나노의 온드를 체크    
```    
<b>온도에 따라 쿨링팬 활성화</b>
```
sudo sh -c 'echo 128 > /sys/devices/pwm-fan/target_pwm' #echo 128의 숫자를 변경함에 따라 쿨링팬의 회전 수가 변경된다.
```
-------------    
Getting Started with AI on Jetson Nano (한국어 진행) Study
-------------
<b> https://courses.nvidia.com/courses/course-v1:DLI+S-RX-02+V2-KR/

    HeadlessMode
    Headless Mode 상태로 구동을 하면 GUI(그래픽 유저 인터페이스)를 사용하지 않는다. 
    GUI 사용시에 드는 많은 메모리를 절약할 수 있어서 장점이 많다.

<b> 노트북에 연결을 하기 위한 서버 연결</b>
``` 
ssh <username>@192.168.55.1 # <username>에 자신이 만든 ubuntu 아이디로 작성
mkdir -p ~/nvdli-data #data #디렉토리 추가
#도커 컨테이너를 실행
#젯슨나노 CSI카메라 메모리를 활용하기 위해 SWAP 변경 코드 작성
``` 
windowPowercell 접속
  
clasficaition
-------------
![스크린샷(289)](https://user-images.githubusercontent.com/108248472/196335548-221745be-0cb5-47fb-8964-fbb866dc4369.png)
    <b> # Adataset / tumbs_up : 100, tumbs_down : 100 </b>

```
# Combine all the widgets into one display
all_widget = ipywidgets.VBox([
    ipywidgets.HBox([data_collection_widget, live_execution_widget]), 
    train_eval_widget,
    model_widget])

display(all_widget)
```
Image Regression Project
-----
![스크린샷(287)](https://user-images.githubusercontent.com/108248472/196352188-59f06367-fd9d-4506-af0c-ad7a7e4818d7.png)
  <b> # Adataset / nose : 50, Right_eye : 50. Left_eye : 50 </b>

  
  
-------- 
 
