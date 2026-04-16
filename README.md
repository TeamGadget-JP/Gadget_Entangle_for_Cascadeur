# Gadget Entangle for Cascadeur (GEC)

Welcome to "Gadget Entangle for Cascadeur" (GEC)! 
This tool provides ultra-low latency, real-time Live Previz synchronization directly between Cascadeur and Unity's Play Mode.

## ⚠️ Important Notice / 免責事項
* **No Support (As-Is):** I am a solo developer working in the industrial engineering field. Therefore, providing individual technical support is practically impossible. This tool is provided "as-is" and completely free, without official support.
* **License Requirement:** To comply with Nekki's licensing terms, **this tool does NOT work with the Cascadeur Free license.** A valid Indie, Pro, or Teams license logged into Cascadeur is strictly required to establish the connection.

## 🙏 Support the Project!
This tool is completely free to use. However, if you find it helpful for your workflow, I would greatly appreciate it if you could **Subscribe to my YouTube channel and Like the videos!**
Your support is my greatest motivation to continue developing tools like this (including an upcoming iClone sync tool!).
▶️ https://youtu.be/kNBWSCf2cIw

---

## 🚀 Installation Guide* **Windows Only:** This tool currently only supports Windows environments. macOS and Linux are not supported.

### 1. Cascadeur Setup
1. Download the `gec_live_link.pyc` file from this repository.
2. Place the `.pyc` file into your Cascadeur Python plugins folder: `[Cascadeur Install Directory]\resources\scripts\python\commands\`
3. Restart Cascadeur.

### 2. Unity Setup
1. Create a **New Empty Project** in Unity (Recommended version: Unity 6 / URP).
2. Download the `GEC_EvaluationBuild.unitypackage` from this repository. *(Note: File name remains 'EvaluationBuild' but is fully functional).*
3. Import the package into your Unity project (`Assets > Import Package > Custom Package...`).

## 🎮 How to Use (Testing the Real-time Sync)
1. **Open the Scene:** Open the `SampleScene` included in the package.
2. **Launch Dashboard:** From the top menu, click `Gadget > Gadget Entangle Dashboard`.
3. **Start Unity:** Press the **Play Button** in Unity to enter Play Mode.
4. **Connect:** Click the `🟢 CONNECT (Start)` button on the Dashboard.
5. **Sync in Cascadeur:** Open Cascadeur, run the script via `Commands > Gadget Entangle for Cascadeur`, and verify that `standing by!` appears in the Event log. You are good to go!

You can now freely control the character in Cascadeur and experience the ultra-low latency synchronization while the Unity Play Mode environment (physics, lighting, etc.) is fully active!

---
---

# Gadget Entangle for Cascadeur (日本語版)

「Gadget Entangle for Cascadeur (GEC)」へようこそ！
このツールは、CascadeurとUnity（プレイモード）を直接繋ぎ、超低遅延のリアルタイム同期（Live Previz）を実現します。

## ⚠️ 重要な注意事項（必ずお読みください）
* **サポートなし（現状渡し）:** 開発者は普段、別の本業を抱える個人エンジニアです。そのため、個別の環境に合わせた技術サポートを提供することは事実上不可能です。本ツールは「完全無料・サポート対象外」として提供されます。
* **ライセンス制限:** 開発元（Nekki）のライセンス規約を厳守するため、**本ツールはCascadeurの「Freeライセンス」では動作しない仕様**となっております。接続には Indie、Pro、Teams のいずれかの有効なライセンスが必要です。

## 🙏 開発者からのお願い
本ツールは完全無料でお使いいただけます。もし皆様の制作のお役に立てましたら、ぜひ**YouTubeチャンネルの登録と高評価**をお願いいたします！
皆様からの応援が、今後の開発（現在進行中のiClone同期ツールなど）の最大のモチベーションになります！
▶️ https://youtu.be/kNBWSCf2cIw

---

## 🚀 導入手順* **Windows専用:** 本ツールは現在、Windows環境でのみ動作します。macOSやLinuxには対応しておりません。

### 1. Cascadeur側の準備
1. このリポジトリから `gec_live_link.pyc` をダウンロードします。
2. CascadeurのPythonプラグインフォルダに配置します：`[Cascadeurインストール先]\resources\scripts\python\commands\`
3. Cascadeurを再起動します。

### 2. Unity側の準備
1. Unityで**空の新規プロジェクト**を作成します（推奨：Unity 6 / URP環境）。
2. このリポジトリから `GEC_EvaluationBuild.unitypackage` をダウンロードします。
3. Unityプロジェクトにインポートします（`Assets > Import Package > Custom Package...`）。

## 🎮 使い方（リアルタイム同期の実行）
1. **シーンを開く:** パッケージ内の `SampleScene` を開きます。
2. **ダッシュボード起動:** Unity上部メニューから `Gadget > Gadget Entangle Dashboard` をクリックします。
3. **Unity再生:** Unityの **Playボタン** を押してプレイモードに入ります。
4. **接続待機:** ダッシュボードの `🟢 CONNECT (Start)` ボタンを押します。
5. **Cascadeurで同期開始:** Cascadeurを開き、`Commands > Gadget Entangle for Cascadeur` スクリプトを実行して、Event logに `standing by!` が表示されればOKです！

これで準備完了です！Cascadeur側でキャラクターを動かすと、Unityのプレイモード上で物理演算やライティングが効いた状態のまま、超低遅延でモーションが同期します！
