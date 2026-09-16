# 🕹️ INFRA QUEST: Resource Tetris v2

> **SRE & インフラエンジニア専用 キャパシティ管理＆パケットスタックアーケード**  
> Webブラウザで動作する、本格レトロスタイルのインフラエンジニア向けテトリスゲーム。

![License](https://img.shields.io/badge/license-MIT-green.svg)
![HTML5](https://img.shields.io/badge/HTML5-SingleFile-orange.svg)
![LocalStorage](https://img.shields.io/badge/Data-LocalStorage-blue.svg)

---

## 🌟 特徴 (Features)

- **🖥️ インフラ・SRE用語に全面チューニング**
  - ブロック配置 → `Pod / コンテナリソース配備`
  - 4ライン消去 (TETRIS) → `K8s AUTO-SCALE!`
  - ライン消去 → `GC NODES (メモリ・ノード解放)`
  - スコア → `THROUGHPUT (RPS / QPS)`
  - ゲームオーバー → `CRASH: KILLED BY OOM-KILLER!`
- **📊 プレイヤーデータ＆SRE称号システム (LocalStorage)**
  - 最高RPS（ハイスコア）、通算デプロイ回数、累計GC解放ノード数、通算稼働時間を自動保存
  - プレイ実績に応じて `JUNIOR OPERATOR` から `GRAND SRE LEGEND` まで称号が自動ステップアップ
  - 直近5回のデプロイログ（スコア履歴）を表示
- **🔊 WebAudio API 8-Bit サウンド＆パーティクル演出**
  - 外部音源ファイル不要。ブラウザ内蔵オシレーターによるリアルタイム8bitレトロ効果音
  - ライン消去時の鮮やかなパーティクル＆画面シェイク演出
- **📱 マルチデバイス＆レスポンシブ対応**
  - キーボード操作（WASD / 矢印 / スペース / C / P / R）
  - スマホ・タブレット用タッチコントローラー対応

---

## 🎮 操作方法 (Controls)

| キー | アクション |
| :--- | :--- |
| `←` `→` / `A` `D` | Pod位置シフト（左右移動） |
| `↑` / `W` `X` | Pod右回転 |
| `Z` | Pod左回転 |
| `↓` / `S` | ローリングドロップ（ソフトドロップ） |
| `Space` | 即時デプロイ（ハードドロップ） |
| `C` / `Shift` | STAGING退避（HOLD） |
| `P` | メンテナンス中断（一時停止） |
| `R` | クラスタ再起動（リスタート） |

---

## 🚀 動作方法 (How to Run)

単体HTMLファイルとして完結しているため、サーバー構築や `npm install` 等の依存関係は不要です。

1. `index.html` をダブルクリックしてブラウザで開く
2. または GitHub Pages にプッシュして公開

---

## 🌐 GitHub Pages での公開手順

```bash
# 1. 新規ディレクトリを作成して移動
mkdir infra-quest-tetris
cd infra-quest-tetris

# 2. リポジトリの初期化
git init

# 3. 変更の追加とコミット
git add .
git commit -m "feat: Initial commit for Infra Quest Tetris v2"

# 4. GitHubに作成した空リポジトリにプッシュ
git branch -M main
git remote add origin https://github.com/<あなたのユーザー名>/infra-quest-tetris.git
git push -u origin main
```

**GitHub Settings -> Pages** より Branch `main` を指定すると、数分で無料配信が完了します。

---

## 📄 ライセンス

MIT License
