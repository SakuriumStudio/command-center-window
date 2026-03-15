# COMMAND_CENTER 最小骨組み案

更新日: 2026-03-15

## 結論

今回の `COMMAND_CENTER` は、入院前に無理なく回せる最小構成に絞る。
役割は「司令塔」「入口」「進行中管理」「接続手順」の4つに限定する。

`SakuriumStudio_Assets` は実データ置き場として並列に置き、`COMMAND_CENTER` の下に入れない。
今回の完成条件は、以下の3つが見えることだけで十分。

- 入口がある
- `today.md` で今の主題が分かる
- タブレットが最低限使える

## 前提

- ルート構成は以下で固定する

```text
X:\COMMAND_CENTER
X:\SakuriumStudio_Assets
```

- `COMMAND_CENTER` は運用側
- `SakuriumStudio_Assets` は実データ側
- `G:` は保管・履歴・再利用側
- 今回は見た目の完成度より、迷わず再開できることを優先する

## 最小骨組み

```text
X:\COMMAND_CENTER
  README.md
  AGENTS.md
  00_DASHBOARD\
    today.md
    quick_links.md
  01_INBOX\
  02_ACTIVE\
  03_RUNBOOKS\
    tablet_minimum_setup.md
    remote_access_notes.md
  _codex\
    current-task.md
```

## 各フォルダの役割

### `README.md`
- 人間が最初に開く入口
- `COMMAND_CENTER` が何を置く場所かを短く説明する
- `SakuriumStudio_Assets` と `G:` への導線を書く

### `AGENTS.md`
- `COMMAND_CENTER` 側の運用ルール正本
- チーム役割、返答形式、判断待ちの扱いを書く
- `SakuriumStudio_Assets` 側の `AGENTS.md` と分けるなら、ここを上位運用ルールにする

### `00_DASHBOARD\`
- 今日どこを見ればいいかを一発で分かるようにする
- `today.md` は今の主題、止めどころ、次の一手
- `quick_links.md` はよく使う絶対パスや起点メモ

### `01_INBOX\`
- 生メモ、音声起こし、仮置きメモの受け皿
- 未整理のものをいったん受ける場所
- ここは整理前提なので、綺麗さを求めない
- 完成物は置かない

### `02_ACTIVE\`
- 今進めている作業メモ、途中案、短期資料
- 「今触るもの」をまとめる
- 完了後は `SakuriumStudio_Assets` または `G:` へ振り分ける

### `03_RUNBOOKS\`
- 繰り返し使う手順書
- 今回は最低限、タブレットと接続系だけでよい
- 例:
  - `tablet_minimum_setup.md`
  - `remote_access_notes.md`

### `04_CONNECTIONS\` 以降
- 接続先一覧、機器名、接続メモ、ネットワーク前提
- 秘密情報を平文で置かない
- 必要なら「何をどこで確認するか」だけを書く
- `04_CONNECTIONS\`、`05_STAGING\`、`06_TOOLBOX\` は必要になった時点で空箱を作ればよい
- 入院前の必須ではない

### `_codex\`
- Codex 運用の核
- 今回の必須は `current-task.md` のみ
- `active_projects.md` と `decision_notes.md` は後追いでよい

## 最低限作るべきファイル

### 必須

- `X:\COMMAND_CENTER\README.md`
- `X:\COMMAND_CENTER\AGENTS.md`
- `X:\COMMAND_CENTER\00_DASHBOARD\today.md`
- `X:\COMMAND_CENTER\00_DASHBOARD\quick_links.md`
- `X:\COMMAND_CENTER\03_RUNBOOKS\tablet_minimum_setup.md`
- `X:\COMMAND_CENTER\_codex\current-task.md`

### 余力があれば

- `X:\COMMAND_CENTER\03_RUNBOOKS\remote_access_notes.md`
- `X:\COMMAND_CENTER\04_CONNECTIONS\`
- `X:\COMMAND_CENTER\05_STAGING\`
- `X:\COMMAND_CENTER\06_TOOLBOX\`
- `X:\COMMAND_CENTER\_codex\active_projects.md`
- `X:\COMMAND_CENTER\_codex\decision_notes.md`
- `X:\COMMAND_CENTER\06_TOOLBOX\tool_index.md`

## `README.md` 冒頭に置く3行

`COMMAND_CENTER` の `README.md` の先頭には、最低限次の3行をそのまま置いてよい。

- 入口がある
- `today.md` で今の主題が分かる
- タブレットが最低限使える

## `today.md` の必須ルール

- 次に開くファイルを1つだけ書く
- 複数候補を書かない
- 作業を止める前に、未完了でも更新する

## 今は作らなくてよいもの

- 四半期棚卸しの本格運用
- 大量のテンプレ整理
- 見た目を整えるためだけのフォルダ追加
- archive 台帳の本格記入
- ツール本体の大移設

## この骨組みの狙い

- まず `COMMAND_CENTER` を「戻る場所」にする
- 実データと運用を分ける
- 入院中でも、何を見ればよいか迷わない状態にする
- 後から拡張しやすいが、今は重くしない

## 完成ライン

以下が揃えば、今回の最低限完成として扱ってよい。

- `COMMAND_CENTER` の入口がある
- 進行中の主題が1枚で分かる
- タブレット関連の最低限手順がある
- `SakuriumStudio_Assets` と役割が混ざっていない
- 余力枠の枝を育てなくても止めてよい
