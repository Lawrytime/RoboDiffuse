# RoboDiffuse

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



## Abstract

The advent of diffusion models has spurred innovations across various domains, rendering them a crucial component in the generation of diverse and realistic data. This research embarks on a pioneering journey to harness the capabilities of diffusion models, specifically focusing on their application in generating 3D motion for robotic arms conditioned on natural language descriptions. The primary objective is to bridge the gap between human articulations and robotic motions, fostering seamless and intuitive interactions with robotic systems.
The research navigates through numerous challenges, primarily stemming from the absence of specialized datasets for Text-to-Robotic Motion tasks, necessitating the meticulous creation and annotation of a tailored dataset. The research methodology encompasses comprehensive motion sequence generation, dataset annotation, and extensive preprocessing to build a reliable foundation for model development.
The model, RoboDiffuse, integrates a transformer encoder to predict clean motion sequences and employs a diffusion process to refine model predictions, all conditioned on CLIP-based textual embeddings. The model is meticulously evaluated using a blend of quantitative and qualitative methods, revealing its proficiency in generating motions reflective of input textual descriptions and its adaptability to real-world dynamics.
Despite the limitations related to dataset availability and diversity, RoboDiffuse demonstrated substantial promise, generating robotic arm motions with high fidelity. The findings of this research are anticipated to act as a catalyst, propelling further innovations in the field of robotics and contributing significantly to enhancing human-robot interactions.


### Prompting

<td align="center">
      <img src="https://github.com/Lawrytime/RoboDiffuse/blob/main/assets/Generated%20Motions/45_Degrees_to_the_Left%20-%20Generated.gif" width="600">
    </td>



![](assets/Generated%20Motions/Perform%20360%20Clockwise%20-%20Generated.gif)
