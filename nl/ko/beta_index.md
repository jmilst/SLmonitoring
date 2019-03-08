---

copyright:
  years: 2017, 2018
lastupdated: "2018-03-29"

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}
# IBM Cloud Monitoring 시작하기(베타)
{: #gettingstartedbeta}

{{site.data.keyword.BluSoftlayer_full}} Monitoring Service를 기반으로 구축된 이 베타 모니터링 애플리케이션은 가상 및 베어메탈 서버에 사용할 수 있습니다. 이 베타 프로그램의 개발에 대한 업데이트는 [IBM Cloud 블로그 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://www.ibm.com/blogs/bluemix/2017/12/beta-release-new-vsi-monitoring-tool-ibm-cloud/){: new_window}를 참조하십시오.
{:shortdesc}

## 전제조건

이 베타 프로그램에 참여하려면 다음 요구사항을 충족해야 합니다.
1. SoftLayer 계정이 IBM ID 인증을 통해 IBM Cloud 계정에 연결되어야 합니다. 계정을 연결하려면 SoftLayer 계정의 마스터 사용자가 [{{site.data.keyword.slportal}} ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://control.softlayer.com){: new_window}에 로그인해야 합니다. **계정** 메뉴에서 **Bluemix 계정을 연결합니다!**를 클릭하십시오.
2. 베타를 확인할 각 사용자가 IBM ID에 연결되어야 합니다. 자세한 정보는 [IBM ID 사용자 계정 연결](/docs/account?topic=account-unifyingaccounts#link_customer_accounts)을 참조하십시오.
3. 베타를 확인할 각 사용자에게 IBM Cloud Monitoring Service에 대한 액세스 권한이 있어야 합니다.
   1. [IBM Cloud 콘솔 ![외부 링크 아이콘](../../icons/launch-glyph.svg "외부 링크 아이콘")](https://console.bluemix.net){: new_window}에서 **관리 -> 계정 -> 사용자**를 선택하십시오.
   2. 사용자를 계정에 초대하거나 목록에서 사용자를 선택하십시오.
   3. 사용자에게 **리소스에 대한 액세스 권한 지정**을 선택하십시오.
   4. **서비스**에서 **IBM Cloud Monitoring Service**를 선택하십시오.
   5. 모든 지역에 대해 사용자에게 부여될 **역할**을 선택하십시오.

이러한 전제조건을 충족하지 않으면 현재 베타 모니터링에 액세스할 수 없습니다.


## 베타에 참여

모니터링 베타 프로그램을 시작하려면 다음 단계를 따르십시오. 베타에 참여하면 계정의 모든 적격 가상 및 베어메탈 서버에 대한 서비스가 사용으로 설정됩니다. 참여를 클릭해도 기존 Nimsoft 모니터링 또는 데이터는 영향을 받지 않습니다.
1. (베어메탈에만 해당) [베어메탈 서버에 모니터링 에이전트를 설치하십시오.](/docs/infrastructure/SLmonitoring?topic=slmonitoring-installing-ibm-cloud-monitoring-service-for-iaas-bare-metal-agent-beta-)
<table>
   <CAPTION>표 1. 위치에서 로그 선택</CAPTION>
   <THEAD>
   <TR>
   <th>참여 방법</th>
   <th>수행할 작업</th>
   </TR>
   </THEAD>
   <TBODY>
   <tr>
   <td>IBM Cloud 카탈로그</td>
   <td>
   <ol>
   <li>새 브라우저 창을 열고 <a href="https://console.bluemix.net/catalog/">https://console.bluemix.net/catalog/</a>를 입력하십시오.</li>
   <li><b>로그인</b> 링크를 클릭하십시오. </li>
   <li>이메일 또는 IBM ID를 입력하고 <b>계속</b>을 클릭하십시오.</li>
   <li>비밀번호를 입력하고 <b>로그인</b>을 클릭하십시오.</li>
   <li>**인프라->디바이스 목록->*디바이스 이름***을 선택하여 디바이스 세부사항에 액세스하십시오.</li>
   </ol>
   </td>
   </tr>
   <tr>
   <td>고객 포털</td>
   <td>
   <ol>
   <li>새 브라우저 창을 열고 <a href="https://control.softlayer.com">https://control.softlayer.com</a>을 입력하십시오.</li>
   <li>사용자 이름 및 비밀번호를 입력하고 <b>로그인</b>을 클릭하십시오. 또는 <b>IBM ID로 로그인</b>을 클릭하십시오. 그런 다음 이메일 또는 IBM ID를 입력하고 <b>계속</b>을 클릭하십시오. 비밀번호를 입력하고 <b>로그인</b>을 클릭하십시오. {{site.data.keyword.slportal}}의 기본 페이지가 열립니다.</li>
     <li>**디바이스**에서 **디바이스 이름**을 클릭하여 디바이스 세부사항에 액세스하십시오.</li>
   </ol>
   </td>
   </tr>
   </TBODY>
  </table>
2. **디바이스 -> 모니터링**을 선택하십시오. **베타에 참여**를 클릭하여 시스템 정책 및 알림 베타 탭을 보십시오.

## 다음 단계
1. 수집된 [메트릭](/docs/infrastructure/SLmonitoring?topic=slmonitoring-metrics-collected-beta-)의 세부사항을 검토합니다.
2. 모니터 알림을 [작성하거나 관리](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-monitor-notifications-beta-)합니다.
3. 시스템 정책을 [작성하거나 관리](/docs/infrastructure/SLmonitoring?topic=slmonitoring-creating-and-managing-system-policies-beta-)합니다.
4. [경보를 봅니다](/docs/infrastructure/SLmonitoring?topic=slmonitoring-viewing-monitoring-alerts-beta-).
5. 선택한 디바이스에 대해 현재 사용 가능한 베타 모니터링 그래프 데이터를 검토합니다.

|메트릭                                      |설명                                        |
| --------------------------------------------------------- | --------------------------------------------------- |
|CPU 사용률                                            | 각 코어에 대한 CPU 사용률(%) 및 전체 코어의 평균을 확인합니다. 그래프에서 데이터를 설정하거나 해제하려면 키의 각 메트릭을 클릭하십시오.
|공용 네트워크                                             | 공용 네트워크에 대한 인바운드 및 아웃바운드 데이터를 확인합니다. 그래프에서 데이터를 설정하거나 해제하려면 키의 각 메트릭을 클릭하십시오.       |
|사설 네트워크                                            | 사설 네트워크에 대한 인바운드 및 아웃바운드 데이터를 확인합니다. 그래프에서 데이터를 설정하거나 해제하려면 키의 각 메트릭을 클릭하십시오.           |
|메모리 사용률    | 서버의 메모리 사용률(%)을 확인합니다.     |
|디스크 사용량    | 디스크에서 읽거나 디스크에 쓰는 평균 데이터의 양(바이트) 또는 디스크 대기 시간을 확인합니다. 그래프에서 데이터를 설정하거나 해제하려면 키의 각 메트릭을 클릭하십시오.    |
|온도                                                 | 베어메탈 디바이스의 온도(섭씨 단위)를 확인합니다. 이 데이터는 일부 디바이스에서만 사용 가능합니다.
{: caption="표 1. 베타 메트릭" caption-side="top"}   

## 제한사항
디바이스가 삭제되는 경우 연관된 모니터링 정책은 삭제되지 않습니다. 이러한 정책에 대한 디바이스를 수동으로 삭제해야 합니다.

메트릭 데이터는 15일 동안만 사용 가능합니다.

동시에 10개의 모니터링 정책만 존재할 수 있습니다. 그러나 하나의 정책을 여러 디바이스에 적용할 수 있습니다.

## 문제점 해결
메모리 사용률과 같은 일부 메트릭을 보려면 서버에 Xen 도구가 있어야 합니다. Xen 도구 설치에 대한 정보는 [이미지 준비 및 가져오기](/docs/infrastructure/image-templates?topic=image-templates-preparing-and-importing-images#preparing-and-importing-images)를 참조하십시오.

## 피드백
이 베타에 대한 피드백을 제공하려면 **디바이스 -> 모니터링** 또는 디바이스 세부사항 페이지를 선택하고 **피드백 남기기**를 클릭하여 간단한 설문조사를 완료하십시오. 베타를 종료하고 표준 보기로 돌아가려면 **디바이스 -> 모니터링** 페이지에서 **베타에서 나가기** 링크를 클릭하십시오.
