## How to use GitPitch?
 - GitPitch란?
```
MicroSoft사의 PowerPoint 프로그램이 필요한 일반적인 프레젠테이션과는 달리,  
그 어떤 다운로드나 설치 없이 오로지 Markdown의 text edit만으로 멋진 슬라이드쇼를 만들수 있는 서비스
```  
  
  
1. PITCHME.md 만들기

![gp_terminal](./images/gp_terminal.png)  
[출처:https://github.com/gitpitch/gitpitch](https://github.com/gitpitch/gitpitch)

README.md 생성 방법과 동일하게 PITCHME.md를 ```add, commit, push``` 해준다.  

  
2. PITCHME.md 작성하기

![gp_markdown](./images/gp_markdown.png)  
(PITCHME.md 작성 예시)

기본적인 작성법은 Markdown 작성법과 동일하기 때문에 누구나 손쉽게 편집이 가능하며, 데이터 타입에 따른 작성법은 아래와 같다.

 - [Markdown](https://github.com/gitpitch/gitpitch/wiki/Slide-Markdown) 슬라이드
 - [Code](https://github.com/gitpitch/gitpitch/wiki/Code-Slides)와 [GIST](https://github.com/gitpitch/gitpitch/wiki/GIST-Slides) 슬라이드
 - [Image](https://github.com/gitpitch/gitpitch/wiki/Image-Slides)와 [Video](https://github.com/gitpitch/gitpitch/wiki/Video-Slides) 슬라이드
 - [Math Notation](https://github.com/gitpitch/gitpitch/wiki/Math-Notation-Slides)과 [Chart](https://github.com/gitpitch/gitpitch/wiki/Chart-Slides) 슬라이드
 - [Fragment](https://github.com/gitpitch/gitpitch/wiki/Fragment-Slides) 슬라이드  


3. GitPitch Layout 정하기

![gp_theme](./images/gp_theme.jpg)

GitPitch는 기본적으로 위와 같은 6개의 Visual Theme을 제공한다.  
사용자는 각 Theme별로 정해진 글꼴, 색상, 표시형식 등을 이용할 수 있으며,  
따로 설정하지 않을 경우 기본적으로 White Theme이 사용된다.  
Theme을 따로 설정하기 위해선 먼저 PITCHME.yaml 파일을 생성해 주어야 한다.  
그 후 PITCHME.yaml 안에 ```theme : (Theme_name)``` 을 입력한다.

![gp_moon](./images/gp_moon.png)

PITCHME.yaml 파일이 정상적으로 저장소에 push 되면 GitPitch의 Theme 설정이 끝난다.  
기본적으로 제공되는 Theme 대신 사용자정의 Theme을 설정하기 위해선 [여기](https://github.com/gitpitch/gitpitch/wiki/Slideshow-Custom-CSS)를 참고하면 된다.  

  
4. GitPitch Presentation 열기

![gp-url](./images/gp-url.jpg)

작성된 PITCHME.md 파일을 Presentation으로 여는 방법은 매우 간단하다.  
위와 같이 ```https://gitpitch.com``` URL 뒤에 ```사용자의 이름/저장소/branch```를 붙여주면 손쉽게 Presentation을 열 수 있다.

![gp_presentation4](./images/gp_presentation4.png)  
(최종 Presentation 화면)

5. Slidenote 추가하기

![gp_slidenote1](./images/gp_slidenote1.png)

각 슬라이드의 마지막위치에 ```Note : (슬라이드노트 작성)```를 추가한다.

![gp_slidenote2](./images/gp_slidenote2.png)

최종 Presentation 화면에서 ```s```키를 누르면 슬라이드노트와 시간이 표시되는 새로운 창이 열린다.
