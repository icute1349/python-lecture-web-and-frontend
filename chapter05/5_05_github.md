# 5-05. Github

Github는 클라우드 형태의 Git 저장소을 제공하는 서비스입니다. 웹 브라우저를 통해 Git 저장소를 관리할 수 있습니다. Git에는 내장되어 있지 않은 다양한 편의기능을 제공하기도 합니다. 멀리 떨어진 저장소, 즉 원격 저장소(Remote Repository)의 개념이라고 생각하시면 되겠습니다.

내 컴퓨터에 저장된 레포지토리를 Github에 업로드하고 변경사항이 생길 때마다 원격 레포지토리에도 반영될 수 있도록 하는 기능뿐 아니라, 과거의 내가 올려둔 혹은 다른 사람들의 레포지토리를 다운로드 받을 수도 있습니다.

먼저, 지난 강의 때 만들었던 txt 파일이 저장된 폴더를 github에 원격 저장소를 만들어 연결해 보도록 하겠습니다. github에서 새로운 레포지토리를 만들겠습니다. 폴더 이름이 같을 필요는 없습니다. 공개 여부를 선택할 수도 있는데요. 저희는 일단 Public으로 만들게요. 설명서를 의미하는 readme.md 파일이나, github에 업로드하지 않을 파일을 적어놓는 문서인 .gitignore를 만들 거냐고 물어보는데요. 저희는 체크하지 않겠습니다. 그리고 나면 연결하는 방법이 나타나는데요. 차례대로 따라해 보겠습니다.

git init, git add, git commit은 이미 완료되어 있으므로 그 다음부터 해보겠습니다. vs code를 켜주세요. ctrl+shift+enter 혹은 cmd+enter를 누르시고, `git: add remote`를 클릭하세요. origin 이라고 쓰신 다음 엔터를 누른 후, HTTPS 부분의 주소를 복사-붙여넣기 하시면 됩니다. 그리고 난 뒤에는 소스제어에서 `푸시`를 누르시면 됩니다. 처음으로 연결하는 것이라는 의미의 알림이 뜰텐데요. 확인을 누르시면 됩니다.

브라우저를 새로고침 하면 원하는 대로 파일이 잘 저장되어 있고요. 여기서 commit도 확인할 수 있습니다.

이후에 변경사항을 스테이징 영역에 올리고, 커밋을 한 뒤, 로컬 영역의 레포지토리에서 리모트 레포지토리로 push 를 하면 됩니다. CLI 명령어로는 `git push origin master`라고 입력하면 됩니다.

원격 저장소에서 변경사항이 생겨서 제 컴퓨터 상의 코드와 달라질 수 있습니다. 가령, 협업하는 누군가가 코드를 수정해서 올려둘 수도 있고, 내 컴퓨터에서 파일을 수정했을 수도 있습니다. 이때, 원격 저장소의 변경사항을 가져오는 명령이 있습니다. 한번, github에서 직접 파일을 수정해 보겠습니다. 브라우저에서 연필 모양의 버튼을 클릭해서 수정을 해 보세요. 그리고, ctrl+shift+enter 혹은 cmd+enter를 누르시고, `git: pull`을 검색한 뒤 실행해 보세요.
