---
layout: default
title: GloZ Secure Investor Materials
permalink: /secure/
---

<script>
// Check for access token
function checkAccess() {
  const urlParams = new URLSearchParams(window.location.search);
  const token = urlParams.get('token');
  
  if (!token) {
    document.body.innerHTML = `
      <div style="text-align: center; padding: 40px; color: white; font-family: 'Spoqa Han Sans Neo', 'Pretendard', Arial, Helvetica, sans-serif;">
        <h1>접근이 제한된 페이지입니다</h1>
        <p>이 페이지는 투자 자료 요청을 완료하신 분들만 접근 가능합니다.</p>
        <a href="/" style="color: #5D3FD3; text-decoration: underline;">메인 페이지로 돌아가기</a>
      </div>
    `;
    return;
  }

  // Show the content
  document.getElementById('secure-content').style.display = 'block';
}

// Run check when page loads
window.onload = checkAccess;
</script>

<div id="secure-content" style="display: none;">
  <div class="secure-container">
    <section class="secure-section">
      <h1>감사합니다!</h1>
      <p>이메일로 자료 전달드렸으며,<br>이 페이지에서도 간편하게 보실 수 있습니다.</p>
    </section>

    <section class="secure-section">
      <h2>📄 피칭 자료 보기</h2>
      <div class="secure-presentation">
        <iframe src="https://glozfundraising2026.my.canva.site" width="100%" height="600" style="border-radius:14px; background:#fff;" frameborder="0" allowfullscreen></iframe>
      </div>
    </section>

    <section class="secure-section">
      <h2>🤖 Gloria's AI에게 질문하기</h2>
      <div class="secure-chatbot">
        <iframe src="https://www.chatbase.co/chatbot-iframe/ezFbMXxV7R06quetaNfCc" width="100%" height="600" style="border-radius:14px; background:#fff;" frameborder="0" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" allowfullscreen></iframe>
      </div>
    </section>

    <section class="secure-section">
      <h2>📅 미팅 예약</h2>
      <a class="cta-btn" href="https://calendly.com/gloria-glozinc/30min" target="_blank">글로리아와 미팅 일정 예약하기</a>
    </section>

    <div class="secure-footer">© 2025 GloZ Inc. All rights reserved.</div>
  </div>
</div>

<style>
  body {
    background: #000;
    color: #fff;
    font-family: 'Spoqa Han Sans Neo', 'Pretendard', Arial, Helvetica, sans-serif;
    margin: 0;
    padding: 0;
  }
  .secure-container {
    max-width: 750px;
    margin: 0 auto;
    padding: 0 16px;
    text-align: center;
  }
  .secure-section {
    padding: 80px 0;
    border: none;
  }
  h1, h2, h3 {
    color: #fff;
    font-family: 'Spoqa Han Sans Neo', 'Pretendard', Arial, Helvetica, sans-serif;
    font-weight: 700;
    margin-bottom: 24px;
    margin-top: 0;
  }
  h1 { font-size: 2.1rem; }
  h2 { font-size: 1.4rem; }
  p, a, .secure-link {
    color: #fff;
    font-size: 1.1rem;
    line-height: 1.7;
    margin-bottom: 18px;
    text-align: center;
    font-family: 'Spoqa Han Sans Neo', 'Pretendard', Arial, Helvetica, sans-serif;
  }
  .secure-link {
    color: #5D3FD3;
    font-weight: 700;
    text-decoration: underline;
    word-break: break-all;
    display: inline-block;
    background: #181818;
    border-radius: 8px;
    padding: 16px 32px;
    margin: 16px 0;
    transition: background 0.2s;
  }
  .secure-link:hover {
    background: #2a2a2a;
  }
  .cta-btn {
    display: inline-block;
    background: #5D3FD3;
    color: #fff;
    font-weight: 700;
    border-radius: 8px;
    padding: 18px 36px;
    margin: 32px 0 0 0;
    text-decoration: none;
    font-size: 1.15rem;
    transition: background 0.2s;
    box-shadow: 0 4px 24px rgba(93,63,211,0.10);
  }
  .cta-btn:hover {
    background: #3d278a;
  }
  .secure-video {
    position: relative;
    width: 100%;
    max-width: 750px;
    padding-bottom: 56.25%;
    height: 0;
    margin: 0 auto 0 auto;
    border-radius: 14px;
    overflow: hidden;
    box-shadow: 0 4px 24px rgba(93,63,211,0.10);
  }
  .secure-video iframe {
    position: absolute;
    top: 0; left: 0; width: 100%; height: 100%; border: 0;
  }
  .secure-chatbot {
    width: 100%;
    max-width: 750px;
    margin: 0 auto;
    border-radius: 16px;
    box-shadow: 0 4px 32px rgba(250,208,44,0.10);
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 600px;
    background: #181818;
  }
  .secure-chatbot iframe {
    width: 100%;
    min-height: 600px;
    border: none;
    border-radius: 14px;
    background: #fff;
    display: block;
    margin: 0 auto;
  }
  .secure-footer {
    color: #888;
    font-size: 0.95rem;
    margin: 60px 0 24px 0;
    text-align: center;
  }
  .secure-presentation {
    width: 100%;
    max-width: 750px;
    margin: 0 auto;
    border-radius: 16px;
    box-shadow: 0 4px 32px rgba(250,208,44,0.10);
    padding: 0;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    min-height: 600px;
    background: #181818;
  }
  .secure-presentation iframe {
    width: 100%;
    min-height: 600px;
    border: none;
    border-radius: 14px;
    background: #fff;
    display: block;
    margin: 0 auto;
  }
  @media (max-width: 900px) {
    .secure-container, .secure-video, .secure-chatbot { max-width: 98vw; }
  }
  @media (max-width: 600px) {
    h1 { font-size: 1.3rem; }
    h2 { font-size: 1.1rem; }
    .secure-container { padding: 0 2vw; }
    .secure-section { padding: 40px 0; }
    .secure-video, .secure-chatbot { border-radius: 8px; }
  }
</style>
