# current task current

更新日: 2026-03-16

## 現在の前提

- 入院予定日は `2026-03-17`
- `COMMAND_CENTER` = 運用の正本
- `X:\SakuriumStudio_Assets` = 実データの正本
- `command-center-window` = 共有窓 / 参照窓

## 結論

今回の主眼は、`hospital-browser-ops` の入口を最小構成で作り、病院中の本線を `GitHub共有窓 + ブラウザ運用` として迷わず使える形にすることです。

## 今回の優先順位

1. 病院ブラウザ入口の実体ファイルを最小構成で置く
2. 病院側の更新先を `hospital_status_current.md` 1 本に固定する
3. `Sunshine / Moonlight` を保険枠として位置づける
4. `外部WOL` は今回は保留のまま据え置く

## 今回やらないこと

- 病院Wi-Fiの実地確認
- テザリング長時間運用の実地確認
- `Sunshine / Moonlight` の本線運用化
- ルーター設定の本番反映
- 外部WOLの本番導入
- 入口以外の資料の大規模整理

## 今回の完成条件

- 入口がある
- `today_current.md` で今の主題が分かる
- 正本の境界が分かる

## 現在地

- private 側の plan と closeout は固定済み
- `hospital_status_current.md` を病院側更新先として使う前提
- `browser_links_current.md` を最小リンク集として使う前提
- `browser_emergency_backup.md` を保険導線として分離する
- 入院中の本線は `GitHub共有窓 + ブラウザ運用`
- `Sunshine / Moonlight` は条件が良い時だけ使う保険枠
- `外部WOL` は Windows 側とルーター側の前提確認までは完了したが、今回は保留

## 今日の止めどころ

- 入口に置く実体を最小構成で作る
- 兄弟側に渡す材料をこの構成で揃える
