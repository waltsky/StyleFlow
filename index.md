<p align="center">
<img src="assets/teaser.png" height="500" />
<h1>Abstract</h1>
 </p>
 
<p align="justify">
High-quality, diverse, and photorealistic images can now be generated by unconditional GANs (e.g., StyleGAN). However, limited options exist to control the generation process using (semantic) attributes, while still preserving the quality of the output. Further, due to the entangled nature of the GAN latent space, performing edits along one attribute can easily result in unwanted changes along other attributes. In this paper, in the context of conditional exploration of entangled latent spaces, we investigate the two sub-problems of attribute-conditioned sampling and attribute-controlled editing. We present StyleFlow as a simple, effective, and robust solution to both the sub-problems by formulating  conditional exploration as an instance of conditional continuous normalizing flows in the GAN latent space conditioned by attribute features. We evaluate our method using the face and the car latent space of StyleGAN, and demonstrate fine-grained disentangled edits along various attributes on both real photographs and StyleGAN generated images. For example, for faces we vary camera pose, illumination variation, expression, facial hair, gender, and age. Finally, via extensive qualitative and quantitative comparisons, we demonstrate the superiority of StyleFlow to other concurrent works. 
</p>
<p align="center">
<img src="assets/1.gif" height="300" /><img src="assets/2.gif" height="300" /></p>

<p align="center">
<img src="assets/car1.gif" width="300" /><img src="assets/car2.gif" height="300" /><img src="assets/car3.gif" height="300" /><img src="assets/car4.gif" height="300" /></p>
<p align="center">
<h1>Overview Video</h1>
 </p>

<div class="container">
  <div style="text-align: center;">
<iframe width="560" height="315" src="https://www.youtube.com/embed/LRAUJUn3EqQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>

<p align="center">
<h1>Method</h1>
 </p>
 
 <p align="center">
<img src="assets/styleFlow_pipeline.png"  height="800" /></p>


<p align="justify">
Attribute-conditioned editing using StyleFlow. Starting from a source image, we support attribute-conditioned editing by using a reverse inference followed by a forward inference though a sequence of CNF blocks. Here, z denotes the variable of the prior distribution and w denotes the intermediate weight vector of the StyleGAN.
</p>

<p align="center">
<h1>Sampling</h1>
 </p>
 
 <p align="center">
<img src="assets/sampling.png" /></p>


<p align="justify">
Attribute-conditioned sampling using StyleFlow. Here we show sampling results for attribute specifications of females with glasses in a target pose(top); 50-year old males with facial hair(middle); and smiling 5-year old children in a target pose(bottom).
</p>

<p align="center">
<h1>Sequential Edits</h1>
 </p>
 
 <p align="center">
<img src="assets/sota.png"  height="800"  /></p>


<p align="justify">
Sequential edits using StyleFlow with `+'/`-' denoting corresponding attribute was increased/decreased.
</p>


<p align="center">
<h1>Real Image Edits</h1>
 </p>
 
 <p align="center">
<img src="assets/comapre.png"  height="1000"  /></p>


<p align="justify">
 Real image non-sequential edits using our StyleFlow framework. Note that the method is able to handle extreme pose (first and second rows),asymmetrical expressions (fourth row) and age diversity (first and last rows) well compared to the concurrent methods.
</p>


<p align="center">
<h1>Bibtex</h1>
 </p>
<p align="justify">
<div class="container">
<pre>
 @misc{abdal2020styleflow,
    title={StyleFlow: Attribute-conditioned Exploration of StyleGAN-Generated Images using Conditional Continuous Normalizing Flows},
    author={Rameen Abdal and Peihao Zhu and Niloy Mitra and Peter Wonka},
    year={2020},
    eprint={2008.02401},
    archivePrefix={arXiv},
    primaryClass={cs.CV}
}
</pre>
</div>
</p>

<p align="center">
<h1>Acknowledgements</h1>
 </p>
<p align="justify">
<div class="container">
  <div class="body" style="font-size: 11pt;;">
   This work was supported by the KAUST Office of Sponsored Research (OSR) and Adobe Research.
  </div>

</div>

</p>

<p align="justify">
<h1>Related Work</h1>
 </p>
<div class="container">
 
   <div class="citation">
    <img src="assets/styleGAN.png">
  </div>
     <div class="citation">
    <a href="https://github.com/NVlabs/stylegan">
      Tero Karras, Samuli Laine, Timo Aila.
      A Style-Based Generator Architecture for Generative Adversarial Networks
      CVPR, 2019.
    </a>
  </div>
  <div class="citation">
    <img src="assets/sg22.png" >
  </div>
    </div>
  <div class="citation">
    <a href="https://github.com/NVlabs/stylegan2">
      Tero Karras, Samuli Laine, Miika Aittala, Janne Hellsten, Jaakko Lehtinen, Timo Aila.
      Analyzing and Improving the Image Quality of StyleGAN
      CVPR, 2020.
    </a>
  </div>
 


