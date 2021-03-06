---
description: GitBook을 이용한 책쓰기 사례를 소개한다. 이건 초보자의 글이고 어떤 더 낫은 방법이 있는 지 모르겠다.
---

# GitBook을 이용한 책쓰기

## 절차

> * 세팅하기
> * 매일 매일의 루틴
> * 확인하기\(다시보기\)

이글을 쓰기 위한 절차

## Typora와 GitBook 글쓰기 자동 세팅하기

세팅하기는 앞장에서 설명을 했고, GitBook

GitHub와 GitBook은 어떻게 연계를 하는가?

모르겠으면 아래의 링크를 찾아간다. [https://www.youtube.com/watch?v=e9DMxI\_XOPI](https://www.youtube.com/watch?v=e9DMxI_XOPI)

GibBook 왼쪽 메뉴 Intergrations에서 GitHub를 클릭한다.

책을 쓸 때는 질문을 한다.

GitHub와 연결을 해봤다. 테스트해보

## GitBook과 GitHub 연결하기

깃북과 갓헙을 연결해야 될 것 같다. 왜냐하면, 그래야지 오프라인 노트북에서 글을 쓰고, 이 글을 온라인에 통합시킬 수 있을 것이다. 반대로 온라인에서 쓰고 오프라인에서 편집하는 것도 하나의 좋은 방법이 될 것 같다.

## 소소한 팁들

### 브랜치 충돌 문제해결

GitBook과 GitHub 연결하면서 브랜치때문에 골치가 아팠었다. 저장소를 처음 만들면 'master' 브랜치가 생긴다\(_맞는 지는 확인해 봐야 한다_\). GitBook은 기본적으로 'master' 브랜치만 이용한다. 깃허브는 'main'이 디폴트 브랜치다. main과 master를 유심히 보지 않은 것이 문제였다. 두개의 브랜치로 각각 저장이 되고있었다. 사실 이것이 유용하고 좋은 기능인데, 나는 이번에 처음 알게 되었다. 각각 진행한 문서를 한명이 요청하면 다른 사람이 검토해서 두 파일을 합치거나 하는 기능이다.

어떻게 이문제를 해결하였는가? 어렵게 어렵게 했는데, 결론은 간단하다. main을 master로 rename 하였다. main이 주로 내가 편집하던 것이고, master는 쓰레기글이 많아서, master를 지우고, 기존 main을 rename하였다.

main은 아마 GitBook Desktop 때문에 생긴 것 같다.

![image-20210414200050920](../.gitbook/assets/image-20210414200050920.png)

### description 넣기

```
---
description: 머라머라...
---
# 제목넣기
```

위와 같이 md문서의 처음에 제목위에 넣어주면 gitbook에서 제목아래 설명이 나온다. `description: `을 넣지않아도 실행이 되는데, Contents부분에 깨지고, 제목이 살짝 꼬인다. gitbook의 제목은 사실 summary.md에서 것으로 정해지고, 내용이 있는 md의 제목은 나타나지 않는데, description을 명기안하면, md파일의 제목이 두번째 레벨의 제목으로 들어가게 된다. 사소한 팁이다.

### md 파일명 한글 vs. 영어

md 파일명이 깃허브에서는 문제가 없으나, 깃북에서는 한글을 인식하지 못한다. 자동으로 untitled(?)인가를 붙혀주는데, 피드백이나 나중에 문제가 되지 않을까 싶다. 깃허브를 주로 사용하고, 깃북은 그냥 보여주기만 한다면 사용에는 문제가 없다.

## .DS_Store files

> *Synopsis* 맥에서 폴더에 대한 특성을 갖고 있는 시스템파일이다.

`.DS_Store` 파일(또는 확장자)을 보게 되는데 이것은 Mac의 시스템파일이다. *Desktop Service Store*의 약자다. 집에서 iMac으로 작업한 이후에 생기기 시작했다. 그냥 지워도 안전하다고 한다(https://superuser.com/questions/757593/what-is-ds-store-file-in-windows). 그리고, 어떻게 방지하는지? 지워도 문제가 없는지에 대한 링크가 연결된다. 또한 자세한 것은 위키에도 설명이 되어있다(https://en.wikipedia.org/wiki/.DS_Store). 폴더의 특성정보를 갖고 있다. 아이콘이라든지 백그라운드 이미지 같은 것 말이다. Finder 앱에서 만들어진다. 신경쓰지 말아야 겠다.

