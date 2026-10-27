# blackcode_web

서비스가 종료된 **블랙코드(BlacKode) 스마트 주차번호판** 단말기의 화면 번호를 웹에서 바로 바꾸는 도구입니다.
설치나 회원가입 없이 주소만 열면 됩니다. 서버를 쓰지 않고, 화면 이미지를 브라우저에서 직접 만들어 블루투스로 보냅니다.

**👉 https://lukekimm.github.io/blackcode_web/**

## 쓰는 방법
1. 단말기 근처에서 위 주소를 엽니다.
2. 번호를 입력합니다. 숫자만 치면 하이픈이 자동으로 들어갑니다. 위쪽 문구도 바꿀 수 있습니다.
3. 「단말기에 연결해서 전송」을 누르고 목록에서 블랙코드 단말기를 고릅니다.
4. 몇 초 뒤 단말기 화면이 바뀝니다. 글씨가 거꾸로 보이면 「180° 뒤집기」, 색이 반대면 「흑백 반전」을 켜고 다시 보내세요.

## 지원 환경
| 기기 | 방법 |
|---|---|
| 안드로이드 | Chrome으로 열기. 메뉴 → 「홈 화면에 추가」 하면 앱처럼 쓸 수 있음 |
| 아이폰 | Safari·Chrome은 웹 블루투스 미지원 → App Store의 [Bluefy](https://apps.apple.com/app/id1492822055) 앱에서 주소 열기 |
| PC·맥 | Chrome 또는 Edge |

한 번 열면 오프라인에서도 동작합니다(지하주차장 대비). 입력한 번호는 그 기기의 브라우저에만 저장됩니다.

## 파일
- `index.html` — 도구 전체 (화면 렌더링 + BLE 전송)
- `manifest.webmanifest`, `sw.js`, `icons/` — 홈 화면 설치·오프라인용

프로토콜 상세는 iOS 앱 저장소 [blackcode_iphone](https://github.com/LukeKimm/blackcode_iphone) README 참고.
