---
title: 🏝 한 줄 코딩! ⌨🔨😆 블로그 사용법
author: 발가락
date: 2021-03-17 17:54:48 +0900
categories: [Tutorial]
tags: [getting started]
pin: true
---

## 1. 한줄코딩 Repository 를 Fork 하기

우선 제일 먼저 [Github][github] 를 방문해서 fork 버튼을 찾아누릅니다.

![fork](/assets/img/20210217/fork.png)

## 2. Fork 한 본인의 Repository 에서 작업하기

git 주소를 복사해서 원하는 위치의 디렉토리에서 clone 을 합니다.

![git_clone](/assets/img/20210217/git_clone.png)

```console
git clone https://github.com/너님_아이디/hanjulcoding.github.io.git .
```

## 3. 내려받아 작업하기

- _posts 에서 연도-월-일-영문제목.md 파일 생성
- 기존의 Posts 를 확인해서 MarkDown 양식으로 작성합니다.
- 양식의 내용은 아래와 같습니다.

```console
---
title: 제목
author: 작성자
date: 2021-03-17 17:54:48 +0900 (리눅스 명령어 date '+%Y-%m-%d %H:%M:%S %z' 을 실행하면 시간이 나옵니다.)
categories: [카테고리]
tags: [태그]
(카테고리, 태그는 자동으로 생성됩니다.
pin: true
---

# 제목

내용

...
...
...

```

마크 다운에 대한 추가 내용 확인은 [여기](https://gist.github.com/ihoneymon/652be052a0727ad59601)에서 확인해보세요.

## 4. Commit, Push, Pull Request

작업 완료 후 Commit 과 push 를 합니다.
```console
git commit -m "first commit"
git push origin main
```

작업 환경에 따라 GUI 로 할 수도 있겠네요!

이후 [Github](https://github.com) 로 가셔서

![pr](/assets/img/20210217/pr.png)

이렇게 생긴 곳을 가서

![pr2](/assets/img/20210217/pr2.png)

Pull Request 를 합니다.

![pr3](/assets/img/20210217/pr3.png)

확인하시고 `Create pull request` 를 누르세요.

![pr4](/assets/img/20210217/pr4.png)

이렇게 댓글을 추가할 수도 있겠죠?

![pr5](/assets/img/20210217/pr5.png)

카톡방에 PR 했다고 알려주시면 바로 Merge 할게요!

꼭 알려주세요~!


## 5. 원본 저장소에서 업데이트 받기

작업 전에 미리 설정해서 꼭! Pull 을 받고 진행해요.


1. 내 로컬 PC에 포크 저장소 Clone

```console
git clone https://github.com/6lueparr0t/hanjulcoding.git
```
2. Clone 한 프로젝트 디렉토리로 이동
3. 리모트 저장소 확인

```console
git remote -v

origin	https://github.com/6lueparr0t/hanjulcoding.github.io.git (fetch)
origin	https://github.com/6lueparr0t/hanjulcoding.github.io.git (push)
```

4. 리모트 저장소에 원본 저장소 추가

```console
git remote add upstream https://github.com/hanjulcoding/

hanjulcoding.github.io.git
```

`git remote -v` 명령어를 입력해보면 upstream으로 원본 저장소가 추가된 것 확인

```console
git remote -v

origin	https://github.com/6lueparr0t/hanjulcoding.github.io.git (fetch)
origin	https://github.com/6lueparr0t/hanjulcoding.github.io.git (push)
upstream	https://github.com/hanjulcoding/hanjulcoding.github.io.git (fetch)
upstream	https://github.com/hanjulcoding/hanjulcoding.github.io.git (push)
```

5. 원본 저장소 fetch, merge

```console
git fetch upstream
git merge upstream/main
```

7. 포크 저장소로 push
```console
git push
```


- - -

### <유튜브 소개 영상>
<iframe width="560" height="315" src="https://www.youtube.com/embed/5huAvcd1DPU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### <Github>
[https://github.com/hanjulcoding/hanjulcoding.github.io](https://github.com/hanjulcoding/hanjulcoding.github.io)

### <카카오 오픈채팅방>
"한 줄 코딩" 검색 또는

[https://open.kakao.com/o/gBCDGDUc](https://open.kakao.com/o/gBCDGDUc)

코드 : 1230

[youtube]: https://www.youtube.com/channel/UCyfUmIe1NMBCEzsO2iXBzBQ
[github]: https://github.com/hanjulcoding/hanjulcoding.github.io
[kakao]: https://open.kakao.com/o/gBCDGDUc