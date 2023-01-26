# CSS(Cascading Style Sheets)

### What is CSS?
CSS는 HTML 문서를 시각적으로 표현하고 나타내기 위해서 사용하는 스타일 시트 언어이다. HTML만으로 웹 페이지를 제작할 경우 HTML 요소의 세부 스타일을 일일이 따로 지정해 주어야 한다. 이 작업은 매우 많은 시간이 걸리며, 완성한 후에도 스타일의 변경 및 유지 보수가 매우 힘들다. 이러한 문제점을 해소하기 위한 스타일 시트 언어가 바로 CSS이다.<br><br>
CSS를 입력하기 위한 규칙은 아래와 같다.
<pre>
<h2><b>CSS RULES</b></h2>
      selector {
          property: value;
      }
      
</pre>
<br><br>

### CSS Reference
: https://developer.mozilla.org/ko/docs/Web/CSS
<br><br>

### 스타일을 올바르게 담기
<ol>
    <li>인라인 스타일(Inline style)</li>
    <p>
      <pre><h2>Example</h2>
      &lt;h1 style="color: purple"&gt;Hello World&lt;/h1&gt;<br>
      &lt;button style="background-color: palegreen"&gt;I AM BUTTON&lt;/button&gt;
      </pre>
    html요소에 직접 스타일을 작성 → 비추천하는 방법.<br>
    해당 요소에만 스타일을 적용할 수 있어 여러 요소에 동일한 스타일을 지정하는 경우 각각 스타일을 지정해야 하는 불편함이 있다. 또한 문서간에 스타일을 공유할 수 없다.
    </p><br>
    <li>내부 스타일 시트(Internal style sheet)</li>
    <p>
    앞선 방식의 개선된 방법으로 &lt;head&gt; 안에 &lt;style&gt; 요소를 사용하여 css를 작성한다. 해당 HTML 문서에만 스타일을 적용할 수 있어 여러 문서에 동일한 스타일을 적용하려는 경우 여전히 문제가 있다.
    </p><br>
    <li>외부 스타일 시트(External style sheet)⭐</li>
    <p>
    가장 좋은 방법!<br>
    html과 완전히 별개인 css 파일을 만든다.(파일 확장자는 .css)<br>
    style 요소를 작성할 때와 같은 방법으로 css를 작성하고 저장 → HTML 파일에 &lt;link&gt; 요소를 사용하여 css 파일의 경로 정보를 넣어줘야 한다. link 요소는 &lt;head&gt;에 들어간다.
    <pre><h2>Example</h2> 
    &lt;link rel="stylesheet" href="css파일경로"&gt;<br>
    rel: 딱히 신경쓸 필요 없음
    </pre>
    </p>
</ol>
