<div align="center">
  
# 👋 나준호, Na Junho

**웹과 시스템 개발에 깊은 관심을 두고 꾸준히 성장하는 개발자입니다.**

</div>

### ✉️ Contact & Socials
<p align="center">
  <a href="mailto:ericna130@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://blog.eric7na.synology.me"><img src="https://img.shields.io/badge/Blog-1A1A1A?style=for-the-badge&logo=blogger&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/junho-na-771005157"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"></a>
  <img src="https://komarev.com/ghpvc/?username=EricNakor&label=Profile%20Visitors&color=9740e0&style=for-the-badge" alt="profile visitors"/>
</p>

---

<table width="100%">
  <tr valign="top">
    <td width="65%">
      
- 🌱 현재 배우고 있는 것: TypeScript, Hypervisor OS
- 👯 협업하고 싶은 분야: 웹 서비스, 시스템 개발
- 🤔 관심사: 클라우드 네이티브, 분산 시스템 등

<br>

## 🚀 프로젝트 (Projects)

- **DoEatFit**
    > 개인 맞춤 식단 추천 및 운동 가이드 웹 애플리케이션
    
    [![Readme Card](https://github-readme-stats.vercel.app/api/pin?username=EricNakor&repo=doeatfit_back&show_icons=true&theme=github_dark_dimmed)](https://github.com/EricNakor/doeatfit_back)

- **DaLabel**
    > 인공지능 학습을 위한 데이터 라벨링 환경 제공 플랫폼

    [![Readme Card](https://github-readme-stats.vercel.app/api/pin?username=EricNakor&repo=Dalabel&show_icons=true&theme=github_dark_dimmed)](https://github.com/EricNakor/Dalabel)

<br>

## 🔧 기술 스택 (Tech Stack)

### 💻 언어 & 프레임워크
![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white) ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black) ![Spring](https://img.shields.io/badge/Spring-6DB33F?style=for-the-badge&logo=spring&logoColor=white) ![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)

### 🗄️ 데이터베이스
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white) ![Oracle](https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white)

### 🛠️ 툴 & 협업
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white) ![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white) ![IntelliJ IDEA](https://img.shields.io/badge/IntelliJ%20IDEA-000000?style=for-the-badge&logo=intellijidea&logoColor=white) ![Eclipse](https://img.shields.io/badge/Eclipse-2C2255?style=for-the-badge&logo=eclipseide&logoColor=white)

    </td>
    <td width="35%">

## 📊 통계 & 활동 (Stats & Activity)

<p align="center">

[![EricNakor's GitHub stats](https://github-readme-stats.vercel.app/api?username=EricNakor&show_icons=true&theme=github_dark_dimmed&rank_icon=github)](https://github.com/anuraghazra/github-readme-stats)

[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=EricNakor&layout=compact&theme=github_dark_dimmed)](https://github.com/anuraghazra/github-readme-stats)

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=EricNakor&theme=github-dark-dimmed&hide_border=true)](https://git.io/streak-stats)

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=EricNakor&theme=github-dimmed&hide_border=true)](https://github.com/ashutosh00710/github-readme-activity-graph)

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=ojw1996)](https://solved.ac/ojw1996/)

[![GitHub Trophies](https://github-profile-trophy.vercel.app/?username=EricNakor&theme=darkhub&margin-w=15&margin-h=15)](https://github.com/ryo-ma/github-profile-trophy)

</p>
      
    </td>
  </tr>
</table>

---

### 🐍 GitHub 기여도 그래프 애니메이션 (Contribution Snake)
**이 애니메이션은 GitHub Actions 설정이 반드시 필요합니다.** 아래 가이드를 따라 직접 만들어보세요!

<details>
<summary><b>⚙️ Snake 애니메이션 설정 가이드 (클릭하여 펼치기)</b></summary>

1.  **프로필 저장소**(`EricNakor/EricNakor`)에 `.github/workflows` 디렉토리를 생성합니다.
2.  해당 디렉토리 안에 `snake.yml` 파일을 만들고 아래 코드를 그대로 붙여넣습니다.

    ```yml
    name: Generate Snake Animation

    on:
      schedule:
        - cron: "0 0 * * *" # 매일 자정에 실행
      workflow_dispatch:

    jobs:
      build:
        runs-on: ubuntu-latest
        steps:
          - uses: actions/checkout@v3
          - uses: Platane/snk@v3
            with:
              github_user_name: ${{ github.repository_owner }}
              outputs: |
                dist/github-snake.svg
                dist/github-snake-dark.svg?palette=github-dark
            env:
              GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
    ```

3.  커밋하고 Push하면 GitHub Actions가 자동으로 실행되어 애니메이션 SVG 파일이 생성됩니다.
4.  애니메이션이 보이지 않는다면, 프로필 저장소의 `Actions` 탭에서 `Generate Snake Animation` 워크플로우를 수동으로 한번 실행(`Run workflow`)해주세요.
5.  모든 준비가 끝났습니다! 이제 아래 코드를 README의 원하는 위치에 추가하면 정상적으로 표시됩니다.

</details>

```markdown
<p align="center">
  <img src="[https://raw.githubusercontent.com/EricNakor/EricNakor/output/github-snake-dark.svg](https://raw.githubusercontent.com/EricNakor/EricNakor/output/github-snake-dark.svg)" alt="snake animation">
</p>
