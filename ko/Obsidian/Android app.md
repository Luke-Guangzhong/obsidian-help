이 도움말 문서는 레거시 문서로서, 링크 깨짐을 방지하기 위한 용도로만 제공됩니다. 모바일 앱에 대한 정보는 [[Sync your notes across devices]] 문서를 참조하십시오.

## Sync

Android 앱에서 동기화에 대한 정보는 [[Sync your notes across devices#Sync notes on Android|Android에서 노트 동기화]] 문서를 참조하십시오.

## Storage permissions

Obsidian을 시작할 때, 기기의 문서 및 미디어에 대한 액세스 권한을 요청하는 메시지가 표시될 수 있습니다.

이상적으로는 사용자가 선택한 보관소 폴더에 대한 액세스 권한만 요청하는 것이 좋습니다. 그러나 Android의 개인 정보 보호를 중시하는 파일 권한 API인 "스코프 저장소"에는 Obsidian이 올바르게 작동하는 것을 불가능하게 하는 몇 가지 제한 사항이 있습니다.

두 가지 주요 문제는 다음과 같습니다:

- 스코프 저장소는 모든 파일 액세스에 대해 많은 추가 권한 확인을 수행하여 Obsidian을 여는 데 사용할 때 중요한 성능 저하를 초래합니다.
- 스코프 저장소는 외부 변경을 모니터하는 방법을 제공하지 않으며, 이것은 Obsidian을 타사 동기화 도구와 사용할 때 중요합니다.

Google은 이러한 종류의 앱 개발자를 위한 특별한 권한을 부여하는 지침을 제공합니다. Obsidian은 "문서 관리 앱" 및 "장치 내 파일 검색"이라는 예외 목록의 두 범주에 속합니다. [여기에서 자세히 알아보기](https://developer.android.com/training/data-storage/manage-all-files).