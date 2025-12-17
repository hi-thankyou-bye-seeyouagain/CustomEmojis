# Custom Emojis 🖼️

커스텀 이모지를 `:커스텀_이모지:` 로 작성하여 웹에서 쉽게 표현할 수 있게 도와주는 스크립트입니다.

## 시작하기

HTML 파일의 `<head>` 태그 안이나 `</body>` 태그 직전에 아래 코드를 한 줄만 추가하면 바로 사용할 수 있습니다.

```html
<script id="Custom-Emoji" defer src="https://cdn.jsdelivr.net/gh/simnple/CustomEmojis@main/script.js"></script>
```

<!-- 티스토리(Tistory) 블로그에 적용하기. -->

## 사용 방법

텍스트를 작성할 때 콜론(`:`) 사이에 이모지 이름을 넣어주면 자동으로 변환됩니다.

폰트 크기에 맞춰 이미지 크기도 자동으로 조절됩니다.

### 작성 예시

```text
블롭이는 기분이 좋다! :blobaww:
블롭이는 슬프다... :blobsad:
```

### 기본 커스텀 이모지 목록

대부분의 이모지들은 [solved.ac 디스코드](https://discord.com/invite/solvedac)의 이미지를 사용했습니다.

|이모지 이름|미리보기|
|:---:|:---:|
|:blobangery:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobangery.webp" width="20">|
|:blobangry:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobangry.webp" width="20">|
|:blobcry:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobcry.webp" width="20">|
|:blobfearful:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobfearful.webp" width="20">|
|:blobimfine:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobimfine.webp" width="20">|
|:blobaww:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobaww.webp" width="20">|
|:blobrofl:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobrofl.webp" width="20">|
|:blobsad:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobsad.webp" width="20">|
|:blobsadrain:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobsadrain.webp" width="20">|
|:blobdead:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobdead.webp" width="20">|
|:blobpats:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobpats.webp" width="20">|
|:blobsob:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobsob.webp" width="20">|
|:blobthinking:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobthinking.webp" width="20">|
|:blobyum:|<img src="https://raw.githubusercontent.com/simnple/CustomEmojis/refs/heads/main/img/blobyum.webp" width="20">|

[이모지가 적용된 블로그 글](https://simnple.tistory.com/22)

## 이모지 추가

자신만의 이모지를 추가하여 사용할 수 있습니다!

1. 이 저장소 우측 상단의 **Fork** 버튼을 눌러 repository를 복사하세요.
2. `script.js` 파일 내의 `CONFIG` 를 원하는대로 수정하세요.

```javascript
const CONFIG = {
    SCALE: 1.2,

    // 여기에 원하는 이모지를 추가하거나 변경하세요.
    // * 이모지들을 줄바꿈할때 쉼표 (,)를 꼭 넣어주세요. *
    EMOJIS: {
        "내이모지": "https://이미지_주소.png",
        "blobaww": "...",
        // ...
    }
};
```

3. 수정한 코드를 저장소에 반영한 뒤, 아래 주소에서 `깃허브_아이디` 부분만 본인의 깃허브 아이디로 바꿔서 적용하세요.

```html
<script id="Custom-Emoji" defer src="https://cdn.jsdelivr.net/gh/깃허브_아이디/CustomEmojis@main/script.js"></script>
```

> [!TIP]
> 만약 프로젝트가 jsdelivr에 캐싱되어 변경된 사항이 바로 적용되지 않을 경우, `https://purge.jsdelivr.net/gh/깃허브_아이디/CustomEmojis@main/script.js` 로 한번 접속하여 캐시를 초기화 해주세요.

## License

이 프로젝트는 [MIT License](https://github.com/simnple/CustomEmojis/blob/main/LICENSE)를 따릅니다.
