# OldTweetDeck
옛날 트윗덱을 공짜로 되돌립니다!
현재 쉽게 설치하는 방법은 없지만, 이 리포지토리를 다운하고 크롬/엣지/오페라/웨일 등의 다른 크로미움 브라우저에 이용하능합니다.
  
2015년과 2018년의 트위터를 다시 이용하는 것에 관심있다면, [OldTwitter](https://github.com/dimdenGD/OldTwitter) 확장프로그램도 한번 보세요.  
  
![Screenshot](https://lune.dimden.dev/9713d947d56.png)  

## 설치
메모: 설치 후에 확장프로그램 파일(크로미움의 경우 압축 해제한 폴더, 파이어폭스의 경우 ZIP파일)을 삭제하지 마세요.
### 크로미움 (크롬, 엣지, 오페라, Brave, 웨일 등) 
1. [배포 페이지](https://github.com/dimdenGD/OldTweetDeck/releases)로 가서 `OldTweetDeckChrome.zip`을 다운로드 합니다.
2. 파일의 압축을 풉니다.
3. 확장 프로그램 페이지(``chrome://extensions``)로 접속합니다.
4. 개발자 모드를 활성화 합니다. (페이지 어딘가에 스위치가 있을 것입니다.)
5. "압축해제된 확장프로그램을 로드합니다" 버튼을 누릅니다.
6. 압축해제한 파일의 폴더를 선택합니다.
7. tweetdeck.twitter.com으로 가서 옛날 트윗덱을 즐깁니다.
8. [지속적인 지원을 위해 기부해주시면 감사합니다](https://www.patreon.com/dimdendev)

### 파이어폭스
#### Nightly / 개발자 버전
1. [배포 페이지](https://github.com/dimdenGD/OldTweetDeck/releases)로 가서 `OldTweetDeckFirefox.zip`을 다운로드 합니다.
2. Firefox Configuration Editor (`about:config`)로 접속합니다.
3. `xpinstall.signatures.required`을 검색하여 false로 바꿔줍니다.
4. 부가 기능 관리자 페이지(``about:addons``)에 접속합니다
5. "파일에서 부가 기능 설치..." 버튼을 누릅니다.
6. 다운로드한 zip 파일을 선택합니다.
7. tweetdeck.twitter.com으로 가서 옛날 트윗덱을 즐깁니다.
8. [지속적인 지원을 위해 기부해주시면 감사합니다](https://www.patreon.com/dimdendev)

#### 안정 버전
**안정 버전에서 확장프로그램을 이용하는 것은 추천하지 않습니다.**
1. `about:debugging#/runtime/this-firefox`으로 갑니다.
2. "임시 부가 기능 로드..."를 누르고 다운로드한 zip 파일을 선택합니다.
3. **이 방법으로 파이어폭스에 설치할 경우, 브라우저가 닫히고 나서 삭제될 것입니다.**

### 사파리
지원안함

## 업데이트
트윗덱 서버쪽의 파일이 업데이트 되면, (설정에서 `localStorage.OTDalwaysUseLocalFiles = 1`을 작성하지 않았을 경우) 재설치할 필요 없이 새로고침만으로 자동으로 새로운 파일이 업데이트 됩니다.
확장 프로그램 파일 자체가 업데이트 되면, 확장프로그램을 삭제후 재설치 하세요.


## Better TweetDeck
Better TweetDeck이 이 확장프로그램과 장동하도록 만든 포크가 있습니다, [여기](https://github.com/dimdenGD/BetterTweetDeck/)에서 찾을 수 있으며. 이 확장프로그램과 같은 방식으로 설치할 수 있으며, [릴리즈 페이지](https://github.com/dimdenGD/BetterTweetDeck/releases)에서 반드시 다운로드해야 합나다.  
 
## FAQ
#### Manifest version 2 is deprecated, and support will be removed in 2023. 이라는 경고가 뜹니다.
무시하세요

#### 유저(User) 또는 검색(Search) 열이 로딩되지 않습니다.
API 제한에 도달했습니다. 일정 시간이 지난 후에 원래대로 돌아올 것입니다.
  

## 업데이트 내역
### 이 프로젝트를 계속 유지하기 위해 [기부](https://dimden.dev/donate/)를 고려해 주세요.
<details>
<summary>업데이트 내역</summary>

#### 3.1.8
* "북마크 트윗" 버튼 추가!
* 일식 심볼이 해시태그와 링크를 부수는 현상 수정
* 트윗 확장이 링크를 비활성화 하는 문제 해결
#### 3.1.7
* 리밋을 우회하는 설정이 추가되었습니다! 사용하려면:

![](https://github-production-user-asset-6210df.s3.amazonaws.com/26517362/269732181-f3eb8979-a452-4080-bc50-a96d1cc41ed6.png)
![](https://github-production-user-asset-6210df.s3.amazonaws.com/26517362/269732138-785187b2-fbdd-456f-b53e-007b9ab0b68f.png)

리밋 우회와 관련하여 유의해야 할 사항:
* 속도 제한을 받은 후에 우회를 활성화한 경우 OldTweetDeck은 작동하지만 웹의 Twitter는 한동안 속도 제한을 받을 수 있습니다.
* 분명히, 이것을 사용하는 것은 안하는 것보다 더 위험합니다. 자신의 위험을 무릅쓰고 사용해야 합니다.
* 한동안 테스트하지 않았기 때문에 실제로 장기적으로 잘 작동하는지 모릅니다. 한동안 이 설정을 활성화했지만 여전히 속도 제한이 있는 경우 모순적이게도 이 설정을 비활성화하면 속도 제한을 제거하는 데 도움이 될 수 있습니다(이론상 입니다)
기타 수정사항:
* 긴 리트윗이 올바르게 확장되지 않는 문제 해결
* 확장된 트윗의 끝에 있는 t.co 링크를 제거했습니다.
#### 3.1.6
* 일부 사용자에 대해 답장이 로드되지 않는 문제 해결.
#### 3.1.5
* 긴 텍스트 트윗을 위한 "트윗 확장" 버튼 추가
* "..."(3개의 점 기호)가 트윗의 시작과 끝에서 제거되는 문제 해결
* 트윗 길이 계산이 미스 해결(트윗-텍스트 라이브러리 업데이트)
#### 3.1.4
대부분 다 고쳤지만:
* 리밋 제한 우회가 더 이상 작동하지 않습니다
* 활동(Activity) 탭이 더 이상 작동하지 않습니다
알려진 문제:
* ~~트윗을 게시할 수 없음~~ 해결
* ~~리트윗이 작동하지 않음~~ 해결
* ~~삭제가 작동하지 않음~~ 해결
* ~~답장이 제대로 표시되지 않음~~ 해결
* ~~인용 트윗에 인용 트윗이 포함되지 않음~~ 해결
#### 3.1.3
답장 해결
#### 3.1.2
트윗 삭제 해결
#### 3.1.1
트윗 해결
#### 3.1.0
katabame/main과 분기 병합
readme 수정
#### 3.0.8
이 버전은 요청에 가로채기를 추가했습니다. 일반 트위터의 요청을 리버스앤지니어링 하여서, 일반 트위터에서 사용하는 해당 요청을 찾을 수 있었습니다. 이제 트윗댁이 종료 API를 사용하려고 하면, 요청이 새 엔드포인트로 리다이렉트 되고, 결과가 옛날 포멧으로 변환됩니다.

이것은 유저(User)와 검색(Search)열을 고칩니다. 저는 더 많은 API가 고장날 것으로 예상합니다. API가 고장나면 작동하는 API로 교체하는 것을 계속 할 것입니다. 제가 작성하는 요청은 일반 트위터 요청과 동일하므로 안전하다는 것을 명심하십시오. 유저 및 검색 열은 이제 속도제한의 영향을 받습니다. 해당 열이 로드되지 않으면 F12를 누른 뒤, 콘솔(Console)탭으로 가서 `localStorage.abuseAPIkeys = '1'`을 작성한 뒤 엔터를 누르세요. 이렇게 하면 리밋이 두 배로 늘어납니다.

BetterTweetDeck을 설치하셨다면 OldTweetdeck V3에 작동하도록 수정한 [새로운 업데이트](https://github.com/dimdenGD/BetterTweetDeck/releases/tag/v4.11.1)가 있습니다.
#### 3.0.7
main 분기 병합
  
#### 3.0.6
로그 제거
#### 3.0.5
버전 업데이트
#### 3.0.4
리밋을 2배로 늘립니다.
#### 3.0.3
고정된 트윗을 보여줍니다(만약에 최신에 있을 경우)
#### 3.0.2
여러 유저의 타임라인이 주계정만 보여주는 문제를 해결했습니다.
#### 3.0.1
버전 충돌
#### 3.0.0
리퍼러 제거
#### 2.0.5
2.0.4의 문제가 파이어폭스에서 여전히 발생하는 문제를 해결했습니다.
#### 2.0.4
신트윗덱이 종종 구트윗덱과 같이 뜨는 문제를 해결했습니다.
#### 2.0.3
manifest V2가 파이어폭스에서 작동안하는 문제를 해결했습니다.
#### 2.0.2
문서를 클릭할 수 없는 현상을 수정하였습니다.
#### 2.0.1
신트윗덱의 head와 body를 제거합니다.
#### 2.0.0
이 버전부터 manifest V2를 사용하여 별도의 서버가 필요하지 않습니다.
#### 1.0.2
효과 있을듯?
</details>

## ~~투명한 면책조항~~
옛날 정보는 만료되었습니다.
확장프로그램을 manifest v2로 다시 만들었고, 외부서버가 필요하지 않습니다.
