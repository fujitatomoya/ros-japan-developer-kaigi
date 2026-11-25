---
marp: true
theme: default
header: "__ROS Japan Developer Kaigi @ Inspired Lab at TriOrb__"
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

- 日時: 2026年11月25日 (水) 18:00 - 20:30
- 場所: TriOrb東京オフィス @ Inspired Lab

### ご参加いただきありがとうございます 🙏
### 皆さんで気持ちよく開発・議論しましょう 🙌

<!---
Opening の冒頭挨拶。
--->

---

# ROS JP Dev会議の趣旨

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

- 飲み物と食事は提供されます 🥤 (TriOrb thanks!)
- Wi-Fiはありません。テザリングをご利用ください 📶
- 発表者はご自身のlaptopを利用してください 💻
- オンライン参加なし／レコーディングもなし 🚫

---

# 運営スタッフ 📝

- Komura Yoko (先端技術研究部, TriOrb Inc.)
- Mishina Yoko (経営推進部, TriOrb Inc.)
- [Tomoya Fujita](https://github.com/fujitatomoya) (TriOrb Inc.)

<!---
Comment here
--->

---

# タイムテーブル 📌

| Time | Presenter | Title / Description |
|------|-----------|---------------------|
| 18:00-18:15 | - | Venue Open |
| 18:15-18:20 | T. Fujita | Opening / 注意事項説明 |
| 18:20-18:35 | Y.Komura | TriOrb紹介 |
| 18:35-19:05 | [dskkato](https://github.com/dskkato) | [rosidl::Buffer の極意](https://docs.google.com/presentation/d/1Ma3RPJTnnF_6iQtJcUrn6-GLHG_pXgC7/edit?slide=id.p1#slide=id.p1) |
| 19:05-19:00 | - | 休憩 |
| 19:10-19:30 | [fujitatomoya](https://github.com/fujitatomoya) | [ROS 2 Executor](https://raw.githack.com/fujitatomoya/ros-japan-developer-kaigi/main/docs/ROSJPDev_20260803/ROS_2_Executor/ROS_2_Executor.html#1) |
| 19:30-19:45 | [MrBearing](https://github.com/MrBearing) | [get-ros2](https://docs.google.com/presentation/d/1dGYy77PtYX8rju3M9fH79T2oLMEntbJKvT4sl2Gmymg/edit?slide=id.p1#slide=id.p1) |
| 19:45-20:15 | - | 写真撮影 / Networking / Open Discussion |
| 20:15-20:30 | - | 撤収 |

<!---
Comment here
--->

---

# Networking / 食事 :cocktail:

## アルコール、ノンアル、食事が提供されます。
## [TriOrb Inc.](https://triorb.co.jp/) ありがとうね('◇')ゞ

<!---
Comment here
--->

---

# それでは始めましょう 🚀

日本でROS`開発`を盛り上げましょう 🥊🥊🥊

<!---
Comment here
--->
