# 플러그인

Plugin Manager를 사용하여 FormIt 팀이 제공하는 유용한 플러그인을 설치하거나 [**자체 FormIt 플러그인을 빌드하는 방법**](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)**을 알아보십시오.**

#### FormIt Plugin Manager

FormIt Plugin Manager는 Formit 플러그인을 검색하고 관리하기 위한 허브로 작동합니다.

FormIt이 인터넷에 액세스할 수 있는 경우, FormIt을 시작하면 Plugin Manager가 자동으로 로드됩니다.

응용프로그램 창 오른쪽에 있는 해당 탭 아이콘을 클릭하면 Plugin Manager에 액세스할 수 있습니다.

![](https://formit3d.github.io/FormItExamplePlugins/docs/images/PluginManagerTab.PNG)

#### Plugin Manager에서 카테고리로 분류하는 플러그인은 다음과 같이 다양합니다.

* **설치된 플러그인**
* **권장 플러그인**
   * FormIt 팀에서 FormIt의 핵심 기능을 확장하고 새 워크플로우를 활용하기 위해 권장하는 플러그인입니다.
   * FormIt 팀의 승인을 받은 후 커뮤니티에서 개발한 플러그인이 여기에 표시됩니다. 이러한 플러그인에 대해서는 이후에 더 자세히 살펴보겠습니다.
* **공용 플러그인**
   * 커뮤니티에서 빌드했지만 FormIt 팀의 검토나 승인을 거치지 않은 플러그인입니다.

#### Plugin Manager는 플러그인 및 해당 리포지토리를 쉽게 관리할 수 있도록 확장 및 축소 가능한 일련의 인터페이스를 사용하여 설계되었습니다.

* **플러그인 관리:**
   * 플러그인 이름을 클릭하면 설명이 표시됩니다.
   * 스위치를 전환하여 설치 또는 설치제거합니다.
      * 플러그인은 플러그인 유형에 따라 응용프로그램 상단의 도구막대, 오른쪽의 패널 또는 가운데의 대화상자로 표시됩니다.
* [자체 플러그인을 개발](https://formit3d.github.io/FormItExamplePlugins/docs/HowToBuild.html)하고 있는 경우 하단의 필드에 비공개 URL을 추가하고 \(+\)를 누르면 됩니다.

![FormIt Plugin Manager](https://formit3d.github.io/FormItExamplePlugins/docs/images/addNew.png)

#### 플러그인 작동 방식

* 플러그인은 웹 기반이며 Windows용 FormIt 및 웹용 FormIt에서 사용할 수 있습니다.
* 플러그인은 GitHub 또는 로컬 서버(자체적으로 빌드하는 경우)에서 호스트되는 일련의 파일 및 폴더로 구성됩니다.
* 외부 플러그인\(로컬로 호스트되지 않은 플러그인\)을 처음 로드하려면 인터넷 연결이 필요합니다. 이는 다음을 의미합니다.
   * FormIt을 시작할 때 인터넷 연결이 감지되지 않으면 외부 플러그인이 로드되지 않습니다.
   * 로드된 일부 외부 플러그인은 해당 세션에 대해 오프라인 모드로 계속 작동할 수 있지만, 그 외의 다른 플러그인은 연결이 복원될 때까지 중단될 수 있습니다.
   * 외부 플러그인은 실행할 때마다 서버에 최신 코드를 로드합니다. 따라서 작성자가 변경사항을 푸시할 때마다 해당 기능이 업데이트됩니다.
* 플러그인은 비동기적으로 로드됩니다. 이는 FormIt 인터페이스의 플러그인 순서가 새 세션이 나올 때마다 변경될 수 있음을 의미합니다.
* Plugin Manager는 Windows의 레지스트리 키를 사용하여 설치된 리포지토리 및 플러그인을 저장합니다.
   * Plugin Manager를 기본값으로 재설정해야 하는 경우 다음 레지스트리 키를 삭제합니다.
      * Computer\HKEY\_CURRENT\_USER\Software\Autodesk\FormIt 360\Plugins
      * 이렇게 하면 사용자가 추가한 모든 리포지토리와 플러그인이 설치제거되어 내장 리포지토리와 플러그인만 포함하도록 Plugin Manager가 재설정됩니다.

