### Rest api 테스트의 모든 것

목차
[1.Open API 란?](#Open-API-란?)
[2. REST API 란?](####REST-API-란?)

스펙기반 테스트 설계
테스트 툴을 이용한 테스트 수행
수행 사례와 빈발 결함

> Open API 의 인기 → 거론 되는 기술이 REST이다. → 구글, 아마존, 네이버 모드가 Open API를 REST 방식으로 지원한다.

#### Open API 란?
- 다양한 기능을 이용할 수 있도록 **공개한 프로그래밍 인터페이스**로 **내부를 모르더라도** 공개된 API를 이용하여 해당 서비스의 기능, 데이터들을 쉽게 이용 가능

#### REST 란?
- 자원을 이름(자원의 표현)으로 구분하여 해당 자원의 상태(정보)를 주고 받는 모든 것을 의미한다.
- HTTP URI(Uniform Resource Indetifier)를 통해 자원(Resource)을 명시하고, HTTP Method(POST, GET, PUT, DELETE)를 통해 해당 자원에 대한 CRUD Operation을 적용하는 것을 의미합니다.

> **CRUD 란?**</br>
> 대부분의 컴퓨터 소프트웨어가 가지는 기본적인 데이터 처리 기능인 Create, Read, Update, Delete를 묶어서 일컫는 말이다. 사용자 인터페이스가 갖춰야할 기능을 가리키는 용어로서도 사용됩니다.
→ 웹 상에 공개되는 Open API의 경우 Restful 웹 서비스로 구현되는 경우가 많다.

___
#### **URI, URL, URN 차이점**</br>
> - URI(Uniform Resource Identifier): 통합 자원 식별자. 인터넷에 있는 자원을 나타내는 유일한 주소이다. URI의 하위 개념으로 URL, URN이 있다.
> - URL(Uniform Resource Locator): 네트워크 상에서 자원이 어디 있는지를 알려주기 위한 규약이다.
> - URN(Uniform Resouce Name): urn:scheme 을 사용하는 URI를 위한 역사적인 이름이다.

![](https://media.vlpt.us/images/jch9537/post/51dcc312-8ecb-4048-80df-cbde40865e7a/image.png)

![](https://media.vlpt.us/images/jch9537/post/88b0c8ac-5870-4cbc-b613-7dd39f510f31/image.png)
___


#### REST(Representational State Transfer)의 장단점
- 장점
    - http 프로토콜의 인프라를 그대로 사용하므로 REST API 사용을 위한 별도의 인프라 구축이 필요 없다.
    - http 프로토콜에 따르는 모든 플랫폼에서 사용이 가능하다.
    - REST API 메시지의 의도하는 바를 쉽게 파악할 수 있다.
    - 서버와 클라이언트의 역할을 명확하게 분리한다.
- 단점
    - 사용할 수 있는 메소드가 4가지 밖에 없다(http method 형태가 제한적이다.)


> **인프라란?**</br>
> 하드웨어, 소프트웨어, 네트워킹 구성 요소 등 IT 환경을 운영하고 관리하는데 필요한 구성 요소</br>
> **플랫폼이란?**</br>
> 응용 소프트웨어를 실행하기 위해 쓰이는 하드웨어와 소프트웨어의 결합이다.


- stateless 함 = 요청을 위해 특정 값, 세션, 쿠키 값을 유지 하지 않음

#### REST API 란?
> **API(Application Programming Interface)란?**
> 데이터와 기능의 집합을 제공하여 컴퓨터 프로그램간 상호작용을 촉진하며, 서로 정보를 교환 가능 하도록 하는 것</br>

> **REST API의 정의**
> - REST 기반으로 서비스 API를 구현한 것


#### RESTful 의 개념
> RESTful은 일반적으로 REST라는 아키텍처를 구현하는 웹 서비스를 나타내기 위해 사용되는 용어이다.
> - 'REST API'를 제공하는 웹 서비스를 'RESTful'하다고 할 수 있다.


![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-7-1024.jpg?cb=1470036438)

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-8-638.jpg?cb=1470036438)

#### REST API의 설계와 스펙

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-12-1024.jpg?cb=1470036438)

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-13-1024.jpg?cb=1470036438)

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-14-1024.jpg?cb=1470036438)

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-15-1024.jpg?cb=1470036438)

![](https://image.slidesharecdn.com/restapi-160801072508/95/rest-api-16-1024.jpg?cb=1470036438)

#### 스펙 기반의 테스트 접근(테스트 설계)