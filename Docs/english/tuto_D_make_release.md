# 릴리스 만드는 방법

> _이 문서는 새로운 릴리스를 발행하고자 하는 개발자를 위한 것입니다._

1. **콘텐츠가 최신 상태인지 확인하세요.**<br>
   [콘텐츠 업그레이드](tuto_D_contribute_assets.md)를 참조하세요.

2. **필요한 곳에서 CARLA 버전을 높이세요.**<br>
   다음 파일들에서 버전을 높이세요: _DefaultGame.ini_, _Carla.uplugin_, 
   _setup.py_, _ContentVersions.txt_. 현재 버전을 grep하여 참조가 누락된 곳이 
   없는지 확인하세요.

3. **CHANGELOG.md를 정리하세요.**<br>
   변경 로그가 최신 상태인지 확인하고, 필요한 경우 문구를 수정하고 재구성하세요.
   사용자에게 더 중요할 수 있는 항목들을 고려하세요.

4. **변경사항을 커밋하고 새 태그를 추가하세요.**<br>
   모든 변경사항이 커밋되면 `git tag -a X.X.X`로 새 태그를 추가하세요
   (`X.X.X`를 최신 버전으로 대체). 이 버전의 변경 로그를 태그 메시지로 
   추가하세요.

5. **콘텐츠 저장소에 태그를 지정하세요.**<br>
   _ContentVersions.txt_에 있는 정확한 커밋에 콘텐츠 저장소에도 유사한 
   태그를 추가하세요.

6. **변경사항을 푸시하세요.**<br>
   두 저장소 모두에 모든 변경사항을 푸시하세요. 태그를 푸시하려면 
   `git push --tags`를 사용해야 할 수 있습니다. 필요한 경우 Pull Request를 
   생성하세요.

7. **GitHub 릴리스를 편집하세요.**<br>
   [GitHub releases](https://github.com/carla-simulator/carla/releases)로 가서
   새로 만든 태그 위에 새 릴리스를 생성하세요. Jenkins가 최신 버전으로 빌드 
   게시를 완료할 때까지 기다린 다음 새로 만든 릴리스에 다운로드 링크를 
   추가하세요.