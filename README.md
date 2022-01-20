# web-rtmp-streamer

이 프로젝트는 js+swf를 사용하여 rtmp 스트리머를 구현합니다. Tencent Cloud와 같은 표준 rtmp 스트리밍 서비스와 효과적으로 호환됩니다. 직접 [DEMO 방문](https://lujunda.github.io/web-rtmp-streamer/)하여 효과를 볼 수 있습니다.

이 프로젝트는 **NetEase Cloud Push Streaming DEMO**를 기반으로 개발되었으며 원본 버전과 비교하여 다음과 같은 개선 사항이 있습니다.
* 원본 버전이 스트림을 NetEase Cloud로만 푸시할 수 있다는 제한을 제거했습니다.
* 새 버전의 크롬과 원본 버전이 호환되지 않는 문제 해결（"Cross-origin plugin content from  must have a visible size larger than 400 x 300 pixels, or it will be blocked. Invisible content is always blocked."）。
* JSON.parse()를 사용하기 전에 원본 버전이 유형을 판단하지 않아 푸시 스트림이 실패하는 버그를 해결했습니다.
* 원본 버전에서 다양한 http 요청(예: 하트비트 인터페이스, NetEase 클라우드 cdn 주소 가져오기 등)을 제거하여 순수하고 모니터링되지 않는 스트림 푸셔를 실현합니다.
