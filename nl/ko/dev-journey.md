---

copyright:
  years: 2016, 2017, 2018
lastupdated: "2018-05-02"

---
{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:codeblock: .codeblock}
{:pre: .pre}
{:tip: .tip}

# {{site.data.keyword.cloud_notm}}의 개발자 과정 탐색
{: #dev-journey}

{{site.data.keyword.cloud}}는 개발자가 몇 분 내에 앱 빌드를 시작할 수 있는 기능 세트를 보유합니다. 개발자 대시보드에서 다음을 수행할 수 있습니다.

* 유스 케이스에 특정적이고 다양한 프로그래밍 언어와 아키텍처 패턴으로 프로덕션 사용 준비된 스타터 앱을 생성하는 스타터 킷 선택
* 스타터 킷에서 자동으로 프로비저닝되거나 사용자가 앱에 수동으로 추가한 리소스 확인 및 관리
* 다양한 클라우드 환경에 배치할 수 있는 이식 가능 앱 코드 가져오기
* 몇 번의 클릭으로 [DevOps 도구 체인](../services/ContinuousDelivery/index.html#cd_getting_started) 작성
* 로컬 개발을 위해 [명령행 인터페이스](/docs/cli/idt/index.html) 사용

{{site.data.keyword.cloud_notm}} 개발자 경험을 이해하면 고품질의 프로덕션 사용 준비된 앱을 빠르게 빌드하는 데 도움이 됩니다. 이러한 요소를 좀 더 자세히 살펴보겠습니다.

## 개발자 대시보드
{: #dev-dashboards}

{{site.data.keyword.cloud_notm}}는 관심 있는 여러 분야(Watson, 보안 또는 재무) 또는 디지털 채널(모바일 또는 웹 앱)에서 개발자 대시보드를 보유합니다. **메뉴 아이콘**  ![메뉴 아이콘](../icons/icon_hamburger.svg)에서 이러한 대시보드에 액세스할 수 있습니다.

각 개발자 대시보드는 개발자의 핵심 분야와 관련된 스타터 킷을 제공하고 일관되고 직관적인 워크플로우를 제공하여 사용자가 몇 분 내에 프로덕션 사용 준비된 앱을 작성 및 실행할 수 있게 합니다.

## 앱
{: #app-projects}

앱은 코드, 데이터, 서비스 및 도구 체인으로 구성됩니다. 예를 들어, {{site.data.keyword.cloud_notm}} 모바일 앱은 백엔드 로직, 데이터 스토리지, 분석 및 보안 서비스와 함께 디바이스 코드를 포함하며 Continuous Delivery에 대해 설정됩니다.

![재사용](images/garage_reuse2.png "재사용이 가능하고 재개발을 없앤 개발자 경험")

{{site.data.keyword.cloud_notm}} 개발자 대시보드 또는 {{site.data.keyword.dev_cli_notm}}을 사용하여 앱을 작성하고 관리할 수 있습니다.

## 스타터 킷
{: #starter-kits}

스타터 킷을 사용하여 {{site.data.keyword.cloud_notm}}에서는 클라우드 배치 준비가 된 스켈레톤 프로덕션 앱을 사용자가 선택한 언어로 어셈블합니다. 각 스타터 킷에는 특정 유스 케이스를 위한 언어, 프레임워크 및 패턴이 포함되며 코드를 재사용할 수 있습니다.

### 스타터 킷이 샘플과 다른 점
스타터 킷은 프로덕션에 사용할 준비가 되어 있고 런타임(예: Node.js 및 Express)을 사용한 키 패턴 구현의 증명에 초점을 맞춥니다. 어떤 경우 스타터 킷은 서비스 통합을 강조하기 위해 단순한 사용자 경험을 제공합니다. 다른 경우에 스타터 킷은 복잡한 유스 케이스의 사용자 정의 가능한 구현을 나타냅니다.

* **스니펫**은 IDE에서 자주 표시되는 몇 행의 코드입니다. 스니펫은 개발자가 프로그래밍 언어 구문을 통합하도록 도와주거나 정의된 API와 통합을 지원합니다.
* **데모**는 일반적으로 품질 및 정확도가 높고 다양한 서비스 및 통합 지점을 사용합니다. 종종 설정 시간이 필요하며 비즈니스 문제점을 증명하거나 플랫폼 기능을 시연할 때 사용됩니다. 클라우드 채택의 평가 단계에 사용됩니다. 때때로 코드가 프로덕션 코드에 포함됩니다.
* **샘플**은 특정 기능, 함수, 서비스 또는 사용자 과정의 작은 예제입니다. 샘플은 프로덕션 애플리케이션에서 재사용되거나 포함될 수 있습니다. 일반적으로 기술적 기능 및 기술 문제점 해결을 위한 가능한 접근 방법을 보여주기 위해 사용됩니다.
* **스타터 킷**은 DevOps 파이프라인 및 Kubernetes 클러스터에 직접 배치될 수 있는 프로덕션 사용 준비된 자산을 생성하기 위해 서비스 세트와 통합될 수 있는 프로덕션 사용 준비된 패턴입니다. 스타터 킷은 킷이 무엇이고 어떤 일을 하는지 알 수 있도록 충분한 정보를 제공하는 설명 메타데이터를 포함합니다. 또한 무엇을 생성할 것인지 {{site.data.keyword.cloud_notm}}에게 알려주는 지시사항을 포함합니다. 즉시 사용 가능한, 프로덕션 사용 준비된 결과물이 생성되고 IBM 우수 사례를 기반으로 추가 개선을 위해 반복할 수 있습니다. 스타터 킷 컨텐츠는 데모만큼 복잡하지 않고 스니펫이나 샘플처럼 간단하지 않습니다. 개발자의 요구사항에 따라 동적으로 작성됩니다.

## 자동 프로비저닝된 리소스
{: #auto-provision}

스타터 킷이 필수 리소스를 지정하는 경우 사용자가 앱을 작성할 때 {{site.data.keyword.cloud_notm}}에서 이러한 리소스를 자동으로 작성합니다. 앱이 작성된 후에 리소스를 수동으로 프로비저닝하거나 앱에 추가할 기존 리소스 인스턴스를 선택할 수 있음을 참고하십시오. 필요한 경우 신임 정보와 함께 앱 세부사항 보기에서 앱과 연관된 서비스 인스턴스 목록을 볼 수 있습니다.

## 이식 가능 코드
{: #portable-code}

스타터 킷에서 앱을 작성하면 일관된 형식을 가지며 런타임 중립적 코드가 자동으로 생성됩니다. 코드를 선택한 환경(예: Kubernetes 또는 Cloud Foundry)에 변경 없이 배치할 수 있습니다.

### 생성된 코드
{{site.data.keyword.cloud_notm}} 스타터 킷에서 생성된 코드는 네 개의 기본 컴포넌트가 있습니다. 즉, 유스 케이스 로직, 언어 컴포넌트, 서비스 인에이블먼트 그리고 클라우드 인에이블먼트입니다. 이러한 컴포넌트를 생성하면 귀중한 시간을 절약하고 최고의 아키텍처를 사용할 수 있습니다.

* **유스 케이스 로직**은 특정 유스케이스의 핵심 기능을 위한 기능을 제공합니다. Watson Conversation 챗봇용 코드 또는 모바일 시각적 인식 앱용 코드가 예가 될 수 있습니다.
* **언어 컴포넌트**는 스타터 킷을 위해 선택한 프로그래밍 언어에 특정한 코드 컴포넌트 및 파일입니다. 예를 들어 node.js 프로그래머는 종속성 관리를 위해 package.json 파일이 필요하며 이 파일은 사용자를 위해 자동으로 작성됩니다.
* **서비스 인에이블먼트**는 앱이 사용자가 추가한 서비스에 연결하고 사용할 수 있게 하는 코드입니다. 신임 정보 관리, 초기화 코드 및 서비스 특정 SDK는 서비스 인에이블먼트 항목의 예입니다.
* **클라우드 인에이블먼트**는 앱을 {{site.data.keyword.cloud_notm}}에서 실행할 수 있게 하는 코드입니다. 예를 들어 앱을 {{site.data.keyword.cloud_notm}} Kubernetes 클러스터에서 실행할 수 있게 하는 Helm 차트가 있습니다.

{{site.data.keyword.cloud_notm}} 스타터 킷으로부터 앱을 작성하면 선택한 언어에 대한 우수 사례를 반영하는 검증된 아키텍처로 앱을 시작할 수 있습니다. 

각 앱에는 앱의 기술적 세부사항과 앱이 즉시 실행되지 않을 경우 앱을 실행하기 위해 필요한 작업에 대해 설명하는 README 파일이 포함되어 있습니다.
{: tip}

## DevOps 도구 체인
{: #devops}

DevOps는 앱에 액세스, 개발, 배치, 운영하기 위한 프로시저 및 도구로 구성됩니다. DevOps 도구 체인은 DevOps 태스크를 자동화하는 링크된 서비스 세트입니다. 아주 단순한 앱으로 DevOps를 수동으로 수행할 수 있지만 앱 복잡도가 증가하면서 자동화 필요성이 빠르게 증가하고 도구 체인 자동화가 Continuous Delivery를 위한 필수 요건이 되었습니다.

DevOps 도구 체인의 핵심 컴포넌트는 GitHub와 같은 코드 버전 제어 저장소입니다. 추가 도구는 백로그 추적, Delivery Pipeline, IDE 및 모니터링 서비스(예: [{{site.data.keyword.cloud_notm}}DevOps Insights](../services/DevOpsInsights/index.html#gettingstarted))를 포함할 수 있습니다.

스타터 킷을 사용하여 앱을 작성한 경우, 새 도구 체인을 작성하고 앱 세부사항 보기에서 **Cloud에 배치**를 클릭하여 쉽게 앱을 배치할 수 있습니다. 코드 저장소, 문제점 저장소, Delivery Pipeline 및 웹 IDE가 있는 도구 체인이 작성됩니다.

그런 다음 여러 팀을 수용하고 개발, 테스트 및 프로덕션을 위한 별도의 환경에 배치하기 위해 이 도구 체인에서 빌드하고, 앱을 위한 엔터프라이즈급 협업 Continuous Delivery 모델을 구축할 수 있습니다.  

![Continuous Delivery ](images/garage_continuous_delivery2.png "개발자 경험은 개발 분기로 Continuous Delivery를 설정합니다.")

또한 개발자 대시보드의 앱 개요 페이지에 있는 **다운로드** 단추를 클릭하여 앱 코드를 한 눈에 볼 수 있습니다. 전체 앱 코드 구조를 포함하는 `.zip` 파일로 코드가 다운로드됩니다. {{site.data.keyword.dev_cli_notm}}을 사용하여 파일을 쉽게 추출하고 로컬로 코드를 실행하거나 코드 관리 저장소에 추가할 수 있습니다.

## 명령행 인터페이스
{{site.data.keyword.dev_cli_notm}}을 통해 앱을 로컬로 코딩, 빌드 및 실행할 수 있습니다.  일반적인 패턴은 개발자 대시보드를 통해 앱을 작성하고, {{site.data.keyword.dev_cli_notm}}을 사용하여 로컬로 개발한 후에 사용자 저장소로 업데이트를 푸시하고 배치 도구 체인을 시작하기 위해 병합하는 것입니다.

## Garage Method 개발
{: #developer_concepts}

[Garage Method](https://www.ibm.com/cloud/garage/)를 확인하여 IBM이 어떻게 사용자의 조직에서 앱 개발을 지원할 수 있는지 알아보십시오.  

![Garage Method 단계 개요](images/garage_phases_overview2.png "Garage Method 단계 개요")*Garage Method 단계 개요*

{{site.data.keyword.cloud_notm}}는 Garage Method 또는 사용자가 선호하는 메소드를 사용하여 성공적인 엔터프라이즈급 프로덕션 앱을 생성하도록 도와줍니다. {{site.data.keyword.cloud_notm}}가 개발자에게 무엇을 제공해야 하는지 더 잘 이해하기 위해서 최신 앱 빌드에 필요한 스킬을 잠깐 살펴보겠습니다.

## 개발자 스킬
{: #skills}

오늘날 사용자는 이전보다 훨씬 더 많은 것을 애플리케이션에 기대합니다. 사용자는 앱이 저장된 데이터 및 실시간 데이터에서 깊이 있는 인사이트를 제공하고, 상시 사용 가능하며 개별적 요구사항에 더 근접하여 충족하기를 원합니다. 이러한 기대치를 충족하기 위해서 애플리케이션 작성자들은 더 다양한 스킬 세트를 이용해야 합니다. 예를 들어 복잡한 코그너티브 애플리케이션에는 디지털 개발자, 클라우드 네이티브 개발자, 스트림 개발자, 데이터 과학자 및 DevOps 전문가의 기여가 필요할 수 있습니다.

 ![개발자 유형](images/developer_skills.png "개발자 관계")

* **디지털 개발자**는 모바일 웹, 음성 및 대화와 같은 특정 디지털 채널을 위한 작성자입니다. 디지털 개발자는 일반적으로 유스 케이스에 초점을 맞추고 포괄적 경험으로서 사용자의 요구사항을 직접적으로 충족시킵니다.
* **클라우드 네이티브 개발자**는 클라우드 컴포넌트를 구성하고 상호 연결하는 것을 전문으로 합니다. 마이크로서비스 및 BFF(back-end-for-frontend) 작성자가 이 카테고리에 해당합니다.
* **스트림 개발자**는 데이터 스트림에서 인사이트 획득 및 처리에 초점을 둡니다. 예를 들어 스트림 개발자는 수신 텍스트, 음성 또는 동영상 스트림을 분석하고 조치를 시작할 수 있습니다.
* **데이터 과학자**는 예측 모델을 생성하기 위해 분석 및 기계 학습을 사용합니다. 이러한 모델은 비즈니스 메트릭에서 사용되고 애플리케이션 사용자에게 심도 있는 인사이트를 제공합니다.
* **DevOps 전문가**는 배치 및 도구 체인 문제 해결의 전문가입니다. 단순한 앱의 경우 개발 팀 구성원이 소단위로 DevOps를 관리하므로 대부분은 전용 전문가가 필요하지 않습니다. 그러나 많은 종속 항목이 있는 복잡한 엔터프라이즈 애플리케이션의 경우 프로덕션 앱을 원활하게 실행하도록 유지하는 데 DevOps 전문가가 필수입니다.

{{site.data.keyword.cloud_notm}}에 빌드된 개발자 기능은 이러한 스킬 세트에 맞게 조정되어 있으며 사용자의 팀이 하나의 플랫폼을 사용하여 앱을 생성, 제공, 실행, 관리할 수 있게 합니다. 예를 들어 모바일 앱을 작성하는 디지털 개발자는 {{site.data.keyword.cloud_notm}} [모바일 개발자 대시보드](https://console.bluemix.net/developer/mobile/dashboard)를, 코그너티브 앱 빌더는 [Watson Studio](https://console.bluemix.net/catalog/services/watson-studio)와 함께 [Watson 개발자 대시보드](https://console.bluemix.net/developer/watson/dashboard)를, 스트림 개발자는 [IBM Real-Time Analytics](../services/StreamingAnalytics/index.html#gettingstarted)를 사용하고, [{{site.data.keyword.cloud_notm}} Continuous Delivery 서비스](../services/ContinuousDelivery/index.html#cd_getting_started)는 DevOps 전문가의 작업을 간소화시킬 수 있습니다.

시작할 준비가 되셨습니까? [여기를 클릭](../apps/index.html)하여 지금 {{site.data.keyword.cloud_notm}}에서 앱을 빌드하십시오!
