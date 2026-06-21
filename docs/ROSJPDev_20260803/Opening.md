---
marp: true
theme: default
header: "__ROS Japan Developer Kaigi @ 筑波大学__"
footer: "[ROS Japan Developer Kaigi Github](https://github.com/fujitatomoya/ros-japan-developer-kaigi)"
paginate: true
style: |
  :root {
    --rjdk-bg: #0d1117;
    --rjdk-bg2: #161b22;
    --rjdk-accent: #22d3ee;
    --rjdk-accent2: #6366f1;
    --rjdk-text: #e6edf3;
    --rjdk-muted: #9aa7b4;
  }
  section {
    background:
      radial-gradient(1200px 600px at 85% -10%, rgba(99, 102, 241, 0.25), transparent 60%),
      radial-gradient(900px 500px at -10% 110%, rgba(34, 211, 238, 0.18), transparent 60%),
      linear-gradient(160deg, var(--rjdk-bg) 0%, var(--rjdk-bg2) 100%);
    color: var(--rjdk-text);
    font-family: "Segoe UI", "Hiragino Sans", "Noto Sans JP", sans-serif;
    padding: 70px 70px 90px;
    letter-spacing: 0.2px;
  }
  h1 {
    font-size: 1.7em;
    font-weight: 800;
    color: #ffffff;
    line-height: 1.2;
    border-left: 10px solid var(--rjdk-accent);
    padding-left: 0.5em;
    margin-bottom: 0.4em;
  }
  h2 {
    color: var(--rjdk-accent);
    font-weight: 700;
  }
  h3 {
    color: #ffffff;
    font-weight: 700;
    background: linear-gradient(90deg, rgba(34, 211, 238, 0.18), transparent);
    border-radius: 8px;
    padding: 0.25em 0.6em;
    display: inline-block;
  }
  a {
    color: var(--rjdk-accent);
    text-decoration: none;
    border-bottom: 1px dashed rgba(34, 211, 238, 0.5);
  }
  strong { color: #ffffff; }
  code {
    background: rgba(99, 102, 241, 0.18);
    color: #c7d2fe;
    border-radius: 6px;
    padding: 0.1em 0.4em;
  }
  ul > li::marker { color: var(--rjdk-accent); }
  ul ul > li::marker { color: var(--rjdk-accent2); }
  li { line-height: 1.5; }
  table {
    border-collapse: collapse;
    font-size: 0.78em;
    width: 100%;
    overflow: hidden;
    border-radius: 10px;
    background: var(--rjdk-bg2);
  }
  th {
    background: linear-gradient(90deg, var(--rjdk-accent2), var(--rjdk-accent));
    color: #0d1117;
    font-weight: 700;
    padding: 0.5em 0.7em;
    text-align: left;
  }
  td {
    background: var(--rjdk-bg2);
    border-bottom: 1px solid rgba(154, 167, 180, 0.18);
    padding: 0.45em 0.7em;
    color: var(--rjdk-text);
  }
  tr:nth-child(even) td { background: #1f2630; }
  header {
    color: var(--rjdk-muted);
    font-weight: 600;
    letter-spacing: 0.5px;
  }
  footer a { color: var(--rjdk-muted); border: none; }
  section::after {
    color: var(--rjdk-muted);
    font-weight: 700;
  }
---

# ROS Japan Developer Kaigi(会議)

- 日時: 2026年8月3日 (月) 14:00 - 17:00
- 場所: 筑波大学 第三エリア 総合研究棟B 1階 0112室

### ご参加いただきありがとうございます 🙏
### 皆さんで気持ちよく開発・議論しましょう 🙌

<!---
Opening の冒頭挨拶。
--->

---

# 本日の趣旨

ROS本線のディープな話、技術課題をシェアしよう🧑‍💻👩‍💻

- 日本のROS／ロボット開発促進
- 技術課題などの情報共有
- 産学連携／コミュニティ技術連携促進
- オープンソース開発促進

<!---
Comment here
--->

---

# 注意事項 ✅

- 飲み物などは各自持参してください 🥤
- Wi-Fiはありません。テザリングをご利用ください 📶
- 発表者はご自身のlaptopを利用してください 💻
- オンライン参加なし／レコーディングもなし 🚫
- 資料は別途公開予定: [https://github.com/fujitatomoya/ros-japan-developer-kaigi](https://github.com/fujitatomoya/ros-japan-developer-kaigi)

<!---
筑波大学の方 (学生／スタッフ) はオブザーバとして登録不要で参加自由です 🎓
--->

---

# 運営スタッフ 📝

- [Tomoya Fujita](https://github.com/fujitatomoya) (TriOrb Inc.)
- [Fumiya Onishi](https://github.com/decwest) (Keio University)
- [nomumu](https://github.com/nomumu) (Eight Knot Inc.)

<!---
Comment here
--->

---

# タイムテーブル 📌 (1/3)

| Time | Facilitator | Presenter | Title / Description |
|------|-------------|-----------|---------------------|
| 14:00-14:05 | T. Fujita | T. Fujita | Opening / 挨拶 / 注意事項説明 |
| 14:05-14:15 | T. Fujita | 筑波大学 | 筑波大学／研究室紹介 |
| 14:15-14:35 | T. Fujita | T. Fujita | ROS 2 Core Full Stack / Governance |
| 14:35-14:55 | T. Fujita | nomumu | ROS 1 → ROS 2 migration deep-dive |
| 14:55-15:05 | T. Fujita | N.A | 休憩 |

<!---
Comment here
--->

---

# タイムテーブル 📌 (2/3)

| Time | Facilitator | Presenter | Title / Description |
|------|-------------|-----------|---------------------|
| 15:05-15:15 | F. Onishi | 発表者① | Issue紹介 + 議論 |
| 15:15-15:30 | F. Onishi | 発表者② | Issue紹介 + 議論 |
| 15:30-15:45 | F. Onishi | 発表者③ | Issue紹介 + 議論 |
| 15:45-15:55 | F. Onishi | N.A | 休憩 |

<!---
Comment here
--->

---

# タイムテーブル 📌 (3/3)

| Time | Facilitator | Presenter | Title / Description |
|------|-------------|-----------|---------------------|
| 15:55-16:50 | nomumu | T. Fujita | Git workflow / ROS branch / Colcon build・test・CI / Issue・PR作成 / QA / Support |
| 16:50-17:00 | nomumu | nomumu | Closing |
| 17:00-17:30 | All | N.A | 退室 |

<!---
Comment here
--->

---

# Networking / 食事 :cocktail:

T.B.D

<!---
Comment here
--->

---

# それでは始めましょう 🚀

日本でROS`開発`を盛り上げましょう 🥊🥊🥊

<!---
Comment here
--->
