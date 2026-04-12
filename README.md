# Gadget Entangle for Cascadeur (Evaluation Build)　Important: This only works in Windows environments.

Welcome to the evaluation repository for "Gadget Entangle."
This package contains the compiled core logic (DLLs/PYC) designed to demonstrate the zero-latency "Real-time Live Previz" capabilities directly within Unity's Play Mode.

## 📥 Installation Guide

### 1. Cascadeur Setup
1. Download the `gec_live_link.pyc` file from this repository.
2. Place the `.pyc` file into your Cascadeur Python plugins folder:
   `[Cascadeur Install Directory]\resources\scripts\python\commands\`
3. Restart Cascadeur.

### 2. Unity Setup
1. Create a **New Empty Project** in Unity (Recommended version: Unity 6 / URP).
2. Download the `GEC_EvaluationBuild.unitypackage` from this repository.
3. Import the package into your Unity project (`Assets > Import Package > Custom Package...`).

## 🚀 How to Evaluate (Testing the Real-time Sync)

1. **Open the Scene:** Open the `SampleScene` included in the package.
2. **Launch Dashboard:** From the top menu, click `Gadget > Gadget Entangle Dashboard`.
3. **Start Unity:** Press the **Play Button** in Unity to enter Play Mode.
4. **Connect:** Click the `🟢 CONNECT (Start)` button on the Dashboard.
5. **Sync in Cascadeur:** Open Cascadeur, run the `Gadget Entangle (Subscribe)` script, and select `Sync on Focus`.

You can now freely control the character in Cascadeur and experience the ultra-low latency synchronization while the Unity Play Mode environment (physics, lighting, etc.) is fully active.

*Note: The authorization module is active in this build. A valid Indie, Pro, or Teams license logged in Cascadeur is required to establish the connection.*
