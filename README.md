<h1><center>Masked Sparse Adversarial Examples for Audio-Visual Speech Recognition</center></h1>

<center><b>Anonymous Author(s)</b></center>

<center>Submission Id: 1514</center> 

## Abstract
Sparse adversarial attacks design imperceptible perturbations onto partial positions of inputs that lead a neural network model to predict incorrect outputs. Until now, most researches focus on the image classification and speech recognition domain. However, research on the adversarial attack against audio-visual speech recognition is limited and faces several challenges: 1) 'dispensable regions': some audio and video regions are less important for the model in the speech recognition process. Attacking these regions brings more noise while contributes less to constructing a successful adversarial example; 2) 'sensitiveness distinction': the perceptibility of humans towards the same noise under different regions is significantly different. Particularly, perturbations are more noticeable in the periods of silences and pauses; 3) 'temporal cues': the temporal information contained in videos should be explored. In this paper, we propose a novel sparse adversarial attack scheme, MSAE, that adopts weighted masks to overcome the difficulties above. Specifically, 1) we introduce grouped selective mask to achieve grouped sparsity through backpropagation automatically; 2) the perceptibility weight matrix is introduced to ensure the imperceptibility of the audio and video respectively; 3) we utilize $l2$-norm within frames and $l1$-norm across frames to achieve spatial and temporal sparsity. Experiments on the LRS2-BBC dataset demonstrate the effectiveness of MSAE: it achieves the lowest noise level among several state-of-the-art attack baselines even when only a portion of the input is perturbed. Moreover, our work is the first attempt to implement a successful sparse attack against the audio-visual speech recognition systems.

## Audio/Video Adversarial Examples
*Note: All samples are in LRS2-BBC dataset[1].*
Here We display two sets of audio examples and video examples of the audio-visual test in the paper. In each set, there is a clean example, adversarial examples generated by baselines in the paper and an imperceptible adversarial example generated with MSAE. Listen to and see them carefully and choose which one is the clean example.


### 1. Audio Adversarial Examples
#### First Set
<div>
	<audio src="MSAE_FPM/BUT BEFORE I DO.wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input1" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input1" type="submit" value="click&show" onclick="display('audio1')" style="display:none">
	<div id="audio1" style="display:none">
		<strong>Clean audio:</strong> “But before I do”
	</div>
</div>
<div>
	<audio src="IPC/BUT BEFORE I DO(PROBABLY AROUND 85).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input2" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input2" type="submit" value="click&show" onclick="display('audio2')" style="display:none">
	<div id="audio2" style="display:none">
		<strong>IPC Attack:</strong> “Probably around 85”
	</div>
</div>
<div>
	<audio src="CW_l2/BUT BEFORE I DO(PROBABLY AROUND 85).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input3" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input3" type="submit" value="click&show" onclick="display('audio3')" style="display:none">
	<div id="audio3" style="display:none">
		<strong>C&W's Attack:</strong> “Probably around 85”
	</div>
</div>
<div>
	<audio src="MSAE_FPM/BUT BEFORE I DO(PROBABLY AROUND 85).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input4" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input4" type="submit" value="click&show" onclick="display('audio4')" style="display:none">
	<div id="audio4" style="display:none">
		<strong>MSAE:</strong> “Probably around 85”
	</div>
</div>

#### Second Set
<div>
	<audio src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input8" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input8" type="submit" value="click&show" onclick="display('audio8')" style="display:none">
	<div id="audio8" style="display:none">
		<strong>MSAE:</strong> “Sometimes it's difficult to know where”
	</div>
</div>
<div>
	<audio src="IPC/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input6" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input6" type="submit" value="click&show" onclick="display('audio6')" style="display:none">
	<div id="audio6" style="display:none">
		<strong>IPC Attack:</strong> “Sometimes it's difficult to know where”
	</div>
</div>
<div>
	<audio src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED.wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input5" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input5" type="submit" value="click&show" onclick="display('audio5')" style="display:none">
	<div id="audio5" style="display:none">
		<strong>Clean audio:</strong> “If it was going to be increased”
	</div>
</div>
<div>
	<audio src="CW_l2/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).wav" controls="controls" style='display:inline-block;'>
	Your browser does not support the audio element.
	</audio>
	<div style='text-align:center; height:54px;display:inline-block; position:absolute;'>
	<label for="input7" style='line-height:54px;font-size:18px;font-weight:bold; text-align:center;'>[Reveal Transcription]</label>
	</div>
	
	<input id="input7" type="submit" value="click&show" onclick="display('audio7')" style="display:none">
	<div id="audio7" style="display:none">
		<strong>C&W's Attack:</strong> “Sometimes it's difficult to know where”
	</div>
</div>


### 2. Video Adversarial Examples
Since the examples listed below is in the audio-visual test, the attack method in "()" means the corresponding audio attack mehtod.

**First Set: But before I do  -->  Probably around 85**
<div>
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/BUT BEFORE I DO.mp4" type="video/mp4">
	  <source src="CW_l2/BUT BEFORE I DO.avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>clean</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/BUT BEFORE I DO(PROBABLY AROUND 85).mp4" type="video/mp4">
	  <source src="MSAE_FPM/BUT BEFORE I DO(PROBABLY AROUND 85).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>MSAE</h4>
	</div>

	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/BUT BEFORE I DO(PROBABLY AROUND 85).mp4" type="video/mp4">
	  <source src="CW_l2/BUT BEFORE I DO.avi(PROBABLY AROUND 85).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>C&W-l2 (C&W's Attack)</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/BUT BEFORE I DO(PROBABLY AROUND 85).mp4" type="video/mp4">
	  <source src="IPC/BUT BEFORE I DO.avi(PROBABLY AROUND 85).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>C&W-l2 (IPC Attack)</h4>
	</div>
</div>

**Second Set: If it was going to be increased  -->  Sometimes it's difficult to know where**
<div>
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="CW_l2/IF IT WAS GOING TO BE INCREASED.mp4" type="video/mp4">
	  <source src="CW_l2/IF IT WAS GOING TO BE INCREASED.avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>clean</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).mp4" type="video/mp4">
	  <source src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>MSAE</h4>
	</div>

	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).mp4" type="video/mp4">
	  <source src="CW_l2/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>C&W-l2 (C&W's Attack)</h4>
	</div>
	
	<div style='text-align:center; display: inline-block;'>
	<video width="224" height="112" controls>
	  <source src="MSAE_FPM/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).mp4" type="video/mp4">
	  <source src="IPC/IF IT WAS GOING TO BE INCREASED(SOMETIMES IT'S DIFFICULT TO KNOW WHERE).avi" type="video/avi">
	  您的浏览器不支持 HTML5 video 标签。
	</video>
	<h4>C&W-l2 (IPC Attack)</h4>
	</div>
</div>


## References
[1] Afouras T, Chung J S, Senior A, et al. Deep audio-visual speech recognition[J]. IEEE transactions on pattern analysis and machine intelligence, 2018.




<script type="text/javascript">
 
    function display(id){  
        var traget=document.getElementById(id);  
        if(traget.style.display=="none"){  
            traget.style.display="";  
        }else{  
            traget.style.display="none";  
      }  
   }  
</script>
