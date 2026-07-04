The beta version of **Cascadeur Entangle for Unity (CEU)**, 
the successor to **Gadget Entangle for Cascadeur (GEC)**, is now available.
While inheriting the core functionality of GEC, CEU has been further refined to make it easier to use and more efficient.
Please give both versions a try and use whichever one works best for your workflow.
**Gadget Entangle for Cascadeur (GEC)**
https://github.com/TeamGadget-JP/Cascadeur_Entangle_for_Unity


Gadget Entangle for Cascadeur (GEC)の後継となる
Cascadeur Entangle for Unity (CEU)をベータ・リリースしています。
基本機能は継承しつつ、より一層使い易く且つ効率良くブラッシュアップしました
是非とも使い比べて使い易い方を使用して下さい。
[Gadget Entangle for Cascadeur (GEC)](https://github.com/TeamGadget-JP/Cascadeur_Entangle_for_Unity)


# Gadget Entangle for Cascadeur (GEC)

Welcome to "Gadget Entangle for Cascadeur" (GEC)! 
This tool provides ultra-low latency, real-time Live Previz synchronization directly between Cascadeur and Unity's Play Mode.

## ⚠️ Important Notice
* **No Support (As-Is):** I am a solo developer working in the industrial engineering field. Therefore, providing individual technical support is practically impossible. This tool is provided "as-is" and completely free, without official support.
* **License Requirement:** To comply with Nekki's licensing terms, **this tool does NOT work with the Cascadeur Free license.** A valid Indie, Pro, or Teams license logged into Cascadeur is strictly required to establish the connection.

## 🙏 Support the Project!
This tool is completely free to use. However, if you find it helpful for your workflow, I would greatly appreciate it if you could **Subscribe to my YouTube channel and Like the videos!**
Your support is my greatest motivation to continue developing tools like this (including an upcoming iClone sync tool!).
▶️ [https://youtu.be/kNBWSCf2cIw](https://www.youtube.com/channel/UCj9OYwzMAIgYAeVkTV4wczw)

---
**Windows Only:** This tool currently only supports Windows environments. macOS and Linux are not supported.

## 🚀 Installation Guide* 

### 1. Cascadeur Setup
1. Download the `gec_live_link.pyc` file from this repository.
2. Place the `.pyc` file into your Cascadeur Python plugins folder: `[Cascadeur Install Directory]\resources\scripts\python\commands\`
3. Restart Cascadeur.

### 2. Unity Setup
1. Create a **New Empty Project** in Unity (Recommended version: Unity 6 / URP).
2. Download the `GEC_v1.0.0.unitypackage` from this repository. *(Note: File name remains 'EvaluationBuild' but is fully functional).*
3. Import the package into your Unity project (`Assets > Import Package > Custom Package...`).

## 🎮 How to Use (Testing the Real-time Sync)
1. **Open the Scene:** Open the `SampleScene` included in the package.
2. **Launch Dashboard:** From the top menu, click `Gadget > Gadget Entangle Dashboard`.
3. **Start Unity:** Press the **Play Button** in Unity to enter Play Mode.
4. **Connect:** Click the `🟢 CONNECT (Start)` button on the Dashboard.
5. **Sync in Cascadeur:** Open Cascadeur, run the script via `Commands > Gadget Entangle for Cascadeur`, and verify that `standing by!` appears in the Event log. You are good to go!

You can now freely control the character in Cascadeur and experience the ultra-low latency synchronization while the Unity Play Mode environment (physics, lighting, etc.) is fully active!

## GEC Multi-Character Synchronization with Identical Bone Names  
### Example: Synchronizing Two Characters
### Prerequisite
GEC uses only bone names as IDs.  
If multiple characters have identical bone names, a prefix must be added to distinguish them.
### Procedure
1. Import the first character normally.  
   Do not use any bone prefix.  
   Then rig the character using **RIG HELPER**.
2. Create a new scene from **File -> New Scene**.  
   Import the second character into that new scene, and rig it using **RIG HELPER**.
3. Save the second character scene as a native Cascadeur file (`.casc`) with any name.
4. Return to the scene containing the first character.  
   Import the `.casc` file saved in step 3 using:  
   **File -> Import -> Import Scene To Current...**
5. The second character will now be imported into the scene containing the first character.  
   If the characters have identical bone names, Cascadeur will automatically add a prefix such as `character1:` to the second character.
6. In Unity, configure the Cascadeur-side bone names for each character individually in the character-specific bone settings.

### ⚠️ Prop meshes not syncing in Unity Editor (URP Environment)
In newer Unity URP environments, you might encounter an issue where a Prop's Transform values update correctly, but the mesh itself remains frozen in the Scene view. 
This is caused by the "GPU Resident Drawer," an aggressive rendering cache feature in URP, interfering during Editor mode. Please follow these steps to resolve it:

1. Select your active **URP Asset** in the Project window (e.g., `Assets/Settings/PC_RPAsset`).
   *(Note: If you cannot find it, go to `Edit > Project Settings > Graphics` and check the asset assigned at the very top.)*
2. In the Inspector window, navigate to the `Rendering` section.
3. Change the `GPU Resident Drawer` setting from `Instanced Drawing` to **`Disabled`**.

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
▶️ [https://youtu.be/kNBWSCf2cIw](https://www.youtube.com/channel/UCj9OYwzMAIgYAeVkTV4wczw)

---
**Windows専用:** 本ツールは現在、Windows環境でのみ動作します。macOSやLinuxには対応しておりません。

## 🚀 導入手順* 

### 1. Cascadeur側の準備
1. このリポジトリから `gec_live_link.pyc` をダウンロードします。
2. CascadeurのPythonプラグインフォルダに配置します：`[Cascadeurインストール先]\resources\scripts\python\commands\`
3. Cascadeurを再起動します。

### 2. Unity側の準備
1. Unityで**空の新規プロジェクト**を作成します（推奨：Unity 6 / URP環境）。
2. このリポジトリから `GEC_v1.0.0.unitypackage` をダウンロードします。
3. Unityプロジェクトにインポートします（`Assets > Import Package > Custom Package...`）。

## 🎮 使い方（リアルタイム同期の実行）
1. **シーンを開く:** パッケージ内の `SampleScene` を開きます。
2. **ダッシュボード起動:** Unity上部メニューから `Gadget > Gadget Entangle Dashboard` をクリックします。
3. **Unity再生:** Unityの **Playボタン** を押してプレイモードに入ります。
4. **接続待機:** ダッシュボードの `🟢 CONNECT (Start)` ボタンを押します。
5. **Cascadeurで同期開始:** Cascadeurを開き、`Commands > Gadget Entangle for Cascadeur` スクリプトを実行して、Event logに `standing by!` が表示されればOKです！

これで準備完了です！Cascadeur側でキャラクターを動かすと、Unityのプレイモード上で物理演算やライティングが効いた状態のまま、超低遅延でモーションが同期します！

## GECで同名ボーンを持つキャラクターをマルチ同期する手順
例：2体同期の場合
### 前提
GECは、ボーン名を同期対象のIDとして使用しています。  
そのため、同名ボーンを持つ複数キャラクターを同時に同期する場合は、2体目以降のボーン名にプレフィックスを付与する必要があります。
### 手順
1. 1体目のキャラクターを通常通りインポートします。  
   この時点では、ボーン・プレフィックスは付けません。  
   その後、RIG HELPERでリギングを行います。
2. `File -> New Scene` で新しいシーンを作成します。  
   その新しいシーンに2体目のキャラクターをインポートし、RIG HELPERでリギングを行います。
3. 2体目のキャラクターが含まれるシーンを、任意の名前でCascadeurネイティブ形式（`.casc`）として保存します。
4. 1体目のキャラクターがいるシーンに戻り、  
   `File -> Import -> Import Scene To Current...` から、手順3で保存した `.casc` ファイルをインポートします。
5. これで、1体目のキャラクターがいるシーンに2体目のキャラクターが追加されます。  
   同名ボーンが存在する場合、Cascadeur側で2体目のキャラクターのボーン名に自動的に `character1:` というプレフィックスが付与されます。
6. Unity側のキャラクター個別ボーン設定で、Cascadeur側のボーン名に合わせて設定してください。

### ⚠️ プロップのメッシュがエディターで同期しない場合 (URP環境)
最新のUnity URP（Universal Render Pipeline）環境において、Cascadeurからの接続時にプロップ（小道具）のTransform数値は更新されるのに、メッシュの見た目がシーンビュー上で追従しない現象が発生する場合があります。
これはURPの強力な描画キャッシュ機能がエディターモードで干渉しているために起こります。以下の手順で設定を変更してください。

1. Projectウィンドウから、現在使用している**URPアセット**を選択します（例: `Assets/Settings/PC_RPAsset` など）。
   *(※場所が不明な場合は、上部メニューの `Edit > Project Settings > Graphics` を開き、一番上に設定されているファイルを確認してください)*
2. Inspectorウィンドウ上部の `Rendering` 項目を開きます。
3. `GPU Resident Drawer` の設定を `Instanced Drawing` から **`Disabled`** に変更します。

## 🚀 Roadmap / Upcoming Features (次期アップデート予定)
We are constantly improving the tool. The following features will be added in the next minor version update:
現在、以下の機能を次期マイナーバージョンアップに向けて開発中です：

- [ ] **Hybrid Lerp Adjustment UI (部位別Lerp調整UI)**
  - Users will be able to adjust Lerp values (0 - 60) per body part to completely prevent foot sliding and control character weight.
  - 足滑りを完全に防ぐため、ユーザーが部位ごと（足、体幹など）の補間強度（0〜60）をUIから直接チューニングできるようになります。

## ⚖️ License
This software is provided under a proprietary license. Unauthorized redistribution, modification, and reverse engineering (decompiling) are strictly prohibited. 
For full details, please read the [LICENSE](./LICENSE) file.

本ソフトウェアは独自ライセンスのもとで提供されています。無断再配布、改変、および逆コンパイル（リバースエンジニアリング）は固く禁じられています。
詳細については、[LICENSE](./LICENSE) ファイルをご確認ください。
