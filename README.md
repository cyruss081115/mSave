# mSave: Motion and Structural Awareness Video Editing

## Introduction:
- **Task**: Replace an object's texture in a video.  
- **Motivation**: Manual, frame-by-frame editing is labor-intensive and inconsistent.  
- **Key Insights**: A representation-based approach can fix motion-related artifacts.  
- **Contribution**: The mSave algorithm enables realistic, **dynamic video retexturing**.  

## Related Works:
- **Video Models**: These models are trained for general video understanding and editing but typically **require compute beyond consumer-grade GPUs**. They often **replace entire objects** instead of preserving structure through retexturing.  
- **Zero-shot Methods**: These approaches edit diffusion latents or attention maps in pre-trained text-to-image models. They are training-free but **struggle with structural consistency** and fine-grained control.  
- **Representation-based Methods**: Videos are encoded into alternative forms, where edits apply across frames. However, these methods often produce **inconsistent motion** or temporal artifacts.  

## Gallary
### Car turn
Prompt: A blue SUV  
<div style="display: flex; justify-content: space-between; align-items: center;">
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/original_car_turn.gif" alt="original" style="width: 100%; height: auto;">
        <p style="text-align: center;">Original Video</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/stablevideo_car_turn_blue.gif" alt="stable_video" style="width: 100%; height: auto;">
        <p style="text-align: center;">StableVideo</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/mSave_car_turn_blue.gif" alt="mSave" style="width: 100%; height: auto;">
        <p style="text-align: center;">mSave (Ours)</p>
    </div>
</div>

Prompt: An orange SUV  
<div style="display: flex; justify-content: space-between; align-items: center;">
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/original_car_turn.gif" alt="original" style="width: 100%; height: auto;">
        <p style="text-align: center;">Original Video</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/stablevideo_car_turn.gif" alt="stable_video" style="width: 100%; height: auto;">
        <p style="text-align: center;">StableVideo</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/mSave_car_turn.gif" alt="mSave" style="width: 100%; height: auto;">
        <p style="text-align: center;">mSave (Ours)</p>
    </div>
</div>

### Bicycle Tali  
Prompt: Kid riding a blue bicycle  
<div style="display: flex; justify-content: space-between; align-items: center;">
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/original_bicycle_tali.gif" alt="original" style="width: 100%; height: auto;">
        <p style="text-align: center;">Original Video</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/stablevideo_bicycle_tali.gif" alt="stable_video" style="width: 100%; height: auto;">
        <p style="text-align: center;">StableVideo</p>
    </div>
    <div style="width: 33.33%; text-align: center;">
        <img src="assets/mSave_bicycle_tali.gif" alt="mSave" style="width: 100%; height: auto;">
        <p style="text-align: center;">mSave (Ours)</p>
    </div>
</div>


