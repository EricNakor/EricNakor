<div align="center">

# 🌌 Na Junho (나준호)
### "소프트웨어 개발부터 탄탄한 인프라 구축까지, 경계 없는 최적화를 추구합니다."

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=24&pause=1000&color=00D1FF&center=true&vCenter=true&width=500&lines=Spring+Boot+%26+Next.js+Developer;HomeLab+%26+Infra+Enthusiast;Problem+Solver+;Continuous+Learner" alt="Typing SVG" />

<p align="center">
  <a href="https://ericna.pages.dev"><img src="https://img.shields.io/badge/Blog-00D1FF?style=for-the-badge&logo=obsidian&logoColor=white" alt="Blog"></a>
  <a href="mailto:ericna130@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail"></a>
  <a href="https://www.linkedin.com/in/junho-na-771005157"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <img src="https://komarev.com/ghpvc/?username=EricNakor&label=Profile%20Visitors&color=00D1FF&style=for-the-badge" alt="profile visitors"/>
</p>

---

</div>

## 👨‍💻 About Me
- 🚀 **Full-Stack Developer**: Spring Boot와 Next.js를 주력으로, 확장 가능하고 유지보수가 쉬운 서비스를 만듭니다.
- 🛡️ **Self-Hoster**: Proxmox 기반의 프라이빗 클라우드를 직접 구축하여 최신 기술들을 실험하고 실제 서비스에 적용합니다.
- ⚡ **Security-Minded**: 네트워크 세분화와 터널링 기술을 통해 보안과 접근성의 균형을 고려한 아키텍처를 지향합니다.

---

## 🛠️ Tech Stack

### ⚙️ Backend
[![My Skills](https://skillicons.dev/icons?i=java,spring,kotlin,gradle,hibernate&perline=10)](https://skillicons.dev)

### 🎨 Frontend
[![My Skills](https://skillicons.dev/icons?i=js,ts,react,nextjs,tailwind,electron&perline=10)](https://skillicons.dev)

### 🗄️ Database & Storage
[![My Skills](https://skillicons.dev/icons?i=mysql,postgres,redis,minio&perline=10)](https://skillicons.dev)

### 🌐 DevOps & Infrastructure
[![My Skills](https://skillicons.dev/icons?i=docker,githubactions,linux,cloudflare,nginx&perline=10)](https://skillicons.dev)

### 📊 Monitoring & Observability
[![My Skills](https://skillicons.dev/icons?i=prometheus,grafana&perline=10)](https://skillicons.dev)

### 🛠️ Tools & Productivity
[![My Skills](https://skillicons.dev/icons?i=idea,webstorm,vscode,eclipse,git,github,postman,figma,obsidian,notion&perline=10)](https://skillicons.dev)

---

## 🏗️ Private Infrastructure Architecture
> 보안과 성능의 균형을 위해 논리적으로 분리된 2개의 네트워크 세그먼트를 운영하고 있습니다.

```mermaid
graph TD
    %% Internet & External Access
    ISP((🌐 ISP)) --> MODEM{ISP Modem}
    CLIENT[📱 External Client] <--> CF[☁️ Cloudflare]
    
    %% HomeLab Segment
    subgraph HomeLab ["🧪 HomeLab (Isolated Branch)"]
        MODEM -- "Public IP" --> OPN[🛡️ OPNsense Firewall]
        OPN -- "Private IP" --> MINI[🖥️ Minisforum UM870 Slim]
        
        subgraph ProdServices ["🚀 Prod Services (LXC)"]
            MINI --> S1["DoEatFit"]
            MINI --> S2["ChoisIntl"]
            MINI --> S3["SeoulHouse"]
            MINI --> MON["Loki / Prom / Grafana"]
        end
    end
    
    %% Connection from Cloudflare
    CF <-->|":443"| MINI

    %% HomeNet Segment
    subgraph HomeNet ["🏠 HomeNet (General Use)"]
        MODEM -- "Public IP" --> MESH1[📡 MESH Router 1]
        MESH1 -- "Private IP" --> HUB[🔌 Switch HUB]
        
        HUB --> NAS["💾 Synology NAS"]
        HUB --> OD1["All other devices"]
        subgraph NAS_Services ["🏠 Home Services"]
            NAS --> PH[Pi-hole]
            NAS --> HA[Home Assistant]
            NAS --> ZB[Zigbee2MQTT]
        end
        
        HUB -- "Private IP" --> MESH2[📡 MESH Router 2]
        MESH2 --> OD2["All other devices"]
    end
```

---

## 🚀 Featured Projects

### 🥗 [DoEatFit](http://www.doeatfit.org)
- **Concept**: 개인 맞춤형 식단 추천 및 운동 가이드 웹 애플리케이션
- **Tech Stack**: `Spring Boot`, `Next.js`, `TypeScript`, `React`, `JPA`, `QueryDSL`, `Redis`, `MinIO`, `Meilesearch`, `Grafana`, `Loki`, `Prometheus`, `Tempo`, `MySQL`, `Github Action`
- **Keywords**: #Observability #Optimization #Customization

### 🏗️ [Chois International](http://steel.choisintl.co)
- **Concept**: 다국어 지원 철강 무역 회사 기업용 반응형 웹사이트
- **Tech Stack**: `Spring Boot`, `Next.js`, `TypeScript`, `React`, `JPA`, `Redis`, `MinIO`, `Swagger`, `Github Action`, `PostgreSQL`
- **Keywords**: #GlobalTrade #ResponsiveWeb #CorporateIdentity

### 🏠 [The Seoul House](http://www.theseoulhouse.com)
- **Concept**: 예약 관리가 가능한 BnB 서비스 웹사이트
- **Tech Stack**: `Kotlin`, `Spring Boot`, `Next.js`, `React`, `JPA`, `Redis`, `MinIO`, `TypeScript`, `PostgreSQL`, `GithubAction`
- **Keywords**: #ReservationSystem #Multilingual #KotlinBackend

### 📑 [Flowright](https://github.com/EricNakor/Flowright)
- **Concept**: 노드 기반의 흐름 시각화 및 에디터 도구
- **Tech Stack**: `TypeScript`, `React`, `Tailwind CSS`, `Electron`
- **Keywords**: #FlowEditor #NodeBased #Visualization

---

## 📂 Other Projects
- **DaLabel**: 데이터 라벨링 웹 서비스 (`Java`, `Spring Framework Legacy`)
- **Algorithm & Data Structure**: 백준(BOJ) 문제 풀이 레포지토리 (`Java`)

---

## 📊 Statistics & Activities

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=EricNakor&layout=compact&theme=tokyonight" alt="Langs" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=EricNakor&show_icons=true&theme=tokyonight&rank_icon=github" alt="Stats" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=EricNakor&theme=tokyonight" alt="Streak" />
</p>

---

## ✍️ Latest Blog Posts
<!-- BLOG-POST-LIST:START -->
- [ISS-Sync&rpar; 분산 환경에서 비동기 요청 순서 보장 &lpar;CRDT 타임스탬프&rpar;](https://ericna.pages.dev/%F0%9F%91%BBProject/%F0%9F%8F%8B%EF%B8%8FDo-Eat-Fit/%F0%9F%9A%A8Issue/ISS-Sync)-%EB%B6%84%EC%82%B0-%ED%99%98%EA%B2%BD%EC%97%90%EC%84%9C-%EB%B9%84%EB%8F%99%EA%B8%B0-%EC%9A%94%EC%B2%AD-%EC%88%9C%EC%84%9C-%EB%B3%B4%EC%9E%A5-(CRDT-%ED%83%80%EC%9E%84%EC%8A%A4%ED%83%AC%ED%94%84)) - 2026-07-05
- [ISS-UX&rpar; History API 오용으로 인한 가상 히스토리 루프 버그 해결](https://ericna.pages.dev/%F0%9F%91%BBProject/%F0%9F%8F%8B%EF%B8%8FDo-Eat-Fit/%F0%9F%9A%A8Issue/ISS-UX)-History-API-%EC%98%A4%EC%9A%A9%EC%9C%BC%EB%A1%9C-%EC%9D%B8%ED%95%9C-%EA%B0%80%EC%83%81-%ED%9E%88%EC%8A%A4%ED%86%A0%EB%A6%AC-%EB%A3%A8%ED%94%84-%EB%B2%84%EA%B7%B8-%ED%95%B4%EA%B2%B0) - 2026-07-05
- [RETRO&rpar; FCM 푸시 알림 시스템 구축 및 CI-CD 자동화 연동](https://ericna.pages.dev/%F0%9F%91%BBProject/%F0%9F%8F%8B%EF%B8%8FDo-Eat-Fit/%F0%9F%93%9DRetrospective/RETRO)-FCM-%ED%91%B8%EC%8B%9C-%EC%95%8C%EB%A6%BC-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EA%B5%AC%EC%B6%95-%EB%B0%8F-CI-CD-%EC%9E%90%EB%8F%99%ED%99%94-%EC%97%B0%EB%8F%99) - 2026-06-25
- [ARCH&rpar; DoEatFit v2.0 다중 계층 인증 및 JWT 생명주기 설계서](https://ericna.pages.dev/%F0%9F%91%BBProject/%F0%9F%8F%8B%EF%B8%8FDo-Eat-Fit/%F0%9F%93%9DRetrospective/ARCH)-DoEatFit-v2.0-%EB%8B%A4%EC%A4%91-%EA%B3%84%EC%B8%B5-%EC%9D%B8%EC%A6%9D-%EB%B0%8F-JWT-%EC%83%9D%EB%AA%85%EC%A3%BC%EA%B8%B0-%EC%84%A4%EA%B3%84%EC%84%9C) - 2026-05-23
- [ARCH&rpar; DoEatFit v2.0 전체 시스템 아키텍처 및 데이터 흐름 가이드](https://ericna.pages.dev/%F0%9F%91%BBProject/%F0%9F%8F%8B%EF%B8%8FDo-Eat-Fit/%F0%9F%93%9DRetrospective/ARCH)-DoEatFit-v2.0-%EC%A0%84%EC%B2%B4-%EC%8B%9C%EC%8A%A4%ED%85%9C-%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98-%EB%B0%8F-%EB%8D%B0%EC%9D%B4%ED%84%B0-%ED%9D%90%EB%A6%84-%EA%B0%80%EC%9D%B4%EB%93%9C) - 2026-05-23<!-- BLOG-POST-LIST:END -->

<p align="right">
  <a href="https://ericna.pages.dev"><img src="https://img.shields.io/badge/Check_Out_My_Latest_Posts-00D1FF?style=for-the-badge&logoColor=white" /></a>
</p>

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=00D1FF&height=120&section=footer" />
</div>
