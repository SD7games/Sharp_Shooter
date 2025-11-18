# Sharp Shooter  
A small first-person action shooter built in Unity as a personal gameplay project.  
The game features multiple weapons, enemy waves, destructible spawn portals, loot drops and polished FPS mechanics such as recoil, ADS accuracy, sprinting and camera shake.

Playable WebGL version:  
👉 **https://sd7games.itch.io/sharp-shooter**

---

## 🎮 Features

### ✅ Completed & Implemented  
- **Multiple Weapons** with ScriptableObject configuration:
  - damage  
  - fire rate  
  - accuracy and hip-fire spread  
  - ADS precision (no spread when aiming)  
  - magazine size  
  - reload time  
  - recoil pattern  
- **Recoil & Camera Shake** for each weapon.  
- **ADS System (Aim Down Sights):**  
  hip-fire is inaccurate, ADS is precise.  
- **Sprint System** with speed boost and custom audio.  
- **Loot Boxes:**  
  - ammo packs  
  - health packs  
- **Enemy & Portal System:**  
  - portals continuously spawn enemies  
  - portals and enemies have different HP  
  - destroying all portals completes the mission  
  - full victory/defeat state logic  

### 🤖 Enemy AI (NavMesh-based)  
- **Unity NavMesh Agents** used for pathfinding.  
- Enemies **actively chase the player** by calculating the shortest available route.  
- AI automatically:
  - goes around obstacles  
  - uses stairs and multi-level navigation  
  - updates the path dynamically when the player moves  
- Simple state machine: **idle → chase → attack**.  
- Designed to be lightweight for WebGL.  

### 🖥 UI & Polish  
- Full HUD: ammo counter, health bar, hit feedback.  
- Settings popup (audio, sensitivity options).  
- Custom animations: idle, firing, reload, ADS.  
- Custom audio: gunshots, reloads, footsteps, sprint.  
- **Post-processing:** bloom, vignette, color grading.  
- Clean project architecture based on low coupling and ScriptableObjects.

---

## 🧠 Tech & Architecture  
- Unity  
- C#  
- ScriptableObjects for weapon data  
- Animator state machines  
- Event-driven UI  
- Unity NavMesh & NavMesh Agents  
- Post-Processing Stack v2  
- Camera-based recoil & shake system  
- Simple enemy FSM (chase logic)

---

## 📂 Project Structure
```
/Assets
    /Animations
    /Audio
    /Prefabs
    /Scripts
        /Weapons
        /Player
        /Enemies
        /UI
        /Systems
    /SO (WeaponData)
    /Materials
    /Scenes

```

## 🎮 How to Play  
1. Play the browser version:  
   👉 https://sd7games.itch.io/sharp-shooter  
2. Destroy all portals to stop enemy waves.  
3. Collect ammo and health from loot boxes.  
4. Use ADS for accurate shooting.  
5. Sprint to reposition quickly.  

---

## 📸 Screenshots (optional)  
_Add gameplay images or GIFs here if you want._

---

## 👨‍💻 Developer  
**Oleksandr Tokarev** — Unity & C# Game Developer based in Finland.  
This project was created to practice and improve core FPS gameplay programming.

Open to work and collaboration.

