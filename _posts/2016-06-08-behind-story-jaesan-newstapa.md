---
layout: post
title: "[춘식이의 코드이야기] 고위공직자 재산 공개, 그 뒷이야기"
date: 2016-06-08
author: 춘식
category: "civic-hacking"
sitemap: false
keywords: "뉴스타파, newstapa, 고위공직자, 고위공직자 재산, http://jaesan.newstapa.org, 코드나무, codenamu"
description: "2016년 코드나무가 뉴스타파와 협력하여 구축한 고위공직자 재산 공개(http://jaesan.newstapa.org) 사이트 개발 이야기"
---

> **전체 자산 데이터: 14만378줄**
>
> **전체 자산 종류: 25가지**
>
> **전체 고위공직자 수: 7010명**
>
> **11년간 전체 고위공직 수: 6만6568**

이번 [고위공직자 재산 공개](http://jaesan.newstapa.org) 사이트를 통해 공개된 데이터의 양이다. 코드나무는 뉴스타파와 함께 '공직자윤리법 제3조 제1항'에 의해 [국민에게 재산을 투명하게 공개할 의무가 있는 고위공직자](http://www.gpec.go.kr/system/registration.jsp)들의 재산 정보를 접근성이 뛰어난 형태로 가공하여 검색 가능하게 만들고 누구나 다운로드 받을 수 있도록 공개한 사이트를 구축하였다. 2016년 코드나무가 외부와 협력한 첫번째 프로젝트로서 오늘은 이 사이트가 만들어지기까지의 이야기를 해보고자 한다.

## 개발 과정

뉴스타파 데이터팀에서는 대한민국 전자관보 사이트에 공개된 정기 재산변동사항 공개 문서를 다운받아 엑셀 데이터로 차곡차곡 쌓아놓고 있었다. 글 맨 아래에 링크를 참조해놓았으니 꼭 한번 이 관보 pdf 파일을 다운받아 보길 바란다. '공개는 하는데 읽지는 말았으면 좋겠어'라는 느낌? 정말 열자마자 끄고싶어진다. 이렇게 뉴스타파가 쌓아놓은 재산 공개 자료가 무려 11년치이다. 바로 이 데이터를 시민들이 함께 검색하고 찾아볼 수 있도록 공개하고 싶은 마음으로 코드나무로 연락이 왔다.

때마침 코드나무에서는 2016년에 들어오면서 오픈 데이터 저장소를 구축하고, 외부 시민단체들과 협력하여 데이터를 공개하면서, 동시에 공개한 데이터를 활용하여 다양한 시각화 작업을 시도해 볼 계획을 가지고 있었다. 2010년부터 오픈데이터 운동을 해오면서 느낀 점은

1. 이미 많은 공공데이터가 공개되어 있지만 정작 각 분야에서 중요한 역할을 가진 시민단체들이 잘 활용하고 있지 못함
2. 많은 자료를 수집하고 동시에 캠페인에 활용하고 있지만 데이터에 대한 의식과 여력이 충분치 않아 보다 효과적으로 활용하지 못함
3. 서로 다른 단체들간의 자료가 데이터의 형태로 공유되지 않아 단체들간의 혹은 일반 시빅 해커들이 활용하여 여러가지 방향으로 시도해볼 수 있는 가능성이 줄어듦

등이다. 이를 해결하기 위하여 공공데이터를 포함한 시민단체들이 수집한 자료들 - 데이터지만 데이터가 아닌 -을 공동으로 구축하고 공개할 저장소를 만들고, 직접적인 기술에 대한 지원을 제공하기로 계획을 세운 것이다. 이런 와중에 뉴스타파의 연락을 받고 퍼즐조각이 맞추어지듯 데이터를 공개하고 검색서비스를 구축하기 위한 작업이 곧바로 시작되었다.

주로 프로젝트는 코드에서 내가 개발을, 뉴스타파 데이터팀에서 김강민님께서 데이터 가공을, 뉴스타파 개발팀에서는 배민효님과 최미정님께서 디자인을 맡아주시면서 주 1~2회씩 함께 작업물을 공유하고 기획을 발전시켜 나가며 진행하였다. 물론 2016년 3월 정기공개 시기를 놓쳤으며, 2016년 4월 제 20대 국회의원 시기를 놓쳤지만 결국 6월 2일 작은 기자간담회와 함께 대중들에게 공개되었다.


## 공개 이후 반응

![고위공직자 재산 정보 사이트 구글 분석 결과](/images/2016/06/jaesan_analytics.png)

*고위공직자 재산 정보 사이트 구글 분석 결과*

공개 첫날 방문자 수는 약 7000명, 둘째날은 약 5000명, 이후 매일 평균 500 ~ 600명이 방문하고 있으며, 현재까지 누적 페이지 뷰 수는 약 73,000명 정도이다. 솔직히 내 경험 내에서는 이런 반응을 비교해볼만한 대상이 없기 때문에 이 숫자들이 크게 와닿지는 않더라. 다만, 페이스북을 통한 지인들의 감사함(?) 표현과 익명의 사람들이 남기는 뉴스타파와 코드[옛 CC Korea]에 대한 감사말들을 보며 이렇게 훌륭한 기회를 결과물로 만들었던 뉴스타파분들에게 나또한 감사를 표하고 싶다.

<blockquote class="twitter-tweet" data-lang="ko"><p lang="ko" dir="ltr">내가 후원하는 두 개의 단체, <a href="https://twitter.com/newstapa">@newstapa</a> 뉴스타파와 <a href="https://twitter.com/cckorea">@cckorea</a> 가 고위공직자 재산을 검색하는 사이트를 공동 제작했다. <a href="https://t.co/h8NQcqLImE">https://t.co/h8NQcqLImE</a> 후원금 내는 보람이 있군.</p>&mdash; 생각 없는 트잉여 (@mirooahn) <a href="https://twitter.com/mirooahn/status/738281774854197248">2016년 6월 2일</a></blockquote>
<script async src="//platform.twitter.com/widgets.js" charset="utf-8"></script>


## 개발 후 생각

#### 1. 오픈데이터에 대한 언론사의 고민

이번 프로젝트를 통해 기존 시빅 해커들이나 시빅 해킹을 하는 단체([코드포아메리카](http://codeforamerica.org), [열린 지식 인터네셔널](http://okfn.org) 등)들이 아닌 언론사가 오픈 데이터에 대해 갖는 생각을 들어볼 수 있었다.

* 데이터의 정합성

	이 프로젝트의 가장 중요한 점은 누구나 데이터를 다운로드 받을 수 있도록 CC라이선스를 적용하여 공개하는 부분이다. 코드나무가 비용없이 협력하게 된 **유일한** 이유도 바로 이 부분이다. 한가지 아쉬운 점은 검색 가능하도록 만든 11년치의 데이터 중 절반에 해당하는 2005년부터 2010년까지의 데이터는 다운로드 받을 수 없다는 것. 뉴스타파의 결정에 대한 이유는 수긍이 간다. 2011년 이후부터는 관보 pdf 파일이 기계적으로 인식이 가능한 형태이기 때문에 데이터의 정합성에 자신이 있지만 2010년 이전까지의 데이터는 기계적으로 인식이 불가능하여 많은 노력을 들여 수작업으로 일일이 옮겨적었던 것. 이로 인해 데이터가 부득이하게 틀리는 경우가 생길 수 있고 이 경우 언론사 입장에서는 언론사가 필연적으로 가져야할 신뢰도에 큰 타격이 올 것이 걱정된다는 것이 이유였다.

	<a data-flickr-embed="true"  href="https://www.flickr.com/photos/bitterlysweet/26131863/in/photolist-3iW6n-pihQxc-6heoCp-6UzGUy-fkThbN-fiQWyu-ftsn7k-9gjDKB-nr8Jz7-bvoeEN-fiAK22-dtdaLj-bo22bc-o4pFUS-7zehox-4BLC29-FKgkfy-7PqpE2-pmVeXu-ahzfJD-bqmNA4-b93qHp-nhqyoA-9kpkv-7M86c7-7jKEH9-bQX8v6-7M85ZC-4TFdaM-fiQU1W-dysm8-4mswnB-fiQV1E-fiQTN1-Bv5VJS-mc7hCL-eDVdiy-NvYJz-rSx7ss-afs3PH-catSkG-p8tskq-7Dasm9-8BwYW7-rupR4P-oFFAbs-azABjM-swDaT7-phcLQ5-eqDJdf" title="Look Left , Look Right ."><img src="https://c8.staticflickr.com/1/22/26131863_ff3c5984da.jpg" width="500" height="375" alt="Look Left , Look Right ."></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

	데이터를 다루는 일을 하면서 데이터의 신뢰도는 당연히 가장 중요한 문제 중 하나이다. 다만, 수작업으로 일일이 옮겨가면서 작성한 5년치 데이터를 과연 나중에라도 대조하면서 100% 정확도를 맞추는 날이 올까? 그렇지 못하다면 평생 5년치의 데이터는 공개하지 않는다는 뜻일까? 우리가 제안한 지점은 데이터 상에서 실수가 발견되더라도 쿨하게 인정하면서 집단지성을 이용하여 잘못된 데이터가 있으면 제보를 통해 바로잡자라는 절충안이였다. 뭐 아시다시피 공개는 11년 이후 데이터만 되어서 큰 아쉬움으로 남는다.

* 국내 언론사들의 잘못된 관행

	아직 관보 pdf 파일을 열어보지 않았다면 지금에라도 열어보고 오면 좋겠다. 이 pdf 자료를 무려 11년치나! 엑셀로 옮기기 위해 뉴스타파가 들인 공이 얼마나 될까 상상이나 되는가? 혹시 그렇다면 뉴스타파에서는 이 데이터를 돈을 주고 판매를 할 생각이였을까? 절대 아니다. 100% 시민들의 후원금으로만 돌아가는 뉴스타파는 어떠한 방법으로라도 영리적인 목적의 활동은 하지 않는다고 한다. 다만, 뉴스타파에서 이번 데이터 뿐만 아니라 다른 상황에서도 아쉬워 했던 부분은 우리나라 언론들이 다른 언론사들에 대한 출처 표기를 명확히 해주지 않는 아쉬운 관행에 대해 여러번 이야기를 하더라. 이번 재산 데이터 또한 물론 궁극적인 자료의 출처는 대한민국 전자관보 홈페이지 이지만 보시다시피 pdf를 읽어내기란 쉽지가 않다. 분명 이렇게 검색사이트를 구축하고 원데이터까지 공개하고 나면 pdf가 아닌 이 사이트나 이 데이터를 이용할 것이다. 과연 얼마나 많은 언론사가 관련 기사를 쓰면서 '뉴스타파의 서비스를...', '뉴스타파가 공개한 데이터를...' 이란 출처 표기를 할지 의문이라는 것이 뉴스타파의 생각이다.

#### 2. 시의성이냐 완성도냐

언론사의 생명 중 하나가 바로 시의성이다. 사회 곳곳에서 지금도 수많은 일들이 벌어지고 있기 때문에, 사람들이 주목할 필요가 있는 사건, 현재 놓쳐서는 안될 이슈들을 주목하게 만들어주는 것이 언론의 큰 역할 중 하나이다. 이번에도 결국 3월 정기공개, 4월 국회의원 선거라는 중요한 시기를 놓쳤지만 처음부터 이 시기를 목표로 시작하였다.

여기서 개발자로서 또 프로젝트를 바라보는 사람으로서 아쉬운 점은 ~~아직 부족한 개발 실력에 대한 핑계로 들어도 좋다~~ 11년치에 해당하는 대형 자료를 '검색'을 목표로 구축했던 이번 프로젝트 만큼은 시의성 보다는 완성도를 더 우선순위에 두었으면 어떨가 하는 생각이다. 결국 짧은 시간 내에 데이터를 검색 가능하고, 차트와 테이블을 통해 데이터를 살펴볼 수도 있고, 다양한 기기들에서도 불편 없이 사이트를 활용할 수 있게 만들기 위해서 담아내지 못한 부분들도 꽤 있다(예를 들어 현재는 자산의 종류를 큰 분류로만 나누어 놓았지만 실제 데이터에는 세부 정보까지 들어있다).

![실제 박근혜 대통령에 대한 재산 정보](/images/2016/06/president_assets_detail.png)

*실제 박근혜 대통령에 대한 재산 정보*

이번 프로젝트는 단순한 시각화 작업과는 달리 앞으로도 매일, 매월 사람들이 수시로 사용할 것이며, 매년 새로 공개되는 고위공직자 재산 정보도 새로 업데이트 될 것이다. 지금은 단순히 검색을 위한 사이트이지만 앞으로 공직자들의 재산을 모든 시민이 감시하는 중요한 플랫폼으로 성장해나갈 수도 있을 것이다. 이 사이트가 갖는 중요한 역할만큼 앞으로 더 완성도 있고 많은 정보와 중요한 이야기를 담아낼 수 있는 플랫폼으로 발전해 나갔으면 좋겠다.


#### 3. 저널리즘이 개발자를 품어야 하는 이유

사회 모든분야에서 웹사이트, 앱서비스는 선택이 아닌 필수가 되었다. 특히 사용자나 독자를 직접 맞닥뜨리는 모든 분야에서는. 이중에서도 언론처럼 직접 시민들과 긴밀하게 소통이 필요한 곳에서 IT라는 수단은 가치만큼 중요한 요소이다. 안타깝게도 국내 시민단체들을 살펴보면 실제 개발자가 직원으로 상주하는 곳이 거의 없다. 많지 않는 것도 아니고 거의 없다 정말. 아무래도 코드나무가 2016년 시민단체들과 협력 계획을 세운 것에 대한 이유 중 큰 부분을 차지하기도 한다.

저널리즘의 1차적 목표는 위에서 언급한대로 이슈를 선정하고 올바른 시각으로 시민들에게 전달하고 설득시키는 일일 것이다. 여기서 내가 갖는 의문점은 시민들에게 충분히 잘 전달하고 있는가이다. 굳이 데이터 저널리즘을 언급하지 않더라도 개발자의 역할은 상당하다. 시민들이 기사를 보다 쉽게 읽도록 웹사이트를 만드는 일, 보다 많은 사람들이 중요한 사안에 접근할 수 있도록 접근성을 높이는 일, 모바일 기기로 대부분의 컨텐츠를 소비하는 대중들에게 이야기를 전달할 수 있도록 앱으로도 제공하는 일 등. 이번 프로젝트에서도 사람들이 쉽게 이해할 수 있는 시각화 작업이 들어가지는 않았지만 과거 pdf를 복잡하게 뒤져야 했던 것에 비해 고위공직자 재산 정보에 대한 접근성이 비교도 안되게 향상되었다. pdf 다운로드 숫자가 겨우 약 3000건에 불과했던 것에 비하면 약 20배도 넘는 조회수를 기록한 것이다. 단 며칠만에.

![정기공개 관보 다운로드 수](/images/2016/06/gwanbo_download.png)

*2016년 6월 8일 현재 정기공개 관보 pdf 다운로드 수, 맨 오른쪽 3463*

굳이 그런것이 필요해라는 생각이 들 수 있다. 하지만 데이터 저널리즘을 언급하면 개발자의 역할은 선택이 아닌 필수가 된다. 더 이상 세상 곳곳에서 일어나는 모든 일들을 발로 쫓고 글과 영상으로 담아내는 것은 불가능하다. 특히 정확한 사실과 통찰을 바탕으로 중요한 이슈를 선정하고 깊은 이야기를 담아내야 하는 언론에서는 이런 불가능을 데이터로 가능하게 만들 수 있다. 데이터 저널리즘이란 데이터를 통해 사회 현상을 읽고 분석하며 분석한 결과를 글이나 영상 뿐만 아니라 시민들이 이해하기 쉬운 시각화 작업 등으로 대중들과 소통하는 방법이다. 정부에서는 이미 수많은 공공데이터를 공개하고 있으며 사회 곳곳에서도 직접 수집하거나 간접적으로 획득할 수 있는 데이터들이 넘쳐난다. 과거처럼 펜과 카메라만으로 사회 현상을 읽거나 이야기를 시민들에게 전달하는 것에 머물러 있어서는 안된다. 저널리즘은 꼭 개발자를 품어야 한다. 더 깊은 이야기를 끌어내려면, 그리고 이 이야기를 시민들에게 잘 전달하려면.

<a data-flickr-embed="true"  href="https://www.flickr.com/photos/jwyg/6892044360/in/photolist-bv2wF3-epZQu9-ehBR2S-ecp3D6-eckTCA-eBjc9n-exdpBT-eArfr6-eLTWFA-ecV8sT-et16pU-6eMSU8-eHaqoG-eh6MEm-eNpxAy-eAwNiL-eKZcGX-erCcqh-eqCSZD-eGEfHT-eKSFj4-bHWiJ6-ezgNZe-eFf3CF-bHWiGT-eL6ETS-bv2wJJ-biqxVa-et32Us-ewxwjF-edhoX9-8eDNaT-eLXyYU-eFc5d9-eBqBbf-eAkay3-61QHcU-eFtcV3-eX5sMZ-fiVrNh-ei8bj9-eqyRHC-eAiavm-9E7S2e-ed3cw9-edgCDm-9GRXSS-9Q19dd-fiGHQr-61CvUx" title="Data Journalism Handbook - Chapter 1: Introduction"><img src="https://c1.staticflickr.com/8/7129/6892044360_78f82b5199_b.jpg" width="500" height="375" alt="Data Journalism Handbook - Chapter 1: Introduction"></a><script async src="//embedr.flickr.com/assets/client-code.js" charset="utf-8"></script>

*[Data Journalism Handbook - Chapter 1: Introduction, CC BY-SA, 출처: jwyg(플리커)](https://www.flickr.com/photos/jwyg/6892044360/in/photolist-bv2wF3-epZQu9-ehBR2S-ecp3D6-eckTCA-eBjc9n-exdpBT-eArfr6-eLTWFA-ecV8sT-et16pU-6eMSU8-eHaqoG-eh6MEm-eNpxAy-eAwNiL-eKZcGX-erCcqh-eqCSZD-eGEfHT-eKSFj4-bHWiJ6-ezgNZe-eFf3CF-bHWiGT-eL6ETS-bv2wJJ-biqxVa-et32Us-ewxwjF-edhoX9-8eDNaT-eLXyYU-eFc5d9-eBqBbf-eAkay3-61QHcU-eFtcV3-eX5sMZ-fiVrNh-ei8bj9-eqyRHC-eAiavm-9E7S2
	e-ed3cw9-edgCDm-9GRXSS-9Q19dd-fiGHQr-61CvUx)*


## 참조

1. 사이트 바로가기: [고위공직자 재산 공개 사이트](http://jaesan.newstapa.org)

2. *정부에서는 매년 3월 25일 '정기 재산변동사항 신고내역'을 정리하여 고위공직자 재산 정보를 [대한민국 전자관보](http://gwanbo.korea.go.kr/) 홈페이지를 통해 pdf 파일로 공개하고 있다. 직접 pdf를 확인하고 싶으신 분들은 [대한민국 전자관보](http://www.moi.go.kr/frt/sub/a05/gwanboPubNo/screen.do)에 들어가서 제18726호 관보를 열어보면 2016년 3월 정기 공개 파일을 볼 수 있다.*
