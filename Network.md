#### 홈페이지가 켜지는 과정

![](http://www.tcpschool.com/lectures/img_webbasic_10.png)

> 1,2) 사용자가 웹 브라우저를 통해 찾고 싶은 웹 페이지의 url 주소를 입력합니다.</br>
> 3) 사용자가 입력한 url 주소 중에서 도메인 네임(domain name)부분을 DNS 서버에서 검색합니다.</br>
> 4) DNS 서버에서 해당 도메인 네임에 해당하는 IP 주소를 찾아 사용자가 입력한 url 정보와 함께 전달합니다.</br>
> 5,6) 웹 페이지 url 정보와 전달 받은 ip 주소는 http 프로토콜을 사용하여 http request 메시지를 생성합니다. 이렇게 생성된 http request 메시지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 해당 ip 주소의 컴퓨터로 전송됩니다.</br>
> 7) 이렇게 도착한 http request 메시지는 http 프로토콜을 사용하여 웹 페이지 url 정보로 변환됩니다.</br>
> 8) 웹 서버는 도착한 웹 페이지 url 정보에 해당하는 데이터를 검색합니다.</br>
> 9,10) 검색된 웹 페이지 데이터는 또 다시 http 프로토콜을 사용하여 http reponse 메시지를 생성합니다. 이렇게 생성된 http response 메시지는 TCP 프로토콜을 사용하여 인터넷을 거쳐 클라이언트로 전송됩니다.</br>
> 11) 도착한 http response 메시지는 http 프로토콜을 사용하여 웹 페이지 데이터로 변환됩니다.</br>
> 12) 변환된 웹 페이지 데이터는 웹 브라우저에 의해 출력되어 사용자가 볼 수 있게 됩니다.</br>

> - 브라우저는 서버에서 데이터를 받아 표현하는 역할을 담당하고 있다.
> - 도메인 네임이란? 넓은 의미로는 네트워크상에서 컴퓨터를 식별하는 호스트명을 가리키며, 좁은 의미에서는 도메인 레지스트리에게서 등록된 이름을 의미한다. 이를 통틀어서 '웹 주소'라고 부르는 경우도 있다.
> - TCP 프로토콜(전송 제어 프로토콜)이란? 네트워크 7계층 중 4계층인 전송계층에 속하는 중요 프로토콜로 네트워크 망에 연결된 컴퓨터의 프로그램 간 데이터를 순서대로, 에러없이 교환할 수 있게 하는 역할을 합니다.

#### 브라우저에게 어떻게 문서가 전달될까?(http 프로토콜과 네트워크에 대해 알아야한다.)
http(hypertext transfer protocol)의 약자로 인터넷상에서 데이터를 주고받기 위한 프로토콜(약속)이다.

데이터는 오디오/비디오/이미지/텍스트 등 어떠한 데이터의 종류를 가리지 않고 모두 Http 프로토콜을 이용해 전달하고 전달 받을 수 있습니다. 
브라우저는 http 통신을 통해서 사이트 문서를 가져오고 이를 해석해 화면에 출력하게 됩니다.

![](https://www.gatevidyalay.com/wp-content/uploads/2018/09/Hyper-Text-Transfer-Protocol-HTTP.png)

모든 컴퓨터와 서버는 네트워크를 통해 외부에서 접근합니다.
이때 IP 주소가 필요하며 사용자는 url를 이용하여 접근하려 합니다.
때문에 이를 해석하기 위해 DNS 서버로 접근하여 해당 도메인 네임에 맞는 IP를 받아 옵니다. 

#### 브라우저는 서버에게 어떻게 데이터를 받아올까?
브라우저는 서버에게 웹사이트 문서를 받아오기 위해 클라이언트에서 Request 요청을 만들어 서버에게 전달합니다. 
서버는 Request를 해석하고, 요청에 해당하는 Response를 전달하게 됩니다. 클라이언트에서는 서버에서 전달해준 Response를 이용해 화면에 표현하게 됩니다.

HTTP 프로토콜의 데이터 형식은 크게 HEADER 와 BODY로 구성되어 있습니다. HEADER에는 서버가 인식할 수 있는 약속된 형식을 따라야합니다.

![](https://lh3.googleusercontent.com/proxy/k_Z9U2rsRIn2oZZn2QM05DeIkm0mljkXhxLYVZZstbWCvnYnaw8U_vWApjdKrNfroiwcHQ6XeNeNKbPkmjO2TH4xHgZeX97My7stOZg7dsQlVCThAiKnsnQvYcuRLhwuxkxQJMHYAsTaxczdJrxXII1Yn3yHOotzYuXwKUro)