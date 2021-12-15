# 질문과 대답(FAQ)

## FormIt 정보

**FormIt과 FormIt Pro란 무엇입니까?**

FormIt은 건축 설계를 위한 3D 모델링, 시각화, 해석 및 계산 환경입니다.

FormIt의 특징:

* 건물 설계에 최적화된 강력한 도구 및 워크플로우를 갖춘 강력한 솔리드 모델링 엔진
* 장면을 사용하여 저장된 모델 상태를 포함한 설계 옵션을 보여 주는 향상된 환경 시각화
* Bing Maps를 사용한 위치, 위성 이미지 및 3D 지형
* Autodesk 재료 라이브러리의 재료
* 그룹, 레이어 및 장면과 같은 모델 구성 및 가시성 도구
* 다음을 포함하는 해석 도구:
   * 솔리드 모델 진단 및 복구를 위한 수밀 및 뒷면 검증
   * 태양 및 그림자
   * 일조 해석
   * 에너지 해석
* Autodesk 제품 통합:
   * BIM 360 Docs
   * Insight\(에너지 해석\)
   * [Dynamo](https://formit.autodesk.com/page/formit-dynamo)
   * [Revit](https://formit.autodesk.com/page/formit-revit)
* 파일 형식 지원:
   * 열기/가져오기
      * AXM, DWG, FBX, SAT, STL, OBJ, WSM, SketchUp, 이미지
   * 내보내기
      * AXM, FBX, OBJ, STL, SAT, DAE, DXF

FormIt은 [iOS](https://itunes.apple.com/us/app/autodesk-formit-360/id575282599?mt=8) 및 [사용 중인 브라우저](https://app.formit.autodesk.com/)에서 무료로 사용할 수 있습니다. **FormIt Pro** 서브스크립션은 가장 강력하고 다양한 기능이 포함된 FormIt 버전인 [Windows용 FormIt](https://formit.autodesk.com/page/download)을 사용하는 데 필요합니다. **FormIt Pro** 서브스크립션을 통해 iOS 및 웹에서 일조 및 에너지 해석과 같은 추가 기능을 사용할 수도 있습니다. **FormIt Pro**는 [Autodesk AEC 컬렉션](https://www.autodesk.co.kr/collections/architecture-engineering-construction/overview)에 포함되어 있습니다.

**Android용 FormIt은 어떻게 되었습니까?**

FormIt 제품 제공을 간소화하기 위해 고심 끝에 Android 앱 서비스를 중단하기로 결정해야 했습니다. 설치한 경우 계속 실행되지만 Play Store에서는 더 이상 다운로드할 수 없습니다.

**FormIt은 어떻게 얻을 수 있습니까?**

Windows 버전을 실행하려면 [AEC 인더스트리 컬렉션](https://www.autodesk.co.kr/collections/architecture-engineering-construction/overview) 서브스크립션에 포함된 **FormIt Pro**에 대한 액세스 권한이 있어야 합니다. 사무실에서 Revit을 보유하고 있다면 이미 FormIt에 액세스할 좋은 기회가 있는 것입니다. [Windows용 FormIt은 Autodesk 웹사이트에서 직접](https://formit.autodesk.com/page/download) 또는 Autodesk 데스크톱 앱에서 다운로드할 수 있습니다.

또한 웹 버전은 Autodesk 웹 사이트([http://formit.autodesk.com](http://formit.autodesk.com))에서 무료로 직접 실행할 수 있습니다.

iOS 버전은 Apple App Store\(iPad만 해당\)에서 무료로 다운로드할 수 있습니다.

**학생 또는 교사인 경우 FormIt Pro를 무료로 이용할 수 있습니까?**

예! [Autodesk 교육 포털](https://www.autodesk.co.kr/education/edu-software/overview?sorting=featured&page=1)을 통해 FormIt Pro 서브스크립션에 액세스할 수 있습니다.

**FormIt에 대해 알아보려면 어떻게 해야 합니까?**

[FormIt Primer 튜토리얼](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Building-the-Farnsworth-House.html)에서 시작하는 것이 가장 좋습니다.

Primer에는 초급\(전체 현대적인 주택 작성\)부터 고급\(고급 방식으로 Revit 및 Dynamo 작업\)에 이르기까지 여러 섹션이 포함되어 있습니다.

FormIt Friday 웨비나 시리즈에는 20개가 넘는 동영상이 있습니다. 해당 동영상은 [YouTube 채널](https://www.youtube.com/playlist?list=PLqumTDi1CVHM7rCHJs83Yb2FyadmuQsiH)에서도 찾을 수 있습니다.

## Revit 작업

**FormIt은 Revit과 어떻게 작동합니까?**

FormIt은 별도의 3D 스케치 및 설계 응용프로그램이지만 [Revit용 FormIt 애드인](https://formit.autodesk.com/page/formit-revit)을 사용하여 Revit으로 쉽게 변환할 수 있는 데이터를 작성합니다.

**Revit으로 가져오면 어떻게 됩니까?**

2016년부터 Revit은 FormIt 데이터 작업을 위한 애드인과 함께 제공됩니다. FormIt AXM 파일을 Revit으로 가져올 때 이 애드인은 파일의 각 객체를 확인하고 API를 사용하여 Revit에서 해당 객체를 다시 작성합니다. 기본적으로 FormIt의 모든 항목은 매스로 분류됩니다.

FormIt 변환기는 각 매스 객체를 가져와 [직접 모양 API](https://knowledge.autodesk.com/search-result/caas/CloudHelp/cloudhelp/2016/KOR/Revit-API/files/GUID-DF7B9D4A-5A8A-4E39-8721-B7782CBD7730-htm.html)를 사용하여 Revit에서 매스 패밀리를 작성합니다.

직접 모양은 IFC 워크플로우에서 사용되는 편집 불가능한 객체입니다. 이 객체는 편집할 수 없지만 FormIt과 Revit 간에 전체 재료 텍스처를 전송한다는 고유한 장점이 있습니다. [다음은 FormIt에서 Revit으로의 워크플로우에 대해 자세히 설명하는 튜토리얼](https://windows.help.formit.autodesk.com/Building-the-Farnsworth-House/Revit-Interop.html)입니다.

**FormIt에서 벽, 바닥 및 기타 Revit 시스템 패밀리를 작성할 수 있습니까?**

직접적으로는 아닙니다. 위에서 설명한 대로 각 객체는 기본적으로 질량 카테고리로 지정됩니다. 벽, 바닥 등을 작성하려면 변환기 애드인을 사용하여 모델을 Revit으로 가져오고 기본 Revit 도구를 사용하여 기본 매스 모델에서 시스템 패밀리를 작성해야 합니다.

**Revit에서 FormIt으로 데이터를 다시 보낼 수 있습니까?**

예. 데이터를 다시 FormIt으로 가져오려면 Revit 파일의 전체 또는 _일부_를 SAT 파일 형식으로 내보냅니다. 일반적으로 Revit 데이터를 FormIt으로 모두 보낼 필요는 없습니다. 대신 SAT에 저장하기 전에 최소 데이터\(예: 바닥 및 벽\)만 포함하는 필터링된 뷰를 Revit에서 작성합니다.

## 다른 앱으로 작업

**기본 파일 형식이 '.AXM'인 이유는 무엇입니까?**

FormIt이 공식적으로 이름이 지정되기 전의 내부에서 사용하던 코드 이름은 XModeler였습니다. 따라서 생성한 파일 형식은 Autodesk X Modeler 즉, AXM이었습니다.

**FormIt에서 가져올 수 있는 3D 형식은 무엇입니까?**

* Windows: AXM, DWG, FBX, OBJ, SAT, SKP, STL
* 웹: OBJ, STL
* iOS: OBJ, STL, SAT

**FormIt에서 내보낼 수 있는 형식 종류는 무엇입니까?**

* Windows: FBX, OBJ, SAT, STL, DAE, DXF
* 웹: OBJ, SAT, STL
* iOS: OBJ

**FormIt은 Dynamo와 어떻게 작동합니까?**

[FormIt과 Dynamo가 어떻게 함께 작동하여](https://formit.autodesk.com/page/formit-dynamo) 계산 설계 워크플로우를 작성하는지 알아보십시오.

**FormIt은 SketchUp과 어떻게 비교할 수 있습니까?**

* [**Revit과의 상호 운용성**](../tool-library/revit.md)이 더 뛰어남 ****
* 계산 설계를 위한 [**Dynamo 통합**](../tool-library/dynamo.md)
* Autodesk Insight에서 제공하는 [**일조 해석**](../tool-library/solar-analysis.md) 및 [**에너지 해석**](../tool-library/energy-analysis.md)을 위한 기본 도구
* 고급 모델링 작업을 가능하게 하는 보다 강력한 솔리드 모델링 커널
* 기본 고급 모델링 도구(예: [**스윕, 피복, 로프트**](../tool-library/cover-sweep-loft.md), 간격띄우기/쉘 솔리드 및 3D 혼합/모깎기 및 [**면 평면화**](../tool-library/flatten-face.md))
* 표시되는 여러 [**단면 기준면** ](../tool-library/section-planes.md)
* [**수밀 문제 표시 및 뒷면 표시**](../tool-library/visual-styles.md)와 같은 진단 도구
* 선택 및/또는 보이는 항목을 기준으로 [**모델의 일부 내보내기**](../tool-library/export-data.md)
* 기본 OBJ, SAT 및 STL 내보내기

**SketchUp 키보드 단축키를 사용할 수 있습니까?**

예! Windows용 FormIt에는 완전히 편집 가능한 키보드 맵이 있습니다. 많은 공통 SketchUp 바로 가기가 기본적으로 이미 있지만 편집 &gt; 기본 설정 메뉴에서 편집할 수 있습니다.

**내 DWG 파일을 사용할 수 있습니까?**

예! FormIt은 2D 및 3D DWG 파일을 가져옵니다.

## 일반적인 지원 질문

**지원은 어떻게 받을 수 있습니까?**

Autodesk 공인협력업체를 방문하거나 [FormIt 포럼](https://forums.autodesk.com/t5/formit-forum/bd-p/142?profile.language=en)에서 문의할 수 있습니다. 먼저 궁금한 내용을 검색하는 것이 가장 좋습니다. 답변을 찾지 못한 경우 새 항목을 게시하면 FormIt 팀이 응답해 드립니다.

**로그인할 수 없는 경우 어떻게 해야 합니까?**

* 이 [포럼 게시물](https://forums.autodesk.com/t5/formit-forum/having-trouble-logging-into-formit-for-windows-try-these-steps/td-p/7179572?profile.language=en)에서는 일반적인 로그인 문제를 다룹니다.
* 전환 가능한 그래픽 프로세서\(GPU\)가 장착된 PC를 사용하는 경우 FormIt이 항상 더 높은 성능의 GPU를 사용하는지 확인해야 합니다. 다음은 [AMD](https://community.amd.com/docs/DOC-1581#jive_content_id_Assigning_Applications_to_GPUs) 및 [NVIDIA](http://nvidia.custhelp.com/app/answers/detail/a_id/2615/kw/manage%203d%20settings/related/1)에 대한 지침입니다.

**Insight 에너지 해석에 실패하면 어떻게 해야 합니까?**

Insight 에너지 해석에서 오류를 보고하거나 결과를 반환하지 못하면 [Insight 에너지 해석 페이지](https://formit.autodesk.com/page/formit-insight)에서 일반적인 문제 해결 팁을 확인하십시오.

