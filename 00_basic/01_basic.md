# Basic



### 3D viewport

- camera
- lamp
- 그리드 1칸 1m

ribbon menu > render > render Image

- 렌더해줌



## Controls

#### move tool

- 움직일 때 이걸로 잡고 움직임.
- shortcut G
  - G로 움직이는 상태에서 휠을 누르면 축에 고정되어 움직임.
  - or axis(x, y, z)를 입력해서 축에 고정할 수 있음.

#### Rotate tool

- shortcut R
  - R로 움직이고, 
  - 똑같이 x, y, z 클릭해서 축에 고정

#### Scale tool

- S





## Cameras

- wheel
  - zoom
- wheel click
  - rotate canvas
- shift + wheel click
  - move canvas



#### Numpad or `

- 물체 기준 좌/우 상/하 등 정렬

##### 1 3 7

- x, y, z축으로 뷰

##### 5

- orthogonal / Perspective view change (원근 적용)

##### 0

- camera view



### reset view

- 오른쪽 위의 뷰큐브로 조정



## Properties

- 오른쪽 밑의 선택지 많은 창.
- Scene property
  - grid unit 변경 가능.



- modifier properties
  - ![img](/img/modifier_properties.png)
  - subdivision Surfaces
    - 끊겨있는 폴리곤을 부드럽게 이어줌.
    - level을 높일수록 렌더링 오래걸림.



## Outliners

- collection
  - folder 같은 개념





# Edit

### Add Objectd

- Shift + a
  - 다양한 형태 물체 있음.
  - 물체를 추가하면 왼쪽 아래 Add _ 물체명 _ 이라는 속성 조절창이 뜸.
    - 조절창을 끈 이후에는 f9 키로 조절창을 불러올 수 있음.
- 조절창
  - segment
    - 물체의 해상도



### Scale fix

- ctrl + a > scale
  - ctrl + a 메뉴는 이것저것 지금의 기준에 맞게 정리해주는 느낌.



### shade

- 모델에서 우클릭 > shade smooth
  - 실제로 면을 부드럽게 하는 것이 아니라, 보이는것만 그렇게 만듬.
- shade flat 하면 원래대로 돌아옴.



### Edit Surface

- vertex
  - 물체 poly의 한 점.
  - 여러개 클릭해서 면이 이루어지면, 면도 색이 활성화됨.
  - 물체 움직이는거랑 똑같이 클릭하고 G키로 움직일 수 있음.

#### Proportional Editing

- ![img2](/img/proportional.png)
- 주변의 vertex를 같이 변형시켜서, 자연스럽게 해줌.





## Mode change

mode change console : ctrl + tab

#### Edit mod

- tab

