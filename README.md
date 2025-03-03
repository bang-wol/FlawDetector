# 🕵🏻‍♂️ Flaw Detector
<img width="700" alt="Flaw Detector" src="https://github.com/user-attachments/assets/aa8ef730-59ee-4feb-ba10-3a59a0a55bac" />

<br/>

## 프로젝트 개요
**FlawDetector**는 AI 기반의 소스코드 보안 취약점 분석 및 해결 가이드 제공 솔루션입니다. SW 개발 환경에서 보안 취약점이 증가함에 따라, 이를 사전 탐지하고 해결 방안을 제공하여 보안 사고를 예방합니다.

<br/>

## MVP (최소 기능 제품)

| 기능 | 설명 |
|------|--------------------------------------------------|
| **코드 보안 취약점 분석** | AI 분석을 통해 코드 내 잠재적인 보안 취약점을 감지 |
| **보안 취약점 데이터 제공** | 취약점 데이터베이스(CVE, CNNVD 등) 정보를 반영하여 사용자에게 제공 |

<br/>

## 개발 기간
2024.08.05 ~ 2024.09.20


<br/>

## 기술 스택
<p>
   <img src="https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=Next.js&logoColor=white">
   <img src="https://img.shields.io/badge/Tailwind CSS-06B6D4?style=for-the-badge&logo=Tailwind CSS&logoColor=white">
   <img src="https://img.shields.io/badge/Firebase-DD2C00?style=for-the-badge&logo=Firebase&logoColor=white">
   <img src="https://img.shields.io/badge/Llama3-0467DF?style=for-the-badge&logo=meta&logoColor=white">
   <img src="https://img.shields.io/badge/Puppeteer-40B5A4?style=for-the-badge&logo=Puppeteer&logoColor=white">
   <img src="https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=Vercel&logoColor=white">
</p>

<br/>


## 기능 정의 사항

| 요구사항 명 | 페이지명 | 상세 설명 |
|------------|---------|-----------------------------|
| 랜딩 페이지 | `/` | 서비스 소개 및 가입 유도 |
| 레포지토리 리스트 | `/repos` | GitHub 레포지토리 목록 표시 |
| 코드 분석 페이지 | `/repos/:userName/:repoName` | 특정 코드 파일 선택 후 AI 보안 검사 실행 |
| 프로필 페이지 | `/me` | 연동된 깃허브 계정 정보, 스크랩한 아티클 조회 |
| 취약점 DB | `/vulnerability-db` | 최신 보안 취약점 리스트 제공(크롤링된 데이터) |

<br/>

## 정보 구조도
<img width="600" alt="정보 구조도" src="https://github.com/user-attachments/assets/734e453a-8f5b-4308-8727-e59ea57506c4" />

<br/>

## 팀원 소개 및 역할

<table width="100%">
  <tbody>
    <tr>
      <td align="center" width="20%">
        <a href="https://github.com/chaduhwan"><img src="https://avatars.githubusercontent.com/u/137901354?v=4" width="100px;" alt="두환"/><br />
</a><b>두환</b>
      </td>
      <td align="center" width="20%>
        <a href="https://github.com/sockki"><img src="https://avatars.githubusercontent.com/u/93645009?v=4" width="100px;" alt="민준"/><br />
</a><b>민준</b>
      </td>
      <td align="center" width="20%">
        <a href="https://github.com/bang-wol"><img src="https://avatars.githubusercontent.com/u/102708198?v=4" width="100px;" alt="수빈"/><br />
</a><b>수빈</b>
      </td>
      <td align="center" width="20%">
        <a href="https://github.com/printjin-gmailcom"><img src="https://avatars.githubusercontent.com/u/161997875?v=4" width="100px;" alt="연진"/><br /></a><b>연진</b>
      </td>
      <td align="center" width="20%>
        <a href="https://github.com/Young2un"><img src="https://avatars.githubusercontent.com/u/132687752?v=4" width="100px;" alt="영은"/><br /></a><b>영은</b>
      </td>
    </tr>
    <tr>
       <td align="center">코드 취약점 검사</td>
       <td align="center">보안 취약점 정보 크롤링</td>
       <td align="center">GitHub 연동, 프로필 페이지</td>
       <td align="center">랜딩 페이지</td>
       <td align="center">랜딩 페이지, 취약점 정보 스크랩, 챗봇 구현</td>
    </tr>
  </tbody>
</table>


<br/>

## 프로젝트 소개 및 시연

### ◼ 랜딩 페이지
<img src="https://raw.githubusercontent.com/bang-wol/FlawDetector/develop/public/images/demo5.gif" width="800px">

- 배경 인터렉션(`AOS`, `Murquee`) 적용
- `GitHub Oauth` 및 `NextAuth`를 활용한 로그인
  
<br/>

### ◼ My 저장소
<img src="https://raw.githubusercontent.com/bang-wol/FlawDetector/develop/public/images/demo4.gif" width="800px">

- `GitHub REST API`를 활용한 저장소 관리
- 최근 방문한 파일, 북마크, 정렬, 필터, 페이지네이션 기능 제공

<br/>

### ◼ 코드 취약점 검사
<img src="https://raw.githubusercontent.com/bang-wol/FlawDetector/develop/public/images/demo3.gif" width="800px">

- `Llama3`를 활용한 코드 취약점 검사
- 단일 검사, 다중 검사 기능
- 검사 상태 및 결과 제공 

<br/>

### ◼ 취약점 DB
<img src="https://raw.githubusercontent.com/bang-wol/FlawDetector/develop/public/images/demo2.gif" width="800px">

- `Puppeteer`를 활용한 크롤링
- `Llama3`로 자동 번역 기능
- 검색, 토픽 기능 제공
- 챗봇을 통해 추가 정보 제공

<br/>

### ◼ 프로필 페이지 & 문의하기
<img src="https://raw.githubusercontent.com/bang-wol/FlawDetector/develop/public/images/demo1.gif" width="800px">

- 개인 정보 확인
- 스크랩한 아티클 확인 가능
- `React Hook From`을 활용한 유효성 검사 적용
- `Nodemailer`를 사용하여 이메일 문의 기능 제공

<br/>

## 참고자료

- [CVE - 미국 취약점 데이터베이스](https://cve.mitre.org/)  
- [CNNVD - 중국 취약점 데이터베이스](https://www.cnnvd.org.cn/)  
- [VulDB - 보안 취약점 데이터베이스](https://vuldb.com/)  
- [OWASP Top Ten - 웹 보안 취약점](https://owasp.org/www-project-top-ten/)  
