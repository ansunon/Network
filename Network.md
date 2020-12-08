#### 홈페이지가 켜지는 과정

1. 사용자가 브라우저를 실행합니다.
2. 접속하고 싶은 사이트의 url를 주소창에 입력합니다.
3. 브라우저는 입력된 url 의 서버에게 사이트 정보를 받아와 이를 화면에 표현합니다.
4. 표현된 정보로 사용자가 활용합니다.

> 브라우저는 서버에서 데이터를 받아 표현하는 역할을 담당하고 있다.

#### 브라우저에게 어떻게 문서가 전달될까?(http 프로토콜과 네트워크에 대해 알아야한다.)
http(hypertext transfer protocol)의 약자로 인터넷상에서 데이터를 주고받기 위한 프로토콜(약속)이다.

데이터는 오디오/비디오/이미지/텍스트 등 어떠한 데이터의 종류를 가리지 않고 모두 Http 프로토콜을 이용해 전달하고 전달 받을 수 있습니다. 
브라우저는 http 통신을 통해서 사이트 문서를 가져오고 이를 해석해 화면에 출력하게 됩니다.

![](https://www.gatevidyalay.com/wp-content/uploads/2018/09/Hyper-Text-Transfer-Protocol-HTTP.png)

모든 컴퓨터와 서버는 네트워크를 통해 외부에서 접근합니다.
이때 IP 주소가 필요하며 사용자는 url를 이용하여 접근하려 합니다.
때문에 이를 해석하기 위해 DNS 서버로 접근하여 해당 도메인 네임에 맞는 IP를 받아 옵니다. (받은 IP를 가지고 한번에 서버에 접근할 수 없으며, IP를 알고 있는 다른 서버에 접근하면서 경유하여 접근하게 됩니다.) 

#### 브라우저는 서버에게 어떻게 데이터를 받아올까?
브라우저는 서버에게 웹사이트 문서를 받아오기 위해 클라이언트에서 Request 요청을 만들어 서버에게 전달합니다. 
서버는 Request를 해석하고, 요청에 해당하는 Response를 전달하게 됩니다. 클라이언트에서는 서버에서 전달해준 Response를 이용해 화면에 표현하게 됩니다.

HTTP 프로토콜의 데이터 형식은 크게 HEADER 와 BODY로 구성되어 있습니다. HEADER에는 서버가 인식할 수 있는 약속된 형식을 따라야합니다.

![](https://lh3.googleusercontent.com/proxy/k_Z9U2rsRIn2oZZn2QM05DeIkm0mljkXhxLYVZZstbWCvnYnaw8U_vWApjdKrNfroiwcHQ6XeNeNKbPkmjO2TH4xHgZeX97My7stOZg7dsQlVCThAiKnsnQvYcuRLhwuxkxQJMHYAsTaxczdJrxXII1Yn3yHOotzYuXwKUro)