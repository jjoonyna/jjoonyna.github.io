---
layout: post
title: "GitHub Pages + Jekyll 블로그 작성 가이드"
date: 2025-07-01 23:30:00 +0900
categories: github-pages
tags: [jekyll, markdown, blog]
---

> **TL;DR**  
> 파일을 `_posts/YYYY-MM-DD-제목.md` 형식으로 만들고, 위에 프런트매터(front-matter)만 적어 두면 Jekyll이 자동으로 글로 변환해 줍니다 ✅

---

## 1️⃣ 폴더·파일 구조

```text
jjoonyna.github.io/
├── index.md               # 홈
└── _posts/                # ✍️ 글 모음
    └── 2025-07-01-github-pages-blog-guide.md  ← 지금 이 파일

```

2️⃣ 필수 프런트매터 표
| 키(key)       | 설명                           | 예시 값                        |
| ------------ | ---------------------------- | --------------------------- |
| `layout`     | 레이아웃 템플릿 (`post` / `home` 등) | `post`                      |
| `title`      | 글 제목                         | `"GitHub Pages 블로그 작성 가이드"` |
| `date`       | ISO 날짜 + 시간 + 타임존            | `2025-07-01 23:30:00 +0900` |
| `categories` | 1단계 분류(폴더처럼)                 | `github-pages`              |
| `tags`       | 다중 태그(검색·필터용)                | `[jekyll, markdown, blog]`  |



3️⃣ Markdown 빠르게 쓰기
| 마크다운                               | 결과            | 비고                 |
| ---------------------------------- | ------------- | ------------------ |
| `# 제목1`                            | `<h1>`        | 한 게시물엔 보통 `#` 한 번만 |
| `## 제목2`                           | `<h2>`        |                    |
| `**굵게**`, `*기울임*`                  | **굵게**, *기울임* |                    |
| <code>\`\`\`java ... \`\`\`</code> | 코드블록          | 언어 지정 시 하이라이팅      |
| `> 인용문`                            | > 인용문         |                    |
| `- 리스트`                            | • 리스트         | `*`, `+` 도 가능      |

