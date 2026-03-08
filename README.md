# Cesium & Naver Panorama Digital Twin Viewer

CesiumJS 3D Globe와 네이버 지도 API 거리뷰(Panorama)를 양방향 연동한 분할 화면(Split-view) 뷰어입니다.

## 🚀 시작하기

이 프로젝트를 로컬 환경에 클론(Clone) 받은 후 아래 과정을 수행하세요.

### 1. 설정 파일 생성 (필수)
이 프로젝트는 보안을 위해 3D Mesh 타일셋 URL을 소스코드에서 분리했습니다.
프로젝트 루트 디렉토리에 `config.js` 파일을 생성하고 아래 코드를 작성해야 애플리케이션이 정상 작동합니다.

```javascript
// config.js
const config = {
    // 본인의 환경에 맞는 3D Tileset URL을 입력하세요.
    SANGAM_TILESET_URL: "https://여러분의_도메인:포트/mago_data/.../tileset.json"
};
```

### 2. 로컬 서버 실행
API 호출을 위해 로컬 웹 서버 환경이 필요합니다. Python이 설치되어 있다면 다음 명령어로 간편하게 실행할 수 있습니다.

```bash
python -m http.server 80
```
브라우저에서 `http://127.0.0.1` 로 접속하세요.

---

### 포함된 기능
- **Naver 거리뷰 & Cesium 카메리 방향 동기화:** 어느 한쪽을 이동/회전해도 다른 한쪽 화면이 실시간으로 따라갑니다.
- **Cesium OSM Buildings:** 기본 베이스로 전 세계 3D 빌딩 레이어가 포함되어 있습니다.
- **사용자 정의 3D Mesh:** `config.js`를 통해 외부 특정 지역의 고해상도 3D Mesh 타일을 올릴 수 있습니다.
