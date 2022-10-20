---
description: 코딩할 때 주의해야 할 방법을 안내합니다.
---

# 정보통신(웹)접근성 관련 코딩

##

## \<audio> 요소의 필수적인 \<track>

음성화일의 캡을 반드시 제공해야 한다.

Captions와 Subtitles의 차이점:\
Captions(캡션) : TV나 영화에서 말하는 것 이외에 환호와 박수, 웃음과 울음, 청중의 소리까지 번역되는 것.

Subtitles(자막) : 언어에 능숙하지 못한 사람들을 위해 주로 다른 언어로 번역하는 것.

kind="subtitles" 보다는 kind="captions"를 반드시 사용한다.

```html
<audio>
   <source src="mySpeech.mp3" type="audio/mp3">
   <track src="captions_ko.vtt" kind="captions" srclang="ko" label="한글 자막">
   <track src="captions_en.vtt" kind="captions" srclang="en" label="영문 자막">
   <track src="captions_es.vtt" kind="captions" srclang="es" label="스페인어 자막">
</audio>
```

오디오 파일에 대한 캡션이 없으면 청각 장애인 사용자는 말하는 사람의 식별, 대화, 음악 신호 또는 음향 효과와 같은 소리를 통해 전달되는 비음성 정보와 같이 오디오가 전달하는 의미있는 정보를 알 수 없다.

캡션은 오디오 트랙을 통해 사용할 수 있는 콘텐츠의 일부를 제공한다.

가장 효과적인 캡션은 대화, 음악 신호, 음향 효과 및 기타 관련 정보를 포함하여 오디오가 전달하는 모든 의미있는 정보를 전달해야 한다.

