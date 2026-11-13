<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover">
<title>مركز الطالب الذكي</title>
<link href="https://fonts.googleapis.com/css2?family=Tajawal:wght@400;500;700&display=swap" rel="stylesheet">
<style>
:root{
  --bg:#F4F7F8; --card:#FFFFFF; --text:#1B2A3A; --muted:#5B6B79; --line:#BFD3D3; --edge:#D5DEE3;
  --hub:#243752; --hub-text:#FFFFFF; --teal:#2F7A78; --gold:#C9A24B; --icon-bg:#E4F0EF;
  box-sizing:border-box; padding-top:env(safe-area-inset-top,0px); padding-bottom:env(safe-area-inset-bottom,0px);
}
@media (prefers-color-scheme:dark){
  :root:not([data-theme="light"]){
    --bg:#0F1A26; --card:#17263A; --text:#E8EEF3; --muted:#9FB0BF; --line:#3C6E6C; --edge:#2A3C52;
    --hub:#2F7A78; --icon-bg:#20405A; --teal:#6CC0BC;
  }
}
:root[data-theme="dark"]{
  --bg:#0F1A26; --card:#17263A; --text:#E8EEF3; --muted:#9FB0BF; --line:#3C6E6C; --edge:#2A3C52;
  --hub:#2F7A78; --icon-bg:#20405A; --teal:#6CC0BC;
}
*{box-sizing:border-box}
html{scroll-padding-top:env(safe-area-inset-top,0px)}
body{margin:0;background:var(--bg);color:var(--text);font-family:"Tajawal",Arial,Tahoma,sans-serif;min-height:100vh}
main{max-width:940px;margin:0 auto;padding:36px 20px 28px}
h1{margin:0 0 6px;font-size:34px;line-height:1.3;font-weight:700;text-align:center}
.lead{margin:0 0 26px;text-align:center;color:var(--muted);font-size:16px}

.stage{position:relative;width:100%;max-width:900px;aspect-ratio:900/480;margin:0 auto}
.lines{position:absolute;inset:0;width:100%;height:100%}
.lines line{stroke:var(--line);stroke-width:2;stroke-dasharray:5 6}
.hub{position:absolute;left:50%;top:50%;width:150px;height:150px;transform:translate(-50%,-50%);border-radius:50%;
  background:var(--hub);color:var(--hub-text);display:flex;flex-direction:column;align-items:center;justify-content:center;text-align:center;
  box-shadow:0 0 0 8px var(--bg),0 0 0 10px var(--gold)}
.hub b{font-size:30px;line-height:1}
.hub span{font-size:15px;font-weight:700;margin-top:6px;line-height:1.3}
.hub small{font-size:12px;opacity:.85;direction:ltr}

.node{position:absolute;left:calc(50% + var(--x));top:calc(50% + var(--y));width:210px;transform:translate(-50%,-50%);
  display:flex;align-items:center;gap:12px;padding:12px 14px;background:var(--card);border:1px solid var(--edge);border-radius:14px;
  color:inherit;text-decoration:none;box-shadow:0 2px 8px rgba(20,40,60,.08);transition:border-color .15s,transform .15s}
.node:hover{border-color:var(--teal);transform:translate(-50%,-50%) scale(1.04)}
.node:focus-visible{outline:3px solid var(--gold);outline-offset:2px}
.ico{flex:none;width:44px;height:44px;border-radius:50%;background:var(--icon-bg);display:grid;place-items:center;font-size:22px}
.node strong{display:block;font-size:16px;line-height:1.3}
.node em{display:block;font-style:normal;font-size:13px;color:var(--muted);line-height:1.4;margin-top:2px}
.n0{--x:0px;--y:-190px}.n1{--x:286px;--y:-95px}.n2{--x:286px;--y:95px}
.n3{--x:0px;--y:190px}.n4{--x:-286px;--y:95px}.n5{--x:-286px;--y:-95px}
@media (max-width:940px){.node{--s:.8}}

.note{margin:30px 0 0;text-align:center;color:var(--muted);font-size:13px}

@media (max-width:720px){
  main{padding-top:24px}
  h1{font-size:28px}
  .stage{aspect-ratio:auto;display:flex;flex-direction:column;gap:12px;padding-top:0}
  .lines{display:none}
  .hub{position:relative;left:auto;top:auto;transform:none;margin:0 auto 14px;width:132px;height:132px}
  .node{position:static;transform:none;width:100%}
  .node:hover{transform:none}
}
</style>
</head>
<body>
<main>
  <h1>مركز الطالب الذكي</h1>
  <p class="lead">اضغط على أي خدمة لفتحها مباشرة</p>

  <div class="stage">
    <svg class="lines" viewBox="0 0 900 480" preserveAspectRatio="none" aria-hidden="true">
      <line x1="450" y1="240" x2="450" y2="50"/>
      <line x1="450" y1="240" x2="736" y2="145"/>
      <line x1="450" y1="240" x2="736" y2="335"/>
      <line x1="450" y1="240" x2="450" y2="430"/>
      <line x1="450" y1="240" x2="164" y2="335"/>
      <line x1="450" y1="240" x2="164" y2="145"/>
    </svg>

    <div class="hub"><b>🎓</b><span>جامعة أم القرى</span><small>Smart Student Hub</small></div>

    <a class="node n0" href="https://uqu.edu.sa/App/Catalog/382" target="_blank" rel="noopener noreferrer">
      <span class="ico">💻</span><span><strong>التعلم الإلكتروني</strong><em>Blackboard: المقررات والواجبات</em></span></a>

    <a class="node n1" href="https://www.google.com/goto?url=CAESSwHrOzAVzAUshL7LIrAdeKsVP-KjMcWiA_kFuxO71FMchGpc7KghNbUhX98-FiilpnypXqgkOWBu8RqeLMaeipucSAx8oKFvM4Xhnw" target="_blank" rel="noopener noreferrer">
      <span class="ico">🏫</span><span><strong>موقع الجامعة</strong><em>الأخبار والخدمات والأدلة</em></span></a>

    <a class="node n2" href="https://www.google.com/goto?url=CAESWwHrOzAVomUZFzyullRHIc9UhIm4Pzz-CtAmGqlDl5-mBFcf7Xpd5N-GCZjQ2UhsHkuOKNqZdkHiummt4PSAsRwKSdxi1Uk60qzA5BwxKGvWS-gsIVIMApKow8g" target="_blank" rel="noopener noreferrer">
      <span class="ico">📧</span><span><strong>البريد الجامعي</strong><em>رسائلك الرسمية من الجامعة</em></span></a>

    <a class="node n3" href="https://www.google.com/goto?url=CAESYgHrOzAV2CB8A2H4UrJWxDySER6i5dFQiIp5tDugw5kNRypEt3jtwBWsQUfAECqiS23ITclMlGzKDISR7U6GDyGkhJJLmNJpKv2iJubzdj6dRqkRrzhO2-OF7ngvEIFUSYlW" target="_blank" rel="noopener noreferrer">
      <span class="ico">📅</span><span><strong>التقويم الأكاديمي</strong><em>مواعيد الفصل والاختبارات</em></span></a>

    <a class="node n4" href="https://library.uqu.edu.sa/ar/" target="_blank" rel="noopener noreferrer">
      <span class="ico">📚</span><span><strong>المكتبة الجامعية</strong><em>الكتب والمصادر الإلكترونية</em></span></a>

    <a class="node n5" href="https://uqu.edu.sa/App/vCard" target="_blank" rel="noopener noreferrer">
      <span class="ico">🎓</span><span><strong>البطاقة الجامعية</strong><em>بطاقتك الجامعية الرقمية</em></span></a>
  </div>

  <p class="note">تفتح الخدمات في تبويب جديد</p>
</main>
</body>
</html>
