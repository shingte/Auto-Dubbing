## Face-Expression-Transfer-by-Audio



### Introduction

Audio-driven facial animation is the process that aotomatically synthesizes talking head video from speech signals.

This project presents an end-to-end system that take an image and a clip of audio to generate the talking video. 
The system can simplify the film animation process through automatic generation from the voice acting.
It can also be applied inpost-production to achieve better lip-synchronization in movie dubbing.

This repository uses the model described in the paper [Hierarchical Cross-modal Talking Face Generation with Dynamic Pixel-wise Loss](http://www.cs.rochester.edu/u/lchen63/cvpr2019.pdf). 

	
### Setup and Running

0. Pytorch environment:[Pytorch 0.4.1](https://pytorch.org/). (conda install pytorch=0.4.1 torchvision cuda90 -c pytorch)
0. Install requirements.txt (pip install -r requirement.txt)
0. Download the pretrained ATnet and VGnet weights at [google drive](https://drive.google.com/file/d/1m8tduoobl_ytyuEjzUbom__7qh7qAwN5/view?usp=sharing). Put the weights under `model` folder.
0. Run the demo code: `python demo.py`
	- `-device_ids`: gpu id
	- `-cuda`: using cuda or not
	- `-vg_model`: pretrained VGnet weight
	- `-at_model`: pretrained ATnet weight
	- `-lstm`:  use lstm or not
	- `-p`:  input example image
	- `-i`:  input audio file
	- `-lstm`:  use lstm or not
	- `-sample_dir`: folder to save the outputs
	- ...


Reference
----
This repository is based on repository [ATVGnet](https://github.com/lelechen63/ATVGnet).



License
----

MIT
