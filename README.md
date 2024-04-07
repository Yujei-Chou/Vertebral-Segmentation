# Vertebral-Segmentation
## Outline:
Build a deep learning method to perform automatic segmentation of vertebral bones.

## Method:
1. UNet architecture is chosen as the fundamental model to implement the segmentation task.
2. During the downsampling process, we utilize deeper networks and incorporate Channel-wise and Pixel-wise attention mechanisms to facilitate better feature extraction and fusion in the model.
   - Deeper networks: ResNet
   - Attention mechanism: Squeeze-and-Excitation Networks, Attention Gate
   <br></br>
   <img src="https://github.com/Yujei-Chou/Vertebral-Segmentation/assets/56510169/54ab6566-3afe-4a7c-8e5e-b80888a97099" alt="drawing" width="600"/>

## Results:
- Dice Score Comparison:
  <br></br>
  | ResNet | SE-block | Attention Gate | 3-fold Average Dice Score |
  | :----: | :------: | :------------: | :-----------------------: |
  |        |          |                |            0.718          |
  |    v   |          |                |            0.806          |
  |    v   |     v    |                |            0.849          |
  |    v   |     v    |       v        |            0.860          |

- Segmentation Results Comparison:
  1. Example 1:
     ![image](https://github.com/Yujei-Chou/Vertebral-Segmentation/assets/56510169/b1737569-4eb4-4789-9ba4-5167b4b6785c)
  2. Example 2:
     ![image](https://github.com/Yujei-Chou/Vertebral-Segmentation/assets/56510169/dd649c9e-7f6f-4f4f-ae15-955334ba8bb8)

 
