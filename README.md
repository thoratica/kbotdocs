## kbotdocs

KBotDocs 작성 방법

<hr>

### 1. 편 만들기

`main` 내에 아래와 같이 작성합니다:
```HTML
<section id="{sectionId}">
   
</section>
```

그리고 `aside div#list-box` 내에 아래와 같이 작성합니다:
```HTML
<ul class="list" id="{sectionId}"><h3 class="list-title">{sectionName}</h3>
  
</ul>
```


### 2. 내용 작성

`section#{sectionId}` 내에 다음과 같이 작성합니다:
```HTML
<div class="con" id="dd{contentId}">
  <h2 class="title">{contentName}</h2>
  <article>
  </article>
  <article>
  </article>
  ...
  <article>
  </article>
</div>
```
세부적인 내용은 `article` 내에 작성합니다. `contentId`은 `0-0`과 같은 형식입니다.

그리고 `aside div#list-box ul.list#{sectionId}` 내에 다음과 같이 작성합니다:
```HTML
<li class="list-el" id="d{contentId1}">{contentName1}</li>
<li class="list-el" id="d{contentId2}">{contentName2}</li>
...
<li class="list-el" id="d{contentIdN}">{contentNameN}</li>
```


> #### 2-1 문장 작성
> 문장 작성은 다음과 같이 합니다:
> ```HTML
> <article>
>   <p>{paragraph1}</p>
>   <p>{paragraph2}</p>
> </article>
> ```
> 줄바꿈은 절대로 `<br />`를 사용하지 않습니다. `<p>`태그를 위 코드처럼 하나를 더 사용하여 줄바꿈을 합니다.


> #### 2-2 
