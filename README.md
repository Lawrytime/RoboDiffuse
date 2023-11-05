# RoboDiffuse

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


## Disclaimer 

This work is produced by **Timilehin Olusegun**, under the supervision of **Prof. Jonathan Loo**, for MSc in Artificial Intelligence at the **University of West London**.

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

## <p align="center">RoboDiffuse Framework.</p>

## 
## Key Features

  - Text-to-Motion Translation: RoboDiffuse is adept at translating high-level textual instructions into precise robotic arm motions, facilitating intuitive human-robot interaction.

  - Diffusion Process Refinement: The integration of a diffusion process refines the generated motion sequences, ensuring they are smooth and accurately reflective of the textual instructions.

  - CLIP-based Textual Embedding: The model leverages CLIP-based textual embeddings to capture the semantic nuances of the input text, which significantly enhances the accuracy of the text-to-motion translation.

## 

![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/embedding_space.png)

## <p align="center">Textual Embeddings Visualisation.</p>


## Performance Evaluation

RoboDiffuse has undergone rigorous evaluation using both quantitative and qualitative metris. The evaluations reveal a high degree of proficiency in generating motions that accurately reflect the input textual descriptions. Additionally, the model exhibits a promising level of adaptability to real-world dynamics, which is crucial for practical deployments.

## Potential Applications

The promise of RoboDiffuse extends across various domains where intuitive human-robot interaction is crucial. Whether it's in industrial settings, healthcare, or domestic applications, the model holds the potential to significantly enhance the ease and effectiveness of human-robot interactions.

## Future Directions

While RoboDiffuse marks a significant step forward, there's a vast scope for further refinement and expansion. Future work may delve into exploring more geometric losses, better noise schedulers, and optimizing model architectures to unlock the full potential of text-to-robotic motion models. Moreover, incorporating real-time sensory feedback and reinforcement learning approaches could further bolster the model's performance and adaptability to dynamic environments.



## <p align="center">Prompting.</p>

![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/45_Degrees_to_the_Left%20-%20Generated.gif) ![](assets/Generated%20Motions/Perform%20360%20Clockwise%20-%20Generated.gif)

## 

For further inquiries or collaborations, feel free to reach out to @Lawrytime or Professor Jonathan Loo at jonathan.loo@uwl.ac.uk.


![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Waving%20Hello.gif)  ![](https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Ground%20Truth%20Samples/Waving%20Hello.gif)
