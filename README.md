# Cesium & Naver Panorama Digital Twin Viewer

CesiumJS 3D Globe와 네이버 지도 API 거리뷰(Panorama)를 양방향 연동한 분할 화면(Split-view) 뷰어입니다.
  
🚀 
최근 세슘에서 구글 스트리트뷰를 연동한 블로그가 게재되었습니다.     
https://cesium.com/learn/cesiumjs-learn/google-street-view/     

파노마라 뷰 사진을 연동하는 방법에 대한 블로그도 게재되었습니다.   
https://cesium.com/blog/2026/03/05/introducing-panoramic-imagery-in-cesiumjs/  

이에 네이버 거리뷰를 적용해봤습니다.   
OSM 빌딩을 적용했는데, 3D Mesh 또는 가우시안 스플래팅 또는 포인트 클라우드 콘텐츠가 적용되어 있다면 훨씬 더 실감나게 비교해볼 수 있을 것 같습니다.   

![3D Mesh 적용 결과](https://github.com/thlee33/cesium_naver_panorama/3dmesh.png)  

### 포함된 기능
- **Naver 거리뷰 & Cesium 카메리 방향 동기화:** 어느 한쪽을 이동/회전해도 다른 한쪽 화면이 실시간으로 따라갑니다.
- **Cesium OSM Buildings:** 기본 베이스로 전 세계 3D 빌딩 레이어가 포함되어 있습니다.


