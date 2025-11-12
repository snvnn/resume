### 1. 일목요연하게 테이블을 작성할 때 사용한 도구
> https://www.tablesgenerator.com/html_tables#

원하는 형식의 테이블을 제작한 다음, 생성된 HTML을 .md 파일에 붙여넣기 하면 쉽게 적용할 수 있다.

``` HTML

<table class="tg"><thead>
  <tr>
    <td class="tg-0pky" rowspan="3"></td>
    <td class="tg-0lax">이름</td>
    <td class="tg-0lax">윤현<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">생년월일</td>
    <td class="tg-0lax">2001. 12. 05.</td>
  </tr>
  <tr>
    <td class="tg-0lax">연락처</td>
    <td class="tg-0lax">32203004@dankook.ac.kr</td>
  </tr></thead>
</table>
```

이렇게 생성된 HTML 문서를 마크다운 문서에 옮기면 간편하게 테이블 추가가 가능하다.

<table class="tg"><thead>
  <tr>
    <td class="tg-0pky" rowspan="3"><img src= "media/profile.jpg" width = "120"></td>
    <td class="tg-0lax">이름</td>
    <td class="tg-0lax">윤현<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">생년월일</td>
    <td class="tg-0lax">2001. 12. 05.</td>
  </tr>
  <tr>
    <td class="tg-0lax">연락처</td>
    <td class="tg-0lax">32203004@dankook.ac.kr</td>
  </tr></thead>
</table>




**HTML을 이용해 테이블을 작성하는 이유**: 마크다운이 지원하는 테이블 기능은 셀 병합 등의 기능이 매우 제한적이기 때문에, 원하는 형태의 테이블을 작성하기 위해서는 HTML을 사용하는 편이 낫다.

추가로, 이렇게 생성된 테이블은 디자인이 깔끔한 편은 아니니 HTML 코드의 수정이 일부 필요할 수 있다.

### 2. 참고한 이력서 양식 및 내용
 > https://help.miricanvas.com/hc/ko/articles/900003333746-%EB%AC%B4%EB%A3%8C-%EC%9D%B4%EB%A0%A5%EC%84%9C-%EC%96%91%EC%8B%9D-%EB%8B%A4%EC%9A%B4%EB%A1%9C%EB%93%9C-10%EC%A2%85-%EC%84%B8%ED%8A%B8
 > https://romanc3.tistory.com/84




### 3. 편집 환경
**Visual Studio Code**와 **Markdown Preview Enhanced** 익스텐션으로 수정 즉시 렌더링되는 마크다운 파일의 모습을 확인할 수 있다.

> https://marketplace.visualstudio.com/items?itemName=shd101wyy.markdown-preview-enhanced


#### 3.1 참고) 마크다운 언어를 사용할 때 주의점
Visual Studio Code의 Markdown Preview Enhanced 익스텐션을 이용해 문서 편집을 할 때, 미려하게 작성되는 마크다운 문서만을 보고 ```git push```를 감행하다 보면 깃허브에서는 다른 모습으로 적용된 모습을 확인할 수 있었다.
그 원인으로 지목되는 것은 GitHub에서 ```<style>``` 태그 블록은 HTML 문서가 아닌 텍스트로 인식을 하게 되어 스타일 지정이 되지 않는다는 것이다.
