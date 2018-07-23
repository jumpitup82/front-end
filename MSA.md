# Frond-end Architecture in MSA (https://micro-frontends.org/)
    
### Core Ideas behind Micro Frontends
 * Be Technology Agnostic
  각 팀은 다른 팀과 조정하지 않고도 스택을 선택하고 업그레이드 할 수 있어야 한다.
 * Isolate Team Code
  모든 팀이 동일한 프레임 워크를 사용하더라도 런타임을 공유하지 마십시오. 독립적 인 앱을 제작하십시오. 공유 상태 또는 전역 변수에 의존하지 마십시오.
 * Establish Team Prefixes
  아직 격리가 불가능한 명명 규칙에 동의하십시오. 충돌을 피하고 소유권을 명확히하기 위해 네임 스페이스 CSS, 이벤트, 로컬 저장소 및 쿠키.
 * Favor Native Browser Features over Custom APIs
  Use Browser Events for communication instead of building a global PubSub system. If you really have to build a cross team API, try keeping it as simple as possible.
 * Build a Resilient Site
  Your feature should be useful, even if JavaScript failed or hasn’t executed yet. Use Universal Rendering and Progressive Enhancement to improve perceived performance.
 