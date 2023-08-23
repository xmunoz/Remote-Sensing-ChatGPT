# RS-ChatGPT: Human-Interactive Remote Sensing Task Solving with ChatGPT
Introduction
----
Remote Sensing ChatGPT(RS-ChatGPT) is an open source tool for solving remote sensing tasks with ChatGPT in an interactive way.ChatGPT acts as an expert to response to users' linguistic resquests based on the input remote sensing image.  It supports various interpretation tasks that are trained on remote sensing datasets. To help ChatGPT better understand remote sensing knowledge, image captioning and scene understanding of remote sensing image are set as prefix.RS-ChatGPT is developed based on the Visual ChatGPT project.

Generally, RS-ChatGPT includes four steps in implementation:
* Prompt Template Generation
* Task Planning
* Task Execution
* Response Genration
  

Remote Sensing ChatGPT is an open source project that welcome any contribution and feedback. Please contact us with haonan.guo@whu.edu.cn

Updates
----
Initial release：2023.08.23
* TODO: Provide an interactive interface
  
The code
----
### Requirements
Please Refer to [requirements.txt](https://github.com/HaonanGuo/Remote-Sensing-ChatGPT/blob/main/requirements.txt)

### Usage
Clone the repository:git clone [https://github.com/HaonanGuo/BFSeg-Efficient-Building-Footprint-Segmentation-Framework.git](https://github.com/HaonanGuo/Remote-Sensing-ChatGPT)<br/>

->Run [rs_chatgpt.py](https://github.com/HaonanGuo/Remote-Sensing-ChatGPT/blob/main/rs_chatgpt.py) 

### Supported Function
| Function |    Description  | Method | Pretrain Dataset     | Model Weights     |
| :--------: | :--------: | :--------: | :--------: | :--------: |
| Image Captioning | Describe the remote sensing image | [BLIP](https://icml.cc/virtual/2022/spotlight/16016) | [BLIP Dataset](https://icml.cc/virtual/2022/spotlight/16016)| [weight](https://github.com/salesforce/BLIP) |
| Scene Classification | Classify the type of scene | [ResNet](https://arxiv.org/abs/1512.03385) | [AID Dataset](http://www.captain-whu.com/project/AID/)| [weight](https://pan.baidu.com/s/1yNgUQKieZBEJZ0axzN4tiw?pwd=RSGP) |
| Object Detection | Detect RS object from image | [YOLO v5](https://zenodo.org/badge/latestdoi/264818686) | [DOTA](http://captain.whu.edu.cn/DOTAweb)| [weight](https://pan.baidu.com/s/1XTG-MLxx5_D0OO6M80OP1A?pwd=RSGP) |
| Instance Segmentation | Extract Instance Mask of certain object | [SwinTransformer+UperNet](https://github.com/open-mmlab/mmsegmentation) | [LoveDA](https://github.com/Junjue-Wang/LoveDA)| [weight](https://pan.baidu.com/s/1m6yOXbT6cKGqJ64z86u7fQ?pwd=RSGP) |
| Landuse Classification | Extract Pixel-wise Landuse Classification | [HRNet](https://github.com/HRNet) | [iSAID](https://captain-whu.github.io/iSAID/index)| [weight](https://pan.baidu.com/s/1Tv6BCt68L2deY_wMVZizgg?pwd=RSGP)|
| Object Counting | Count the number of certain object in an image | [SwinTransformer+UperNet](https://github.com/open-mmlab/mmsegmentation) | [LoveDA](https://github.com/Junjue-Wang/LoveDA)| [weight](https://pan.baidu.com/s/1m6yOXbT6cKGqJ64z86u7fQ?pwd=RSGP) |
| Edge Detection | Extract edge of remote sensing image | Canny |None| None |

 More funtions to be updated~

Help
----
Remote Sensing ChatGPT is an open source project that welcome any contribution and feedback. Please contact us with: haonan.guo@whu.edu.cn
