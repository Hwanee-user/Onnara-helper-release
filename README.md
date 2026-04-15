# 온나라 도우미 Release v0.7

이 저장소는 공개 배포용 release 레포입니다.
사용자 배포에 필요한 zip 패키지만 올리는 구성을 기준으로 정리했습니다.

## 포함 파일

- `release/onnara-helper-v0.7-win64.zip`

zip 안에는 아래 파일이 들어갑니다.

- `온나라도우미.exe`
- `config.example.json`
- `server_config.example.json`
- `msedgedriver.exe`
- `LICENSE.chromedriver`
- `README.md`
- `사용설명서.md`
- `프로그램_구조_기능_참조.md`

## 빌드 확인

release 작업용 로컬 워크트리에서 `build.bat`를 실행해 아래를 확인했습니다.

- PyInstaller 빌드 성공
- `release/onnara-helper-v0.7-win64.zip` 생성
- `release/package` 내부에 `.py` 파일 없음

참고로 PyInstaller는 평문 `.py`를 같이 배포하지 않게 해주지만, 실행 파일이 완전한 난독화나 역공학 방지를 보장하는 방식은 아닙니다.

## 설치 안내

1. `release/onnara-helper-v0.7-win64.zip` 다운로드
2. 압축 해제
3. `config.example.json`을 참고해 `config.json` 작성
4. `server_config.example.json`을 참고해 `server_config.json` 작성
5. `온나라도우미.exe` 실행

## 버전 메모

v0.7 기준 반영 사항:

- 결재대기함 문서처리 과제카드 팝업 복구
- 윈도우 알림 클릭 시 프로그램 전면 복원
- 공개 배포용 민감정보 제거 및 release 패키지 정리
