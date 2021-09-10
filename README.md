<h1><center>Masked Sparse Adversarial Examples for Audio-Visual Speech Recognition</center></h1>

<center><b>Anonymous Author(s)</b></center>

<center>Submission Id: 1514</center> 

## Abstract
Sparse adversarial attacks design imperceptible perturbations onto partial positions of inputs that lead a neural network model to predict incorrect outputs. Until now, most researches focus on the image classification and speech recognition domains. Compared with images, adversarial examples for an audio-visual speech recognition system are redundant in spatial and temporal domains. Due to adversarial error propagation, perturbations should be added on as few temporal frames and spatial points as possible (i.e. adversarial perturbations are sparse) to improve imperceptibility. Therefore, how to determine the positions to be perturbed becomes a challenge for sparse audio-visual adversarial examples. In this paper, we propose a novel masked sparse adversarial attack algorithm, MSAE, that adopts selective masks to overcome the difficulties above. Specifically, we introduce selective masks to automatically determine the perturbed positions through backpropagation. Since the binary selective masks can not be directly optimized with gradient descent, we optimize the binary masks with the alternating direction method of multipliers algorithm by projecting them into the intersection of two continuous spaces. Experiments on the LRS2-BBC dataset demonstrate the effectiveness of MSAE: it improves the performances of several state-of-the-art attack baselines with controllable sparsity. Moreover, our work is the first attempt to implement a successful optimization-based sparse attack against an audio-visual speech recognition system.
## Audio/Video Adversarial Examples
*Note: All samples are in LRS2-BBC dataset[1].*
Here We display three sets of audio examples and video examples of the audio-visual test in the paper. In each set, there is clean examples, the adversarial examples generated by baselines in the paper and the adversarial examples generated by the corresponding baselines combined with MSAE. Observe them carefully and find the differences.


### 1. Adversarial Examples for Audio-Visual Speech Recognition

**First Set: AND TURNING UPSTAIRS INTO AN OPEN PLAN AREA IS DEFINITELY THE WAY TO GO  -->  EVERY SEPTEMBER THIS PLACE WOULD BE TRANSFORMED INTO WHAT WAS**
<div>
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW_MSAE/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2 with MSAE</h4>
	</div>

	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC_MSAE/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible_MSAE/1.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/1_gt.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Clean Video</h4>
	</div>
</div>

**Second Set: IF YOU ARE LOOKING ROUND AUCTION PROPERTIES BEFORE THE AUCTION  -->  IT WOULD HAVE BEEN COMPLETELY ALIEN TO THE REST OF LONDON**
<div>
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW_MSAE/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2 with MSAE</h4>
	</div>

	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC_MSAE/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible_MSAE/2.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/2_gt.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Clean Video</h4>
	</div>
</div>

**Third Set: IT'S A VERY ATTRACTIVE GUIDE PRICE FOR A SUBSTANTIAL HOUSE SO WELL  -->  BUT I THINK WHAT WE'RE SEEING HERE IS KIND OF THE BLUEPRINT**
<div>
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW_MSAE/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>CW + CW_l2 with MSAE</h4>
	</div>

	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="IPC_MSAE/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>IPC + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="Imperceptible_MSAE/3.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Imperceptible + CW_l2 with MSAE</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW/3_gt.mp4" type="video/mp4">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>Clean Video</h4>
	</div>
</div>



## References
[1] Afouras T, Chung J S, Senior A, et al. Deep audio-visual speech recognition[J]. IEEE transactions on pattern analysis and machine intelligence, 2018.

[2] Zhang H, Zhou P, Yan Q, et al. Generating robust audio adversarial examples with temporal dependency[C]//Proc. Int. Joint Conf. Artif. Intell. 2020: 1-5.

[3] Carlini N, Wagner D. Audio adversarial examples: Targeted attacks on speech-to-text[C]//2018 IEEE Security and Privacy Workshops (SPW). IEEE, 2018: 1-7.

[4] Carlini N, Wagner D. Towards evaluating the robustness of neural networks[C]//2017 ieee symposium on security and privacy (sp). IEEE, 2017: 39-57.