# RoboDiffusion: 
## A Natural Language Driven Robotic Arm Motion Generation using Diffusion Mode

##  

### Framework

![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/RoboDiffuse.png)


##  

##  

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Bend%20to%20the%20Left.gif" width="400">
    </td>
    <td align="center">
      <img src="https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Bend%20to%20the%20Right.gif" width="400">
    </td>
  </tr>
</table>


##  


## Disclaimer 

This work is produced by **Timilehin Olusegun**, under the supervision of **Prof. Jonathan Loo**, for MSc in Artificial Intelligence at the **University of West London**.


## 

## Content
- [Introduction](#introduction)
- [Model Overview](#model-overview)
- [Key Features](#key-features)
- [Dataset](#dataset)
- [Simulation Enviroments](#simulation-enviroments)
- [RoboDiffuse Framework](#roboDiffuse-framework)
- [Sample Prompts](#sample-prompts)

##  

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/Extend%20to%20top%20Left%20Diagonal%20-%20Generated.gif" width="400">
      <p>Extend to top Left Diagonal</p>
    </td>
    <td align="center">
      <img src="https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/Extend%20to%20top%20Right%20Diagonal%20-%20Generated.gif" width="400">
      <p>Extend to top Right Diagonal</p>
    </td>
  </tr>
</table>



## Introduction

The RoboDiffuse model stems from a compelling endeavor to bridge the gap between human natural language and robotic motion generation. In a world where robotics is rapidly evolving, having a robotic system that understands and accurately interprets human commands into precise motions is pivotal. This model is a stride towards enhancing the intuitive interaction between humans and robots, paving the way for more dynamic and responsive robotic systems.


## Model Overview

RoboDiffuse employs advanced diffusion processes alongside a transformer encoder to translate high-level textual descriptions into a series of robotic arm motions. The core of the model is grounded on a diffusion process that refines the motion predictions generated by the transformer encoder, ensuring a smooth and accurate transition from text to motion.

The model architecture integrates a transformer encoder that digests textual descriptions and generates initial motion sequences. These sequences are further refined by a diffusion process, ensuring the generated motions are coherent and reflective of the input textual descriptions. The entire model is conditioned on CLIP-based textual embeddings which encapsulate the semantic essence of the input text, facilitating a more accurate translation into robotic motions.

## 


![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/RoboDiffuse.png)

## <p align="center">RoboDiffuse Framework</p>

## 

## Key Features

  - **Natural Language Understanding:** Interprets complex instructions given in human language.
    
  - **Generative Motion Modeling:** Generates 3D motion sequences for a robotic arm based on textual descriptions.
    
  - **Diffusion-Based Refinement:** Utilizes a diffusion process to improve the quality and accuracy of motion sequences.
    
  - **CLIP-Based Conditioning:** Employs Contrastive Language-Image Pretraining (CLIP) embeddings to condition the generative process.
    
  - **Custom Dataset:** Features a meticulously annotated dataset specifically designed for Text-to-Robotic Motion tasks.


![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/embedding_space.png)

## <p align="center">Textual Embeddings Visualisation.</p>


## Simulation Enviroments

### ROS Visualization (RViz)
![ROS](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/ros_env.png)

### MoveIt (Motion Planning)
![MoveIt](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/moveit.png)


## Performance Evaluation

RoboDiffuse has undergone rigorous evaluation using both quantitative and qualitative metris. The evaluations reveal a high degree of proficiency in generating motions that accurately reflect the input textual descriptions. Additionally, the model exhibits a promising level of adaptability to real-world dynamics, which is crucial for practical deployments.

### Experiment Tracking (WandB)

![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Wandb_.png)

## Potential Applications

The promise of RoboDiffuse extends across various domains where intuitive human-robot interaction is crucial. Whether it's in industrial settings, healthcare, or domestic applications, the model holds the potential to significantly enhance the ease and effectiveness of human-robot interactions.

## Future Directions

While RoboDiffuse marks a significant step forward, there's a vast scope for further refinement and expansion. Future work may delve into exploring more geometric losses, better noise schedulers, and optimizing model architectures to unlock the full potential of text-to-robotic motion models. Moreover, incorporating real-time sensory feedback and reinforcement learning approaches could further bolster the model's performance and adaptability to dynamic environments.



## <p align="center">Sample Prompts.</p>

![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/45_Degrees_to_the_Left%20-%20Generated.gif) ![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/45_Degrees_to_the_Left%20-%20Generated.gif)

## 


![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Waving%20Hello.gif) ![](assets/Generated%20Motions/Perform%20360%20Clockwise%20-%20Generated.gif) ![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Waving%20Hello.gif)

## UWL AI
