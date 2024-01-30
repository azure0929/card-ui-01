## 'card-ui-01'

<br>

### • 배포 주소: [https://card-ui-01.netlify.app/](https://card-ui-01.netlify.app/)

<br>

#### - 작업 기간: 2021.06

#### - 리팩토링: 2024.01

<br>

### 기술 스택

Development

<p>
<img src="https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=HTML5&logoColor=white" />
<img src="https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=CSS3&logoColor=white" />
</p>

Config

<p>
<img src="https://img.shields.io/badge/npm-CB3837?style=flat&logo=npm&logoColor=white"/></a>
</p>

Environment

<p>
<img src="https://img.shields.io/badge/Visual Studio Code-007ACC?style=flat&logo=Visual Studio Code&logoColor=white"/></a>
<img src="https://img.shields.io/badge/Git-F05032?style=flat&logo=Git&logoColor=white"/></a>
<img src="https://img.shields.io/badge/GitHub-181717?style=flat&logo=GitHub&logoColor=white"/></a>
</p>
<br>

### 전체 페이지

<img src="https://github.com/azure0929/card-ui-01/assets/128226527/24f67220-94ae-4d81-8590-51288abb9023" />

<br><br>

### 💻 주요 기능

---

- flex-wrap, @media

```html
<div class="card">
  <div class="content">
    <img class="face" src="images/profile-01.png" alt="" />
    <h2>멸망 / 나이 미상 (서인국)</h2>
    <p>
      그는 빛과 어둠 사이에서 태어났다. 빛의 마지막 자리, 어둠의 첫 번째 자리.
      그곳이 그의, '멸망'의 고향인 셈이다. 무언가를 멸망시키기 위해 그가 하는
      일은 그저 존재하는 것뿐이다. 그것은 그의 의지도, 그의 사명도
    </p>
    <img src="images/back-01.png" alt="" class="preview" />
  </div>
  <div class="links">
    <a href="#none">article</a>
    <a href="#none">process</a>
  </div>
</div>
```

```css
.card {
  flex: 1;
  padding: 12px;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.15);
  height: 530px;
  border-radius: 10px;
  display: flex;
  flex-direction: column;
}

/* Tablet Break Point */
@media (min-width: 768px) and (max-width: 1024px) {
  section {
    align-items: flex-start;
    padding: 20px;
  }
  .card-items {
    width: 100%;
    flex-wrap: wrap;
    gap: 0;
  }
  .card {
    flex-basis: 50%;
  }
  .preview {
    width: 100%;
  }
}

/* Mobile Break Point */
@media (max-width: 767px) {
  section {
    align-items: flex-start;
  }
  .card-items {
    width: 100%;
    flex-wrap: wrap;
    padding: 15px;
  }
  .card {
    flex-basis: 100%;
  }
}
```
