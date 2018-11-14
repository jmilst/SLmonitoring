---

copyright:
  years: 2014, 2018
lastupdated: "2018-02-02"

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 취약성 스캔
{{site.data.keyword.BluSoftlayer_full}}는 Nessus와 협력하여 {{site.data.keyword.BluSoftlayer_notm}} 네트워크의 디바이스에 대한 취약성 스캔을 제공합니다. 취약성 스캔은 디바이스의 취약한 영역을 테스트하고 호스트 디바이스에 대한 분석, 보안 문제 및 수정사항의 보고서를 리턴합니다. 디바이스에 대한 취약성 스캔을 수행하면 해당 디바이스가 항상 안전한 상태로 유지되며 디바이스가 취약하거나 손상될 수 있다고 판단되는 경우 사용할 첫 번째 리소스가 됩니다. 계정과 연관된 디바이스에서 [고객 포털 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com/)을 사용하여 취약성 스캔을 완료할 수 있습니다.
{:shortdesc}

## Nessus 보안 스캐너 
{{site.data.keyword.BluSoftlayer_notm}}에서는 오픈 소스 Nessus 스캔 도구로 구동되는 온라인 보안 스캐너를 제공합니다. 이 보안 스캐너는 보안 탭에서 **스캐너**를 클릭하여 액세스할 수 있습니다. 자세한 정보는 [Nessus 스캔 도구 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](http://www.nessus.org/nessus/)를 참조하십시오.

**스캐너** 페이지에서는 {{site.data.keyword.BluSoftlayer_notm}}에서 호스팅되는 Nessus 도구에 사용 가능한 하드웨어 목록을 제공합니다. 서버를 스캔하거나 이전 스캔의 결과를 보려면 검사할 서버에 대한 세부사항 링크를 클릭하십시오. 취약성 스캔 세부사항 페이지에는 서버에 대한 간단한 요약(서버 이름, 스캔될 IP 주소 및 서버가 위치한 데이터 센터 포함)이 표시됩니다. **스캔 시작**은 가능한 빨리 Nessus 스캔 서버를 사용하여 취약성이 스캔되도록 서버를 스케줄합니다.

이후 서버 요약에 현재 및 이전 Nessus 취약성 스캔의 표가 표시됩니다. 각 스캔에 대해 스캔이 요청된 날짜, 스캔이 시작된 날짜, 스캔의 상태, 스캔이 완료된 경우 Nessus 보고서에 대한 링크가 나열됩니다.

Nessus 보고서의 상태는 다음 중 하나일 수 있습니다.

* 스캔 보류 중: 스캔이 Nessus 스캐너 상자에 스케줄되었습니다.
* 스캔 처리 중: 스캔이 현재 진행 중입니다.
* 보고서 생성 중: 스캔이 완료되었지만 테스트 결과가 보고서로 컴파일되는 중입니다.
* 스캔 완료: 스캔이 성공적으로 완료되었으며 취약성 보고서가 생성되었습니다.
* 스캔이 취소됨: {{site.data.keyword.BluSoftlayer_notm}} 기술자가 수동으로 Nessus 스캔을 취소했습니다.

**보고서 보기**를 클릭하여 이 표에 나열되어 있는 성공적으로 완료된 모든 Nessus 스캔에 대한 보고서를 볼 수 있습니다. 보고서에는 두 개의 표가 있습니다. 스캔 세부사항 표에는 스캔된 호스트 수, 발견된 열린 보안 취약성 수(허점) 및 발견된 가능한 보안 취약성(경고) 수가 나열됩니다. 두 번째 표에는 발견된 모든 보안 문제, 취약성이 발견된 호스트 및 가능한 취약성에 대한 설명이 나열됩니다.

오픈 소스 Nessus 도구는 취약성이 발견될 때 새 테스트가 개발되도록 하는 플러그인 기반 도구입니다. {{site.data.keyword.BluSoftlayer_notm}}에서 내부 Nessus 도구를 정기적으로 업데이트하기 때문에 새로운 위협에 대한 최신 정보를 얻으려면 보안 스캐너를 정기적으로 스캔하는 것이 좋습니다.

스캔에 성공하려면 173.192.255.232 및 172.17.19.38 모두의 연결이 서버에 액세스할 수 있어야 합니다.