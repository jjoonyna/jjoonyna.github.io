---
layout: default
title: "jjoonyna의 개발 노트"
subtitle: "문제 해결 & 재사용 코드 모음"
---

# jjoonyna’s Blog

### 🔍 무엇을 다루나요?
- **문제 해결 기록**  
  업무·사이드 프로젝트에서 마주친 버그·설계 이슈, 그리고 해결 과정과 배운 점을 정리합니다.
- **재사용 가능한 코드**  
  Spring Boot, Java, React, TypeScript, JSP, CSS, JavaScript, Python, Node.js 등에서 자주 쓰는 코드를 모아둡니다.

---

### 🗂 최근 글
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
