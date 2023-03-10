# Basic



### 3D viewport

- camera
- lamp
- 그리드 1칸 1m

ribbon menu > render > render Image

- 렌더해줌



- 오른쪽 경계에서 우클릭하면, view를 나눌 수 있음.

![image-20230304155402553](/img/split.png)



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



드래그로 조절하는 것들 shift 누르고 하면 미세하게 됨.



## Camera

- wheel
  - zoom
- wheel click
  - rotate canvas
- shift + wheel click
  - move canvas



- viewport
  - 카메라 유효거리 조정 가능.



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



## View

- object
- wireframe
  - 면 날리고 선만 보여줌.
- material
  - material 적용할 때 사실적으로 보여줌.
- render



## Light

- Power
  - 빛 세기 조절
- SHadow
  - Bias > 범위? 조절



## Properties

- 오른쪽 밑의 선택지 많은 창.
- Scene property
  - grid unit 변경 가능.



- modifier properties
  - ![img](/img/modifier_properties.png)
  - subdivision Surfaces
    - 끊겨있는 폴리곤을 부드럽게 이어줌.
    - level을 높일수록 렌더링 오래걸림.
  
  
  
  - 적용되는 순서가 중요함.
    - 위에꺼부터 적용됨.
  - 적용되어 있는 필터같은 느낌이고, 이를 실제 물체 속성으로 넣으려면 각 옵션에서 apply를 누르면 됨.



## Outliners

- collection
  - folder 같은 개념





## Selecting

- alt + left click

  ​	그 선이 이어진 것들을 전부 선택해줌





- h 
  - 선택된 물체를 안보이게 함.
- alt + h
  - 숨긴 물체 전부 킴.



# Edit

### Add Objectd

- Shift + a
  - 다양한 형태 물체 있음.
  - 물체를 추가하면 왼쪽 아래 Add _ 물체명 _ 이라는 속성 조절창이 뜸.
    - 조절창을 끈 이후에는 f9 키로 조절창을 불러올 수 있음.
- 조절창
  - segment
    - 물체의 해상도



### move

- alt + g
  - 현재 선택한 물체를 원점으로 이동시킴.

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

- 중앙 상단

  ![img2](/img/proportional.png)

  - 주변의 vertex를 같이 변형시켜서, 자연스럽게 해줌.



- 우측 상단
  ![i3](/img/toggle.png)
  - 물체를 투명하게 만들어서, 뒤에 있는것도 클릭이 가능하게 함.



### Duplicate

- shift + D
  - 복사중인 상태로 esc를 누르면, 원래 위치에 고정됨.



#### Seperate Object

- P
  - 선택
  - material 등으로 오브젝트를 구분함.



#### select object

- ctrl + l
  - 연결된 vetex를 전부 선택해줌.



#### Extrude

- 면, vertex 등을 복사해서 늘림.



## Sculpting

붓 등으로 직접 모델링을 깍기.

modifier가 다 적용된 상태에서 하는 것이 좋음.

sculping mode에 들어와서 시장.



### Hot keys

- f
  - 브러시 크기 변경
- shift + f
  - strength  변경



> sculp가 준비된 상태.
> ![img](/img/sculpready.png)



- 기본적으로 면을 꺼내는 식으로 작동함.
  - ctrl 누르면 반대로 작동.



### Tools (shortcut)



#### Inflate (i)

- 확장시킴
- 전체적으로 부풀게 하는 느낌



#### Grab (g)

- 특정한 지점을 잡아당김.







## Mode change

mode change console : ctrl + tab

#### Edit mod

- tab





---



#### Snap

- 여러 환경(그리드, 물체 등)에 맞춰서 물체를 움직이거나 확대하게 해줌.

- face 를 선택한 상태로 점을 편집하면, 다른 objecet의 면에 맞춰서 움직임.

  - Project individual Elements
    - 움직일 때 주변의 vertex도 snap의 영향을 받음.

  ![i4](/img/snap.png)

  











## modifiers

- Shrinkwrap
  - 다른 물체에 snap해줌.\





## Scene

- Render Engine
  - Eevee
    - Real time render engine
  - Cycle
    - raytracing 처리



- Shadows
  - Cube Size > Shadow 디테일 조정.
- Ambient Occulusion
  - real time render에서 빛 반사 등을 더 사실적으로 처리해줌.



## Material

> node로 적용하면 기깔나게 가능하나, 어려움.

#### properties

- base color
  - color 설정
- Subsurface
  - scattering
    - 빛이 물체를 동과하는 것.
- Subsurface Radius
  - rgb를 정함.
- Subsurface color



## Render

GPU render 설정

- preference > System > Cycle Render option 선택
- 안하면 CPU로 렌더링함.



리본메뉴 Render > Render Image (F12) or 오른쪽 위의 render view mode  

> 렌더링은 리소스를 많이 먹음.

ctrl + alt + 0 > 카메라 뷰로 이동.



slot에 렌더 설정을 저장해놓고 돌려가며 쓸 수 있음.



view 탭에서 Camera to View 클릭하면, view를 움직일 때 camera가 따라옴.

- 카메라 위치 이동하고 싶을 때 사용.



## Texture

### Texturing

- material에 여러 작업을 위해 노드 에디터 필요.





#### nodes

- Noise Texture

  - 랜던한 노이즈를 섞음

- Color Ramp

  - 레벨링 조절의 확장판.
  - 그라데이션 등을 색을 지정해서 넣어줌.

  ![i](/img/colorramp.png)



- Image Texture
  - 2D Image를 3D에 매핑해야 함.
- Texture Coodinate
  - 적용될 좌표 배열을 적용함.

- Bump
  - 표면을 울퉁불퉁하게 하기 위해서,
    특정 값을 물체에 수직인 방향의 무언가로 바꾸어줌.





### Texture Painting



# Node editor

- 리본메뉴 shading 클릭시 뜸.

![i6](C:\Users\User\Documents\Github\study-blender\00_basic\nodeeditor.png)

- 노드들은 left 에서 right 방향으로 작동함.



#### Shortcuts

- shift + a
  - node 추가

- right click drag
  - 연결된 노드들을 자름.
- ctrl + shift
  - 지금 선택한 노드까지만 적용된 결과를 보여줌.
  - 이걸 쓰면 노드를 자르고 연결할 필요 없이 각각이 어떻게 작용하는지 알 수 있음.
