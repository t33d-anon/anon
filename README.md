# T323D: Creative Text+3D-to-3D Object Generation via Multi-view Inversion

<p align="center">
<br>
    <img src="resources\images\0-first.png">
<br>
<p

In this paper, we tackle a new task of 3D object synthesis, where a 3D model is combined with another object text to create a novel 3D model. However, most existing text/image/3D-to-3D methods struggle to effectively integrate multiple content sources, often resulting in inconsistent textures and inaccurate shapes. To overcome these challenges, we propose a straightforward yet powerful approach, Text+3D-to-3D (T33D), for generating novel and compelling 3D models. Our method begins by rendering multi-view images and normal maps from the input 3D model, then generating a novel, surprising 2D object using ATIH with the front-view image and the another object text as inputs. To ensure texture consistency, we introduce texture multi-view diffusion, which refines the textures of the remaining multi-view RGB images based on the novel 2D object. For enhanced shape accuracy, we propose shape multi-view diffusion to improve the 2D shapes of both the multi-view RGB images and the normal maps, also conditioned on the novel 2D object. Finally, these outputs are used to reconstruct a complete and novel 3D model. Extensive experiments demonstrate the effectiveness of our method, yielding impressive 3D creations.