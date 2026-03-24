---
marp: true
theme: default
paginate: true
style: |
  section {
    font-family: "Helvetica Neue", "Arial", "Hiragino Sans", "Yu Gothic", sans-serif;
    font-size: 34px;
    line-height: 1.4;
    letter-spacing: 0.02em;
    color: #1e293b;
    background: #f8f7f4;
    padding: 54px 72px 46px 72px;
  }
  h1 { font-size: 68px; font-weight: 700; color: #111827; margin: 0 0 20px 0; border-bottom: none; }
  h2 { font-size: 52px; font-weight: 700; color: #111827; margin: 0 0 14px 0; }
  h3 { font-size: 36px; font-weight: 700; color: #475569; margin: 10px 0 8px 0; }
  strong { color: #111827; font-weight: 700; }
  em { color: #0369a1; font-style: normal; font-weight: 700; }
  blockquote {
    margin: 24px 0 0 0;
    padding: 20px 24px;
    border-left: 6px solid #0369a1;
    background: rgba(3, 105, 161, 0.07);
    color: #111827;
    font-size: 48px;
    font-weight: 700;
    line-height: 1.5;
    border-radius: 0 8px 8px 0;
  }
  blockquote p { margin: 0; }
  table { width: 100%; border-collapse: collapse; margin-top: 18px; font-size: 34px; background: #f8f7f4 !important; }
  table th, table td { background: #f8f7f4 !important; }
  thead th { color: #475569; font-weight: 700; font-size: 30px; text-transform: uppercase; letter-spacing: 0.05em; border-bottom: 2px solid #d1d5db; padding: 12px 14px; text-align: center; }
  tbody td { border-bottom: 1px solid #e5e7eb; padding: 14px; text-align: center; color: #1e293b; }
  tbody tr:nth-child(even) td { background: rgba(0,0,0,0.02) !important; }
  tbody td strong { color: #0369a1; font-size: 1.15em; }
  .accent { color: #0369a1 !important; }
  .sub { font-size: 32px; color: #6b7280; margin-top: 12px; }
  section.title {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
    background: linear-gradient(135deg, #f8f7f4 0%, #f0ede8 50%, #f8f7f4 100%);
  }
  section.title h1 { font-size: 88px; margin-bottom: 24px; letter-spacing: 0.03em; }
  section.title p, section.title strong { font-size: 34px; color: #475569; }
  section.message {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
  }
  section.message h1 { font-size: 74px; line-height: 1.3; max-width: 90%; }
  section.kpi-hero {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
  }
  section.kpi-hero h1 { font-size: 54px; color: #475569; font-weight: 500; margin-bottom: 16px; }
  .hero-number { font-size: 210px; font-weight: 800; color: #0369a1; line-height: 1.0; margin: 8px 0 16px 0; letter-spacing: -0.02em; }
  .hero-unit { font-size: 64px; font-weight: 500; color: #6b7280; margin-left: 4px; }
  .hero-row { display: flex; align-items: center; justify-content: center; gap: 32px; margin: 16px 0; }
  .hero-item { text-align: center; }
  .hero-label { display: block; font-size: 32px; color: #6b7280; margin-bottom: 8px; text-transform: uppercase; letter-spacing: 0.05em; }
  .hero-number-sm { display: block; font-size: 98px; font-weight: 800; color: #6b7280; line-height: 1.0; }
  .hero-number-sm.accent { color: #0369a1; }
  .hero-arrow { font-size: 64px; color: #9ca3af; font-weight: 300; }
  section.before-after { text-align: center; }
  section.before-after h1 { text-align: center; margin-bottom: 24px; }
  .ba-row { display: flex; gap: 32px; justify-content: center; align-items: stretch; margin-top: 8px; }
  .ba-box { flex: 1; max-width: 420px; border-radius: 12px; padding: 28px 32px; text-align: center; }
  .ba-box h3 { font-size: 32px; text-transform: uppercase; letter-spacing: 0.08em; margin: 0 0 12px 0; }
  .ba-box.before { background: rgba(0,0,0,0.02); border: 1px solid #d1d5db; }
  .ba-box.before h3 { color: #6b7280; }
  .ba-box.after { background: rgba(3,105,161,0.07); border: 1px solid rgba(3,105,161,0.25); }
  .ba-box.after h3 { color: #0369a1; }
  .ba-number { font-size: 88px; font-weight: 800; color: #475569; line-height: 1.1; margin: 8px 0; }
  .ba-unit { font-size: 34px; font-weight: 500; color: #6b7280; }
  .ba-number.accent { color: #0369a1; }
  .ba-box p { font-size: 32px; color: #6b7280; margin: 8px 0 0 0; }
  section.quote { display: flex; flex-direction: column; justify-content: center; }
  section.quote h1 { margin-bottom: 20px; }
  section.action { display: flex; flex-direction: column; justify-content: center; }
  section.action h1 { margin-bottom: 24px; }
  .action-list { margin: 0; padding: 0; }
  .action-list ol { margin: 0; padding: 0; list-style: none; counter-reset: action-counter; }
  .action-list li, .action-list ol li { counter-increment: action-counter; font-size: 36px; line-height: 1.5; margin-bottom: 18px; padding-left: 52px; position: relative; }
  .action-list li::before, .action-list ol li::before { content: counter(action-counter); position: absolute; left: 0; top: 2px; width: 44px; height: 44px; background: #0369a1; color: #ffffff; font-weight: 800; font-size: 28px; border-radius: 50%; display: flex; align-items: center; justify-content: center; }
  section.closing {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
    background: linear-gradient(135deg, #f8f7f4 0%, #f0ede8 50%, #f8f7f4 100%);
  }
  section.closing h1 { font-size: 68px; margin-bottom: 32px; }
  section.closing p, section.closing strong { font-size: 32px; color: #6b7280; }
  section::after { font-size: 18px; color: #9ca3af; right: 28px; bottom: 18px; }
  .wall-label { font-size: 30px; color: #b45309; font-weight: 700; letter-spacing: 0.05em; margin-bottom: 4px; }
  .role-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 16px; }
  .role-card { border-radius: 12px; padding: 24px 28px; border: 1px solid #d1d5db; background: rgba(0,0,0,0.02); }
  .role-card .role-name { font-size: 50px; font-weight: 800; color: #0369a1; margin: 0 0 8px 0; line-height: 1.2; }
  .role-card .role-desc { font-size: 32px; color: #475569; margin: 0; line-height: 1.4; }
---

<!-- _class: title -->

# 倫理 × AI 実践セミナー

**草津市倫理法人会**
2026.3.17

---

<!-- _class: message -->

<div style="text-align:center;">
<p style="font-size:32px; color:#475569; margin-bottom:8px;">草津市倫理法人会 副専任幹事</p>
<p style="font-size:76px; font-weight:800; color:#111827; margin:0 0 16px 0;">今宿 裕昭</p>
<p style="font-size:34px; color:#475569; line-height:1.6;">マツダ → 博報堂（29年）→ 独立<br>ステップアウトマーケティング合同会社 代表</p>
<p style="font-size:62px; font-weight:800; color:#0369a1; margin-top:24px;">コードは一行も書けません</p>
<p class="sub">この会社のサイトも、AIと二人で作りました</p>
</div>

---

<!-- _class: message -->

<img src="stepout-site.png" alt="ステップアウトマーケティング Webサイト" style="max-width:85%; border-radius:12px; box-shadow:0 4px 24px rgba(0,0,0,0.12);">

---

<!-- _class: message -->

# 倫理を学んでいる人こそ、<br>AIを使いこなせる

<p class="sub">「あり方」は倫理。「やり方」はAI。</p>

---

<!-- _class: kpi-hero -->

# 中小企業のAI方針「未決定」

<div class="hero-number">50.9<span class="hero-unit">%</span></div>
<p class="sub">東京商工リサーチ 2025年調査（6,645社）</p>

---

<!-- _class: kpi-hero -->

# 大企業との活用格差

<div class="hero-row">
<div class="hero-item">
<span class="hero-label">中小企業</span>
<span class="hero-number-sm">23.4<span class="hero-unit">%</span></span>
</div>
<div class="hero-arrow">vs</div>
<div class="hero-item">
<span class="hero-label">大企業</span>
<span class="hero-number-sm accent">43.3<span class="hero-unit">%</span></span>
</div>
</div>

---

<!-- _class: kpi-hero -->

# AI導入を阻む壁

<div class="hero-number">5<span class="hero-unit">つ</span></div>
<p class="sub">壁は「お金」でも「技術」でもない</p>

---

<!-- _class: kpi-hero -->

# 壁① 怖い

<div class="hero-number">68.5<span class="hero-unit">%</span></div>
<p class="sub">情報漏洩・失敗への不安</p>

---

<!-- _class: kpi-hero -->

# 壁② 人がいない

<div class="hero-number">55.1<span class="hero-unit">%</span></div>
<p class="sub">専門人材がいない</p>

---

<!-- _class: kpi-hero -->

# 壁③ 決められない

<div class="hero-number">50.9<span class="hero-unit">%</span></div>
<p class="sub">方針が決まらない</p>

---

<!-- _class: kpi-hero -->

# 壁④ 判断できない

<div class="hero-number">43.8<span class="hero-unit">%</span></div>
<p class="sub">良し悪しを評価できない</p>

---

<!-- _class: kpi-hero -->

# 壁⑤ わからない

<div class="hero-number">41.9<span class="hero-unit">%</span></div>
<p class="sub">何に使うかわからない</p>

---

<!-- _class: message -->

# これだけの壁があれば、<br>使えなくて当然だった

---

<!-- _class: before-after -->

# 経営者の「あり方」が成果を分ける

<div class="ba-row">
<div class="ba-box before">
<h3>経営者が理解していない</h3>
<div class="ba-number">50<span class="ba-unit">%</span></div>
<p>しか効果を実感できない</p>
</div>
<div class="ba-box after">
<h3>経営者が理解している</h3>
<div class="ba-number accent">95.5<span class="ba-unit">%</span></div>
<p>が効果を実感</p>
</div>
</div>
<p class="sub">BuddieS 2025年調査（111社）</p>

---

<!-- _class: message -->

# 5つの壁の根っこは1つ。<br>「あり方」の不在

<p class="sub">何のために経営しているか。何のために使うか。</p>

---

<!-- _class: message -->

# 「あり方」は倫理。<br>「やり方」はAI。

<p class="sub">わたしたちは「あり方」を日々磨いている</p>

---

<!-- _class: message -->

# わたしたちは、<br>すでにハンドルを握れる人間だ

<p class="sub">5つの壁を越える力は、栞の中にある</p>

---

<!-- _class: message -->

<img src="porsche-azemichi.png" alt="ポルシェ畦道" style="max-width:85%; border-radius:12px; box-shadow:0 4px 24px rgba(0,0,0,0.12);">

---

<!-- _class: kpi-hero -->

<div class="wall-label">WALL 1 / 怖い ― 68.5%が感じる壁</div>

# 第15条：<br>信ずれば成り、憂えれば崩れる

<blockquote>
憂えて止まることが、最大のリスク。<br>
理解して踏み出した経営者の95.5%が効果を実感
</blockquote>

---

<!-- _class: kpi-hero -->

<div class="wall-label">WALL 2 / 人がいない ― 55.1%が感じる壁</div>

# 第4条：<br>人は鏡、万象はわが師

<blockquote>
人がいないなら、AIを師にする。<br>
学ぶ姿勢がある人に、AIは最大の力を返す
</blockquote>

---

<!-- _class: kpi-hero -->

<div class="wall-label">WALL 3 / 決められない ― 50.9%が感じる壁</div>

# 第1条：<br>今日は最良の一日、今は無二の好機

<blockquote>
「来月やろう」で3年が過ぎた。<br>
始める最良の日は、今日
</blockquote>

---

<!-- _class: kpi-hero -->

<div class="wall-label">WALL 4 / 判断できない ― 43.8%が感じる壁</div>

# 第3条：<br>運命は自らまねき、境遇は自ら造る

<blockquote>
自分の事業は自分で判断するしかない。<br>
やってみて初めてわかる
</blockquote>

---

<!-- _class: kpi-hero -->

<div class="wall-label">WALL 5 / わからない ― 41.9%が感じる壁</div>

# 第16条：<br>己を尊び人に及ぼす

<blockquote>
何に使うか？<br>
自分を楽にし、それを人に及ぼすために使う
</blockquote>

---

<!-- _class: message -->

# 5つの壁を越える力が、<br>すでにわたしたちの中にある

<p class="sub">栞の教えは、AI活用の土台そのものだった</p>

---

<!-- _class: message -->

# 一人会社の社長には、<br>止めてくれる人がいない

<p class="sub">案件の抜け漏れ、採算度外視、先送り…全部、自分では気づけない</p>

---

# AIに「役職」を与えた

単なるチャットではない。**会社の経営構造として組み込んだ**

<div class="role-grid">
<div class="role-card">
<p class="role-name">CEO</p>
<p class="role-desc">毎朝10秒で全案件の状態を把握</p>
</div>
<div class="role-card">
<p class="role-name">CFO</p>
<p class="role-desc">案件の採算を数字で判断・無理なら止める</p>
</div>
<div class="role-card">
<p class="role-name">PM</p>
<p class="role-desc">締切を管理し「やらないこと」を決める</p>
</div>
<div class="role-card">
<p class="role-name">取締役会</p>
<p class="role-desc">4視点で新規案件の受け入れを判断</p>
</div>
</div>

---

# 毎朝5分で、会社が回る

<div class="action-list">

1. 朝、スマホに**声で日記を録る**（ボイスジャーナル）
2. AIが案件別に自動振り分け → **PM取締役が起動**
3. 台帳の締切・カレンダーと突き合わせ
4. <strong>「今日やること3つ」と「今日やらないこと」</strong>が出る

</div>

<p class="sub">朝の案件把握: 30分 → 5分</p>

---

<!-- _class: message -->

# 孤独な判断が、なくなった

<p class="sub">一番変わったのは、数字ではなく「意思決定の質」</p>

---

<!-- _class: before-after -->

# 提案書の作成時間が6分の1に

<div class="ba-row">
<div class="ba-box before">
<h3>Before</h3>
<div class="ba-number">3<span class="ba-unit">時間</span></div>
<p>手作業で構成・執筆</p>
</div>
<div class="ba-box after">
<h3>After</h3>
<div class="ba-number accent">30<span class="ba-unit">分</span></div>
<p>AIと対話で完成</p>
</div>
</div>

---

<!-- _class: before-after -->

# メール1通あたり85%の時間削減

<div class="ba-row">
<div class="ba-box before">
<h3>Before</h3>
<div class="ba-number">20<span class="ba-unit">分</span></div>
<p>文面を一から作成</p>
</div>
<div class="ba-box after">
<h3>After</h3>
<div class="ba-number accent">3<span class="ba-unit">分</span></div>
<p>AIが下書き→確認のみ</p>
</div>
</div>

---

<!-- _class: before-after -->

# 議事録整理が5分で完了

<div class="ba-row">
<div class="ba-box before">
<h3>Before</h3>
<div class="ba-number">1<span class="ba-unit">時間</span></div>
<p>手動で書き起こし・整理</p>
</div>
<div class="ba-box after">
<h3>After</h3>
<div class="ba-number accent">5<span class="ba-unit">分</span></div>
<p>AIが自動要約</p>
</div>
</div>

---

<!-- _class: message -->

# AIを使うことは、<br>効率化ではない

<p class="sub">生まれた時間を、大切なことに使う</p>

---

<!-- _class: quote -->

# 己を尊び、人に及ぼす

<blockquote>
自分 → 家族 → 職場 → 地域 → 日本<br>
わたしたちの幸せが、波紋のように広がる
</blockquote>

---

<!-- _class: message -->

# 「私は実践する」と決めた瞬間から、<br>あなたは倫理AI実践士

<p class="sub">仲間と一緒に、今日から始める</p>

---

# ここからは「どうやって」の話

ここまでは<strong>「なぜ」と「何を」</strong>の話をしました

ここからは<strong>実際にAIを触って体験</strong>する時間です

<blockquote>
中野 充博 さんにバトンタッチします
</blockquote>

---

<!-- _class: closing -->

# わたしたちの周りの人を<br>幸せにする第一歩

**この後、中野さんの体験ワークで実際にAIを触ります**

---

<!-- _class: closing -->

# アンケートにご協力ください

<div style="display:flex; align-items:center; justify-content:center; gap:48px; margin-top:24px;">
<img src="survey-qr.png" alt="アンケートQRコード" style="width:280px; height:280px; border-radius:12px; background:#fff; padding:12px;">
<div style="text-align:left;">
<p style="font-size:30px; color:#475569; margin-bottom:12px;">スマートフォンで<br>QRコードを読み取ってください</p>
<p style="font-size:22px; color:#6b7280;">所要時間：約2分</p>
</div>
</div>
