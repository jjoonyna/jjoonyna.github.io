# 홈(index.md) 작성
cat <<'EOF' > index.md
---
layout: home
title: "jjoonyna의 개발 노트"
subtitle: "문제 해결 & 재사용 코드 모음"
---

### 🔍 무엇을 다루나요?
- **문제 해결 기록**  
  업무·사이드 프로젝트에서 마주친 버그·설계 이슈, 그리고 해결 과정과 배운 점을 정리합니다.
- **재사용 가능한 코드**  
  Spring Boot 헬퍼, 쉘 원라이너, Git 꿀팁 등 자주 쓰는 코드를 모아둡니다.

---

### 🗂 최근 글
{% for post in site.posts limit:5 %}
- [{{ post.title }}]({{ post.url }})
{% endfor %}
EOF

# 새 글 예시 (_posts/)
mkdir -p _posts
cat <<'EOF' > _posts/2025-07-01-spring-validation-tip.md
---
title: "Spring Boot Bean Validation 꿀팁"
tags: [spring, validation]
---

`@Validated` + `@InitBinder` 를 함께 쓰면 그룹별 검증을 깔끔하게 처리할 수 있습니다…

(이하 본문)
EOF

# GitHub에 커밋 & 푸시
git add index.md _posts/2025-07-01-spring-validation-tip.md
git commit -m "홈 index.md 및 첫 글 추가"
git push origin main
