---
description: 키보드를 이용할 수 없는 부분에 추가 스크립트로 접근할 수 있는 구조
---

# 접근성 지원 스크립트

### 링크가 없는 마우스만 이용할 경우(키보드 사용불가)

{% embed url="https://regexr.com/3h62s" %}
정규식 패턴 적용의 접근성 사용불가
{% endembed %}

태그의 구조를 파악할 수 있어야 한다.(data-id 속성의 모든 태그들)

```javascript
document.querySelectorAll('[data-id]').forEach(function(el) {
  // set tabindex and role attributes
  el.setAttribute('tabindex', '0');
  el.setAttribute('role', 'button');

  // add event listener for keydown event
  el.addEventListener('keydown', function(event) {
    // check if the Enter key was pressed
    if (event.key === 'Enter' || event.keyCode === 13) {
      event.preventDefault();

      // If the Ctrl key was also pressed
      if (event.ctrlKey) {
        // create a new double click event
        var dblclickEvent = new MouseEvent('dblclick', {
          bubbles: true,
          cancelable: true,
          view: window
        });

        // dispatch the double click event
        el.dispatchEvent(dblclickEvent);
      } else {
        // create a new click event
        var clickEvent = new MouseEvent('click', {
          bubbles: true,
          cancelable: true,
          view: window
        });

        // dispatch the click event
        el.dispatchEvent(clickEvent);
      }
    }
  });
});

```







{% embed url="https://chat.openai.com" %}

### \<a> 링크 부분에 키보드로 접근하기 어려울 경우

링크 요소 내부에 별도의 버튼들을 제공하여 상세 항목으로 이동한다.

```javascript
// <a> 링크 태그내에 href 속성이 없는 경우에만 다음의 이벤트를 추가한다.
document.querySelectorAll('a:not([href])').forEach(function(el) {
  // add href attribute and set to 'javascript:void(0)'
  el.setAttribute('href', 'javascript:void(0)');

  // add event listener for keydown event
  el.addEventListener('keydown', function(event) {
    // check if the key pressed was the Enter key
    if (event.key === 'Enter' || event.keyCode === 13) {
      // prevent the default action
      event.preventDefault();

      // create a new click event
      var clickEvent = new MouseEvent('click', {
        bubbles: true,
        cancelable: true,
        view: window
      });

      // dispatch the click event
      el.dispatchEvent(clickEvent);
    }
  });
});
```





