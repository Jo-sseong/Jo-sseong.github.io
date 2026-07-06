# 자산 디렉토리

이 디렉토리에는 학술 홈페이지에서 사용되는 자산을 저장합니다.

## 사용 방법

### 프로젝트 썸네일 추가
프로젝트 카드에 썸네일을 추가하려면 이 디렉토리에 이미지를 저장한 후, `index.html`의 프로젝트 카드에 다음과 같이 추가할 수 있습니다:

```html
<div class="project-card">
    <img src="assets/project-thumbnail.jpg" alt="프로젝트 제목" class="project-thumbnail">
    <div class="project-title">프로젝트 제목</div>
    <!-- ... -->
</div>
```

그리고 `style.css`에 다음을 추가하세요:

```css
.project-thumbnail {
    width: 100%;
    height: auto;
    border-radius: 4px;
    margin-bottom: var(--spacing-md);
    object-fit: cover;
}
```

### CV (PDF) 추가
헤더의 CV 링크를 활성화하려면 PDF 파일을 이 디렉토리에 저장한 후, `index.html`의 링크를 수정하세요:

```html
<a href="assets/cv.pdf" download>CV (PDF)</a>
```

## 파일 구조 예시

```
assets/
├── cv.pdf
├── project-1-thumbnail.jpg
├── project-2-thumbnail.jpg
└── project-3-thumbnail.jpg
```

## 주의사항

- 모든 자산은 가볍게 최적화하여 페이지 로딩 속도를 유지하세요.
- 민감한 정보(개인 데이터, 서버 경로 등)는 포함하지 마세요.
