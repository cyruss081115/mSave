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

## Gallery

### Car Turn

| Prompt            | Original Video                          | StableVideo                          | mSave (Ours)                          |
|--------------------|-----------------------------------------|---------------------------------------|---------------------------------------|
| A blue SUV        | ![Original](assets/original_car_turn.gif) | ![StableVideo](assets/stablevideo_car_turn_blue.gif) | ![mSave](assets/mSave_car_turn_blue.gif) |
| An orange SUV     | ![Original](assets/original_car_turn.gif) | ![StableVideo](assets/stablevideo_car_turn.gif) | ![mSave](assets/mSave_car_turn.gif) |

### Bicycle Tali

| Prompt                     | Original Video                          | StableVideo                          | mSave (Ours)                          |
|-----------------------------|-----------------------------------------|---------------------------------------|---------------------------------------|
| Kid riding a blue bicycle  | ![Original](assets/original_bicycle_tali.gif) | ![StableVideo](assets/stablevideo_bicycle_tali.gif) | ![mSave](assets/mSave_bicycle_tali.gif) |
