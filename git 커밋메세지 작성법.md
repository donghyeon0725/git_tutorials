좋은 Git 커밋 메세지 작성하기
-

기본 수칙
-
* 동명사보다 명사 사용
* 꼭 필요한 경우가 아니면 a, an, the 등 관사 사용 X
* 부정문은 Not use 대신 Don't use 사용
* 오타수정의 경우 "Correct misspelled text" 대신 Fix typo 사용

자주 사용하는 명령문 모음
-

📌 FIX
-
보통 올바르지 않은 동작은 고친 경우 사용
<details>
    <summary>펼쳐보기</summary>

* Fix A : A를 수정합니다.
    - Fix stat cache : stat 캐시를 고칩니다.
    
<br/>
    
* Fix A in B : B 부분의 A를 수정합니다.
    - Fix calculation in process.uptime() method: process.uptime() 메소드의 게산을 고칩니다.

<br/>
    
* Fix A which B, Fix A that B : B 하는(인) A를 수정합니다. (부가설명)
    - Fix incorrect type which makes animated gifs not loop forever on device : 기기에서 애니메이션을 영원히 돌지 않게 하는 문제를 고칩니다.

<br/>

* Fix A to B, Fix A to be B : B를 위해 A를 수정합니다.
    - Fix HTTP connection timeout callback to be appropriately called : 적절한 호출을 위해 HTTP 콜백 연결 제한 시간을 변경함 

<br/>

* Fix A so that B : A를 수정해서 B상태가 되었습니다. (강조)
    - Fix Android 28's inverted ScrollView so that momentum is in the proper direction : 안드로이드 28의 거꾸로된 스크롤뷰를 고쳐서 적절한 방향으로 가도록 힘

<br/>

* Fix A where B : A 에는 보통 'issue', 'error', 'crash' 등이 들어감. B에는 문제가 발생한 모습을 보통 넣음 
    - Fix case where inline view is visible even though it should have been truncated : 잘리지 않았음에도 인라인 뷰가 보이지 않는 경우를 고침

<br/>

* Fix A when B : B 일 때 발생하는 A 수정
    - Fix crash when removing root nodes : 노드를 추가할 때 충돌나는 문제를 해결

<br/>


</details>

<br/>

📌 ADD
-
코드나 테스트, 예제, 문서 등의 추가가 있을 때 사용합니다.
<details>
    <summary>펼쳐보기</summary>

* Add A : A를 추가함 (보통 목표나 목적이 같이 들어가야함) 
    - Add ERR_INSPECTOR_COMMAND error :  상수 ERR_INSPECTOR_COMMAND 에러를 추가

<br/>

* Add A for B : B를 위해 A추가
    - Add documentation for the defaultPort option : defaultPort 옵션을 위해 문서 추가
    
<br/>

* Add A to B : B에 A추가
    - Add displayName to ActivityIndicator : 활성화 인디케이터에 이름표기 추가

<br/>


</details>

<br/>


📌 REMOVE
-
코드의 삭제가 있을 때 사용. 'Clean'이나 'Eliminate'를 사용하기도 하고 수식어로 'unnecessary', 'useless', 'unneeded', 'unused', 'duplicated' 등등이 많이 붙음  
<details>
    <summary>펼쳐보기</summary>

* Remove A : A를 삭제합니다.
    - Remove fallback cache : fallback 캐시를 제거함

<br/>

* Remove A from B : B에서 A를 삭제합니다.
    - Remove absolute path parameter from transformers : 변환기에서 절대경로 매개변수를 삭제합니다.

<br/>



</details>

<br/>

📌 USE
-
특별히 무언가를 사용해서 구현한 경우 사용
<details>
    <summary>펼쳐보기</summary>


* Use A : A를 사용합니다. 대체적으로 목적과 같이 사용하기에 이 용법은 잘 사용 안됨
    - Use more stable cast where possible : 가능한 더 안정적인 변환을 사용하세요.
    
<br/>

* Use A for B : B에 A를 사용
    - Use object writer for thrown errors : 에러를 던지기 위해 object writer를 사용합니다.

<br/>

* Use A to B : B가 되도록 A를 사용
    - use triggerReport() to handle signals : 신호를 다루기 위해 triggerReport 메소드 사용

<br/>

* Use A in B : B에서 A를 사용
    - Use same parameter name in node_report.cc : 같은 매개변수 이름을 node_report.cc 파일에서 사용

<br/>

* Use A instead of B : B대신 A 사용
    - Use babel runtime instead of relying on global babelHelpers and regenerator : 전역 babelHelpers 와 재생기에 의존하는 런타임 대신 바벨을 사용함

<br/>


</details>

<br/>

📌 REFACTOR
-
전면적인 수정이 있을 때 사용

* Refactor tick objects prune function : 함수를 제거하는 체크용 객체 개편


<br/>


📌 SIMPLIFY
-
복잡한 코드를 단순화 할 때 많이 사용. REFACTOR 보다는 약한 수정

* Simplify A : A를 단순화 합니다.
    - Simplify code and remove obsolete checks : 구식 무늬를 제거하고 코드를 단순화 함 



<br/>
 
📌 UPDATE
-
업데이트 있을 때 사용. Fix 와 달리 원래 정상 작동하던 것을 수정, 추가, 보완하는 개념.  
코드보다는 문서나 리소스, 라이브러리 등에 사용
    
* Update A to B : A를 B로 업데이트
    - Update acorn to 6.1.0 : acorn 을 6.1.0 버전으로 업데이트

<br/>

📌 IMPROVE
-
향샹된 내용이 있을 때 사용. 호환성, 테스트 커버리지, 성능, 검증 기능, 접근성 등등의 항목이 포함됨

* Improve A : A 를 향상시킵니다.
    - Improve Unicode handling : 유니코드 호환성을 향상시킴 

<br/>

📌 MAKE
-
주로 기존 동작의 변경을 명시


* Make A B : A를 B하게 만듬 
    - Make 'config object' read-only : 설정 객체를 읽기 전용으로 만듬

<br/>

📌 IMPLEMENT
-
코드가 추가된 정도보다 더 주목할 만한 구현체를 완성시켰을 때 

* Implement A : 특히 모듈이나 클래스 등의 단위에 사용되기 때문에 특별히 목적을 부여 해주지 않아도 되는 경우가 많음.
    - Implement date object : 날짜 객체 구현

<br/>

* Implement A to B : B를 위해 A 구현 
    - Implement requiresMainQueueSetup in RCTTVNavigationEventEmitter to satisfy Xcode warning ; xcode 경로를 충족시키기 위해 RCTTVNavigationEventEmitter 내부에 requiresMainQueueSetup 구현
    

<br/>
    
📌 REVISE : 
-
Update와 유사. 문서의 개성이 있을 때 주로 사용

* REVISE A : A 를 개정합니다.
    - Revise deprecation semverness info in Collaborator Guide : 쓰이지 않을 공동작업자 가이드에 semverness 정보를 개편

<br/>

📌 ENSURE 
-
'Make sure'과 같은 표현으로 사용 가능   
if 구문과 같이 사용 되곤 함. 무엇인가 확실하게 보장 하는 것을 의미

* Ensure A : A가 확실히 보장되도록 함
    - Ensure quiet always takes precedence : 항상 우선적으로 정숙하도록 함
    

<br/>

📌 PREVENT
-
특정 처리를 못하도록 막음

* Prevent A : A 하지 못하게 막음
    - Prevent multiple connection errors : 다중 연결 오류를 막음
     
<br/>

* Prevent A from B : A가 B하지 못하게 막음 
    - Prevent event handlers from receiving extra argument in development : 이벤트 핸들러가 발달 중인 여분의 인자를 받는 것을 막음

<br/>
    
📌 AVOID
-
if와 같이 특정 동작을 제외시키려고 사용하기도 함. prevent와 달리 회피성을 강조

*  Avoid : 
    - Avoid flusing uninitialized traces : 초기화 되지 않은 추적 플러싱 방지


<br/>
    
* Avoid A if B, Avoid A when B : B인 상황에선 A를 회피 
    - Avoid importing entire crypto dependency tree if not in Node.js. 노드 js 환경이 아니라면 암호화 모듈을 완전히 포함하는 것은 피하라


<br/>

📌 MOVE
-
코드의 이동이 있을 때 사용

* Move A to B, Move A into B : A를 B로 옮김
    - Move function from header to source file : 소스 파일의 해더 함수를 옮김

<br/>


📌 RENAME
-
이름 변경이 있을 때 사용

* Rename A to B : A를 B로 이름 변경합니다.


<br/>

📌 ALLOW
-
Make와 비슷하나 허용을 할 때 주로 사용

* Allow A to B : A가 B할 수 있도록 허용 
    - Allow passing parseOptions to ApolloServerBase constructor : ApolloServerBase 생성자에 parseOptions 전달을 허용합니다.
    
<br/>


📌 VERIFY
-
검증 코드를 넣을 때 주로 사용

* Verify A : A를 검증합니다.
    - Verify heap buffer allocations occur : 힙 버퍼 할당이 나타나는지 검증

<br/>

📌 SET
-
변수값을 변경하는 등, 작은 수정에 주로 사용

* Set A to B : A를 B로 설정합니다.
    - set tls.DEFAULT_ECDH_CURVE to 'auto' : tls.DEFAULT_ECDH_CURVE 변수를 '자동'으로 설정

<br/>

📌 PASS
-
파라미터를 넘기는 처리에 주로 사용

* Pass A to B : A를 B로 넘깁니다. 
    - Pass the response toolkit to the context function : 응답 툴킷을 컨텍스트 함수로 넘깁니다.
