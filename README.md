# 星域戦記 (Pick Duel) — オフライン版

5枚の防衛線をめぐるカードバトルゲーム

## ⚙️ セットアップ（GitHub Pages）

### 1. リポジトリ作成
```
リポジトリ名: pick-duel
Public
```

### 2. ファイルアップロード
```
pick_duel_package/
├── index.html
├── sw.js
└── README.md
```
をリポジトリにpush

### 3. Pages設定
Settings → Pages → Deploy from branch → Save

### 4. アクセス
```
https://ユーザー名.github.io/pick-duel
```

## 📱 iPhoneで遊ぶ

1. Safari で ↑ のURLを開く
2. 下のシェアボタン → 「ホーム画面に追加」
3. **重要：一度ホーム画面から起動** （Service Worker登録のため）
4. 以降、オフラインでも遊べます

## 🔄 リロード対策

- **localStorageで自動保存** — ゲーム状態は自動保存
- **network-first キャッシュ** — リロード時は最新版を取得
- **ネット無い時** — キャッシュから読み込み

誤ってリロード → 引き直し（状態は保持）→ 続行 OK

## 📝 更新したい場合

```
git add .
git commit -m "update"
git push
```

GitHub Pages が自動デプロイ。少し待つと新版が反映されます。

## ⚠️ キャッシュをクリアしたい

iPhone設定 → Safari → 履歴とWebサイトデータを削除

---

**開発**: Koki | **v59** | Service Worker対応 ✓
