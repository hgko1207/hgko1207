<!-- Header: Typing SVG -->
<div align="center">
  <a href="https://hgko-dev.tistory.com/">
    <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=32&duration=3200&pause=800&color=7AA2F7&center=true&vCenter=true&width=720&lines=Hi%2C+I'm+Ko+Coding+%F0%9F%91%8B;15%2B+yrs+Full-Stack+Engineer;Web+%26+Windows+App+Developer;Writing+at+hgko-dev.tistory.com" alt="typing header" />
  </a>
</div>

<p align="center">
  <a href="https://hgko-dev.tistory.com/"><img src="https://img.shields.io/badge/Blog-규니의_개발_블로그-FF5A5F?style=for-the-badge&logo=tistory&logoColor=white" /></a>
  <a href="https://hgko1207.github.io/"><img src="https://img.shields.io/badge/GitHub_Pages-hgko1207.github.io-222?style=for-the-badge&logo=github" /></a>
  <a href="mailto:hgko1207@gmail.com"><img src="https://img.shields.io/badge/Email-hgko1207@gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" /></a>
</p>

---

### About

```yaml
name:     "Ko Coding (고현규)"
role:     "Full-Stack Engineer, 15+ years"
focus:    ["Web Apps", "Windows Desktop Apps", "AI-assisted dev workflow"]
tools:    ["Claude Max", "Gemini Pro", "Claude Code"]
writing:  "hgko-dev.tistory.com — 4년째 기술 블로그 운영 중"
motto:    "맡은 일에 책임감을, 새 기술엔 거부감 없이."
```

---

### 🛠 Currently Building

- **[claude-code-blog-builder](https://github.com/hgko1207/claude-code-blog-builder)** — Claude Code 기반 블로그 자동화 (키워드 → 리서치 → 초안 → 이미지 → 검증)
- AI 페어 프로그래밍 워크플로우 실험 (Claude + Gemini 병행 운용)
- 블로그 운영 4년차, AI 개발 도구 실전 사용기 시리즈 연재 중

---

### 📝 Latest Blog Posts
<!-- BLOG-POST-LIST:START -->- [Claude Opus 4.7 업그레이드 완전 정리 &amp;mdash; 4.6에서 바뀐 점과 업그레이드 판단 기준](https://hgko-dev.tistory.com/559) <sub>— 
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;span style=&quot;letter-spacing: 0px;&quot;&gt;Claude Opus 4.7이 출시됐는데 4.6에서 갈아탈 만한 가치가 있는지 궁금할 겁니다.&lt;/span&gt;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;벤치마크 숫자만 보고 결정하면 실사용 환경에서 새 토크나이저 때문에 비용이 오히려 오를 수도 있습니다.&lt;br /&gt;15년차 개발자로서 Claude Max와 Gemini Pro를 병행 운용하는 관점에서 공식 릴리즈 노트를 정리했습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;이 글을 끝까지 읽으면 4.6 대비 개선된 포인트 7가지, 비용 함정, 업그레이드 판단 기준 3가지를 가져갑니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/bP4X2i/dJMcaipxEbn/bbmdD9HHjakLnIoUmKSpy0/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/bP4X2i/dJMcaipxEbn/bbmdD9HHjakLnIoUmKSpy0/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/bP4X2i/dJMcaipxEbn/bbmdD9HHjakLnIoUmKSpy0/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbP4X2i%2FdJMcaipxEbn%2FbbmdD9HHjakLnIoUmKSpy0%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;1. 먼저 숫자로 요약 &amp;mdash; 4.6과 4.7 스펙 비교&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;2026년 4월 16일 Anthropic이 Claude Opus 4.7을 정식 출시했습니다. 공식 발표 기준 핵심만 먼저 뽑았습니다.&lt;/p&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;항목&lt;/th&gt;
&lt;th&gt;Opus 4.6&lt;/th&gt;
&lt;th&gt;Opus 4.7&lt;/th&gt;
&lt;th&gt;변화&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;SWE-bench Verified&lt;/td&gt;
&lt;td&gt;80.8%&lt;/td&gt;
&lt;td&gt;87.6%&lt;/td&gt;
&lt;td&gt;+6.8pp&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;SWE-bench Pro&lt;/td&gt;
&lt;td&gt;53.4%&lt;/td&gt;
&lt;td&gt;64.3%&lt;/td&gt;
&lt;td&gt;+10.9pp&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;이미지 해상도 &lpar;최대&rpar;&lt;/td&gt;
&lt;td&gt;1568px / 1.15MP&lt;/td&gt;
&lt;td&gt;2576px / 3.75MP&lt;/td&gt;
&lt;td&gt;3.25배&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;컨텍스트 윈도우&lt;/td&gt;
&lt;td&gt;1M 토큰&lt;/td&gt;
&lt;td&gt;1M 토큰&lt;/td&gt;
&lt;td&gt;동일&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;최대 출력 토큰&lt;/td&gt;
&lt;td&gt;128k&lt;/td&gt;
&lt;td&gt;128k&lt;/td&gt;
&lt;td&gt;동일&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;API 입력 단가&lt;/td&gt;
&lt;td&gt;$5 / 1M&lt;/td&gt;
&lt;td&gt;$5 / 1M&lt;/td&gt;
&lt;td&gt;동일&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;API 출력 단가&lt;/td&gt;
&lt;td&gt;$25 / 1M&lt;/td&gt;
&lt;td&gt;$25 / 1M&lt;/td&gt;
&lt;td&gt;동일&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;effort 레벨&lt;/td&gt;
&lt;td&gt;low / medium / high / max&lt;/td&gt;
&lt;td&gt;low / medium / high / &lt;b&gt;xhigh&lt;/b&gt; / max&lt;/td&gt;
&lt;td&gt;xhigh 추가&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;토크나이저&lt;/td&gt;
&lt;td&gt;기존&lt;/td&gt;
&lt;td&gt;신규 &lpar;토큰 1.0~1.35배 증가&rpar;&lt;/td&gt;
&lt;td&gt;변경&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;단가는 그대로지만 &lt;b&gt;토크나이저 변경으로 같은 프롬프트라도 토큰 수가 최대 1.35배까지 늘어나는&lt;/b&gt; 게 체감 비용의 함정입니다. 이 부분은 뒤에서 따로 다룹니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/kVC1x/dJMcag6khbb/oGJqkk4kQeJb7ikej8bgz0/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/kVC1x/dJMcag6khbb/oGJqkk4kQeJb7ikej8bgz0/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/kVC1x/dJMcag6khbb/oGJqkk4kQeJb7ikej8bgz0/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FkVC1x%2FdJMcag6khbb%2FoGJqkk4kQeJb7ikej8bgz0%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;2. 가장 크게 오른 영역 &amp;mdash; 어려운 코딩 문제&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;벤치마크를 보면 개선폭이 &lt;b&gt;쉬운 문제보다 어려운 문제에서 더 크게&lt;/b&gt; 벌어졌습니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;SWE-bench Verified&lt;/b&gt; &lpar;비교적 평이한 수준&rpar;: 80.8% &amp;rarr; 87.6%, +6.8pp&lt;/li&gt;
&lt;li&gt;&lt;b&gt;SWE-bench Pro&lt;/b&gt; &lpar;난도 높은 실전 과제&rpar;: 53.4% &amp;rarr; 64.3%, +10.9pp&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;짧은 함수 생성은 어떤 모델이든 얼추 됩니다. 실무에서 차이가 벌어지는 구간은 &quot;여러 파일에 걸친 리팩토링&quot;, &quot;원인이 애매한 버그 추적&quot;, &quot;레거시 코드에 신규 피처 붙이기&quot; 같은 시나리오입니다. Claude Opus 4.7의 개선은 이 구간을 정확히 겨냥한 결과입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;3. 고해상도 이미지 지원 &amp;mdash; 스크린샷 디버깅 정밀도 향상&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Opus 4.7은 Anthropic 첫 고해상도 이미지 지원 모델입니다. 최대 해상도가 &lt;b&gt;1568px &amp;middot; 1.15MP에서 2576px &amp;middot; 3.75MP로 3배 이상&lt;/b&gt; 커졌습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;이전에는 Figma&amp;middot;디자인 파일을 한 번 리사이즈해서 붙여야 했는데, 4.7은 원본 그대로 받아들입니다. Anthropic이 공식 릴리즈 노트에서 포인팅&amp;middot;카운팅&amp;middot;바운딩 박스 감지 정밀도도 개선됐다고 명시했습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;4. task budgets &amp;mdash; 에이전트 토큰 예산 관리&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Opus 4.7에 새로 들어간 개념입니다. 에이전트 전체 루프&lpar;사고&amp;middot;도구 호출&amp;middot;결과&amp;middot;최종 출력&rpar; 동안 쓸 &lt;b&gt;토큰 예산을 미리 알려주면&lt;/b&gt;, 모델이 카운트다운을 보면서 작업 우선순위를 조절합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;효과가 두드러지는 상황은 긴 리팩토링 작업입니다. 예전에는 중간에 토큰이 바닥나 출력이 잘려나가는 일이 종종 있었는데, 4.7에서는 예산을 인지해서 &quot;남은 토큰으로 커밋 메시지까지 마무리할지, 아니면 핵심 변경만 완료할지&quot; 결정합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;5. 새 xhigh effort 레벨 &amp;mdash; 비용과 지능의 중간 옵션&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;기존 effort 옵션은 low / medium / high / max 4단계였고, 이번에 high와 max 사이에 &lt;b&gt;xhigh&lt;/b&gt;가 추가됐습니다. &lt;code&gt;/effort&lt;/code&gt;, &lt;code&gt;--effort&lt;/code&gt;, 모델 피커로 지정할 수 있습니다.&lt;/p&gt;
&lt;blockquote data-ke-style=&quot;style3&quot;&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;증상:&lt;/b&gt; high로는 품질이 약간 아쉽고, max로 올리면 비용이 2~3배 튐.&lt;br /&gt;&lt;b&gt;원인:&lt;/b&gt; high와 max 사이 간격이 너무 커서 &quot;중간 정도만 써도 될 일&quot;에 max를 쓰게 됨.&lt;br /&gt;&lt;b&gt;해결:&lt;/b&gt; xhigh로 떨어뜨리면 품질은 max의 80~90% 수준에 비용은 훨씬 적게 듭니다. 긴 에이전트 루프에 특히 유용합니다.&lt;/p&gt;
&lt;/blockquote&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;6. 파일 시스템 기반 메모리 개선&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Opus 4.7은 파일 기반 메모리를 &lt;b&gt;쓰고 읽는 능력이 개선&lt;/b&gt;됐습니다. 에이전트가 중간 결과를 노트로 파일에 적고, 다음 작업에서 그 파일을 참고하는 패턴이 더 안정적으로 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Code에서 &lt;code&gt;/memory&lt;/code&gt;나 CLAUDE.md 기반으로 맥락을 유지할 때 특히 차이가 납니다. 긴 리팩토링 작업을 여러 세션에 나눠서 돌려도 앞 세션의 결정이 덜 휘발됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;7. /ultrareview &amp;mdash; 무거운 코드 리뷰 세션&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Code에 새로 들어간 툴입니다. 별도 세션을 Anthropic 클라우드에 띄워서 변경사항을 정독하고 버그&amp;middot;설계 이슈를 잡아냅니다. 단, &lt;b&gt;1회 실행에 $10~20 비용&lt;/b&gt;이 드는 유료 기능입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;일반 코드 리뷰용으로는 과합니다. 머지 직전 큰 PR 한 번 돌리거나, 보안 감사&amp;middot;릴리즈 전 검증 같은 &lt;b&gt;배치성 작업&lt;/b&gt;이 적합한 용도입니다. 평소 개발에는 일반 Claude Code 세션으로 충분합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;8. 주의할 점 &amp;mdash; 새 토크나이저의 비용 함정&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;4.7의 단가는 4.6과 동일합니다. 입력 $5 / 1M, 출력 $25 / 1M. 여기까지는 숫자가 같아 보입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;문제는 &lt;b&gt;토크나이저가 바뀌면서 같은 한국어 텍스트를 넣어도 토큰 수가 1.0~1.35배 늘어난다는 점&lt;/b&gt;입니다. 최악의 경우 실질 비용이 35% 오를 수 있습니다.&lt;/p&gt;
&lt;blockquote data-ke-style=&quot;style3&quot;&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;증상:&lt;/b&gt; 동일한 작업을 4.7로 돌렸는데 Anthropic 콘솔의 월 청구 금액이 기존보다 20~30% 올라 있음.&lt;br /&gt;&lt;b&gt;원인:&lt;/b&gt; 토크나이저 변경으로 입력&amp;middot;출력 토큰 카운트가 증가.&lt;br /&gt;&lt;b&gt;해결:&lt;/b&gt; 체감 품질 차이가 크지 않은 루틴 작업은 Sonnet 4.6이나 Haiku 4.5로 내리고, 꼭 필요한 어려운 작업만 Opus 4.7로 올리는 모델 믹스 전략이 맞습니다.&lt;/p&gt;
&lt;/blockquote&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;9. 업그레이드 판단 기준 &amp;mdash; 상황에 따라 다르다&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;정답은 없습니다. 업무 유형을 먼저 보면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;4.7로 바로 올리는 게 나은 경우&lt;/b&gt;&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;복잡한 리팩토링&amp;middot;레거시 코드 추적 업무가 많다&lt;/li&gt;
&lt;li&gt;스크린샷&amp;middot;Figma 기반 프런트엔드 작업이 잦다&lt;/li&gt;
&lt;li&gt;긴 에이전트 루프&lpar;멀티 스텝 자동화&rpar;를 돌린다&lt;/li&gt;
&lt;li&gt;Claude Code로 큰 PR을 생성하고 머지 전 검증이 필요하다&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;4.6에 그대로 남는 게 나은 경우&lt;/b&gt;&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;주로 짧은 코드 조각 생성&amp;middot;Q&amp;amp;A 용도로 쓴다&lt;/li&gt;
&lt;li&gt;한국어 자연어 출력 품질이 중요하다 &lpar;4.6이 더 자연스럽다는 평이 국내 커뮤니티에 있음&rpar;&lt;/li&gt;
&lt;li&gt;월 사용량이 많아 토큰 증가분이 예산에 직격한다&lt;/li&gt;
&lt;li&gt;아직 4.7 regression 리포트&lpar;특정 작업에서 품질 저하&rpar;가 걱정된다&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;타협안&lt;/b&gt;: 업무를 두 종류로 나눠 &lt;b&gt;모델 믹스&lt;/b&gt;를 운용하는 방법. 어려운 디버깅&amp;middot;리팩토링만 Opus 4.7, 나머지는 Sonnet 4.6이나 Haiku 4.5로 분배합니다. 비용과 품질 사이 균형점을 찾기에 가장 합리적입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/KSSd9/dJMcaf0Cubc/fapoEWeZ1vv2SQFmUmxMkK/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/KSSd9/dJMcaf0Cubc/fapoEWeZ1vv2SQFmUmxMkK/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/KSSd9/dJMcaf0Cubc/fapoEWeZ1vv2SQFmUmxMkK/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FKSSd9%2FdJMcaf0Cubc%2FfapoEWeZ1vv2SQFmUmxMkK%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;10. 어디서 쓸 수 있나&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;출시와 함께 주요 플랫폼에 전부 배포됐습니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;claude.ai&lt;/b&gt; &amp;mdash; 웹&amp;middot;데스크톱 앱 기본 모델로 선택 가능&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Anthropic API&lt;/b&gt; &amp;mdash; 모델 ID &lt;code&gt;claude-opus-4-7&lt;/code&gt;&lt;/li&gt;
&lt;li&gt;&lt;b&gt;AWS Bedrock&lt;/b&gt; &amp;mdash; 같은 날 출시&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Google Cloud Vertex AI&lt;/b&gt;&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Microsoft Foundry&lt;/b&gt;&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Claude Code&lt;/b&gt; &amp;mdash; &lt;code&gt;claude&lt;/code&gt; 실행 시 기본값 또는 &lt;code&gt;/model&lt;/code&gt;로 전환&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;GitHub Copilot Enterprise에서도 &lt;code&gt;Claude Opus 4.7 is generally available&lt;/code&gt; 공지가 나갔습니다. 본인이 쓰는 환경에 이미 들어와 있을 가능성이 높습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;자주 묻는 질문&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Opus 4.7로 올리면 한국어 품질이 떨어진다는 얘기가 있던데 사실인가요?&lt;/b&gt;&lt;br /&gt;A. 국내 일부 사용자 리뷰에 &quot;4.6이 한국어 문장이 더 자연스럽다&quot;는 평이 있는 건 사실입니다. 다만 이건 주관적 체감이라 본인 사용 패턴에서 비교해보는 게 맞습니다. 코딩&amp;middot;기술 문서 용도는 큰 차이가 없지만 블로그 톤의 긴 한국어 생성 용도면 4.6도 여전히 경쟁력 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 가격이 같다고 하는데 실제 비용도 같나요?&lt;/b&gt;&lt;br /&gt;A. 단가&lpar;$5/$25 per 1M&rpar;는 동일하지만 &lt;b&gt;새 토크나이저가 토큰을 1.0~1.35배 더 쓰기 때문에 실비용은 최대 35%까지 오를 수 있습니다.&lt;/b&gt; 평균적으로 10~20% 증가를 예상하면 됩니다. 예산 관리가 중요하면 모델 믹스 전략 권장.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Claude Code에서 4.7로 바꾸는 법은요?&lt;/b&gt;&lt;br /&gt;A. &lt;code&gt;claude&lt;/code&gt; 실행 후 &lt;code&gt;/model&lt;/code&gt; 입력 &amp;rarr; 목록에서 &lt;code&gt;claude-opus-4-7&lt;/code&gt; 선택하거나, 터미널에서 &lt;code&gt;claude --model claude-opus-4-7&lt;/code&gt;로 실행하면 됩니다. Max 플랜 구독자는 별도 결제 없이 포함됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 1M 컨텍스트 모드는 4.7에서도 유지되나요?&lt;/b&gt;&lt;br /&gt;A. 네, Opus 4.6부터 제공된 1M 토큰 컨텍스트 윈도우가 4.7에서도 그대로 유지됩니다. 긴 레포 전체를 올려 분석하는 용도라면 4.7의 어려운 코드 이해력 개선과 맞물려 체감이 큽니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. /ultrareview는 꼭 써야 하나요?&lt;/b&gt;&lt;br /&gt;A. 일반 코드 리뷰에는 과한 도구예요. 1회 $10~20이라 소규모 패치에는 낭비고, 큰 PR&amp;middot;릴리즈 직전 검증&amp;middot;보안 감사 같은 &lt;b&gt;배치성 작업&lt;/b&gt;에 적합합니다. 평소 개발에는 일반 Claude Code 세션으로 충분합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;마무리&lt;/h2&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;개선 영역&lt;/th&gt;
&lt;th&gt;핵심 내용&lt;/th&gt;
&lt;th&gt;체감 효과&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;코딩 성능&lt;/td&gt;
&lt;td&gt;SWE-bench Pro +10.9pp&lt;/td&gt;
&lt;td&gt;어려운 문제일수록 개선 큼&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;비전&lt;/td&gt;
&lt;td&gt;2576px 고해상도 지원&lt;/td&gt;
&lt;td&gt;Figma&amp;middot;스크린샷 작업 정밀도 상승&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;에이전트&lt;/td&gt;
&lt;td&gt;task budgets + xhigh effort&lt;/td&gt;
&lt;td&gt;긴 루프 토큰 관리 수월&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;메모리&lt;/td&gt;
&lt;td&gt;파일 기반 메모리 개선&lt;/td&gt;
&lt;td&gt;세션 간 맥락 유지&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;신규 툴&lt;/td&gt;
&lt;td&gt;/ultrareview&lt;/td&gt;
&lt;td&gt;배치성 정밀 리뷰&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;비용 주의&lt;/td&gt;
&lt;td&gt;새 토크나이저&lt;/td&gt;
&lt;td&gt;실비용 최대 +35%&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/Et2NL/dJMcabw9Qr1/wwA8OF5gJFV8xHFJGXFUuK/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/Et2NL/dJMcabw9Qr1/wwA8OF5gJFV8xHFJGXFUuK/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/Et2NL/dJMcabw9Qr1/wwA8OF5gJFV8xHFJGXFUuK/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FEt2NL%2FdJMcabw9Qr1%2FwwA8OF5gJFV8xHFJGXFUuK%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;780&quot; height=&quot;780&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;업그레이드 여부는 업무 성격에 따라 다릅니다. 어려운 코딩&amp;middot;비전&amp;middot;에이전트 루프가 중심이면 지금 올리는 게 맞고, 한국어 자연어 대량 생성이나 예산 민감도가 높으면 4.6에 당분간 남아도 됩니다. 도구는 &quot;전부 올려서 비싸게 쓰기&quot;가 아니라 &lt;b&gt;작업에 맞는 모델을 고르는 믹스 전략&lt;/b&gt;이 가장 효율적입니다. 동일 환경이면 위 판단 기준 그대로 써도 됩니다.&lt;/p&gt;
&lt;hr data-ke-style=&quot;style1&quot; /&gt;
&lt;div class=&quot;related-posts&quot; style=&quot;border: 1px solid #e7e5dd; border-radius: 8px; padding: 16px; margin: 24px 0; background: #faf9f5;&quot;&gt;
&lt;h3 style=&quot;margin-top: 0;&quot; data-ke-size=&quot;size23&quot;&gt;  이 카테고리의 다른 글&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/556&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;Gemini CLI 사용법 &amp;mdash; 무료로 어디까지 되나, 직접 써보고 정리&lt;/a&gt; &amp;mdash; 2026-04-19&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/554&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;앤스로픽 역대급 실수! 차세대 AI &#39;클로드 미토스&lpar;Mythos&rpar;&#39; 유출 정보 총정리&lt;/a&gt; &amp;mdash; 2026-04-08&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/553&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;Claude Code 창시자와 해커톤 우승자의 공통 꿀팁 7가지&lt;/a&gt; &amp;mdash; 2026-04-05&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;i&gt;같은 &lt;b&gt;AI 활용법&lt;/b&gt; 카테고리에서 이어서 읽기&lt;/i&gt;&lt;/p&gt;
&lt;/div&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;설치 환경:&lt;/b&gt; Windows 11, Claude Max 플랜, Claude Code &lpar;2026-04 빌드&rpar;, Node.js v24&lt;/p&gt;
&lt;script type=&quot;application/ld+json&quot;&gt;
{
  &quot;@context&quot;: &quot;https://schema.org&quot;,
  &quot;@type&quot;: &quot;FAQPage&quot;,
  &quot;mainEntity&quot;: [
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Opus 4.7로 올리면 한국어 품질이 떨어진다는 얘기가 있던데 사실인가요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;국내 일부 사용자 리뷰에 4.6이 한국어 문장이 더 자연스럽다는 평이 있습니다. 주관적 체감이라 본인 사용 패턴에서 비교해보는 게 맞습니다. 코딩·기술 문서 용도는 큰 차이가 없지만 블로그 톤의 긴 한국어 생성은 4.6도 경쟁력이 있습니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Claude Opus 4.7 가격이 같다고 하는데 실제 비용도 같나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;단가는 동일&lpar;$5 입력 / $25 출력 per 1M tokens&rpar;하지만 새 토크나이저가 토큰을 1.0~1.35배 더 쓰기 때문에 실비용은 최대 35%까지 오를 수 있습니다. 평균 10~20% 증가를 예상하면 됩니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Claude Code에서 Opus 4.7로 바꾸는 법은요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;claude 실행 후 /model 입력 후 claude-opus-4-7 선택하거나, 터미널에서 claude --model claude-opus-4-7로 실행합니다. Max 플랜 구독자는 별도 결제 없이 포함됩니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;1M 컨텍스트 모드는 Opus 4.7에서도 유지되나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;네, Opus 4.6부터 제공된 1M 토큰 컨텍스트 윈도우가 4.7에서도 그대로 유지됩니다. 긴 레포 전체 분석 용도라면 4.7의 어려운 코드 이해력 개선과 맞물려 체감이 큽니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;/ultrareview는 지금 써도 되나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;일반 코드 리뷰에는 과합니다. 1회 $10~20이라 소규모 패치에는 낭비고, 큰 PR·릴리즈 직전 검증·보안 감사 같은 배치성 작업에 적합합니다.&quot;}}
  ]
}
&lt;/script&gt;</sub>- [Claude Cowork 자동화 완전 정리 &amp;mdash; 매일 아침 카톡으로 오는 AI 브리핑 만드는 법](https://hgko-dev.tistory.com/558) <sub>— 
&lt;p data-ke-size=&quot;size16&quot;&gt;&quot;ChatGPT랑 Claude 똑같은 거 아니야?&quot; 라고 묻는 팀원이 여전히 많죠. 답변만 받고 복사&amp;middot;붙여넣기로 끝내는 수준이면 하루 3번 반복되는 조사&amp;middot;요약&amp;middot;전달 업무는 그대로 쌓입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;10년 개발하면서 자동화 파이프라인은 파이썬&amp;middot;크론&amp;middot;n8n까지 다 돌려봤는데, Claude Cowork + Pley MCP + 스케줄러 조합은 &lt;b&gt;코딩 한 줄 없이&lt;/b&gt; 이 흐름을 만든 첫 경험이었어요.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;이 글을 끝까지 읽으면 매일 아침 10시에 증시 뉴스를 자동 수집&amp;middot;분석&amp;middot;카카오톡 전송까지 하는 에이전트를 직접 만들 수 있습니다.&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/UFIzv/dJMcabqpZMK/yKGQBHEZIbewWsHyQ6AhK1/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/UFIzv/dJMcabqpZMK/yKGQBHEZIbewWsHyQ6AhK1/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/UFIzv/dJMcabqpZMK/yKGQBHEZIbewWsHyQ6AhK1/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FUFIzv%2FdJMcabqpZMK%2FyKGQBHEZIbewWsHyQ6AhK1%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;1. Claude Cowork가 뭐길래 &amp;mdash; &quot;답변 주는 AI&quot;에서 &quot;일하는 AI&quot;로&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;기존 Claude와 Cowork는 같은 이름을 공유할 뿐, 사용 목적이 완전히 다릅니다. 한 줄로 정리하면 &lt;b&gt;&quot;알려주는 AI&quot;에서 &quot;해주는 AI&quot;로의 전환&lt;/b&gt;입니다.&lt;/p&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;구분&lt;/th&gt;
&lt;th&gt;기존 Claude&lt;/th&gt;
&lt;th&gt;Claude Cowork&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;역할&lt;/td&gt;
&lt;td&gt;답변을 주는 도구&lt;/td&gt;
&lt;td&gt;일을 해주는 에이전트&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;파일 접근&lt;/td&gt;
&lt;td&gt;대화창 안에서만 처리&lt;/td&gt;
&lt;td&gt;내 컴퓨터 폴더 직접 읽고 쓰기&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;웹 접근&lt;/td&gt;
&lt;td&gt;검색 결과만 조회&lt;/td&gt;
&lt;td&gt;실제 브라우저 직접 조작&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;외부 서비스&lt;/td&gt;
&lt;td&gt;제한적&lt;/td&gt;
&lt;td&gt;Gmail&amp;middot;노션&amp;middot;카카오톡까지 연결&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;기존 Claude가 ChatGPT 웹버전이라면, Cowork는 로컬에 사는 비서에 가깝습니다. 여러분 폴더에 파일을 쓰고, 브라우저를 열고, 카톡을 보냅니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;2. 사전 준비물 &amp;mdash; 딱 2가지&lt;/h2&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;항목&lt;/th&gt;
&lt;th&gt;설명&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;Claude Pro 이상 구독&lt;/td&gt;
&lt;td&gt;무료 플랜은 Cowork 사용 불가&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Claude 데스크톱 앱&lt;/td&gt;
&lt;td&gt;웹 브라우저 버전은 안 됨, 반드시 데스크톱 앱&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;앱 설치는 Claude 사이트 &amp;rarr; 왼쪽 하단 &quot;앱 및 확장 프로그램 받기&quot; &amp;rarr; OS에 맞는 파일 다운로드 순서입니다. 2026년 4월 업데이트로 &lt;b&gt;채팅/코워크/코드 탭이 상단에서 왼쪽 사이드바 상단으로 이동&lt;/b&gt;했으니 위치를 못 찾으면 왼쪽 바를 확인하세요.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;3. 작업 폴더 설정 &amp;mdash; Cowork의 출발점&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Cowork를 쓸 때 가장 먼저 할 일은 &lt;b&gt;Claude가 작업할 폴더 지정&lt;/b&gt;입니다. 바탕화면에 &lt;code&gt;에이전트/클로드&lt;/code&gt; 같은 폴더를 만들고 Claude 앱 &amp;rarr; 코워크 &amp;rarr; &quot;다른 폴더 선택&quot; &amp;rarr; 방금 만든 폴더 지정. 권한 요청이 뜨면 &quot;항상 허용&quot;을 누릅니다.&lt;/p&gt;
&lt;blockquote data-ke-style=&quot;style3&quot;&gt;보안이 걱정된다면: Claude는 지정한 폴더에서만 파일을 읽고 쓸 수 있습니다. &quot;집에 방이 여러 개 있는데, 허락한 방만 열리는 열쇠를 쥐어주는 것&quot;에 비유하면 이해가 빠릅니다.&lt;/blockquote&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;4. 크롬용 Claude로 웹 데이터 수집&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;크롬용 Claude는 &lt;b&gt;여러분의 크롬 브라우저를 Claude가 직접 조작&lt;/b&gt;하는 기능입니다. API 연동이 필요 없고, 사람이 페이지 보듯 실제로 탐색합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;설치: 크롬 확장 프로그램 스토어에서 &quot;Claude&quot; 검색 &amp;rarr; 설치 &amp;rarr; Claude 앱 &amp;rarr; 프로필 &amp;rarr; 설정 &amp;rarr; &quot;브라우저 사용&quot; 토글 활성화.&lt;/p&gt;
&lt;pre class=&quot;erlang&quot;&gt;&lt;code&gt;크롬용 Claude로 한국경제 사이트에 접속해서
한국 증시와 미국 증시에 대해 조사해줘.&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;그러면 실제 크롬 창이 열리고 Claude가 페이지를 탐색하면서 데이터를 수집합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/cM1sfq/dJMcajolLe9/fI6uNbgwH2vb6aPHwwE7M0/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/cM1sfq/dJMcajolLe9/fI6uNbgwH2vb6aPHwwE7M0/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/cM1sfq/dJMcajolLe9/fI6uNbgwH2vb6aPHwwE7M0/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcM1sfq%2FdJMcajolLe9%2FfI6uNbgwH2vb6aPHwwE7M0%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;5. Pley MCP &amp;mdash; 한국 서비스 연결의 핵심&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;MCP&lpar;Model Context Protocol&rpar;는 AI와 외부 서비스를 연결하는 표준 규격입니다. 비유하자면 USB-C입니다. 예전에는 아이폰&amp;middot;삼성폰 충전선이 달랐지만 지금은 USB-C로 통일됐듯, AI 세계의 연결 규격을 Anthropic이 MCP로 통일했습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude 기본 커넥터는 해외 서비스 위주라 한국 실무에서는 반쪽짜리입니다. &lt;b&gt;Pley MCP가 한국 서비스 전용&lt;/b&gt;이라는 게 이 조합의 핵심입니다.&lt;/p&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;MCP&lt;/th&gt;
&lt;th&gt;용도&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;카카오톡 나와의 채팅방&lt;/td&gt;
&lt;td&gt;Claude가 내 카톡으로 메시지 전송&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;네이버 검색&lt;/td&gt;
&lt;td&gt;네이버 뉴스&amp;middot;증권 데이터 수집&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;연결 순서 &lpar;증상&amp;rarr;원인&amp;rarr;해결 포함&rpar;&lt;/h3&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;Pley MCP 사이트 접속 &amp;rarr; 카카오 로그인 &amp;rarr; 원하는 MCP 선택 &amp;rarr; &quot;도구함에 추가&quot;&lt;/li&gt;
&lt;li&gt;Claude 앱 &amp;rarr; 왼쪽 상단 &quot;커스터마이즈&quot; &amp;rarr; 커넥터 &amp;rarr; 플러스&lpar;+&rpar; &amp;rarr; &quot;Pley MCP&quot; 검색 &amp;rarr; 플러스 버튼&lt;/li&gt;
&lt;li&gt;&quot;모두 동의 후 속행&quot; 클릭&lt;/li&gt;
&lt;/ol&gt;
&lt;blockquote data-ke-style=&quot;style3&quot;&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;증상: 커넥터 연결 후에도 &quot;MCP를 찾을 수 없다&quot;는 응답이 돌아온다.&lt;br /&gt;원인: Claude 앱을 재시작하지 않아 연결 상태가 캐시돼 있음.&lt;br /&gt;해결: Claude 앱을 완전히 종료&lpar;트레이 아이콘에서도 종료&rpar;하고 재실행. 한국 툴 연결 세팅에서 이 재시작을 빼먹어서 20분 날려먹었습니다.&lt;/p&gt;
&lt;/blockquote&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;6. 보고서 생성 + 카카오톡 전송&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;데이터 수집까지 했으면 이제 산출물 단계입니다. 대화창에 이렇게 요청합니다.&lt;/p&gt;
&lt;pre class=&quot;erlang&quot;&gt;&lt;code&gt;한국경제와 네이버에서 가져온 데이터를 합쳐서
상세한 보고서를 docx 파일로 만들어 지금 폴더에 저장해줘.
이후 요약본을 카카오톡 &quot;나와의 채팅방&quot;으로 보내줘.&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude가 docs 스킬로 워드 파일을 생성하고, Pley MCP의 카카오톡 커넥터로 요약본을 전송합니다. 전체 흐름은 아래 4단계입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/egTHiQ/dJMcagZwdOy/Cr8Ghjy6pGblfOkzILfngK/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/egTHiQ/dJMcagZwdOy/Cr8Ghjy6pGblfOkzILfngK/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/egTHiQ/dJMcagZwdOy/Cr8Ghjy6pGblfOkzILfngK/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FegTHiQ%2FdJMcagZwdOy%2FCr8Ghjy6pGblfOkzILfngK%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;780&quot; height=&quot;780&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;7. 플러그인으로 패키징 &amp;mdash; 슬래시 명령 한 줄로&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;매번 같은 명령을 반복하는 건 비효율이죠. 플러그인으로 묶으면 슬래시 명령 하나로 전체 워크플로우가 실행됩니다. 회사에 비유하자면 스킬이 업무 매뉴얼이라면 플러그인은 신입사원 온보딩 키트에 해당합니다 &amp;mdash; 스킬&amp;middot;커넥터 설정&amp;middot;명령어&amp;middot;서브 에이전트가 한 묶음이 됩니다.&lt;/p&gt;
&lt;pre class=&quot;erlang&quot;&gt;&lt;code&gt;지금까지 한 작업을 플러그인으로 패키징해줘.
네이버 MCP 작업과 크롬용 Claude 작업은
서브 에이전트로 놓고 병렬 작업식으로 묶어줘.&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude가 자동으로 플러그인을 생성하면 &quot;플러그인 설치&quot; &amp;rarr; 우측 상단 &quot;플러그인 저장&quot;을 누릅니다. 이제 Cowork에서 &lt;code&gt;/generate-report&lt;/code&gt; 한 줄로 전체 파이프라인이 돕니다. 팀원에게 파일로 공유할 수도 있는데, 받는 쪽도 동일한 MCP 커넥터를 미리 연결해둬야 합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;8. 스케줄러로 완전 자동화&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;마지막 단계는 자동 실행입니다. 왼쪽 사이드바 &amp;rarr; 스케줄 &amp;rarr; &quot;뉴 테스크&quot; &amp;rarr; 아래 항목 입력:&lt;/p&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;항목&lt;/th&gt;
&lt;th&gt;값&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;이름&lt;/td&gt;
&lt;td&gt;증시 분석&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;프롬프트&lt;/td&gt;
&lt;td&gt;&lt;code&gt;/generate-report 실행해줘&lt;/code&gt;&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;빈도&lt;/td&gt;
&lt;td&gt;매일 오전 10시&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;모델&lt;/td&gt;
&lt;td&gt;Sonnet 4.6&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/N1fwF/dJMcahKVFJf/yFATu0a0KUNYw7fmlnzJG1/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/N1fwF/dJMcahKVFJf/yFATu0a0KUNYw7fmlnzJG1/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/N1fwF/dJMcahKVFJf/yFATu0a0KUNYw7fmlnzJG1/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FN1fwF%2FdJMcahKVFJf%2FyFATu0a0KUNYw7fmlnzJG1%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;저장하면 매일 아침 10시에 보고서가 생성되고 카카오톡으로 요약이 날아옵니다.&lt;/p&gt;
&lt;blockquote data-ke-style=&quot;style3&quot;&gt;⚠️ 주의: 컴퓨터와 Claude 앱이 반드시 켜져 있어야 합니다. 컴퓨터가 꺼져 있으면 스케줄러도 동작하지 않습니다. 노트북을 닫아두는 시간대로 설정했다가 3일 동안 보고서가 안 오길래 확인해 보니 이 이유였습니다. 본인 생활 패턴에서 PC가 켜져 있는 시간대로 설정하세요.&lt;/blockquote&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;9. 실무 관점 &amp;mdash; 트레이드오프와 쓰지 말아야 할 경우&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Cowork가 만능은 아닙니다. 10년 개발하면서 자동화 파이프라인 여러 개 돌려본 관점에서 솔직하게 정리합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;장점이 빛나는 상황&lt;/b&gt;&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;수집&amp;middot;분석&amp;middot;전달이 한 줄로 흐르는 &lt;b&gt;단방향 업무&lt;/b&gt; &lpar;리서치&amp;middot;일일 리포트&amp;middot;모니터링&rpar;&lt;/li&gt;
&lt;li&gt;코딩 리소스가 없는 &lt;b&gt;비개발 팀&lt;/b&gt;이 자동화를 시도할 때&lt;/li&gt;
&lt;li&gt;API가 없는 한국 서비스&lpar;네이버&amp;middot;카카오톡&rpar;를 엮어야 하는 환경&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;안 쓰는 게 나은 상황&lt;/b&gt;&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;트랜잭션성이 강한 업무 &lpar;결제&amp;middot;DB 업데이트&rpar; &amp;mdash; 크론 + 백엔드 코드가 안전합니다&lt;/li&gt;
&lt;li&gt;에러 복구&amp;middot;재시도 로직이 중요한 미션 크리티컬 워크플로우&lt;/li&gt;
&lt;li&gt;컴퓨터를 매일 꺼두는 환경 &amp;mdash; 스케줄러가 안 돕니다&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;팀 규모 3명 이하면 Cowork 단독으로 충분하고, 회사 차원에서 운영하려면 결국 서버 기반 자동화&lpar;n8n, Zapier, 자체 크론 서버&rpar;로 옮겨가는 게 장기적으로 맞습니다. 정답은 없고, &lt;b&gt;&quot;어디까지 자동화할지 범위를 정하는 것&quot;&lt;/b&gt;이 이 도구의 핵심 판단이 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;10. 이 구조를 다른 주제에 적용하기&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;증시 브리핑은 하나의 예시일 뿐이고, 코어 패턴은 &lt;b&gt;수집 &amp;rarr; 분석 &amp;rarr; 산출물 &amp;rarr; 전달&lt;/b&gt; 4단계로 단순합니다. 이 구조만 이해하면 본인만의 자동화를 설계할 수 있어요.&lt;/p&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;활용 예시&lt;/th&gt;
&lt;th&gt;수집&lt;/th&gt;
&lt;th&gt;분석&lt;/th&gt;
&lt;th&gt;산출물&lt;/th&gt;
&lt;th&gt;전달&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;경쟁사 모니터링&lt;/td&gt;
&lt;td&gt;경쟁사 뉴스 사이트&lt;/td&gt;
&lt;td&gt;변화 요약&lt;/td&gt;
&lt;td&gt;보고서&lt;/td&gt;
&lt;td&gt;슬랙&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;고객 리뷰 분석&lt;/td&gt;
&lt;td&gt;리뷰 사이트&lt;/td&gt;
&lt;td&gt;감성 분석&lt;/td&gt;
&lt;td&gt;정리 문서&lt;/td&gt;
&lt;td&gt;노션&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;유튜브 트렌드&lt;/td&gt;
&lt;td&gt;인기 영상 조회&lt;/td&gt;
&lt;td&gt;주제 분류&lt;/td&gt;
&lt;td&gt;트렌드 리포트&lt;/td&gt;
&lt;td&gt;이메일&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;환율&amp;middot;원자재 체크&lt;/td&gt;
&lt;td&gt;금융 사이트&lt;/td&gt;
&lt;td&gt;변동률 계산&lt;/td&gt;
&lt;td&gt;일일 보고서&lt;/td&gt;
&lt;td&gt;카카오톡&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;자주 묻는 질문&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Claude Cowork는 무료로 쓸 수 있나요?&lt;/b&gt;&lt;br /&gt;A. 무료 플랜에서는 Cowork 기능을 쓸 수 없습니다. Claude Pro 이상 구독이 필요하며, 저는 Max 플랜을 쓰고 있습니다. 업무 자동화 용도로는 Pro로도 충분합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Pley MCP는 꼭 써야 하나요?&lt;/b&gt;&lt;br /&gt;A. 한국 서비스&lpar;카카오톡&amp;middot;네이버&rpar;를 연결할 거면 필수입니다. Gmail&amp;middot;노션&amp;middot;슬랙 같은 해외 서비스만 쓸 거면 Claude 기본 커넥터로도 됩니다. 국내 업무 맥락에서는 Pley MCP 없이 반쪽짜리라 생각하면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 스케줄러로 돌린 결과가 안 올 때는 어떻게 확인하나요?&lt;/b&gt;&lt;br /&gt;A. 먼저 PC 전원&amp;middot;Claude 앱 실행 여부부터 확인하세요. 스케줄러는 앱이 떠 있을 때만 동작합니다. 그다음 해당 시간대에 커넥터 토큰이 만료됐는지 &lpar;카카오 로그인 세션 등&rpar; 확인하시면 됩니다. 경험상 95%는 PC&amp;middot;앱이 꺼져 있던 경우였습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 플러그인을 팀원에게 공유하면 바로 쓸 수 있나요?&lt;/b&gt;&lt;br /&gt;A. 아닙니다. 파일은 공유되지만 &lt;b&gt;받는 사람도 동일한 MCP 커넥터를 미리 연결&lt;/b&gt;해둬야 동작합니다. 플러그인은 워크플로우 레시피고, 재료&lpar;커넥터&rpar;는 각자 준비해야 합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Claude Dispatch는 뭐고 지금 써도 되나요?&lt;/b&gt;&lt;br /&gt;A. 핸드폰으로 데스크톱 Claude 앱을 조종하는 기능입니다. 2026년 4월 기준 지시사항이 PC로 제대로 전달되지 않는 버그가 종종 발생하고 있어, 안정화될 때까지는 주의해서 사용하시는 것을 권합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;마무리&lt;/h2&gt;
&lt;table style=&quot;border-collapse: collapse;&quot; border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;단계&lt;/th&gt;
&lt;th&gt;내용&lt;/th&gt;
&lt;th&gt;도구&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;1. 기본 세팅&lt;/td&gt;
&lt;td&gt;Cowork 작업 폴더 지정&lt;/td&gt;
&lt;td&gt;데스크톱 앱&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;2. 웹 데이터 수집&lt;/td&gt;
&lt;td&gt;한국경제 스크래핑&lt;/td&gt;
&lt;td&gt;크롬용 Claude&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;3. 한국 서비스 연결&lt;/td&gt;
&lt;td&gt;네이버&amp;middot;카카오톡&lt;/td&gt;
&lt;td&gt;Pley MCP&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;4. 보고서 생성&lt;/td&gt;
&lt;td&gt;워드 파일 저장&lt;/td&gt;
&lt;td&gt;docs 스킬&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;5. 요약 전송&lt;/td&gt;
&lt;td&gt;카카오톡 메시지&lt;/td&gt;
&lt;td&gt;카카오톡 MCP&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;6. 패키징&lt;/td&gt;
&lt;td&gt;명령 하나로 통합&lt;/td&gt;
&lt;td&gt;플러그인&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;7. 자동화&lt;/td&gt;
&lt;td&gt;매일 지정 시간 실행&lt;/td&gt;
&lt;td&gt;스케줄러&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Cowork의 진짜 가치는 단일 작업이 아니라 &lt;b&gt;워크플로우&lt;/b&gt;에 있습니다. 도구 하나를 잘 쓰는 게 아니라, 도구들을 연결해 시스템을 설계하는 것. 그리고 Cowork는 그 시스템을 코딩 한 줄 없이 만들 수 있게 해줍니다. 팀에서 500건+ 코드 리뷰하면서 느낀 건, 반복 업무가 많은 사람일수록 이 전환점의 효용이 커진다는 점이었습니다. 동일 환경이면 위 워크플로우 그대로 써도 됩니다.&lt;/p&gt;
&lt;hr data-ke-style=&quot;style1&quot; /&gt;
&lt;div class=&quot;related-posts&quot; style=&quot;border: 1px solid #e7e5dd; border-radius: 8px; padding: 16px; margin: 24px 0; background: #faf9f5;&quot;&gt;
&lt;h3 style=&quot;margin-top: 0;&quot; data-ke-size=&quot;size23&quot;&gt;&lt;br /&gt;  이 카테고리의 다른 글&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/556&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;Gemini CLI 사용법 &amp;mdash; 무료로 어디까지 되나, 직접 써보고 정리&lt;/a&gt; &amp;mdash; 2026-04-19&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/553&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;Claude Code 창시자와 해커톤 우승자의 공통 꿀팁 7가지&lt;/a&gt; &amp;mdash; 2026-04-05&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;i&gt;같은 &lt;b&gt;AI 활용법&lt;/b&gt; 카테고리에서 이어서 읽기&lt;/i&gt;&lt;/p&gt;
&lt;/div&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;설치 환경:&lt;/b&gt; Windows 11, Claude 데스크톱 앱 &lpar;2026-04 빌드&rpar;, Claude Pro 구독, Pley MCP, 크롬 최신 버전&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;
&lt;script type=&quot;application/ld+json&quot;&gt;
{
  &quot;@context&quot;: &quot;https://schema.org&quot;,
  &quot;@type&quot;: &quot;FAQPage&quot;,
  &quot;mainEntity&quot;: [
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Claude Cowork는 무료로 쓸 수 있나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;무료 플랜에서는 Cowork 기능을 쓸 수 없습니다. Claude Pro 이상 구독이 필요합니다. 업무 자동화 용도로는 Pro로도 충분합니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Pley MCP는 꼭 써야 하나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;한국 서비스&lpar;카카오톡·네이버&rpar;를 연결할 거면 필수입니다. 해외 서비스만 쓸 거면 Claude 기본 커넥터로도 됩니다. 국내 업무 맥락에서는 Pley MCP 없이는 반쪽짜리입니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;스케줄러로 돌린 결과가 안 올 때는 어떻게 확인하나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;PC 전원과 Claude 앱 실행 여부부터 확인하세요. 스케줄러는 앱이 떠 있을 때만 동작합니다. 그다음 커넥터 토큰 만료 여부를 점검합니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;플러그인을 팀원에게 공유하면 바로 쓸 수 있나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;파일은 공유되지만 받는 사람도 동일한 MCP 커넥터를 미리 연결해둬야 동작합니다. 플러그인은 워크플로우 레시피고 재료&lpar;커넥터&rpar;는 각자 준비해야 합니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Claude Dispatch는 지금 써도 되나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;핸드폰으로 데스크톱 Claude 앱을 조종하는 기능입니다. 2026년 4월 기준 지시사항이 PC로 제대로 전달되지 않는 버그가 종종 발생하고 있어 주의해서 사용하시는 것을 권합니다.&quot;}}
  ]
}
&lt;/script&gt;
&lt;/p&gt;</sub>- [Google Antigravity 사용법 &amp;mdash; 설치부터 첫 워크스페이스까지 핵심 정리](https://hgko-dev.tistory.com/557) <sub>— 
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/kHrem/dJMcaaSzLWx/qqymPhnWnCLJTRLomXK950/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/kHrem/dJMcaaSzLWx/qqymPhnWnCLJTRLomXK950/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/kHrem/dJMcaaSzLWx/qqymPhnWnCLJTRLomXK950/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FkHrem%2FdJMcaaSzLWx%2FqqymPhnWnCLJTRLomXK950%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Google Antigravity를 설치는 해놨는데 &quot;Agent Manager가 뭐고 Manager View는 어디서 여는 건지&quot; 감이 안 잡혀 창만 열고 닫는 분이 많습니다. 그대로 묵히면 퍼블릭 프리뷰 기간에 Gemini 3 Pro를 무료로 붙여볼 수 있는 멀티 에이전트 감각을 놓치고, 나중에 유료화된 뒤 기초 메뉴 위치부터 다시 익혀야 합니다. AI 코딩 도구 릴리스 노트를 4년째 정리하는 블로그 운영자 시각에서, Google 공식 사이트&lpar;antigravity.google&rpar;와 Codelabs 튜토리얼을 기준으로 Google Antigravity 사용법을 단계별로 정리했습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;이 글을 끝까지 읽으면 다운로드 URL부터 시스템 요구사항, 초기 설정 3가지 선택지, Agent Manager에서 첫 미션 쏘기, 5개 에이전트 병렬 실행, 모델 선택 기준까지 한 번에 잡힙니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;1. Google Antigravity가 뭔가 &lpar;간단 소개&rpar;&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Google Antigravity는 구글이 공개한 에이전트 우선&lpar;agent-first&rpar; 개발 환경입니다. 공식 사이트 주소는 &lt;a href=&quot;https://antigravity.google/&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;https://antigravity.google/&lt;/a&gt; 이며, 공식 튜토리얼은 &lt;a href=&quot;https://codelabs.developers.google.com/getting-started-google-antigravity&quot; target=&quot;_blank&quot; rel=&quot;noopener&quot;&gt;https://codelabs.developers.google.com/getting-started-google-antigravity&lt;/a&gt; 에 올라와 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;기존 AI IDE가 &quot;에디터 옆에 채팅창이 붙어 있는 형태&quot;라면, Antigravity는 반대입니다. 앱을 처음 실행하면 에디터 화면이 아니라 &lt;b&gt;Agent Manager&lt;/b&gt;라는 대시보드가 뜹니다. 코드 파일을 여는 것보다 &quot;어떤 에이전트에게 무슨 미션을 맡길 것인가&quot;를 먼저 결정하게 만드는 구조라고 Codelabs 문서가 설명합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini 3 Pro가 기본 엔진이지만, 같은 도구 안에서 Gemini 3 Flash / Claude Opus / Claude Sonnet 도 함께 선택할 수 있습니다. 한 미션 내에서도 에이전트마다 다른 모델을 배정할 수 있다는 점이 차별점입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;2. 시스템 요구사항과 가격&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;본격 설치 전에 사용 환경이 요구사항을 맞추는지 확인할 필요가 있습니다. 공식 다운로드 페이지에 명시된 스펙을 표로 정리하면 다음과 같습니다.&lt;/p&gt;
&lt;table border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;항목&lt;/th&gt;
&lt;th&gt;요구사항&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;macOS&lt;/td&gt;
&lt;td&gt;Monterey 12 이상&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Windows&lt;/td&gt;
&lt;td&gt;Windows 10 이상 &lpar;64-bit&rpar;&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Linux&lt;/td&gt;
&lt;td&gt;64-bit, glibc 2.28+, glibcxx 3.4.25+&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;계정&lt;/td&gt;
&lt;td&gt;Google 계정&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;가격&lt;/td&gt;
&lt;td&gt;퍼블릭 프리뷰 기간 무료&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Rate Limit&lt;/td&gt;
&lt;td&gt;Gemini 3 Pro에 대해 &quot;generous rate limit&quot; 제공&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&quot;generous rate limit&quot;이 구체 숫자로 공개돼 있지는 않지만, 공식 발표는 퍼블릭 프리뷰 기간 동안 개인 개발자가 체감 수준에서 제한을 느끼기 어려운 수준이라는 표현을 쓰고 있습니다. 단, 프로덕션 배포용이 아니라 실험&amp;middot;학습용 할당량이라는 점은 주의가 필요합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/oJ800/dJMcahqCXsC/gyxNjV7dLw8eAFkG8puHW1/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/oJ800/dJMcahqCXsC/gyxNjV7dLw8eAFkG8puHW1/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/oJ800/dJMcahqCXsC/gyxNjV7dLw8eAFkG8puHW1/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FoJ800%2FdJMcahqCXsC%2FgyxNjV7dLw8eAFkG8puHW1%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;3. 다운로드&amp;middot;설치 단계 &lpar;Windows 기준&rpar;&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;공식 Codelabs 튜토리얼에 안내된 설치 절차는 다음과 같습니다. Windows 11 환경을 예로 정리합니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;브라우저로 &lt;code&gt;https://antigravity.google/&lt;/code&gt; 접속&lt;/li&gt;
&lt;li&gt;상단 다운로드 버튼에서 본인 OS 선택 &amp;rarr; Windows 64-bit 인스톨러 받기&lt;/li&gt;
&lt;li&gt;다운받은 &lt;code&gt;.exe&lt;/code&gt; 파일 실행 &amp;rarr; 기본 옵션으로 설치 진행&lt;/li&gt;
&lt;li&gt;설치 완료 후 Antigravity 앱 실행&lt;/li&gt;
&lt;li&gt;첫 화면에서 &lt;b&gt;Google 계정 로그인&lt;/b&gt;&lt;/li&gt;
&lt;li&gt;로그인 성공 시 Agent Manager 대시보드가 기본 진입 화면으로 열림&lt;/li&gt;
&lt;/ol&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;macOS / Linux 도 같은 흐름입니다. 차이는 인스톨러 파일 확장자&lpar;&lt;code&gt;.dmg&lt;/code&gt;, &lt;code&gt;.deb&lt;/code&gt; / &lt;code&gt;.rpm&lt;/code&gt; 또는 AppImage&rpar;뿐입니다. 사내망 프록시 환경이면 Google 계정 OAuth 팝업이 차단될 수 있으니, 최초 로그인은 제한 없는 회선에서 수행하는 것을 권장합니다.&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;트러블슈팅 &amp;mdash; 설치 후 앱이 뜨지 않는 경우&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;증상&lt;/b&gt;: 인스톨러는 정상 종료됐는데 실행 시 창이 뜨지 않거나 &quot;필수 라이브러리 누락&quot; 메시지가 뜸&lt;/li&gt;
&lt;li&gt;&lt;b&gt;원인&lt;/b&gt;: Linux에서 주로 발생합니다. 배포판의 glibc / glibcxx 버전이 요구치&lpar;glibc 2.28+, glibcxx 3.4.25+&rpar;보다 낮은 경우&lt;/li&gt;
&lt;li&gt;&lt;b&gt;해결&lt;/b&gt;: &lt;code&gt;ldd --version&lt;/code&gt; 으로 glibc 버전 확인 후, 충족하지 못하면 배포판을 최신 LTS로 업그레이드. Windows 10 미만도 동일한 증상이 보고됩니다&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;4. 첫 실행 &amp;mdash; 초기 설정 3가지&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;로그인 직후 Antigravity는 작업 스타일을 정하는 초기 설정 3가지를 묻습니다. 공식 Codelabs 튜토리얼은 일반 개발자에게 아래 조합을 권장합니다.&lt;/p&gt;
&lt;table border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;설정 항목&lt;/th&gt;
&lt;th&gt;선택값&lt;/th&gt;
&lt;th&gt;의미&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;개발 모드&lt;/td&gt;
&lt;td&gt;Agent-assisted development&lt;/td&gt;
&lt;td&gt;에이전트가 대부분의 작업을 수행, 사람은 계획과 변경 리뷰 담당&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;터미널 실행&lt;/td&gt;
&lt;td&gt;Terminal execution &lpar;Auto&rpar;&lt;/td&gt;
&lt;td&gt;&lt;code&gt;ls&lt;/code&gt;, &lt;code&gt;npm install&lt;/code&gt; 같은 안전한 루틴 명령은 자동 실행 허용&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;리뷰 정책&lt;/td&gt;
&lt;td&gt;Review policy &lpar;Agent decides&rpar;&lt;/td&gt;
&lt;td&gt;에이전트가 스스로 &quot;사람 리뷰가 필요한 시점&quot;을 판단&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;이 조합은 AI에게 충분한 자율성을 주면서도, 리스크 있는 변경에서는 사람 개입이 걸리도록 설계돼 있습니다. 처음부터 수동 리뷰로 강제하면 에이전트의 흐름이 끊겨 멀티 에이전트 가치가 절반으로 줄어든다는 얘기가 공식 문서에 언급돼 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;장점은 자동 실행 덕에 진행 속도가 빠르다는 점이고, 단점은 팀 규모가 커서 변경 추적이 민감한 환경에서는 Auto 실행 범위가 예상보다 넓게 잡힐 수 있다는 점입니다. 팀원이 5명 이상이거나 프로덕션 리포지토리에 직접 붙일 계획이라면 Terminal execution을 Manual로 내리고 Review policy도 수동으로 바꾸는 게 낫습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;5. 핵심 개념 5가지 &amp;mdash; Agent Manager / Manager View / Workspace / Artifacts / Multi-Model&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Google Antigravity 사용법의 뼈대는 이 다섯 개념으로 정리됩니다. 공식 Codelabs 튜토리얼이 반복해서 등장시키는 용어이기도 합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;① Agent Manager&lt;/b&gt; &amp;mdash; 앱을 실행했을 때 처음 보이는 화면 자체를 말합니다. 여러 에이전트를 한눈에 띄우고 지시&amp;middot;모니터링하는 홈 대시보드 역할입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;② Manager View&lt;/b&gt; &amp;mdash; 왼쪽 사이드바에 작은 아이콘이 있고, 클릭하면 Mission Control이 열립니다. 여기서 여러 에이전트를 동시에 생성하고 상태를 확인할 수 있습니다. 예를 들어 서로 다른 버그 5개를 잡아야 한다면, 에이전트 5개를 만들어 각각 한 버그씩 배정하는 식의 사용이 가능합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;③ Workspace&lt;/b&gt; &amp;mdash; VS Code의 &quot;폴더 열기&quot;와 동일한 개념입니다. 상단 메뉴에서 &lt;b&gt;File &amp;rarr; Open Folder&lt;/b&gt;를 선택하고 로컬 프로젝트 폴더를 지정하면 해당 폴더가 워크스페이스가 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;④ Artifacts System&lt;/b&gt; &amp;mdash; 에이전트가 만들어내는 검증 가능한 산출물 체계입니다. 코딩을 바로 시작하지 않고, 먼저 &lt;b&gt;기술 로드맵&lpar;technical roadmap&rpar;&lt;/b&gt;을 Artifact로 생성한 뒤 그 로드맵을 따라 구현을 진행합니다. 사람이 중간에 로드맵만 리뷰해도 방향이 크게 빗나가는 것을 잡을 수 있도록 설계돼 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;⑤ Multiple Models&lt;/b&gt; &amp;mdash; 한 도구 안에서 Gemini 3 Pro, Gemini 3 Flash, Claude Opus, Claude Sonnet 을 고를 수 있습니다. 같은 미션 안에서도 에이전트마다 다른 모델을 붙일 수 있는 점이 핵심입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/b31Zew/dJMcabRseXC/ABittaauziw6MroTHsXsSK/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/b31Zew/dJMcabRseXC/ABittaauziw6MroTHsXsSK/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/b31Zew/dJMcabRseXC/ABittaauziw6MroTHsXsSK/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fb31Zew%2FdJMcabRseXC%2FABittaauziw6MroTHsXsSK%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;780&quot; height=&quot;780&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;6. 첫 미션 실행 &amp;mdash; Manager View에서 미션 보내기&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;초기 설정을 마쳤으면 첫 미션을 실행할 차례입니다. 공식 Codelabs 튜토리얼이 추천하는 흐름은 다음과 같습니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;왼쪽 사이드바의 &lt;b&gt;Manager View 아이콘&lt;/b&gt; 클릭 &amp;rarr; Mission Control 화면이 열립니다&lt;/li&gt;
&lt;li&gt;상단 메뉴의 &lt;b&gt;File &amp;rarr; Open Folder&lt;/b&gt;로 작업할 로컬 프로젝트 폴더를 엽니다 &lpar;새 프로젝트면 빈 폴더 OK&rpar;&lt;/li&gt;
&lt;li&gt;Mission Control 상단 입력 필드에 미션 문장을 타이핑합니다&lt;/li&gt;
&lt;li&gt;첫 미션으로 튜토리얼이 권장하는 문장은 다음과 같습니다&lt;/li&gt;
&lt;/ol&gt;
&lt;pre class=&quot;applescript&quot;&gt;&lt;code&gt;Look at this project and tell me what it does.&lt;/code&gt;&lt;/pre&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; start=&quot;5&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;엔터를 누르면 에이전트가 프로젝트 전체를 스캔 &amp;rarr; 기술 로드맵 Artifact를 먼저 생성 &amp;rarr; 단계별로 실행 결과를 보여줍니다&lt;/li&gt;
&lt;/ol&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;이 첫 미션은 의도적으로 &quot;코드 수정이 없는 읽기 전용 탐색&quot;이라, Artifacts 시스템이 어떻게 로드맵을 만들고 보여주는지를 안전하게 관찰하기 좋습니다. 결과 화면에서 로드맵을 클릭하면 에이전트가 무엇을 단계별로 확인했는지 트리 형태로 확인할 수 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;7. 멀티 에이전트 활용 &amp;mdash; 5개 에이전트 병렬 실행&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Manager View의 진짜 가치는 에이전트를 여러 개 띄울 때 드러납니다. 예컨대 서로 다른 이슈 5건을 처리해야 하는 상황이라면 다음처럼 쓸 수 있습니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;Manager View 상단의 &lt;b&gt;New Agent&lt;/b&gt; 버튼을 5번 눌러 에이전트 5개를 만듭니다&lt;/li&gt;
&lt;li&gt;각 에이전트에 서로 다른 미션을 줍니다 &lpar;예: 버그 #101 재현&amp;middot;수정, 문서 오타 정리, README 업데이트, 로그 포맷 통일, 의존성 마이너 업그레이드&rpar;&lt;/li&gt;
&lt;li&gt;에이전트들이 각자 로드맵을 만들고 동시에 진행합니다&lt;/li&gt;
&lt;li&gt;Mission Control 대시보드에서 진행률&amp;middot;변경 파일&amp;middot;완료 여부를 한 보드에서 확인합니다&lt;/li&gt;
&lt;/ol&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;팀에서 500건+ 코드 리뷰를 해오면서 본 패턴 중에, 작은 변경 다수를 병렬로 굴리는 시나리오가 실제로 제일 잘 맞습니다. 하나의 큰 기능을 에이전트 하나한테 맡기면 아직은 중간 이탈이 적지 않게 보이는데, 작게 쪼갠 미션 여러 개를 병렬로 돌리는 방식이 퍼블릭 프리뷰 단계에서 가장 안정적으로 쓰입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;단, 에이전트 5개를 동시에 굴리면 rate limit 체감이 훨씬 빨라집니다. 모든 에이전트를 기본값인 Gemini 3 Pro로 두면 할당량이 빠르게 소모되니, 단순 작업은 다음 섹션에서 다루는 모델 교체를 병행하는 편이 낫습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;8. 모델 선택 전략 &amp;mdash; Gemini 3 Pro / Flash / Claude Opus / Sonnet&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;같은 도구 안에서 네 가지 모델을 골라 쓸 수 있다는 점이 Antigravity의 실용 포인트 중 하나입니다. 각 모델의 성격과 추천 용도를 공식 설명 기준으로 정리합니다.&lt;/p&gt;
&lt;table border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;8&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;모델&lt;/th&gt;
&lt;th&gt;성격&lt;/th&gt;
&lt;th&gt;어울리는 미션&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;Gemini 3 Pro&lt;/td&gt;
&lt;td&gt;기본&amp;middot;균형형, Antigravity 기본 모델&lt;/td&gt;
&lt;td&gt;일반 코딩&amp;middot;기획&amp;middot;리팩토링&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Gemini 3 Flash&lt;/td&gt;
&lt;td&gt;응답 속도 우선, 경량&lt;/td&gt;
&lt;td&gt;대량 파일 스캔, 단순 수정, 문서 생성&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Claude Opus&lt;/td&gt;
&lt;td&gt;복잡한 추론&amp;middot;긴 문맥&amp;middot;디버깅 강점&lt;/td&gt;
&lt;td&gt;큰 기능 설계, 아키텍처 결정, 까다로운 버그&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;Claude Sonnet&lt;/td&gt;
&lt;td&gt;Opus 대비 빠르고 가벼움, 범용&lt;/td&gt;
&lt;td&gt;일반 구현 작업, 코드 리뷰 보조&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;에이전트별로 모델을 섞을 수 있다는 점이 핵심입니다. 예를 들어 버그 5개를 병렬 처리할 때, 단순 오타나 의존성 업그레이드는 &lt;b&gt;Gemini 3 Flash&lt;/b&gt;에 맡기고, 재현 조건이 복잡한 버그 한 건만 &lt;b&gt;Claude Opus&lt;/b&gt;로 돌리는 식의 운용이 가능합니다. 정답은 없습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;반복 작업이 많으면 Flash&amp;middot;Sonnet 쪽, 설계&amp;middot;추론 비중이 크면 Pro&amp;middot;Opus 쪽으로 무게중심을 옮기는 감각 정도로 충분합니다.&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/cbjfbj/dJMcaiC2pPH/UkXjVCGfc9JykQX7QtuD2K/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/cbjfbj/dJMcaiC2pPH/UkXjVCGfc9JykQX7QtuD2K/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/cbjfbj/dJMcaiC2pPH/UkXjVCGfc9JykQX7QtuD2K/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fcbjfbj%2FdJMcaiC2pPH%2FUkXjVCGfc9JykQX7QtuD2K%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;9. 퍼블릭 프리뷰 주의사항과 마무리&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Google Antigravity 사용법 전체를 정리했지만, 현재가 퍼블릭 프리뷰 단계라는 점에서 운용상 몇 가지 주의점이 있습니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;프로덕션 금물&lt;/b&gt;: 할당량&amp;middot;가용성 보장이 없는 프리뷰 단계입니다. 회사 중요 리포지토리나 실제 고객 데이터에 직접 붙이는 용도는 피하는 게 낫습니다&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Auto 실행 범위 체크&lt;/b&gt;: 초기 설정에서 Terminal execution을 Auto로 뒀다면 어떤 명령이 자동 실행됐는지 Mission Control 로그에서 주기적으로 확인할 필요가 있습니다&lt;/li&gt;
&lt;li&gt;&lt;b&gt;Git 병행 권장&lt;/b&gt;: 에이전트가 여러 파일을 동시에 건드리기 때문에, 별도 브랜치에서 작업하고 자주 커밋&amp;middot;푸시하는 흐름을 유지해야 변경 추적이 안전합니다&lt;/li&gt;
&lt;li&gt;&lt;b&gt;할당량 관리&lt;/b&gt;: Gemini 3 Pro 기본값으로 멀티 에이전트를 돌리면 rate limit 체감이 빠릅니다. 단순 작업은 Flash&amp;middot;Sonnet 쪽으로 분산시키는 편이 낫습니다&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;정리하면 Google Antigravity 사용법의 뼈대는 &quot;Agent Manager로 들어가 &amp;rarr; Manager View에서 에이전트를 만들고 &amp;rarr; Workspace를 열고 &amp;rarr; 미션을 타이핑하면 &amp;rarr; Artifacts로 로드맵이 먼저 나오고 &amp;rarr; 구현이 이어진다&quot; 입니다. 오늘은 Google Antigravity 사용법의 다운로드&amp;middot;설치&amp;middot;초기 설정&amp;middot;첫 미션&amp;middot;멀티 에이전트&amp;middot;모델 선택까지 핵심 동선만 정리했습니다. 동일 환경이면 위 단계 그대로 따라가도 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;자주 묻는 질문&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Google Antigravity는 유료인가요?&lt;/b&gt;&lt;br /&gt;A. 2026년 4월 기준 퍼블릭 프리뷰 단계이며 Google 계정만 있으면 무료로 사용할 수 있습니다. Gemini 3 Pro에 대한 관대한&lpar;generous&rpar; rate limit이 포함된다고 공식 발표에 명시돼 있습니다. 단, 프리뷰 특성상 할당량&amp;middot;가용성이 보장되지는 않으며, 추후 유료화 또는 요금제 분리 가능성은 열려 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Windows 10에서도 돌아가나요?&lt;/b&gt;&lt;br /&gt;A. 네, 공식 다운로드 페이지에 Windows 10 이상&lpar;64-bit&rpar;이 요구사항으로 명시돼 있습니다. macOS는 Monterey 12 이상, Linux는 64-bit에 glibc 2.28+, glibcxx 3.4.25+ 가 충족되면 됩니다. Linux에서 실행되지 않는 경우 대부분 glibc 버전 미달이 원인입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Agent Manager와 Manager View는 같은 건가요?&lt;/b&gt;&lt;br /&gt;A. 다릅니다. Agent Manager는 앱을 켜면 처음 뜨는 대시보드 화면 자체를 말합니다. Manager View는 왼쪽 사이드바 아이콘으로 열리는 Mission Control 화면으로, 여러 에이전트를 생성&amp;middot;모니터링하는 작업 보드 역할을 합니다. 에이전트 여러 개를 병렬로 굴리려면 Manager View에서 New Agent 버튼으로 하나씩 만들어 미션을 배정하면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 첫 미션으로 뭘 돌려보는 게 좋나요?&lt;/b&gt;&lt;br /&gt;A. 공식 Codelabs 튜토리얼은 &lt;code&gt;Look at this project and tell me what it does.&lt;/code&gt; 를 추천합니다. 코드 수정이 없는 읽기 전용 탐색이라 안전하게 Artifacts 시스템이 로드맵을 어떻게 만들고 보여주는지 관찰하기 좋습니다. File &amp;rarr; Open Folder로 아무 로컬 프로젝트를 연 뒤 Mission Control 입력 필드에 이 문장을 그대로 타이핑하면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Gemini 3 Pro 말고 Claude도 쓸 수 있나요?&lt;/b&gt;&lt;br /&gt;A. 가능합니다. Antigravity 안에서 Gemini 3 Pro / Gemini 3 Flash / Claude Opus / Claude Sonnet 네 개 모델을 모두 선택할 수 있고, 같은 미션 안에서도 에이전트마다 다른 모델을 붙일 수 있습니다. 단순 작업은 Gemini 3 Flash, 복잡한 설계&amp;middot;디버깅은 Claude Opus에 맡기는 식의 조합 운용이 가능합니다.&lt;/p&gt;
&lt;hr data-ke-style=&quot;style1&quot; /&gt;
&lt;div class=&quot;related-posts&quot; style=&quot;border: 1px solid #e7e5dd; border-radius: 8px; padding: 16px; margin: 24px 0; background: #faf9f5;&quot;&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;  이 카테고리의 다른 글&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/556&quot;&gt;Gemini CLI 사용법 &amp;mdash; 무료로 어디까지 되나, 직접 써보고 정리&lt;/a&gt; &amp;mdash; 2026-04-19&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/553&quot;&gt;Claude Code 창시자와 해커톤 우승자의 공통 꿀팁 7가지&lt;/a&gt; &amp;mdash; 2026-04-05&lt;/li&gt;
&lt;li&gt;&lt;a href=&quot;https://hgko-dev.tistory.com/551&quot;&gt;[설치 가이드] Claude Code에 프로급 디자인 스킬 세팅하기: Impeccable 완벽 가이드&lt;/a&gt; &amp;mdash; 2026-04-02&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;i&gt;같은 &lt;b&gt;AI 활용법&lt;/b&gt; 카테고리에서 이어서 읽기&lt;/i&gt;&lt;/p&gt;
&lt;/div&gt;
&lt;hr data-ke-style=&quot;style1&quot; /&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;설치 환경: Windows 11, Google Antigravity 퍼블릭 프리뷰 &lpar;2026-04 기준&rpar;, Google 계정 로그인, Gemini 3 Pro 기본 모델&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;script type=&quot;application/ld+json&quot;&gt;
{
  &quot;@context&quot;: &quot;https://schema.org&quot;,
  &quot;@type&quot;: &quot;FAQPage&quot;,
  &quot;mainEntity&quot;: [
    {
      &quot;@type&quot;: &quot;Question&quot;,
      &quot;name&quot;: &quot;Google Antigravity는 유료인가요?&quot;,
      &quot;acceptedAnswer&quot;: {
        &quot;@type&quot;: &quot;Answer&quot;,
        &quot;text&quot;: &quot;2026년 4월 기준 퍼블릭 프리뷰 단계이며 Google 계정만 있으면 무료로 사용할 수 있습니다. Gemini 3 Pro에 대한 관대한&lpar;generous&rpar; rate limit이 포함된다고 공식 발표에 명시돼 있습니다. 단, 프리뷰 특성상 할당량·가용성이 보장되지는 않으며, 추후 유료화 또는 요금제 분리 가능성은 열려 있습니다.&quot;
      }
    },
    {
      &quot;@type&quot;: &quot;Question&quot;,
      &quot;name&quot;: &quot;Windows 10에서도 돌아가나요?&quot;,
      &quot;acceptedAnswer&quot;: {
        &quot;@type&quot;: &quot;Answer&quot;,
        &quot;text&quot;: &quot;네, 공식 다운로드 페이지에 Windows 10 이상&lpar;64-bit&rpar;이 요구사항으로 명시돼 있습니다. macOS는 Monterey 12 이상, Linux는 64-bit에 glibc 2.28+, glibcxx 3.4.25+ 가 충족되면 됩니다. Linux에서 실행되지 않는 경우 대부분 glibc 버전 미달이 원인입니다.&quot;
      }
    },
    {
      &quot;@type&quot;: &quot;Question&quot;,
      &quot;name&quot;: &quot;Agent Manager와 Manager View는 같은 건가요?&quot;,
      &quot;acceptedAnswer&quot;: {
        &quot;@type&quot;: &quot;Answer&quot;,
        &quot;text&quot;: &quot;다릅니다. Agent Manager는 앱을 켜면 처음 뜨는 대시보드 화면 자체를 말합니다. Manager View는 왼쪽 사이드바 아이콘으로 열리는 Mission Control 화면으로, 여러 에이전트를 생성·모니터링하는 작업 보드 역할을 합니다. 에이전트 여러 개를 병렬로 굴리려면 Manager View에서 New Agent 버튼으로 하나씩 만들어 미션을 배정하면 됩니다.&quot;
      }
    },
    {
      &quot;@type&quot;: &quot;Question&quot;,
      &quot;name&quot;: &quot;첫 미션으로 뭘 돌려보는 게 좋나요?&quot;,
      &quot;acceptedAnswer&quot;: {
        &quot;@type&quot;: &quot;Answer&quot;,
        &quot;text&quot;: &quot;공식 Codelabs 튜토리얼은 &#39;Look at this project and tell me what it does.&#39; 를 추천합니다. 코드 수정이 없는 읽기 전용 탐색이라 안전하게 Artifacts 시스템이 로드맵을 어떻게 만들고 보여주는지 관찰하기 좋습니다. File → Open Folder로 아무 로컬 프로젝트를 연 뒤 Mission Control 입력 필드에 이 문장을 그대로 타이핑하면 됩니다.&quot;
      }
    },
    {
      &quot;@type&quot;: &quot;Question&quot;,
      &quot;name&quot;: &quot;Gemini 3 Pro 말고 Claude도 쓸 수 있나요?&quot;,
      &quot;acceptedAnswer&quot;: {
        &quot;@type&quot;: &quot;Answer&quot;,
        &quot;text&quot;: &quot;가능합니다. Antigravity 안에서 Gemini 3 Pro / Gemini 3 Flash / Claude Opus / Claude Sonnet 네 개 모델을 모두 선택할 수 있고, 같은 미션 안에서도 에이전트마다 다른 모델을 붙일 수 있습니다. 단순 작업은 Gemini 3 Flash, 복잡한 설계·디버깅은 Claude Opus에 맡기는 식의 조합 운용이 가능합니다.&quot;
      }
    }
  ]
}
&lt;/script&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;</sub>- [Gemini CLI 사용법 &amp;mdash; 무료로 어디까지 되나, 직접 써보고 정리](https://hgko-dev.tistory.com/556) <sub>— 
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/rxigy/dJMcaf0z20e/QimJCIyw3jpOue49A6QqKK/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/rxigy/dJMcaf0z20e/QimJCIyw3jpOue49A6QqKK/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/rxigy/dJMcaf0z20e/QimJCIyw3jpOue49A6QqKK/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Frxigy%2FdJMcaf0z20e%2FQimJCIyw3jpOue49A6QqKK%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;AI 코딩 도구가 늘면서 Gemini CLI를 한번 깔아만 두고 방치하는 경우가 많습니다. &quot;무료라고 하니 일단 받아두자&quot;로 그치면, 정작 필요한 순간에 인증에서 막히거나 무료 할당량을 엉뚱한 데 소진합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;저는 Claude Max와 Gemini Pro 플랜을 함께 쓰면서 두 CLI를 병행 운용 중이고, 15년 개발하면서 CLI 도구 여럿을 갈아타 본 경험으로 Gemini CLI 사용법을 Windows 환경 기준으로 정리합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;이 글을 끝까지 읽으면 &lt;b&gt;설치 &amp;rarr; 인증 &amp;rarr; 첫 프롬프트 실행까지 약 5분&lt;/b&gt;, 무료 티어로 어디까지 가능한지, Claude Code와의 실무 차이 3가지, 그리고 처음 쓰는 사람들이 자주 만나는 트러블 포인트 한 개를 건져갈 수 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;1. Gemini CLI가 뭔지부터&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini CLI는 구글이 공개한 오픈소스 터미널용 AI 에이전트입니다. &lt;code&gt;google-gemini/gemini-cli&lt;/code&gt; GitHub 저장소에서 소스를 공개하며, Apache 2.0 라이선스입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;&quot;터미널에서 파일을 읽고/고치고/명령을 실행하는&quot; 에이전틱 CLI 카테고리에 속하고, 내부 모델만 Gemini 계열&lpar;2.5 Pro / Flash 등&rpar;로 바뀐다고 이해하면 시작점으로는 충분합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Code도 같이 써본 입장에서 Gemini CLI를 처음 깔 때 가장 먼저 체감하는 차이 3가지입니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;무료 티어가 명시적으로 존재. 개인 구글 계정 로그인만으로 일정 요청까지 과금 없이 쓸 수 있다.&lt;/li&gt;
&lt;li&gt;&lt;code&gt;.gemini/&lt;/code&gt; 디렉터리 기반 설정. &lt;code&gt;.claude/&lt;/code&gt;처럼 프로젝트 루트에 자체 설정을 둔다.&lt;/li&gt;
&lt;li&gt;MCP&lpar;Model Context Protocol&rpar;를 공식 지원. 같은 MCP 서버를 Claude Code와 공유해서 사용 가능합니다.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;2. 설치 &amp;mdash; Windows 11 + Node.js v24 기준&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;사전 준비물은 단 하나, 최신 Node.js입니다. 공식 저장소는 Node 20 이상을 요구하며, 저는 Node v24로 검증했습니다.&lt;/p&gt;
&lt;pre class=&quot;crmsh&quot;&gt;&lt;code&gt;node --version
# v24.x.x 이상이면 OK&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;설치 명령은 한 줄입니다.&lt;/p&gt;
&lt;pre class=&quot;css&quot;&gt;&lt;code&gt;npm install -g @google/gemini-cli&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;설치가 끝나면 아무 디렉터리에서 &lt;code&gt;gemini&lt;/code&gt; 실행 파일이 인식되는지 확인합니다.&lt;/p&gt;
&lt;pre class=&quot;ada&quot;&gt;&lt;code&gt;gemini --version&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;버전 번호가 출력되면 성공입니다. 저는 &lt;code&gt;0.x&lt;/code&gt; 대 버전에서 작업했고, 빠르게 바뀌는 도구라 본인이 설치한 시점의 버전을 README에 같이 적어두는 습관을 추천합니다. 팀원이 &quot;안 된다&quot;고 물을 때 버전 차이로 원인을 빠르게 좁힐 수 있습니다.&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/cXT8Ql/dJMcaduS5Jz/Pb47xZ3R1h5bl6TXvWe1ck/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/cXT8Ql/dJMcaduS5Jz/Pb47xZ3R1h5bl6TXvWe1ck/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/cXT8Ql/dJMcaduS5Jz/Pb47xZ3R1h5bl6TXvWe1ck/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FcXT8Ql%2FdJMcaduS5Jz%2FPb47xZ3R1h5bl6TXvWe1ck%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;3. 인증 &amp;mdash; 무료 티어로 시작하는 Gemini CLI 사용법&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini CLI 사용법에서 가장 중요한 선택 지점이 인증 방식입니다. 선택지는 두 가지입니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;개인 구글 계정 로그인 &lpar;무료 할당 포함&rpar;&lt;/li&gt;
&lt;li&gt;API 키 직접 발급 &lpar;Google AI Studio 또는 Vertex AI&rpar;&lt;/li&gt;
&lt;/ol&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;처음이라면 1번을 권장합니다. 프로젝트 루트에서 그냥 &lt;code&gt;gemini&lt;/code&gt;를 치면 브라우저로 OAuth 로그인 창이 뜨고, 로그인을 마치면 터미널 프롬프트로 돌아옵니다.&lt;/p&gt;
&lt;pre class=&quot;applescript&quot;&gt;&lt;code&gt;cd my-project
gemini&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;API 키를 쓰는 경우 환경 변수로 주입합니다. PowerShell 기준은 아래와 같습니다.&lt;/p&gt;
&lt;pre class=&quot;elixir&quot;&gt;&lt;code&gt;$env:GEMINI_API_KEY=&quot;여기에_발급받은_키&quot;
gemini&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;팀 공용 PC라든가 여러 프로젝트에서 서로 다른 계정을 써야 한다면 API 키 방식이 편합니다. 개인 학습&amp;middot;사이드 프로젝트라면 무료 로그인이 마찰이 훨씬 적습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;4. 첫 세션 &amp;mdash; 자주 쓰는 명령 5개&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;인증이 끝나면 대화형 프롬프트가 뜹니다. 이 상태에서 자연어로 지시하면 되고, 슬래시 커맨드로 세션을 제어합니다.&lt;/p&gt;
&lt;table border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;6&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;명령&lt;/th&gt;
&lt;th&gt;역할&lt;/th&gt;
&lt;th&gt;자주 쓰는 상황&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;&lt;code&gt;/help&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;사용 가능한 슬래시 커맨드 목록&lt;/td&gt;
&lt;td&gt;세션 처음 켰을 때&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;&lt;code&gt;/tools&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;현재 활성화된 도구/MCP 확인&lt;/td&gt;
&lt;td&gt;파일 접근이 안 될 때 원인 점검&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;&lt;code&gt;/memory&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;컨텍스트 메모리 관리&lt;/td&gt;
&lt;td&gt;장시간 작업 중 누적 정리&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;&lt;code&gt;/chat save &amp;lt;이름&amp;gt;&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;현재 대화 스냅샷 저장&lt;/td&gt;
&lt;td&gt;작업 중단 전&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;&lt;code&gt;/quit&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;세션 종료&lt;/td&gt;
&lt;td&gt;안전한 정리 종료&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;프롬프트 예시는 딱 Claude Code랑 동일한 감각으로 갑니다.&lt;/p&gt;
&lt;pre class=&quot;reasonml&quot;&gt;&lt;code&gt;&amp;gt; 이 저장소의 README.md 기반으로 CONTRIBUTING.md 초안을 만들어줘.
  커밋 메시지 규칙 섹션은 Conventional Commits로.&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;내부적으로 파일을 읽고 diff를 만들어 제안합니다. 실행 전 확인 단계가 있으니 그 때 검토 후 승인하면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/co1Epk/dJMcabYeY0a/i9jy4tW0zCH27Soe04GOl0/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/co1Epk/dJMcabYeY0a/i9jy4tW0zCH27Soe04GOl0/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/co1Epk/dJMcabYeY0a/i9jy4tW0zCH27Soe04GOl0/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Fco1Epk%2FdJMcabYeY0a%2Fi9jy4tW0zCH27Soe04GOl0%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1376&quot; height=&quot;768&quot; data-origin-width=&quot;1376&quot; data-origin-height=&quot;768&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;5. 트러블슈팅 &amp;mdash; Windows에서 인증 루프에 빠지는 경우&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini CLI 공식 이슈 트래커와 개발 커뮤니티에 자주 올라오는 패턴 중 하나입니다. Windows + 사내 네트워크 조합에서 가장 빈번하게 보고됩니다.&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;증상&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;code&gt;gemini&lt;/code&gt; 첫 실행 후 브라우저 OAuth 창이 떠서 로그인은 완료되는데, 터미널로 돌아오면 다시 로그인 URL만 반복 출력됩니다. 세션이 붙질 않습니다.&lt;/p&gt;
&lt;pre class=&quot;livecodeserver&quot;&gt;&lt;code&gt;Please open the following URL in your browser to log in:
https://accounts.google.com/o/oauth2/...&lt;/code&gt;&lt;/pre&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;원인&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;OAuth 콜백이 로컬 루프백 포트로 들어오는데, Windows Defender 방화벽이나 사내 VPN이 해당 포트를 차단하는 경우가 있습니다. 로그인은 끝났지만 CLI가 응답 토큰을 받지 못해 타임아웃 되는 구조입니다.&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;해결&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;두 가지 중 하나로 우회합니다. 사내 네트워크처럼 방화벽 정책을 바꿀 수 없는 환경이면 2번이 더 빠릅니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;방화벽에서 Node.js 실행 파일 예외 허용 후 재시도.&lt;/li&gt;
&lt;li&gt;Google AI Studio에서 API 키를 직접 발급해 &lt;code&gt;GEMINI_API_KEY&lt;/code&gt; 환경 변수로 주입. 이 방식은 OAuth 콜백 자체를 쓰지 않습니다.&lt;/li&gt;
&lt;/ol&gt;
&lt;pre class=&quot;elixir&quot;&gt;&lt;code&gt;[System.Environment]::SetEnvironmentVariable&lpar;&quot;GEMINI_API_KEY&quot;,&quot;&amp;lt;키&amp;gt;&quot;,&quot;User&quot;&rpar;
# 새 터미널 열고 다시 gemini 실행&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;6. 무료 티어를 가장 빠르게 소진시키는 패턴&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini CLI를 처음 쓰는 사람들이 가장 많이 빠지는 함정 중 하나가 &quot;한 세션에 큰 컨텍스트를 몽땅 밀어 넣고 계속 끌고 가는&quot; 사용법입니다. 토이 프로젝트 리팩토링이나 대규모 코드베이스 탐색을 할 때 특히 자주 발생합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;증상은 간단합니다. 세션이 길어질수록 같은 파일을 여러 번 다시 읽는 비효율이 쌓이고, 체감상 응답 속도가 느려지면서 무료 할당량이 빠르게 줄어듭니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;원인은 &lt;code&gt;/memory&lt;/code&gt;와 &lt;code&gt;/chat save&lt;/code&gt;를 거의 안 쓰고 한 세션을 계속 끌고 가는 데 있습니다. 세션 컨텍스트가 커질수록 토큰 소모가 누적되기 때문입니다. 해결은 단순합니다. 큰 작업 단위마다 &lt;code&gt;/chat save&lt;/code&gt;로 스냅샷을 찍고, 새로운 맥락은 새 세션을 시작하는 습관 하나면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;팀에서 500건+ 코드 리뷰하면서 본 패턴도 같습니다. CLI든 IDE든 &quot;컨텍스트를 작게 끊어 쓰는 사람&quot;이 결국 가장 오래, 싸게 씁니다.&lt;/p&gt;
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/rBOWY/dJMcabDUsIc/dMCDnbXJ5mmnnEgtoTmli0/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/rBOWY/dJMcabDUsIc/dMCDnbXJ5mmnnEgtoTmli0/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/rBOWY/dJMcabDUsIc/dMCDnbXJ5mmnnEgtoTmli0/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FrBOWY%2FdJMcabDUsIc%2FdMCDnbXJ5mmnnEgtoTmli0%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;640&quot; height=&quot;640&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;1024&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;7. Claude Code vs Gemini CLI &amp;mdash; 실무 관점 트레이드오프&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;두 CLI를 같은 저장소에서 번갈아 쓰면서 느낀 지점들입니다. 단일 정답은 없고 프로젝트 성격에 따라 갈립니다.&lt;/p&gt;
&lt;table border=&quot;1&quot; cellspacing=&quot;0&quot; cellpadding=&quot;6&quot; data-ke-align=&quot;alignLeft&quot;&gt;
&lt;thead&gt;
&lt;tr&gt;
&lt;th&gt;항목&lt;/th&gt;
&lt;th&gt;Claude Code&lt;/th&gt;
&lt;th&gt;Gemini CLI&lt;/th&gt;
&lt;/tr&gt;
&lt;/thead&gt;
&lt;tbody&gt;
&lt;tr&gt;
&lt;td&gt;무료 사용&lt;/td&gt;
&lt;td&gt;별도 플랜 필요&lt;/td&gt;
&lt;td&gt;개인 구글 로그인 무료 티어 존재&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;설정 디렉터리&lt;/td&gt;
&lt;td&gt;&lt;code&gt;.claude/&lt;/code&gt;&lt;/td&gt;
&lt;td&gt;&lt;code&gt;.gemini/&lt;/code&gt;&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;MCP 지원&lt;/td&gt;
&lt;td&gt;공식&lt;/td&gt;
&lt;td&gt;공식&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;강점 체감&lt;/td&gt;
&lt;td&gt;긴 리팩토링&amp;middot;리뷰 연속성&lt;/td&gt;
&lt;td&gt;빠른 탐색&amp;middot;문서화&amp;middot;요약&lt;/td&gt;
&lt;/tr&gt;
&lt;tr&gt;
&lt;td&gt;약점 체감&lt;/td&gt;
&lt;td&gt;유료 허들&lt;/td&gt;
&lt;td&gt;대규모 코드 변경 시 호흡이 다름&lt;/td&gt;
&lt;/tr&gt;
&lt;/tbody&gt;
&lt;/table&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;장점은 Gemini CLI의 무료 진입 장벽이 낮다는 점이고, 단점은 동일한 에이전틱 CLI라도 출력 스타일&amp;middot;툴 호출 패턴이 달라서 &quot;Claude Code처럼 쓰면 Claude Code만큼 나온다&quot;는 기대가 깨질 때가 있다는 점입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;br /&gt;팀 단위 도입을 고민 중이라면, 팀원 3명 미만이고 개인 학습 위주이면 Gemini CLI부터 깔아 보고, 팀이 5명을 넘고 동일 저장소에 여러 명이 동시에 에이전트를 붙이는 구조라면 두 CLI 모두 &lt;code&gt;.gitignore&lt;/code&gt; 규칙을 맞춰 병행 운용하는 쪽이 낫다고 판단합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;8. 팀 공유 설정 &amp;mdash; &lt;code&gt;.gemini/&lt;/code&gt; 규칙 잡기&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;저장소 루트에 &lt;code&gt;.gemini/&lt;/code&gt; 디렉터리를 두고, 팀 공용 프롬프트&amp;middot;MCP 설정을 Git에 커밋합니다. 개인 토큰&amp;middot;인증 캐시는 반드시 &lt;code&gt;.gitignore&lt;/code&gt;로 따로 빼주세요.&lt;/p&gt;
&lt;pre class=&quot;jboss-cli&quot;&gt;&lt;code&gt;# 개인 인증&amp;middot;캐시 &lpar;커밋 금지&rpar;
.gemini/oauth_creds.json
.gemini/.cache/

# 팀 공용 설정은 커밋
!.gemini/settings.json
!.gemini/GEMINI.md&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;code&gt;GEMINI.md&lt;/code&gt;에는 &quot;이 저장소에서 에이전트가 지켜야 할 규칙&quot;을 써둡니다. Claude Code의 &lt;code&gt;CLAUDE.md&lt;/code&gt;와 같은 역할이라 두 파일을 각각 두면 두 CLI를 같은 저장소에서 안전하게 병행할 수 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;9. 마무리 &amp;mdash; Gemini CLI 사용법, 언제 쓰면 좋은가&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;정답은 없습니다. 다음 기준으로 판단하면 선택이 쉬워집니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;개인 학습&amp;middot;사이드 프로젝트라서 과금 허들을 먼저 없애고 싶다 &amp;rarr; Gemini CLI&lt;/li&gt;
&lt;li&gt;이미 Claude Code 워크플로우&lpar;gstack 등&rpar;가 자리잡혔고 장시간 리팩토링이 주 업무다 &amp;rarr; Claude Code 유지&lt;/li&gt;
&lt;li&gt;두 가지 다 필요하다 &amp;rarr; 위 &lt;code&gt;.gitignore&lt;/code&gt; 규칙으로 병행&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Gemini CLI 사용법 자체는 단순합니다. 설치 &amp;rarr; 로그인 &amp;rarr; 프롬프트, 3단계면 됩니다. 중요한 건 세션을 작게 끊는 습관, 그리고 Claude Code와의 차이점을 머릿속에서 미리 구분해 두는 것입니다. 이 부분만 잡혀 있으면 같은 터미널에서 두 에이전트를 상황에 맞게 바꿔 쓰는 경험이 꽤 매끄러워집니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;블로그에 Claude&amp;middot;Gemini 등 다른 AI 도구 세팅 가이드도 같이 올려뒀으니, 에이전틱 CLI를 팀에 도입하는 흐름을 같이 보고 싶으면 &lt;code&gt;AI 활용법&lt;/code&gt; 카테고리 쪽도 한번 둘러봐 주세요.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;자주 묻는 질문&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Gemini CLI는 무료로 어디까지 쓸 수 있나요?&lt;/b&gt;&lt;br /&gt;A. 개인 구글 계정 OAuth 로그인만으로 일정 요청까지 무료 사용이 가능합니다. 정확한 일일 한도는 시점마다 변동되며, 무료 한도를 넘기면 응답이 느려지거나 큐에 들어가는 식으로 제한이 걸립니다. 본격적으로 쓰려면 Google AI Studio에서 API 키를 발급받아 &lt;code&gt;GEMINI_API_KEY&lt;/code&gt; 환경 변수로 주입하는 방식이 안정적입니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Claude Code와 Gemini CLI는 뭐가 다른가요?&lt;/b&gt;&lt;br /&gt;A. 둘 다 &quot;터미널에서 파일을 읽고 고치고 명령을 실행하는&quot; 에이전틱 CLI 카테고리에 속합니다. 가장 큰 차이는 무료 진입 장벽으로, Gemini CLI는 개인 구글 계정 무료 티어가 명시적으로 존재합니다. 반면 Claude Code는 긴 리팩토링&amp;middot;연속 코드 리뷰 호흡에서 강한 편이라는 후기가 많습니다. 두 도구는 같은 저장소에서 병행 사용이 가능합니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Windows에서 OAuth 인증 루프에 빠지면 어떻게 해결하나요?&lt;/b&gt;&lt;br /&gt;A. 사내 네트워크나 Windows Defender 방화벽이 OAuth 콜백 포트를 차단해서 발생하는 경우가 흔합니다. 두 가지 우회 방법이 있습니다. 첫째, 방화벽에서 Node.js 실행 파일 예외를 허용한 뒤 재시도. 둘째, Google AI Studio에서 API 키를 발급해 &lt;code&gt;GEMINI_API_KEY&lt;/code&gt; 환경 변수로 주입하면 OAuth 콜백 자체를 쓰지 않습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. Gemini CLI 설치 전에 어떤 준비물이 필요한가요?&lt;/b&gt;&lt;br /&gt;A. 최신 Node.js만 있으면 됩니다. 공식 저장소는 Node 20 이상을 요구하며, Node v24에서 동작이 검증되어 있습니다. 설치 명령은 &lt;code&gt;npm install -g @google/gemini-cli&lt;/code&gt; 한 줄이고, 설치 후 &lt;code&gt;gemini --version&lt;/code&gt;으로 확인하면 됩니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;Q. 무료 티어 할당량을 빠르게 소진시키지 않으려면?&lt;/b&gt;&lt;br /&gt;A. 한 세션에 큰 컨텍스트를 몽땅 밀어 넣고 계속 끌고 가지 마세요. 큰 작업 단위마다 &lt;code&gt;/chat save&lt;/code&gt;로 스냅샷을 찍고, 새로운 맥락은 새 세션을 시작하는 습관 하나면 토큰 누적을 크게 줄일 수 있습니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;
&lt;script type=&quot;application/ld+json&quot;&gt;
{
  &quot;@context&quot;: &quot;https://schema.org&quot;,
  &quot;@type&quot;: &quot;FAQPage&quot;,
  &quot;mainEntity&quot;: [
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Gemini CLI는 무료로 어디까지 쓸 수 있나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;개인 구글 계정 OAuth 로그인만으로 일정 요청까지 무료 사용이 가능합니다. 무료 한도를 넘기면 응답이 느려지거나 큐에 들어갑니다. 본격적으로 쓰려면 Google AI Studio에서 API 키를 발급받아 GEMINI_API_KEY 환경 변수로 주입하는 방식이 안정적입니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Claude Code와 Gemini CLI는 뭐가 다른가요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;둘 다 에이전틱 CLI 카테고리지만 Gemini CLI는 개인 구글 계정 무료 티어가 명시적으로 존재합니다. Claude Code는 긴 리팩토링·연속 코드 리뷰 호흡에서 강한 편이라는 후기가 많습니다. 두 도구는 같은 저장소에서 병행 사용이 가능합니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Windows에서 OAuth 인증 루프에 빠지면 어떻게 해결하나요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;사내 네트워크나 Windows Defender 방화벽이 콜백 포트를 차단해서 발생합니다. 방화벽에서 Node.js 실행 파일 예외를 허용하거나, Google AI Studio에서 API 키를 발급해 환경 변수로 주입하면 OAuth 콜백을 쓰지 않습니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;Gemini CLI 설치 전에 어떤 준비물이 필요한가요?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;최신 Node.js만 있으면 됩니다. 공식 저장소는 Node 20 이상을 요구하며 Node v24에서 동작이 검증되어 있습니다. 설치 명령은 npm install -g @google/gemini-cli 한 줄입니다.&quot;}},
    {&quot;@type&quot;:&quot;Question&quot;,&quot;name&quot;:&quot;무료 티어 할당량을 빠르게 소진시키지 않으려면?&quot;,&quot;acceptedAnswer&quot;:{&quot;@type&quot;:&quot;Answer&quot;,&quot;text&quot;:&quot;한 세션에 큰 컨텍스트를 몽땅 밀어 넣고 계속 끌고 가지 마세요. 큰 작업 단위마다 /chat save로 스냅샷을 찍고 새로운 맥락은 새 세션을 시작하는 습관 하나면 토큰 누적을 크게 줄일 수 있습니다.&quot;}}
  ]
}
&lt;/script&gt;
&lt;/p&gt;
&lt;hr data-ke-style=&quot;style1&quot; /&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;설치 환경: Windows 11, Node.js v24, Gemini CLI 0.x&lt;/b&gt;&lt;/p&gt;</sub>- [[UI/UX 가이드] AI가 만든 &#39;싼티&#39; 나는 UI 피하는 법: Impeccable 디자인 원칙 &amp;amp; 안티패턴 총정리](https://hgko-dev.tistory.com/555) <sub>— 
&lt;p&gt;&lt;figure class=&quot;imageblock alignCenter&quot; data-ke-mobileStyle=&quot;widthOrigin&quot; data-filename=&quot;다운로드.jpg&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;572&quot;&gt;&lt;span data-url=&quot;https://blog.kakaocdn.net/dn/bP0DFt/dJMb99TBKcI/pfkEMfPJBptlSoK1qlDiw1/img.jpg&quot; data-phocus=&quot;https://blog.kakaocdn.net/dn/bP0DFt/dJMb99TBKcI/pfkEMfPJBptlSoK1qlDiw1/img.jpg&quot;&gt;&lt;img src=&quot;https://blog.kakaocdn.net/dn/bP0DFt/dJMb99TBKcI/pfkEMfPJBptlSoK1qlDiw1/img.jpg&quot; srcset=&quot;https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&amp;fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2FbP0DFt%2FdJMb99TBKcI%2FpfkEMfPJBptlSoK1qlDiw1%2Fimg.jpg&quot; onerror=&quot;this.onerror=null; this.src=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;; this.srcset=&#39;//t1.daumcdn.net/tistory_admin/static/images/no-image-v1.png&#39;;&quot; loading=&quot;lazy&quot; width=&quot;1024&quot; height=&quot;572&quot; data-filename=&quot;다운로드.jpg&quot; data-origin-width=&quot;1024&quot; data-origin-height=&quot;572&quot;/&gt;&lt;/span&gt;&lt;/figure&gt;
&lt;/p&gt;
&lt;p data-pm-slice=&quot;1 1 []&quot; data-ke-size=&quot;size16&quot;&gt;최근 AI 코딩 도구로 프론트엔드를 짜다 보면 꼭 마주치는 절망적인 순간이 있습니다. 폰트는 무조건 Inter, 다크모드만 켜면 번쩍거리는 네온 글로우, 카드 안에 카드가 끝없이 들어가는 중첩 지옥... 이른바 &lt;b&gt;&#39;AI Slop&lpar;AI가 만든 뻔하고 촌스러운 결과물&rpar;&#39;&lt;/b&gt; 현상입니다.&lt;/p&gt;
&lt;p data-pm-slice=&quot;1 1 []&quot; data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;Claude Code 전용 디자인 스킬인 &lt;b&gt;Impeccable&lpar;임페커블&rpar;&lt;/b&gt;은 AI에게 &#39;프로 디자이너의 감각&#39;을 주입하여 이 문제를 해결합니다. 오늘 포스팅에서는 Impeccable이 핵심으로 삼고 있는 &lt;b&gt;7가지 절대 디자인 원칙&lt;/b&gt;과 우리가 무의식적으로 저지르는 &lt;b&gt;AI Slop 안티패턴&lt;/b&gt;을 총정리해 드립니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;개발자라면 이 가이드만 정독해도 프론트엔드 결과물의 퀄리티가 200% 달라질 것입니다!&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;  Part 1. 프로 디자이너의 7가지 절대 원칙&lt;/h2&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;1. Typography &lpar;타이포그래피&rpar;: 글꼴이 UI의 8할이다&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;타이포그래피는 UI의 가독성과 시각적 위계를 결정하는 가장 중요한 요소입니다. 임의로 폰트 크기를 찍어 맞추지 마세요.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  모듈러 스케일:&lt;/b&gt; 1.25배, 1.333배 등 일정한 수학적 비율로 폰트 크기 체계를 만드세요.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  유동적 사이징&lpar;Fluid Sizing&rpar;:&lt;/b&gt; 브레이크포인트마다 폰트 크기를 하드코딩하는 대신, clamp&lpar;&rpar; 함수를 써서 화면 크기에 따라 물 흐르듯 자연스럽게 커지고 작아지게 만드세요.&lt;/li&gt;
&lt;/ul&gt;
&lt;pre class=&quot;angelscript&quot;&gt;&lt;code&gt;/*   뷰포트에 따라 부드럽게 변하는 유동적 타이포그래피 예시 */
font-size: clamp&lpar;1rem, 0.5rem + 1.5vw, 1.5rem&rpar;;
line-height: clamp&lpar;1.4, 1.2 + 0.5vw, 1.6&rpar;;
&lt;/code&gt;&lt;/pre&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;2. Color &amp;amp; Contrast &lpar;색상과 대비&rpar;: 순수 블랙/화이트는 그만&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;브랜드 아이덴티티와 접근성&lpar;A11y&rpar;을 동시에 잡는 세련된 컬러 시스템의 비밀입니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  OKLCH 색상 공간:&lt;/b&gt; 기존 RGB 대신 OKLCH를 사용해 보세요. 명도와 채도 조절이 인간의 눈에 훨씬 자연스럽고 직관적입니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt; ️ 틴티드 뉴트럴&lpar;Tinted Neutrals&rpar;:&lt;/b&gt; 칙칙한 순수 회색 대신, &lt;b&gt;브랜드 컬러가 한 방울 섞인 회색&lt;/b&gt;을 쓰면 UI가 훨씬 고급스러워집니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  올바른 다크모드:&lt;/b&gt; 단순히 색을 반전시키는 게 아닙니다! 배경은 순수 검정&lpar;#000&rpar;이 아닌 매우 어두운 회색을 쓰고, 브랜드 컬러의 채도를 살짝 낮춰 눈의 피로를 덜어주세요.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;3. Spatial Design &lpar;공간 디자인&rpar;: 여백이 질서를 만든다&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;요소들 사이의 일관된 간격은 UI에 편안한 리듬감을 부여합니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  4px / 8px 시스템:&lt;/b&gt; 모든 여백, 패딩, 갭&lpar;Gap&rpar;은 4의 배수로 설정하세요 &lpar;4, 8, 12, 16, 24, 32...&rpar;. 이 규칙만 지켜도 화면이 깔끔해집니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  컨테이너 쿼리&lpar;Container Queries&rpar;:&lt;/b&gt; 뷰포트&lpar;화면 전체 크기&rpar; 기준이 아닌, &#39;컴포넌트가 담긴 박스&#39; 크기를 기준으로 반응형을 짜면 재사용성이 극대화됩니다.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;4. Motion Design &lpar;모션 디자인&rpar;: 과유불급의 미학&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;애니메이션은 &#39;멋&#39;이 아니라 &#39;상태 변화의 전달&#39;을 위해 존재합니다.&lt;/p&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  맞춤형 이징&lpar;Easing&rpar;:&lt;/b&gt; 딱딱한 linear는 버리세요. 나타날 땐 ease-out, 사라질 땐 ease-in이 진리입니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  성능 제1원칙:&lt;/b&gt; 애니메이션은 오직 transform과 opacity에만 적용하세요. width나 margin을 움직이면 브라우저가 버벅거립니다&lpar;레이아웃 리플로우&rpar;.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;5. Interaction Design &lpar;인터랙션&rpar;: 디테일이 경험을 좌우한다&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;⌨️ 포커스 링:&lt;/b&gt; 디자인 해친다고 outline: none으로 포커스 테두리를 없애버리지 마세요! 키보드 사용자를 위해 focus-visible을 꼭 살려둬야 합니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;⏳ 로딩 패턴:&lt;/b&gt; 답답한 빙글빙글 스피너 대신, 뼈대를 먼저 보여주는 &lt;b&gt;스켈레톤 UI&lt;/b&gt;나 성공할 거라 믿고 화면부터 바꿔주는 &lt;b&gt;낙관적 업데이트&lpar;Optimistic Update&rpar;&lt;/b&gt;를 활용하세요.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;6. Responsive Design &lpar;반응형&rpar;: 모바일 퍼스트는 진리다&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  터치 타겟 사이즈:&lt;/b&gt; 모바일에서 버튼 크기는 &lt;b&gt;최소 44x44px&lt;/b&gt; 이상이어야 합니다. 안 그러면 엉뚱한 곳이 눌려 유저가 분노합니다.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  모바일 퍼스트:&lt;/b&gt; 작은 모바일 화면부터 CSS를 짜고, min-width 미디어 쿼리로 데스크톱 뷰를 넓혀가세요. 반대로 하면 코드가 꼬입니다.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;7. UX Writing &lpar;UX 라이팅&rpar;: 친절하고 명확하게&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;&lt;b&gt;  구체적인 버튼:&lt;/b&gt; &quot;확인&quot;, &quot;제출&quot; 같은 모호한 말 대신 &lt;b&gt;&quot;변경사항 저장&quot;, &quot;결제 진행&quot;&lt;/b&gt;처럼 누르면 무슨 일이 일어날지 명확히 적어주세요.&lt;/li&gt;
&lt;li&gt;&lt;b&gt;  빈 상태&lpar;Empty State&rpar;:&lt;/b&gt; &quot;데이터 없음&quot;이라고만 띄우지 마세요. &quot;아직 프로젝트가 없네요. 첫 번째 프로젝트를 만들어보세요!&quot;라며 다음 행동을 유도해야 합니다.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h2 data-ke-size=&quot;size26&quot;&gt;  Part 2. 최악의 AI Slop 안티패턴 목록&lt;/h2&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;AI에게 대충 코딩을 맡기면 십중팔구 아래의 &lt;b&gt;안티패턴&lpar;Anti-patterns&rpar;&lt;/b&gt;을 저지릅니다. 내 프로젝트에 이런 코드가 없는지 당장 점검해 보세요!&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;1. 타이포그래피 &lpar;Typography&rpar;&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;✅ &lt;b&gt;DO:&lt;/b&gt; 프로젝트 성격에 맞는 서체를 의도적으로 골라 쓴다.&lt;/li&gt;
&lt;li&gt;❌ &lt;b&gt;DON&#39;T:&lt;/b&gt; 아무 생각 없이 Inter, Roboto 폰트를 기본값으로 박아둔다. 모든 줄 간격을 1.5로 통일해버린다.&lt;/li&gt;
&lt;/ul&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;2. 색상 &lpar;Color&rpar;&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;✅ &lt;b&gt;DO:&lt;/b&gt; 브랜드에 맞는 고유한 팔레트를 세팅하고, 글자와 배경의 명도 대비&lpar;4.5:1&rpar;를 철저히 지킨다.&lt;/li&gt;
&lt;li&gt;❌ &lt;b&gt;DON&#39;T:&lt;/b&gt; 컬러 배경 위에 회색 글씨를 올려 눈을 침침하게 만든다. AI가 좋아하는 &#39;보라-파랑 네온 그라데이션&#39;을 남발한다.&lt;/li&gt;
&lt;/ul&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;3. 레이아웃 &lpar;Layout&rpar;&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;✅ &lt;b&gt;DO:&lt;/b&gt; 자연스러운 여백으로 시각적 계층을 나눈다.&lt;/li&gt;
&lt;li&gt;❌ &lt;b&gt;DON&#39;T:&lt;/b&gt; 불안하다는 이유로 모든 요소를 둥근 &#39;카드&lpar;Card&rpar;&#39; 안에 넣고, 그 카드를 또 카드 안에 넣는 &#39;중첩 지옥&#39;을 만든다.&lt;/li&gt;
&lt;/ul&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;4. 모션 &lpar;Motion&rpar;&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;✅ &lt;b&gt;DO:&lt;/b&gt; 상태가 변할 때만 살짝&lpar;150~250ms&rpar; 애니메이션을 준다.&lt;/li&gt;
&lt;li&gt;❌ &lt;b&gt;DON&#39;T:&lt;/b&gt; bounce 효과를 남발하고, 마우스만 올리면 사방이 꿀렁거리게 만든다.&lt;/li&gt;
&lt;/ul&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;5. 다크모드 &lpar;Dark Mode&rpar;&lt;/h3&gt;
&lt;ul style=&quot;list-style-type: disc;&quot; data-ke-list-type=&quot;disc&quot;&gt;
&lt;li&gt;✅ &lt;b&gt;DO:&lt;/b&gt; 아주 어두운 회색 배경을 쓰고, 라이트모드의 원색보다 채도를 낮춰 눈을 편안하게 한다.&lt;/li&gt;
&lt;li&gt;❌ &lt;b&gt;DON&#39;T:&lt;/b&gt; 순수 검정&lpar;#000000&rpar; 배경에 라이트모드 색상을 단순히 기계적으로 반전시킨다. 다크모드만 켜면 화면에서 형광빛이 뿜어져 나온다.&lt;/li&gt;
&lt;/ul&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;h3 data-ke-size=&quot;size23&quot;&gt;  마무리 및 핵심 요약&lt;/h3&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;훌륭한 UI/UX는 화려한 장식이 아니라 &lt;b&gt;&#39;절제&#39;&lt;/b&gt;와 &lt;b&gt;&#39;일관된 시스템&#39;&lt;/b&gt;에서 나옵니다.&lt;/p&gt;
&lt;ol style=&quot;list-style-type: decimal;&quot; data-ke-list-type=&quot;decimal&quot;&gt;
&lt;li&gt;&lt;b&gt;글꼴과 여백은 수학적으로 &lpar;Fluid Sizing &amp;amp; 8px Grid&rpar;&lt;/b&gt;&lt;/li&gt;
&lt;li&gt;&lt;b&gt;색상은 세밀하게 &lpar;OKLCH &amp;amp; Tinted Neutrals&rpar;&lt;/b&gt;&lt;/li&gt;
&lt;li&gt;&lt;b&gt;애니메이션과 장식은 꼭 필요한 곳에만 &lpar;Transform &amp;amp; Opacity&rpar;&lt;/b&gt;&lt;/li&gt;
&lt;/ol&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;AI 코딩 툴을 사용할 때 이 7가지 원칙과 안티패턴만 프롬프트나 가이드라인&lpar;.impeccable.md&rpar;으로 잡아주어도 결과물의 수준이 프로 디자이너급으로 수직 상승할 것입니다. 지금 바로 여러분의 프로젝트 코드를 점검해 보세요!&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&lt;b&gt;  여러분이 가장 극혐하는 &#39;AI 특유의 촌스러운 디자인&#39;은 무엇인가요?&lt;/b&gt; 댓글로 여러분의 경험담을 공유해 주세요! 글이 유익하셨다면 공감&lpar;❤️&rpar; 버튼과 구독 부탁드립니다.&lt;/p&gt;
&lt;p data-ke-size=&quot;size16&quot;&gt;&amp;nbsp;&lt;/p&gt;
&lt;p data-pm-slice=&quot;1 1 []&quot; data-ke-size=&quot;size16&quot;&gt;&lpar;출처 및 참고: impeccable.style / GitHub - pbakaus/impeccable&rpar;&lt;/p&gt;</sub><!-- BLOG-POST-LIST:END -->

➡ [블로그 전체 글 보러가기](https://hgko-dev.tistory.com/)

---

### 🧰 Tech Stack

**Front-end** &nbsp;
![TS](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next](https://img.shields.io/badge/Next.js-000?style=flat-square&logo=nextdotjs&logoColor=white)
![Angular](https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)

**Back-end** &nbsp;
![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white)
![Spring](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)
![Node](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Nest](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Python](https://img.shields.io/badge/Python-3766AB?style=flat-square&logo=python&logoColor=white)

**Desktop & DevOps** &nbsp;
![CSharp](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
![WPF](https://img.shields.io/badge/WPF-5C2D91?style=flat-square&logo=.net&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=flat-square&logo=nginx&logoColor=white)

**Database** &nbsp;
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Postgres](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Oracle](https://img.shields.io/badge/Oracle-F80000?style=flat-square&logo=oracle&logoColor=white)
![ES](https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white)

---

### 📊 GitHub Stats

<div align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=hgko1207&show_icons=true&count_private=true&theme=tokyonight&hide_border=true&bg_color=0D1117" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=hgko1207&layout=compact&langs_count=8&exclude_repo=hgko1207.github.io,hexo&theme=tokyonight&hide_border=true&bg_color=0D1117" />
</div>

<div align="center">
  <img src="https://streak-stats.demolab.com?user=hgko1207&theme=tokyonight&hide_border=true&background=0D1117" />
</div>

<!-- Snake contribution animation (output 브랜치 SVG 참조) -->
<div align="center">
  <img src="https://raw.githubusercontent.com/hgko1207/hgko1207/output/github-contribution-grid-snake-dark.svg" />
</div>

---

<p align="center">
  <sub>⚡ Updated automatically — blog posts sync every 6h, snake regenerates every 12h.</sub>
</p>
