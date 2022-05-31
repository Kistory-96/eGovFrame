# eGovFrame

1. 전자정부프레임워크가 뭐냐

https://www.egovframe.go.kr/EgovIntro.jsp?menu=1&submenu=1

전자정부프레임워크의 소개 페이지

​

​

위 페이지에 나온 내용은 아래와 같습니다.

​

등장배경 및 목적

개발프레임워크는 정보시스템 개발을 위해 필요한 기능 및 아키텍처를 미리 만들어 제공함으로써 효율적인 어플리케이션 구축을 지원합니다.

“전자정부 표준프레임워크”는 공공사업에 적용되는 개발프레임워크의 표준 정립으로 응용 SW 표준화, 품질 및 재 사용성 향상을 목표로 합니다.

이를 통해“전자정부 서비스의 품질향상” 및 “정보화 투자 효율성 향상”을 달성하고, 대ㆍ중소기업이 동일한 개발기반 위에서 공정 경쟁이 가능하게 됩니다.

※ 표준프레임워크는 기존 다양한 플랫폼(.NET, php 등) 환경을 대체하기 위한 표준은 아니며, java 기반의 정보시스템 구축에 활용하실 수 있는 개발·운영 표준 환경을 제공하기 위한 것입니다.


​

즉, 전자정부프레임워크란 행정안전부 산하 한국정보화진흥원에서 만든 웹 기반 어플리케이션 프레임워크로서 정부 및 공공기관, 공기업 등의 웹사이트에 자주 쓰이는 공통 기능들을 Java의 Spring 프레임워크와 유명 Java 라이브러리(iBatis/MyBatis, Jackson, Apache Commons 등)를 가지고 미리 만들어 놓은 공통컴포넌트와 이를 개발하는 개발환경, 실행환경, 운영환경, 관리환경 등으로 구성되어있다.

​

​

​

뭐.. 그렇다고 한다.

​

​

2. 왜 이걸 쓰나?

먼저 이 전자정부프레임워크를 주로 사용하는 발주처가 정부기관이며 이러한 프로젝트를 수주하는 사업에는 필수 요구사항이라는게 있습니다.

주로 수주를 할때 해당 발주처에서 필요한 하드웨어는 어떠한 것을 사용하며 소프트웨어는 어떤걸 쓰겠다 라는 것이 다 기술 되어있습니다.

그래서 이러한 문서인 사업제안서는 이 요구사항을 기반으로 작성되어 있습니다.

전자정부프레임워크를 '왜 사용하나요?' 라는 질문을 하면 고객이 요구했기 때문에 라고 답하는게 제일 정확한 답변입니다.

고객이 원하는 대로 시스템 및 프로그램을 개발해주는 것이 기본이기 때문입니다.

그런데 고객이 왜 그걸 원하느냐 라는 의문이 여기서 발생합니다.

실제로 프레임워크의 장단점과 보안이 좋다 안좋다의 주제는 중요하지 않습니다.

전자정부 프레임워크는 아시다시피 Spring + 기타 플러그인(컴포넌트)를 하나로 묶어 패키지화 한 것 입니다.

그렇기에 Spring을 사용해보신분들은 아시겠지만 Spring의 장점은 확장성이 뛰어나며 JAVA로 이루어져 있습니다. 그런데 그 뛰어난 범용성과 확장성 만큼 플러그인들끼리의 층돌로 인한 오동작이 있을 수 있기에 개인 또는 프로젝트를 수주받은 개발사에서 플러그인을 자기들 편하대로 사용을 한다면 해당 웹사이트에는 어떤 코드가 들어 있는지 알 수가 없는 신뢰 할 수 없는 코드가 됩니다.

그렇기에 전자정부프레임워크 처럼 이런 프레임워크를 신뢰할 수 있고 책임질 수 있는 개인이나 단체가 한가지 형태로 통합해서 그걸 패키지로 배포하는 경우는 개인이나 개발사에서 중구난방으로 플러그인을 적용하고 이것저것 추가 하는 것 보다는 적어도 정상적으로 프로그램이 작동 됨과 동시에 코드에 문제가 없음을 알리는 신뢰성이 있는 즉, 검증된 코드가 됩니다.

마찬가지로 이러한 프레임워크를 관리를 하는 곳이 존재 하니 문제가 생기면 기술지원도 받을 수 있다는 것이 장점입니다.

프레임워크라는 단어에서 보듯이 이 하나의 공통된 프레임워크를 사용하면 특정 개발사에 종속되지 않고 여러 곳의 개발사에 그때그때 조건에 따라 발주가 가능하며 개발 했던 개발사가 유지보수를 하지 않더라도 다른 개발사에서 이어받아서 유지보수가 가능하게 됩니다.

즉, 정부기관에서 관리하는 검증된 오픈 소스로 구성된 무료 프레임워크라는 점이 강점입니다.

아래 이미지는 공식 홈페이지에서 소개하는 적용효과 입니다.


하지만 이것은 일반적인 사용이유이며 사실은 정부에서 모든 정부기관에 무조건 사용하라고 지침이 내려졌기 때문에 사용이유를 따지지 않고 사용하는 경향이 강합니다.

​

​

한마디로.. 그냥 검증된 무료 프레임워크이고 다들 비슷한걸 써야 이직도 하고 취업도 할거니까 방향을 정한거다.

​

​

​

3. 그렇다면 단점은 없을까요?

있습니다.

실제 정부에서 생각하는 것과 개발하는 개발 당사자인 개발자들 입장에서는 생각의 차이가 존재 하기 때문에 단점 또한 명확합니다.

전자정부표준프레임워크, 약칭 eGov는 공공기관 웹사이트 개발 과정을 표준화하기 위한 의도에서 시작되었으나, 그러한 의도로 인해 구조가 경직되고 최신 기술을 반영하지 못하는 보수적인 기술이라는 것이 문제점으로 작용하고 있다. 특히 정부발 프로젝트에 기대는 SI 회사가 절대 다수를 차지하는 현실로 인해 한국의 SW 시장이 Java + Spring으로 획일화되다시피 하는 결과를 낳았으며, 이는 곧 국내 소프트웨어 기술력 자체의 저하로 이어졌다. SI는 기본적으로 안정성과 유지보수를 추구하는 업계이지, 새로운 기술과 변화를 추구하는 곳이 아니기 때문. 그런데 사용하는 프레임워크와 제반 기술들까지 일원화되니 다양성이 죽어버린 것이다. 그나마 삼성전자와 네이버 등의 극소수 대기업들이 어느 정도 커버를 하는 상황.

물론 이것이 eGov의 잘못이라 하기는 어렵고, 진짜 원인은 SI 쪽으로 편중된 한국의 S/W 시장에 있다. 어지간한 대기업이 아니라면 SI를 빼고는 소프트웨어 사업을 벌이는 것이 불가능할 정도로 우리나라의 시장 상황은 열악하다. 어느 나라든 관공서가 아닌 민간 시장을 대상으로 자사 솔루션을 개발, 판매하는 기업들이 소프트웨어 시장의 기술 발전을 선도하는 편인데, 한국에는 이런 업체가 상대적으로 부족하다는 것이 근본적인 문제인 것이다.

또한 오라클이 나날이 자바 라이선스에 관련해서 갑질을 하고 있고 이로 인해 자바에서 이탈하는 기업도 늘어나고 있는데, 오라클의 갑질에 의한 피해를 막기 위해서는 장기적으로 자바기반에서 벗어나야 할 것이다.

-출처 나무위키-

스프링이나 자바를 하지 못하고 싫어하는 개발자라면 단점이 될 수도 있겠네요.

그 외에 공통 컴포넌트들에 대한 자잘한 이슈 문제는 계속 관리처에 이슈를 제기 하고 공론화 시켜야 문제가 해결될 것으로 보이고 다른 좋은 프레임워크가 나오지 않는 이상 향후 10년간은 문제없이 사용 될 것으로 보입니다.

​

단점도 당연히 있다. 거의 비슷비슷해지고, 최신기술이 아니다. 그래도 검증된 프레임워크라는 것만으로 개발자에게 엄청난 장점이기도 하다.(이것만 알아도 밥줄안끊김)

​

​

​

최근 리액트 관련 이슈가 있다. 링크 걸어놓겠다.

이슈라기보단 거의 확정같다..

https://blog.naver.com/pss91617/222597619878


전자정부 리액트를 표준으로?
https://blog.naver.com/pss91617/222597787159 어제 16일 전자정부 프론트엔드 프레임워크로 node.js/npm ...

blog.naver.com

​
[출처] 전자정부프레임워크란?[spring]|작성자 뮤믐매

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html lang="ko"><head>
<meta http-equiv="Pragma" content="no-cache">
<meta http-equiv="Expires" content="-1">
<meta name="robots" content="noindex,follow">
<meta name="referrer" content="always">
<meta http-equiv="content-type" content="text/html;charset=UTF-8">
<meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1">
<link rel="shortcut icon" type="image/x-icon" href="/favicon.ico?3">
<link rel="alternate" type="application/rss+xml" href="https://rss.blog.naver.com/pss91617.xml" title="RSS feed for pss91617 Blog">
<link rel="wlwmanifest" type="application/wlwmanifest+xml" href="https://blog.naver.com/NBlogWlwLayout.naver?blogId=pss91617">




<title>전자정부프레임워크란?[spring] : 네이버 블로그</title>
<script type="text/javascript" src="https://ssl.pstatic.net/t.static.blog/mylog/versioning/Frameset-347491577_https.js" charset="UTF-8"></script><script type="text/javascript" charset="UTF-8">
var photoContent="";
var postContent="";

var videoId 	  = "";
var thumbnail 	  = "";
var inKey 		  = "";
var movieFileSize = "";
var playTime 	  = "";
var screenSize 	  = "";

var blogId = 'pss91617';
var blogURL = 'https://blog.naver.com';
var eventCnt = '';

var g_ShareObject = {};
g_ShareObject.referer = "https%3A%2F%2Fsearch.naver.com%2Fsearch.naver%3Fsm%3Dtab_sug.top%26where%3Dnexearch%26query%3D%25EC%25A0%2584%25EC%259E%2590%25EC%25A0%2595%25EB%25B6%2580%25ED%2594%2584%25EB%25A0%2588%25EC%259E%2584%25EC%259B%258C%25ED%2581%25AC%26oquery%3D%25EA%25B9%2583%25ED%2597%2588%25EB%25B8%258C%26tqi%3DhpUvswp0YiRssmMZDyVsssssteK-498366%26acq%3D%25EC%25A0%2584%25EC%259E%2590%25EC%25A0%2595%25EB%25B6%2580%25ED%2594%2584%26acr%3D2%26qdt%3D0";


jsMVC.setController("framesetTitleController", FramesetTitleController);
jsMVC.setController("framesetUrlController", FramesetUrlController);
jsMVC.setController("framesetMusicController", FramesetMusicController);
var oFramesetTitleController = jsMVC.getController("framesetTitleController");
var oFramesetUrlController = jsMVC.getController("framesetUrlController");
var oFramesetMusicController = jsMVC.getController("framesetMusicController");
var sTitle = document.title;

var topFrameAlert = function(message){
	alert(message);
};

var topFrameConfirm = function(message){
	if(confirm(message)){
		return true;
	} else {
		return false;
	}
};
</script><style type="text/css">
    html{width:100%;height:100%;}
    body{width:100%;height:100%;margin:0;padding:0;font-size:0;}
    #mainFrame{width:100%;height:100%;margin:0;padding:0;border:0;}
    #hiddenFrame{width:0;height:0;margin:0;padding:0;border:0;}
</style></head>




<body>
    <iframe id="mainFrame" name="mainFrame" allowfullscreen="true" src="/PostView.naver?blogId=pss91617&amp;logNo=222597787159&amp;redirect=Dlog&amp;widgetTypeCall=true&amp;topReferer=https%3A%2F%2Fsearch.naver.com%2Fsearch.naver%3Fsm%3Dtab_sug.top%26where%3Dnexearch%26query%3D%25EC%25A0%2584%25EC%259E%2590%25EC%25A0%2595%25EB%25B6%2580%25ED%2594%2584%25EB%25A0%2588%25EC%259E%2584%25EC%259B%258C%25ED%2581%25AC%26oquery%3D%25EA%25B9%2583%25ED%2597%2588%25EB%25B8%258C%26tqi%3DhpUvswp0YiRssmMZDyVsssssteK-498366%26acq%3D%25EC%25A0%2584%25EC%259E%2590%25EC%25A0%2595%25EB%25B6%2580%25ED%2594%2584%26acr%3D2%26qdt%3D0&amp;directAccess=false" scrolling="auto" onload="oFramesetTitleController.start(self.frames['mainFrame'], self, sTitle);oFramesetTitleController.onLoadFrame();oFramesetUrlController.start(self.frames['mainFrame']);oFramesetUrlController.onLoadFrame()"></iframe>

</body></html>
