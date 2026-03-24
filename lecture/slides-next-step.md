---
marp: true
theme: default
paginate: true
style: |
  section {
    font-family: "Helvetica Neue", "Arial", "Hiragino Sans", "Yu Gothic", sans-serif;
    font-size: 24px;
    line-height: 1.4;
    letter-spacing: 0.02em;
    color: #e2e8f0;
    background: #0a0f1a;
    padding: 54px 72px 46px 72px;
  }
  h1 { font-size: 44px; font-weight: 700; color: #ffffff; margin: 0 0 20px 0; border-bottom: none; }
  h2 { font-size: 32px; font-weight: 700; color: #ffffff; margin: 0 0 14px 0; }
  h3 { font-size: 24px; font-weight: 700; color: #94a3b8; margin: 10px 0 8px 0; }
  strong { color: #ffffff; font-weight: 700; }
  em { color: #00b4d8; font-style: normal; font-weight: 700; }
  blockquote {
    margin: 24px 0 0 0;
    padding: 20px 24px;
    border-left: 6px solid #00b4d8;
    background: rgba(0, 180, 216, 0.08);
    color: #ffffff;
    font-size: 34px;
    font-weight: 700;
    line-height: 1.5;
    border-radius: 0 8px 8px 0;
  }
  blockquote p { margin: 0; }
  .role-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 16px; }
  .role-card { border-radius: 12px; padding: 24px 28px; border: 1px solid #1e293b; background: rgba(255,255,255,0.03); }
  .role-card .role-pain { font-size: 22px; color: #94a3b8; margin: 0 0 8px 0; line-height: 1.4; }
  .role-card .role-name { font-size: 32px; font-weight: 800; color: #00b4d8; margin: 0; line-height: 1.2; }
  .accent { color: #00b4d8 !important; }
  .sub { font-size: 22px; color: #64748b; margin-top: 12px; }
  section.message {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
  }
  section.message h1 { font-size: 54px; line-height: 1.3; max-width: 90%; }
  section.action { display: flex; flex-direction: column; justify-content: center; }
  section.action h1 { margin-bottom: 24px; }
  .action-list { margin: 0; padding: 0; }
  .action-list ol { margin: 0; padding: 0; list-style: none; counter-reset: action-counter; }
  .action-list li, .action-list ol li { counter-increment: action-counter; font-size: 26px; line-height: 1.5; margin-bottom: 18px; padding-left: 48px; position: relative; }
  .action-list li::before, .action-list ol li::before { content: counter(action-counter); position: absolute; left: 0; top: 2px; width: 36px; height: 36px; background: #00b4d8; color: #0a0f1a; font-weight: 800; font-size: 20px; border-radius: 50%; display: flex; align-items: center; justify-content: center; }
  section.closing {
    display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center;
    background: linear-gradient(135deg, #0a0f1a 0%, #0f172a 50%, #0a0f1a 100%);
  }
  section.closing h1 { font-size: 50px; margin-bottom: 32px; }
  section.closing p, section.closing strong { font-size: 22px; color: #64748b; }
  section::after { font-size: 14px; color: #334155; right: 28px; bottom: 18px; }
  .step-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 20px; margin-top: 16px; }
  .step-card { border-radius: 12px; padding: 24px 28px; border: 1px solid #1e293b; background: rgba(255,255,255,0.03); }
  .step-card .step-num { font-size: 14px; color: #00b4d8; font-weight: 700; text-transform: uppercase; letter-spacing: 0.1em; margin: 0 0 8px 0; }
  .step-card .step-title { font-size: 28px; font-weight: 800; color: #ffffff; margin: 0 0 8px 0; line-height: 1.2; }
  .step-card .step-desc { font-size: 20px; color: #94a3b8; margin: 0; line-height: 1.4; }
  .step-card .step-time { font-size: 16px; color: #00b4d8; margin: 8px 0 0 0; font-weight: 700; }
  .qa-box { border-radius: 12px; padding: 28px 32px; margin-bottom: 20px; }
  .qa-box.question { background: rgba(255,255,255,0.04); border: 1px solid #334155; }
  .qa-box.answer { background: rgba(0,180,216,0.08); border: 1px solid rgba(0,180,216,0.3); }
  .qa-label { font-size: 14px; font-weight: 700; letter-spacing: 0.1em; margin: 0 0 8px 0; }
  .qa-label.q { color: #f59e0b; }
  .qa-label.a { color: #00b4d8; }
  .qa-text { font-size: 26px; color: #ffffff; margin: 0; line-height: 1.5; font-weight: 700; }
  .chat-wrap { max-width: 85%; margin: 0 auto; }
  .chat-bubble { border-radius: 18px; padding: 20px 28px; margin-bottom: 16px; font-size: 24px; line-height: 1.6; position: relative; }
  .chat-bubble.user { background: #1e293b; color: #e2e8f0; margin-left: 60px; border-bottom-right-radius: 4px; }
  .chat-bubble.ai { background: rgba(0,180,216,0.12); border: 1px solid rgba(0,180,216,0.25); color: #ffffff; margin-right: 60px; border-bottom-left-radius: 4px; }
  .chat-who { font-size: 14px; font-weight: 700; letter-spacing: 0.08em; margin-bottom: 6px; }
  .chat-who.you { color: #64748b; text-align: right; }
  .chat-who.bot { color: #00b4d8; }
  section.kpi-hero { display: flex; flex-direction: column; justify-content: center; align-items: center; text-align: center; }
  section.kpi-hero h1 { font-size: 38px; color: #94a3b8; font-weight: 500; margin-bottom: 16px; }
  .hero-number { font-size: 160px; font-weight: 800; color: #00b4d8; line-height: 1.0; margin: 8px 0 16px 0; letter-spacing: -0.02em; }
  .hero-unit { font-size: 48px; font-weight: 500; color: #64748b; margin-left: 4px; }
---

<!-- _class: message -->

# 「うちにも導入したい」<br>と思ったら

<p class="sub">AI取締役の始め方</p>

---

<!-- _class: kpi-hero -->

# 最初に聞くべきこと

<div class="hero-number">1<span class="hero-unit">つ</span></div>

<blockquote>「今、一番困っていることは何ですか？」</blockquote>

---

# 困りごと → AIの役割が決まる

<div class="role-grid">
<div class="role-card">
<p class="role-pain">判断を相談する相手がいない</p>
<p class="role-name">→ 取締役会</p>
</div>
<div class="role-card">
<p class="role-pain">案件の抜け漏れ・先送り</p>
<p class="role-name">→ PM（進行管理）</p>
</div>
<div class="role-card">
<p class="role-pain">採算が見えない・止められない</p>
<p class="role-name">→ CFO（財務判断）</p>
</div>
<div class="role-card">
<p class="role-pain">毎朝の段取りに時間がかかる</p>
<p class="role-name">→ CEO（全体把握）</p>
</div>
</div>

<p class="sub">全部入れる必要はない。一番痛いところから1つだけ</p>

---

# 4ステップで始める

<div class="step-grid">
<div class="step-card">
<p class="step-num">Step 1</p>
<p class="step-title">まず話しかける</p>
<p class="step-desc">ChatGPTやClaudeに「壁打ち相手」として相談してみる</p>
<p class="step-time">今日からできる</p>
</div>
<div class="step-card">
<p class="step-num">Step 2</p>
<p class="step-title">案件を書き出す</p>
<p class="step-desc">自社の案件一覧・売上・期限を1枚にまとめる</p>
<p class="step-time">1〜2時間</p>
</div>
<div class="step-card">
<p class="step-num">Step 3</p>
<p class="step-title">役割を1つ与える</p>
<p class="step-desc">「あなたは私のPMです」と役割を指定して使う</p>
<p class="step-time">半日</p>
</div>
<div class="step-card">
<p class="step-num">Step 4</p>
<p class="step-title">朝の習慣にする</p>
<p class="step-desc">毎朝5分、AIに今日の優先順位を聞く</p>
<p class="step-time">1週間で定着</p>
</div>
</div>

---

# 今日、帰ったらこれを打ってみて

<div class="chat-wrap">
<p class="chat-who you">あなた</p>
<div class="chat-bubble user">あなたは私の会社のPMです。<br>今抱えている仕事を整理してください。<br>・A社の見積もり作成<br>・ホームページのリニューアル<br>・来月のセミナー準備</div>
<p class="chat-who bot">AI</p>
<div class="chat-bubble ai">優先度を整理しました。<br><strong>今日やること：</strong>A社の見積もり（締切が最も近い）<br><strong>今週中：</strong>セミナー準備（会場予約の期限確認）<br><strong>来週以降：</strong>HP リニューアル（急がない）</div>
</div>

<p class="sub">「おっ」と思ったら、それが第一歩</p>

---

<!-- _class: message -->

# 良い問いには、<br>良い答えが返る

<p class="sub">第4条：人は鏡、万象はわが師。AIも同じ</p>

---

# 次回オンラインセミナーのご案内

<div style="display: flex; align-items: center; gap: 48px; margin-top: 16px;">
<div style="flex: 1;">

## 「発信が続かない」を終わらせる

**SNS・ブログ・note — 週1で続く発信の仕組みづくり**

<div style="margin-top: 20px; font-size: 22px; color: #94a3b8; line-height: 2;">

*3/20（金）* オンライン開催
参加費 *¥5,000*（定員5名・少人数制）
講師：今宿裕昭（ステップアウトマーケティング）

</div>

> 「何を書けばいいかわからない」を、AIと一緒に解決します

</div>
<div style="flex-shrink: 0; text-align: center;">
<img src="qr-imajuku.png" alt="QR" style="width: 240px; height: 240px; border-radius: 12px;">
<p style="font-size: 16px; color: #00b4d8; margin-top: 8px; font-weight: 700;">▲ お申し込みはこちら</p>
</div>
</div>

---

# 次回セミナーのご案内

<div style="display: flex; align-items: center; gap: 48px; margin-top: 24px;">
<div style="flex: 1;">

## 倫理×AI実践セミナー vol.2

<div style="margin-top: 20px; font-size: 22px; color: #94a3b8; line-height: 2.2;">

*5/18（月）18:30〜* 草津市倫理法人会
参加費 **無料**（会員・ゲスト歓迎）

</div>

<div style="margin-top: 20px; font-size: 24px; color: #e2e8f0; line-height: 1.6;">

今日の続きを、さらに深掘り。
「実際にやってみた」を持ち寄って、
次のステップへ進みましょう。

</div>

> まずは今日から2ヶ月、AIと一緒に仕事してみてください

</div>
<div style="flex-shrink: 0; text-align: center;">
<div style="width: 220px; height: 220px; border-radius: 16px; background: rgba(0,180,216,0.10); border: 2px solid rgba(0,180,216,0.3); display: flex; flex-direction: column; align-items: center; justify-content: center;">
<p style="font-size: 80px; font-weight: 800; color: #00b4d8; margin: 0; line-height: 1;">5/18</p>
<p style="font-size: 20px; color: #94a3b8; margin: 4px 0 0 0; font-weight: 700;">MON 18:30〜</p>
</div>
</div>
</div>

---

<!-- _class: closing -->

# 本格的に仕組み化したい方は<br>個別にご相談ください

**まずは今日、1回だけAIに話しかけてみる**
