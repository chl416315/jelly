# 젤리 메이커 · Material Studies No. 059

사진을 젤리 3D로 만들어 주는 인터랙티브 소프트바디 실험 (three.js + XPBD).

- `index.html` 한 파일로 동작합니다. 빌드가 필요 없습니다.
- 데모 젤리(고래, 곰젤리)는 어디서나 동작합니다.
- 사진 → 젤리 변환은 Claude 연동이 필요합니다. 이 파일을 GitHub Pages에 그대로 올리면 변환 기능은 동작하지 않고 데모만 동작합니다.

## GitHub Pages로 공개하기
1. 새 저장소를 만들고 `index.html`, `README.md`를 올립니다.
2. Settings → Pages → Branch를 `main` / `(root)`로 선택하고 Save.
3. 잠시 뒤 `https://<아이디>.github.io/<저장소>/` 로 접속됩니다.

## 구조
설계도(JSON) → 거리장(SDF) → 표면 메시 + 사면체 격자 → XPBD 소프트바디 → three.js 렌더링.
