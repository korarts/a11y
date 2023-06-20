---
description: Regular expression, Regexp, regex, rational expression, 정규 표현식, 정규식
---

# Regex 정규 표현식

{% embed url="https://ko.wikipedia.org/wiki/%EC%A0%95%EA%B7%9C_%ED%91%9C%ED%98%84%EC%8B%9D" %}
정규 표현식 정의- 위키피디아
{% endembed %}

{% embed url="https://regexr.com/" %}
정규 표현식 시험의 온라인 도구
{% endembed %}

{% embed url="https://regex101.com/" %}
생성기 디버거
{% endembed %}

{% embed url="https://extendsclass.com/regex-tester.html" %}
시각적 표현식 테스터
{% endembed %}

{% embed url="https://www.w3schools.com/jsref/jsref_obj_regexp.asp" %}
w3Schools
{% endembed %}

{% embed url="https://www.regexplanet.com/" %}
프로그램 언어별 정규식
{% endembed %}



정규 표현식(正規表現式, [영어](https://ko.wikipedia.org/wiki/%EC%98%81%EC%96%B4): regular expression, 간단히 regexp[\[1\]](https://ko.wikipedia.org/wiki/%EC%A0%95%EA%B7%9C\_%ED%91%9C%ED%98%84%EC%8B%9D#cite\_note-1) 또는 regex, rational expression)[\[2\]](https://ko.wikipedia.org/wiki/%EC%A0%95%EA%B7%9C\_%ED%91%9C%ED%98%84%EC%8B%9D#cite\_note-Mitkov2003-2)[\[3\]](https://ko.wikipedia.org/wiki/%EC%A0%95%EA%B7%9C\_%ED%91%9C%ED%98%84%EC%8B%9D#cite\_note-Lawson2003-3) 또는 정규식(正規式)은 특정한 규칙을 가진 문자열의 집합을 표현하는 데 사용하는 [형식 언어](https://ko.wikipedia.org/wiki/%ED%98%95%EC%8B%9D\_%EC%96%B8%EC%96%B4)이다. 정규 표현식은 많은 [텍스트 편집기](https://ko.wikipedia.org/wiki/%ED%85%8D%EC%8A%A4%ED%8A%B8\_%ED%8E%B8%EC%A7%91%EA%B8%B0)와 [프로그래밍 언어](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D\_%EC%96%B8%EC%96%B4)에서 문자열의 검색과 치환을 위해 지원하고 있으며, 특히 [펄](https://ko.wikipedia.org/wiki/%ED%8E%84)과 [Tcl](https://ko.wikipedia.org/wiki/Tcl)은 언어 자체에 강력한 정규 표현식을 구현하고 있다.

컴퓨터 과학의 [정규 언어](https://ko.wikipedia.org/wiki/%EC%A0%95%EA%B7%9C\_%EC%96%B8%EC%96%B4)로부터 유래하였으나 구현체에 따라서 정규 언어보다 더 넓은 언어를 표현할 수 있는 경우도 있으며, 심지어 정규 표현식 자체의 문법도 여러 가지 존재하고 있다. 현재 많은 [프로그래밍 언어](https://ko.wikipedia.org/wiki/%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D\_%EC%96%B8%EC%96%B4), 텍스트 처리 프로그램, 고급 텍스트 편집기 등이 정규 표현식 기능을 제공한다. 일부는 [펄](https://ko.wikipedia.org/wiki/%ED%8E%84), [자바스크립트](https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8), [루비](https://ko.wikipedia.org/wiki/%EB%A3%A8%EB%B9%84\_\(%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D\_%EC%96%B8%EC%96%B4\)), [Tcl](https://ko.wikipedia.org/wiki/Tcl)처럼 문법에 내장되어 있는 반면 [닷넷 언어](https://ko.wikipedia.org/wiki/%EB%8B%B7%EB%84%B7\_%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC), [자바](https://ko.wikipedia.org/wiki/%EC%9E%90%EB%B0%94\_\(%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D\_%EC%96%B8%EC%96%B4\)), [파이썬](https://ko.wikipedia.org/wiki/%ED%8C%8C%EC%9D%B4%EC%8D%AC), [POSIX C](https://ko.wikipedia.org/wiki/C\_POSIX\_%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC), [C++](https://ko.wikipedia.org/wiki/C%2B%2B) ([C++11](https://ko.wikipedia.org/wiki/C%2B%2B11) 이후)에서는 [표준 라이브러리](https://ko.wikipedia.org/wiki/%ED%91%9C%EC%A4%80\_%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC)를 통해 제공한다. 그 밖의 대부분의 언어들은 별도의 라이브러리를 통해 정규 표현식을 제공한다.

정규 표현식은 [검색 엔진](https://ko.wikipedia.org/wiki/%EA%B2%80%EC%83%89\_%EC%97%94%EC%A7%84), [워드 프로세서](https://ko.wikipedia.org/wiki/%EC%9B%8C%EB%93%9C\_%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C)와 [문서 편집기](https://ko.wikipedia.org/wiki/%EB%AC%B8%EC%84%9C\_%ED%8E%B8%EC%A7%91%EA%B8%B0)의 찾아 바꾸기 대화상자, 그리고 [sed](https://ko.wikipedia.org/wiki/Sed), [AWK](https://ko.wikipedia.org/wiki/AWK)와 같은 문자 처리 유틸리티, [어휘 분석](https://ko.wikipedia.org/wiki/%EB%82%B1%EB%A7%90\_%EB%B6%84%EC%84%9D)에 사용된다.

\_\_\_위키 피디아



정규 표현식, 또는 정규식은 문자열에서 특정 문자 조합을 찾기 위한 패턴입니다. JavaScript에서는 정규 표현식도 객체로서, [`RegExp`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp)의 [`exec()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/exec)와 [`test()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/test) 메서드를 사용할 수 있습니다. [`String`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String)의 [`match()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/match), [`matchAll()` (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String/matchAll), [`replace()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/replace), [`replaceAll()` (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String/replaceAll), [`search()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/search), [`split()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/split) 메서드와도 함께 사용할 수 있습니다. 이 장에서는 JavaScript의 정규 표현식을 설명합니다.

\_\_MDN



## 정규 표현식 만들기



### 그룹과 범위 지정

|(Vertical Line) : 또는(or)

()(괄호) : 그룹

\[]\(대괄호) : 문자셋, 괄호안의 모든 문자들

\[^] (대괄호의 Carrot) : 부정문, 대괄호의 어떤 문자가 아닐때 지정

(?:) (괄호 그룹안의 물음표와 콜론) : 찾지만 기억하지 않음



### 한정자(변수의 범위를 지정, 명제와  범위)&#x20;

?(물음표) : 없거나 있거나(Zero or one)

\*(별표) : 없거나 있거나 많거나(zero or More)

\+(더하기) : 하나 또는 많이 ( one or More)

{n} (중괄호 안의 수) : n번 반복

{min, } : 최소&#x20;

{min, max} : 최소와 최대



### 경계의 유형 (Boundary-type)

\b : 단어와 단어 사이

\B : 단어의 경계가 아닌 부분

^ : 줄의 시작

$ : 줄의 끝부분



### 문자열 선택(Character classes)

\ : 특수 문자가 아닌 문자

. : 어떤 글자(줄바꿈 제외)

\d : 숫자(0123456789)

\D : 숫자가 아님

\w : word 문자

\W : word 문자가 아님

\s : space 공백

\S : space 공백 아님





* ^ : 문자열 또는 줄의 시작을 지정한다. \
  ^A 는 A로 시작하는 단어\
  ^\n 는 줄바꿈으로 시작하는 줄단위\
  ^\t 는 탭으로 시작하는 단어\
  <mark style="color:red;">\[^A] 는 Not의 의미</mark>로 A로 시작하지 않는 단어\
  ^\[^\t].\* 는 탭으로 시작하지 않는 줄을 선택
* $ : 문자열 또는 줄의 끝에서 지정한다. \
  A$ 는 A로 끝나는 줄을 선택\
  :$ 는 :로 끝나는 부분을 선택
* .(마침표) : 모든 문자 하나와 일치\
  \\. 은 점을 찾을 때 이용
* \d : 0123456789 범위의 모든 숫자를 지정한다.    \
  \[0-9] 숫자를 써서 표현 가능
* \w : 모든 글자, 숫자, 밑줄(\_)을 지정한다.\
  \[a-zA-Z] 는 모든 영문 지정\
  \[^a-zA-Z] 는 영문이 아닌 모든 글자를 지정

### 한글만 찾기

```javascript
/[ㄱ-ㅎㅏ-ㅣ가-힣]/g // 키로 찾기
/[\uAC00-\uD7A3]+\ *(?:[\uAC00-\uD7A3]| )*/g // 유니코드로 찾기
// 한글 음절의 유니코드 범위는 U+AC00에서 U+D7A3
```



### E-mail 찾기

```javascript
/[a-z0-9!#$%&'*+/=?^_`{|}~-]+(?:\.[a-z0-9!#$%&'*+/=?^_`{|}~-]+)*@(?:[a-z0-9](?:[a-z0-9-]*[a-z0-9])?\.)+[a-z0-9](?:[a-z0-9-]*[a-z0-9])?/g
```





### 1. 정규 표현식 리터럴 (연결된 패턴의 / )

```javascript
const re = /ab+c/
```

* 스크립트를 불러올 때 컴파일 됩니다.&#x20;
* 바뀔 수 없는 패턴의 경우 리터럴을 사용(성능 향상)

### 2. RegExp 객체의 생성자 호출

```javascript
const re = new RegExp('ab+c')
```

* 생성자 함수의 사용은 정규 표현식이 런타임에 컴파일 됩니다.
* 바뀔 수 있는 패턴이나 사용자 입력 등과 같은 외부에서 가져오는 패턴의 경우에 사용



## 정규 표현식 패턴

/abc/와 같은 단순 문자열 패턴으로 구성하거나, /ab+c/와 /(\d+)\\.\d\*/처럼 단순 문자열과 특수 문자의 조합으로 구성할 수 있습니다.  (\d+)에 나타난 괄호는 그룹으로 기억 장치 처럼 쓰여서 변환에 활용될 수 있습니다.



#### [단순 패턴 사용하기](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%EB%8B%A8%EC%88%9C\_%ED%8C%A8%ED%84%B4\_%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0) <a href="#_-_" id="_-_"></a>

단순 패턴은 문자열을 있는 그대로 탐색할 때 사용합니다. 예를 들어, `/abc/` 패턴은 문자열에서 정확한 순서로 `"abc"`라는 문자의 조합이 나타나는 부분과 일치합니다. 그러므로 이 패턴은 `"Hi, do you know your abc's?"`와 `"The latest airplane designs evolved from slabcraft."` 두 문자열에서 일치에 성공하고, 일치하는 부분은 `"abc"`일 것입니다. 반면 `"Grab crab"`에서는 일치하지 않는데, 이 문자열은 부분 문자열로 `"ab c"`를 포함하긴 하지만, 정확하게 `"abc"`를 포함하지는 않기 때문입니다.

#### [특수 문자 사용하기](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%ED%8A%B9%EC%88%98\_%EB%AC%B8%EC%9E%90\_%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0) <a href="#_-_" id="_-_"></a>

하나 이상의 "b"를 찾는다거나 공백 문자를 찾는 등 직접적인 일치 이상의 탐색이 필요할 땐 특수 문자를 사용합니다. 예컨대 "하나의 `"a"` 이후에 0개 이상의 `"b"`, 그 뒤의 `"c"`"와 일치해야 하면 `/ab*c/` 패턴을 사용할 수 있습니다. `"b"` 뒤의 `*`는 "이전 항목의 0번 이상 반복"을 의미합니다. 이 패턴을 문자열 `"cbbabbbbcdebc"`에 대해 사용하면, 일치하는 부분 문자열은 `"abbbbc"`일 것입니다.

아래의 문서들에선 각각의 범주에 속하는 다양한 특수 문자의 목록과 설명, 예제를 찾아볼 수 있습니다.

[어서션](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Assertions)

어서션에는 줄이나 단어의 시작과 끝을 나타내는 경계와, 일치가 가능한 방법을 나타내는 패턴(전방탐색, 후방탐색, 조건 표현식 등)이 포함됩니다.

[문자 클래스 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Character\_Classes)

글자와 숫자처럼 다른 유형의 문자를 구분합니다.

[그룹과 범위](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Groups\_and\_Backreferences)

표현 문자의 그룹과 범위를 나타냅니다.

[수량자 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Quantifiers)

일치할 문자나 표현이 반복되어야 할 횟수를 나타냅니다.

[유니코드 속성 이스케이프 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Unicode\_Property\_Escapes)

대/소문자, 수학 기호, 문장 부호처럼, 유니코드 문자 속성에 따라 문자를 구분합니다.

아래 표는 정규 표현식에서 사용하는 모든 특수문자의 목록입니다.

| 문자 / 조합                                                                                                          | 문서                                                                                                                                     |
| ---------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| `\`, `.`, `\cX`, `\d`, `\D`, `\f`, , , `\s`, `\S`, , `\v`, `\w`, `\W`, `\0`, `\xhh`, `\uhhhh`, `\uhhhhh`, `[\b]` | [문자 클래스 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Character\_Classes)                |
| `^`, `$`, `x(?=y)`, `x(?!y)`, `(?<=y)x`, `(?<!y)x`, `\b`, `\B`                                                   | [어서션](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Assertions)                                      |
| `(x)`, `(?:x)`, `(?<Name>x)`, `x\|y`, `[xyz]`, `[^xyz]`, `\`_`Number`_                                           | [그룹과 범위](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Groups\_and\_Backreferences)                  |
| `*`, `+`, `?`, `x{`_`n`_`}`, `x{`_`n`_`,}`, `x{`_`n`_`,`_`m`_`}`                                                 | [수량자 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Quantifiers)                          |
| `\p{`_`UnicodeProperty`_`}`, `\P{`_`UnicodeProperty`_`}`                                                         | [유니코드 속성 이스케이프 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Unicode\_Property\_Escapes) |

**참고:** 위 문서의 일부만 발췌해 정리해놓은, [더 큰 치트 시트도 있습니다 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Cheatsheet).



```javascript
const text = 'A quick fox';

const regexpLastWord = /\w+$/;
console.log(text.match(regexpLastWord));
// expected output: Array ["fox"]

const regexpWords = /\b\w+\b/g;
console.log(text.match(regexpWords));
// expected output: Array ["A", "quick", "fox"]

const regexpFoxQuality = /\w+(?= fox)/;
console.log(text.match(regexpFoxQuality));
// expected output: Array ["quick"]

```

#### [이스케이핑](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%EC%9D%B4%EC%8A%A4%EC%BC%80%EC%9D%B4%ED%95%91) <a href="#undefined" id="undefined"></a>

특수 문자를 있는 그대로 탐색(`"*"`을 직접 찾는 등)해야 하는 경우, 특수 문자 앞에 역슬래시(\\)를 배치해서 이스케이프 해야 합니다. 예를 들어 `"a"` 뒤의 별표(`"*"`) 뒤의 `"b"`와 일치해야 하면 `/a\*b/`를 사용하면 됩니다. 역슬래시가 `"*"`를 "이스케이프"해서, 특수 문자가 아닌 문자 리터럴로 취급합니다.

마찬가지로, 슬래시(/)와 일치해야 하는 경우에도 이스케이프를 해야 합니다. 그냥 빗금을 사용하면 패턴이 끝나버립니다. 예를 들어 문자열 "/example/"과 그 뒤 하나 이상의 알파벳을 찾으려면 `/\/example\/[a-z]/`를 사용할 수 있습니다. 각각의 슬래시 앞에 놓인 역슬래시가 슬래시를 이스케이프합니다.

리터럴 역슬래시에 일치하려면 역슬래시를 이스케이프합니다. "A:\\", "B:\\", "C:\\", ..., "Z:\\"와 일치하는 패턴은 `/[A-Z]:\\/`입니다. 앞의 역슬래시가 뒤의 역슬래시를 이스케이프해서, 결과적으로 하나의 리터럴 역슬래시와 일치하게 됩니다.

`RegExp` 생성자와 문자열 리터럴을 사용하는 경우, 역슬래시가 문자열 리터럴의 이스케이프로도 작동한다는 것을 기억해야 합니다. 그러므로 정규 표현식의 역슬래시를 나타내려면 문자열 리터럴 수준의 이스케이프도 해줘야 합니다. 즉, 앞서 살펴본 `/a\*b/` 패턴을 생성하려면 `new RegExp("a\\*b")`가 되어야 합니다.

이스케이프 되지 않은 문자열을 이미 가지고 있을 땐 [`String.replace`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/replace)를 활용해 이스케이프를 해줄 수 있습니다.

```javascript
function escapeRegExp(string) {
  return string.replace(/[.*+?^${}()|[\]\\]/g, '\\$&') // $&은 일치한 문자열 전체를 의미
}
```

Copy to Clipboard

정규 표현식 뒤의 "g"는 전체 문자열을 탐색해서 모든 일치를 반환하도록 지정하는 전역 탐색 플래그입니다. 플래그에 대해서는 아래의 [플래그를 활용한 고급 탐색](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%ED%94%8C%EB%9E%98%EA%B7%B8%EB%A5%BC\_%ED%99%9C%EC%9A%A9%ED%95%9C\_%EA%B3%A0%EA%B8%89\_%ED%83%90%EC%83%89)에서 확인할 수 있습니다.

"왜 `escapeRegExp()`가 JavaScript의 일부가 아닌가요?" 관련 제안은 있었으나 [TC39가 거부했습니다](https://github.com/benjamingr/RegExp.escape/issues/37).

#### [괄호 사용하기](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%EA%B4%84%ED%98%B8\_%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0) <a href="#_" id="_"></a>

정규 표현식의 아무 부분이나 괄호로 감싸게 되면, 그 부분과 일치하는 부분 문자열을 기억하게 됩니다. 기억한 부분 문자열은 불러와서 다시 사용할 수 있습니다. [그룹과 범위](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Groups\_and\_Backreferences#%ea%b7%b8%eb%a3%b9\_%ec%82%ac%ec%9a%a9%ed%95%98%ea%b8%b0) 문서에서 자세히 알아보세요.

### [JavaScript에서 정규 표현식 사용하기](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#javascript%EC%97%90%EC%84%9C\_%EC%A0%95%EA%B7%9C\_%ED%91%9C%ED%98%84%EC%8B%9D\_%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0) <a href="#javascript-_-_-_" id="javascript-_-_-_"></a>

정규 표현식은 [`RegExp`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp)의 메서드 [`test()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/test)와 [`exec()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/exec), [`String`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String)의 메서드 [`match()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/match), [`replace()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/replace), [`search()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/search), [`split()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/split)에서 사용할 수 있습니다.

| 메서드                                                                                                                           | 설명                                                                |
| ----------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| [`exec()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/exec)                        | 문자열에서 일치하는 부분을 탐색합니다. 일치 정보를 나타내는 배열, 또는 일치가 없는 경우 `null`을 반환합니다. |
| [`test()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/test)                        | 문자열에 일치하는 부분이 있는지 확인합니다. `true` 또는 `false`를 반환합니다.                |
| [`match()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/match)                      | 캡처 그룹을 포함해서 모든 일치를 담은 배열을 반환합니다. 일치가 없으면 `null`을 반환합니다.           |
| [`matchAll()` (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String/matchAll)     | 캡처 그룹을 포함해서 모든 일치를 담은 반복기를 반환합니다.                                 |
| [`search()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/search)                    | 문자열에서 일치하는 부분을 탐색합니다. 일치하는 부분의 인덱스, 또는 일치가 없는 경우 `-1`을 반환합니다.     |
| [`replace()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/replace)                  | 문자열에서 일치하는 부분을 탐색하고, 그 부분을 대체 문자열로 바꿉니다.                          |
| [`replaceAll()` (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String/replaceAll) | 문자열에서 일치하는 부분을 모두 탐색하고, 모두 대체 문자열로 바꿉니다.                          |
| [`split()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/split)                      | 정규 표현식 또는 문자열 리터럴을 사용해서 문자열을 부분 문자열의 배열로 나눕니다.                    |

문자열 내부에 패턴과 일치하는 부분이 존재하는지만 알아내려면 `test()`나 `search()` 메서드를 사용하세요. 더 느리더라도 일치에 관한 추가 정보가 필요하면 `exec()`과 `match()` 메서드를 사용하세요. 일치하는 부분이 존재하면, `exec()`과 `match()`는 일치에 관한 데이터를 포함한 배열을 반환하고, 일치에 사용한 정규 표현식 객체의 속성을 업데이트합니다. 일치하지 못한 경우 `null`을 반환합니다. (`null`은 조건 평가 시 `false`와 같습니다)

아래의 예제에서는, 문자열에서 일치하는 부분을 찾기 위해 `exec()` 메서드를 사용합니다.

```javascript
const myRe = /d(b+)d/g;
const myArray = myRe.exec('cdbbdbsbz');
```

Copy to Clipboard

만약 정규 표현식 객체의 속성에 접근할 필요가 없으면 아래와 같이 짧게 쓸 수도 있습니다.

```javascript
const myArray = /d(b+)d/g.exec('cdbbdbsbz');
// 'cdbbdbsbz'.match(/d(b+)d/g); 와 비슷하지만,
// 'cdbbdbsbz'.match(/d(b+)d/g)의 반환 값은 [ 'dbbd' ]인 반면
// /d(b+)d/g.exec('cdbbdbsbz')의 반환 값은 [ 'dbbd', 'bb', index: 1, input: 'cdbbdbsbz' ]
```

Copy to Clipboard

(아래의 [`exec()`과 전역 탐색 플래그 사용하기](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#exec%EA%B3%BC\_%EC%A0%84%EC%97%AD\_%ED%83%90%EC%83%89\_%ED%94%8C%EB%9E%98%EA%B7%B8\_%EC%82%AC%EC%9A%A9%ED%95%98%EA%B8%B0)에서 동작 방식의 차이에 대해 더 알아보세요)

정규 표현식을 문자열에서 만들고 싶으면 아래처럼 사용할 수도 있습니다.

```javascript
const myRe = new RegExp('d(b+)d', 'g');
const myArray = myRe.exec('cdbbdbsbz');
```

Copy to Clipboard

아래의 표는 위 스크립트에서 일치를 성공한 후, 반환하는 배열과 업데이트되는 정규 표현식 객체의 속성입니다.

<table><thead><tr><th width="125">객체</th><th width="153">속성 또는 인덱스</th><th width="316">설명</th><th>위 예제에서의 값</th></tr></thead><tbody><tr><td><code>myArray</code></td><td></td><td>일치한 문자열 및 기억한 모든 부분 문자열.</td><td><code>['dbbd', 'bb', index: 1, input: 'cdbbdbsbz']</code></td></tr><tr><td><code>index</code></td><td>일치한 부분이 주어진 문자열에서 위치한 인덱스. (0부터 시작)</td><td><code>1</code></td><td></td></tr><tr><td><code>input</code></td><td>주어진 원본 문자열.</td><td><code>'cdbbdbsbz'</code></td><td></td></tr><tr><td><code>[0]</code></td><td>마지막으로 일치한 부분 문자열.</td><td><code>'dbbd'</code></td><td></td></tr><tr><td><code>myRe</code></td><td><code>lastIndex</code></td><td>다음 일치를 시작할 인덱스. (g 옵션을 지정한 정규 표현식의 경우에만 설정됩니다. <a href="https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular_Expressions#%ED%94%8C%EB%9E%98%EA%B7%B8%EB%A5%BC_%ED%99%9C%EC%9A%A9%ED%95%9C_%EA%B3%A0%EA%B8%89_%ED%83%90%EC%83%89">플래그를 활용한 고급 탐색</a>을 참고하세요)</td><td><code>5</code></td></tr><tr><td><code>source</code></td><td>패턴의 텍스트. 정규 표현식이 생성될 때 갱신됩니다. 실행 시점에는 갱신되지 않습니다.</td><td><code>'d(b+)d'</code></td><td></td></tr></tbody></table>

위 예제의 두 번째 형태처럼, 정규 표현식 객체를 변수에 대입하지 않고도 사용할 수 있습니다. 하지만, 이러면 매 사용마다 정규 표현식 객체가 새로 생성되며, 업데이트되는 속성에 접근할 수 없습니다. 다음과 같은 코드를 생각해보겠습니다.

```javascript
const myRe = /d(b+)d/g;
const myArray = myRe.exec('cdbbdbsbz');
console.log(`lastIndex의 값은 ${myRe.lastIndex}`);

// "lastIndex의 값은 5"
```

Copy to Clipboard

그러나 위의 코드 대신 아래 코드를 사용하게 되면...

```javascript
const myArray = /d(b+)d/g.exec('cdbbdbsbz');
console.log(`lastIndex의 값은 ${/d(b+)d/g.lastIndex}`);

// "lastIndex의 값은 0"
```

Copy to Clipboard

두 개의 `/d(b+)d/g` 는 서로 다른 정규 표현식 객체이므로 별개의 `lastIndex` 속성을 갖습니다. 정규 표현식 객체의 속성에 접근해야 하면, 우선 변수에 할당하세요.

#### [플래그를 활용한 고급 탐색](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%ED%94%8C%EB%9E%98%EA%B7%B8%EB%A5%BC\_%ED%99%9C%EC%9A%A9%ED%95%9C\_%EA%B3%A0%EA%B8%89\_%ED%83%90%EC%83%89) <a href="#_-_-_" id="_-_-_"></a>

정규 표현식은 전역 탐색이나 대소문자 무시와 같은 특성을 지정하는 플래그를 가질 수 있습니다. 플래그는 단독으로 사용할 수도 있고, 순서에 상관 없이 한꺼번에 여럿을 지정할 수도 있습니다.

<table><thead><tr><th width="112.33333333333331">플래그</th><th width="334">설명</th><th>대응하는 속성</th></tr></thead><tbody><tr><td><code>d</code></td><td>부분 문자열 일치에 대해 인덱스 생성.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/hasIndices"><code>RegExp.prototype.hasIndices</code> (en-US)</a></td></tr><tr><td><code>g</code></td><td>전역 탐색.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/global"><code>RegExp.prototype.global</code> (en-US)</a></td></tr><tr><td><code>i</code></td><td>대소문자를 구분하지 않음.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/ignoreCase"><code>RegExp.prototype.ignoreCase</code> (en-US)</a></td></tr><tr><td><code>m</code></td><td>여러 줄에 걸쳐 탐색.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/multiline"><code>RegExp.prototype.multiline</code> (en-US)</a></td></tr><tr><td><code>s</code></td><td>개행 문자가 <code>.</code>과 일치함.</td><td><a href="https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global_Objects/RegExp/dotAll"><code>RegExp.prototype.dotAll</code></a></td></tr><tr><td><code>u</code></td><td>"unicode", 패턴을 유니코드 코드 포인트의 시퀀스로 간주함.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/unicode"><code>RegExp.prototype.unicode</code> (en-US)</a></td></tr><tr><td><code>y</code></td><td>"접착" 탐색, 대상 문자열의 현재 위치에서 탐색을 시작함. <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/sticky"><code>sticky</code> (en-US)</a>를 참고하세요.</td><td><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp/sticky"><code>RegExp.prototype.sticky</code> (en-US)</a></td></tr></tbody></table>

플래그는 다음과 같은 구문으로 정규 표현식에 지정할 수 있습니다.

```javascript
const re = /pattern/flags;
```

Copy to Clipboard

생성자를 사용할 경우 이렇게 지정합니다.

```javascript
const re = new RegExp('pattern', 'flags');
```

Copy to Clipboard

플래그는 정규식과 완전히 합쳐지므로 나중에 추가하거나 제거할 수 없습니다.

예를 들어, `re = /\w+\s/g`는 한 개 이상의 글자와 그 뒤의 공백 하나를, 문자열 전체에 대해 탐색합니다.

```javascript
const re = /\w+\s/g;
const str = 'fee fi fo fum';
const myArray = str.match(re);
console.log(myArray);

// ["fee ", "fi ", "fo "]
```

Copy to Clipboard

아래 코드는...

```javascript
const re = /\w+\s/g;
```

Copy to Clipboard

이렇게 생성자를 사용하도록 바꿀 수도 있습니다.

```javascript
const re = new RegExp('\\w+\\s', 'g');
```

Copy to Clipboard

두 구문 모두 동일한 결과를 낳습니다.

`m` 플래그는 여러 줄에 걸친 입력 문자열을 여러 줄로 취급하게 합니다. 달리 말해, `m` 플래그를 지정할 경우, `^`와 `$`는 각각 전체 입력 문자열의 시작과 끝이 아니라, 각 줄의 시작과 끝에 대응하게 됩니다.

**exec()과 전역 탐색 플래그 사용하기**

[`RegExp.prototype.exec()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/exec) 메서드와 `g` 플래그를 사용하면, 일치한 부분 문자열들과 각각의 인덱스를 하나씩 순차적으로 반환합니다.

```javascript
const str = 'fee fi fo fum'
const re = /\w+\s/g

console.log(re.exec(str)) // ["fee ", index: 0, input: "fee fi fo fum"]
console.log(re.exec(str)) // ["fi ", index: 4, input: "fee fi fo fum"]
console.log(re.exec(str)) // ["fo ", index: 7, input: "fee fi fo fum"]
console.log(re.exec(str)) // null
```

Copy to Clipboard

반면, [`String.prototype.match()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/match) 메서드는 모든 일치를 한 번에 반환하지만, 각각의 인덱스는 포함하지 않습니다.

```
console.log(str.match(re)) // ["fee ", "fi ", "fo "]
```

Copy to Clipboard

### [예제](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%EC%98%88%EC%A0%9C) <a href="#undefined" id="undefined"></a>

**참고:** 다음 문서에서도 정규 표현식의 사용 예제를 볼 수 있습니다.

* [`exec()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/exec), [`test()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/RegExp/test), [`match()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/match), [`matchAll()` (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global\_Objects/String/matchAll), [`search()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/search), [`replace()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/replace), [`split()`](https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/String/split) 메서드 참조
* 이 안내서의 하위 문서: [문자 클래스 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Character\_Classes), [어서션](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Assertions), [그룹과 범위](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions/Groups\_and\_Backreferences), [수량자 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Quantifiers), [유니코드 속성 이스케이프 (en-US)](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Regular\_Expressions/Unicode\_Property\_Escapes)

#### [정규 표현식 특수 문자를 사용한 입력 값 검증](https://developer.mozilla.org/ko/docs/Web/JavaScript/Guide/Regular\_Expressions#%EC%A0%95%EA%B7%9C\_%ED%91%9C%ED%98%84%EC%8B%9D\_%ED%8A%B9%EC%88%98\_%EB%AC%B8%EC%9E%90%EB%A5%BC\_%EC%82%AC%EC%9A%A9%ED%95%9C\_%EC%9E%85%EB%A0%A5\_%EA%B0%92\_%EA%B2%80%EC%A6%9D) <a href="#_-_-_-_-_-_-_" id="_-_-_-_-_-_-_"></a>

아래 예제에서는 사용자가 전화번호를 입력해야 합니다. 사용자가 "확인" 버튼을 누르면 입력한 값을 스크립트로 검증합니다. 값이 유효하면, 즉 정규 표현식과 일치하는 문자의 시퀀스를 받았으면, 스크립트는 감사 메시지를 출력합니다. 값이 유효하지 않으면, 사용자에게 올바르지 않은 값임을 알려줍니다.

정규 표현식의 구조는 다음과 같습니다.

1. 데이터의 시작점(`^`)
2. 비캡처 그룹(`(?:)`)으로, 1의 뒤를 잇는 세 개의 숫자(`\d{3}`), 또는(`|`), 여는 괄호(`\(`)의 뒤를 잇는 세 개의 숫자(`\d{3}`)의 뒤를 잇는 닫는 괄호(`\)`)
3. 캡처 그룹(`()`)으로, 2의 뒤를 잇는 하나의 대시, 슬래시, 또는 마침표
4. 3의 뒤를 잇는 네 개의 숫자(`\d{4}`)
5. 4의 뒤를 잇는, 첫 번째 캡처 그룹에서 기억한 부분 문자열(`\1`)
6. 5의 뒤를 잇는 네 개의 숫자(`\d{4}`)
7. 데이터의 끝점(`$`)

**HTML**

```html
<p>
  전화번호를 입력 후 "확인" 버튼을 누르세요.
  <br />
  ###-####-####의 형식으로 입력하세요.
</p>
<form id="form">
  <input id="phone" />
  <button type="submit">확인</button>
</form>
<p id="output"></p>
```

Copy to Clipboard

**JavaScript**

```javascript
const form = document.querySelector('#form')
const input = document.querySelector('#phone')
const output = document.querySelector('#output')

const re = /^(?:\d{3}|\(\d{3}\))([-\/\.])\d{4}\1\d{4}$/

function testInfo(phoneInput) {
  const ok = re.exec(phoneInput.value)

  if (!ok) {
    output.textContent = `형식에 맞지 않는 전화번호입니다. (${phoneInput.value})`
  } else {
    output.textContent = `감사합니다. 전화번호는 ${ok[0]} 입니다.`
  }
}

form.addEventListener('submit', (event) => {
  event.preventDefault()
  testInfo(input)
})
```





## URL Hash link

```
/(#[A-Za-z0-9-._~:/?#[\]@!$&'()*+,;=%]*)?/

#newsletter
https://some.url.com#ccccd
https://some.url.com?thing=blah&thong=%25#newsletter
https://some.url.com
https://some.url.com?thing=blah&thong=%25
https://some.url.com?thing=blah&thong=%25/
https://some.url.com/
https://some.url.com/#newsletter
https://some.url.com/#newsletter?thing=blah&thong=%25
https://some.url.com/#newsletter?thing=blah&thong=%25/

http://some.url.com
http://some.url.com?thing=blah&thong=%25
http://some.url.com?thing=blah&thong=%25/
http://some.url.com/
http://some.url.com/#newsletter
http://some.url.com/#newsletter?thing=blah&thong=%25
http://some.url.com/#newsletter?thing=blah&thong=%25/


```



## URL 올바른 값만 체크

```
/^(http:\/\/www\.|https:\/\/www\.|http:\/\/|https:\/\/)?[a-z0-9]+([\-\.]{1}[a-z0-9]+)*\.[a-z]{2,5}(:[0-9]{1,5})?(\/.*)?$/

https://www.google.com
http://www.google.com
www.google.com
htt://www.google.com
://www.google.com
```

