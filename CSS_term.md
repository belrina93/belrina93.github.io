## 1. WAI-AREA

Web Accessibility Initiative - the Accessible Rich Internet Applications Suite

장애를 가진 사람들의 접근성을 더욱 높이기 위한 방법. 특히 동적인 컨텐츠나 자바스크립트, 에이젝스,HTML  그리고 관련 기술들과 함께 개발된 진화된 유저 인터페이스 제어를 도움



## 2. inline

인라인 함수는 함수의 길이가 매우 짧을 경우에 효율을 높이기 위해서 도입된 방법. 함수 호출 시 별도로 분리된 위치의 레이블로 점프하여 실행되는 일반 함수와는 달리 호출 부분을 함수 전체 코드로 치환하여 컴파일함.

함수의 선언부 앞에 inline 이라는 키워드로 구현됨

## 3.block

 [GCC](https://ko.wikipedia.org/wiki/GNU_%EC%BB%B4%ED%8C%8C%EC%9D%BC%EB%9F%AC_%EB%AA%A8%EC%9D%8C), [MSVC](https://ko.wikipedia.org/wiki/%EB%B9%84%EC%A3%BC%EC%96%BC_C%2B%2B)를 포함한 여러 [컴파일러](https://ko.wikipedia.org/wiki/%EC%BB%B4%ED%8C%8C%EC%9D%BC%EB%9F%AC)를 지원하는 [자유](https://ko.wikipedia.org/wiki/%EC%9E%90%EC%9C%A0_%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4), [오픈 소스](https://ko.wikipedia.org/wiki/%EC%98%A4%ED%94%88_%EC%86%8C%EC%8A%A4), [크로스플랫폼](https://ko.wikipedia.org/wiki/%ED%81%AC%EB%A1%9C%EC%8A%A4%ED%94%8C%EB%9E%AB%ED%8F%BC) [IDE](https://ko.wikipedia.org/wiki/%ED%86%B5%ED%95%A9_%EA%B0%9C%EB%B0%9C_%ED%99%98%EA%B2%BD)이다. [wxWidgets](https://ko.wikipedia.org/wiki/WxWidgets)를 GUI 툴킷으로 사용하는 [C++](https://ko.wikipedia.org/wiki/C%2B%2B) 언어로 개발되어 있다. 플러그인 구조를 이용하여 여러 기능을 사용할 수 있게 되어 있다. 현재 Code::Blocks는 [C](https://ko.wikipedia.org/wiki/C_(%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D_%EC%96%B8%EC%96%B4))와 [C++](https://ko.wikipedia.org/wiki/C%2B%2B), [포트란](https://ko.wikipedia.org/wiki/%ED%8F%AC%ED%8A%B8%EB%9E%80)을 지원하고 있다.



## 4. inline-block



​       			 											 									 							 				  

 

 

 

 

 

​			 			          			 		 	  

 

 







**{ display: inline; }**

대표적으로 <span>이라는 태그의 성질로 content/text 크기만큼만 점유하고
동일 라인에 붙는 성질입니다.
'이 글씨는 **두꺼운** **효과**를 주었다.'와 같이 text 내에 특정 부분에만 스타일을 간단히 줄때 많이 사용되죠.
*- width/height 적용 불가*
*- margin/paddin**g-top/bottom 적용 불가*
*- line-height 원하는 대로 적용 불가(span에 적용안되고 감싸고 있는 div 전체 크기에만 영향 등)*

**{ display: block; }**

반면 block은 무조건 한줄을 점유하고, 다음 태그는 다음 줄로 가버리죠.

**{ display: inline-block; }**

2개의 짬뽕입니다. 제일 중요한 성질 자체는 inline과 비슷합니다.
동일 라인에 여러 태그를 붙일 때 쓸 수 있습니다. 
다만 위 inline의 단점들을 커버하는 것이 inline-block입니다.
*- width/height 적용 가능- margin/padding-top/bottom 적용 가능- line-height 적용 가능***
다만 고려해야 할 것이 있습니다.
*- inline-block 끼리 공백이 생기게 되는데, 이때는 상위 div에 { font-size: 0; } 를 적용하면 해결이 됩니다.*
*- inline-block 끼리 높이가 안맞을시 상위 공백이 생기는데, 이때는 { vertical-align: ---; } 값으로 top 등을 줘서 맞춰주시면 됩니다. *

그래서 결론은? 그렇다면 무조건 inline-block 쓰는게 낫지 않나?

디테일한 보정이 필요하고 예민하신 분들은 inline-block 쓰시는게 낫고,
text 내의 특정 부분 스타일 등 간단한 것들은 그냥 inline 쓰시면 됩니다.

inline 쓴다는 것은 <span>을 그냥 쓰는 것을 뜻하고(default 값이기 때문에), inline-block은 따로 div 등에 display: inline-block 속성 코드를 타이핑하고 여타 속성에 신경을 써줘야한다는 것을 뜻합니다.(손이 좀 더 간다~ 뭐 이 정도입니다.)**[출처]** [ display: inline 과 inline-block 차이 / 인라인 인라인블록 차이](http://blog.naver.com/leesd88/220682157303)|**작성자** [삼계탕](http://blog.naver.com/leesd88)