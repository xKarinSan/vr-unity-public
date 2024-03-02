# Boilerplate for Unity VR
## 📦 Package(s) used
- XR Interaction Toolkit (2.5.2 at the time of writing this)

### 🗂 Folder structure
```
|- Materials
|- Prefabs
   |- Container.prefab
   |- GrabInteractableCube.prefab
   |- SimpleInteractableCube.prefab
   |- XR Device Controller Handler.prefab

|- Samples
   |- XR Interaction Toolkit
|- Scenes
   |- BasicActions
      |- ControllerSceneTemplate.unity
      |- Interactors.unity
      |- Socket.unity
      |- Teleporter.unity
   |- Maps
|- Scripts
|- XR (don't touch)
|- XRI (don't touch)
```
### ⚠️🗂 Important folders
- ```Materials```: Where you put your materials
- ```Prefabs```: Where you put your reusable prefabs
- ```Samples```: Where the imported content samples are at
- ```Scenes```: Where you put all your scenes
- ```BasicActions```: Where the boilerplate is at
- ```Map```: Where you put all map-related scenes
- ```Scripts```: Where you put all your scripts

### ⚠️🧊 Important Prefabs
- ```Container.prefab```: This contains a sockets slot to allow 3D GameObjects to be placed inside by the VR controller
- ```GrabInteractableCube.prefab```: A cube that can be grabbed with the VR controller.
- ```SimpleInteractableCube.prefab```: A cube that **cannot** be grabbed with the VR controller, but **it is detected** by the VR Controller's ray interactor
- ```XR Device Controller Handler.prefab```: This contains the basic boilerplate of the VR origin (from the XR Interaction Toolkit), combined with the VR Device Simulator

### ⚠️🌁 Important Scenes
- ```ControllerSceneTemplate.unity```: Where the barebones scene with the basic controller is at (Reusable)
- ```Interactors.unity```: Where the basic interactable scene are at (Mainly for hovering & grabbing)
- ```Socket.unity```: Where the socket interactable scene is at (For placing items inside their socket slots)
- ```Teleporter.unity```: Where the teleporter scene is at

## ❓ How do we implement each basic action?
- Basic VR Controller: Can be found at: ```Samples``` > ```XR Interaction Toolkit``` > ```2.5.2``` > ```Starter Assets``` > ```Prefabs``` > ```Prefabs``` > ```XR Interaction Setup.prefab```
- Socket Interaction: Just place a ```XR Socket Interactor``` script (inside XR Interaction Toolkit).
- Grab Interaction: Just place a ```XR Socket Interactor``` script component (inside XR Interaction Toolkit) inside your 3D GameObject.
- Socket Interaction: Just place a ```XR Grab Interactor``` script component (inside XR Interaction Toolkit) inside your 3D GameObject.
- Hovering glow effect (3D GameObjects): Just place a ```XR Grab Interactor``` or a ```XR Simple Interactor``` script (inside XR Interaction Toolkit) inside your 3D GameObject. Then, go to ```Interactable Events``` and then follow this <a target="_blank" href="https://github.com/xKarinSan/unity-vr-boilerplate/assets/47315402/f25e0dc3-a157-4709-84b8-2f848d58c420">screenshot</a>.
- Teleportation: Just place a ```Teleportation Area``` script component inside your 3D GameObject. (You can even place it in specific areas to limit the teleportation to fall within said area) 

## ❤️ Usage of the boilerplate
1. Clone the repository/download as zip (and extract the zip)
2. Open it inside your Unity Hub. (We assume you already have this installed)
3. Explore and have fun!


