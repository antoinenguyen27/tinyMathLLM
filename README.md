# tinyMathLLM
An experiment to see how far I can push latent space reasoning and CoT via RL in tiny (and quantized!) models by finetuning on math datasets on consumer hardware. This experiment utilises huginn-125, the 3.5B parameter latent space reasoning model introduced in the paper "Scaling up Test-Time Compute with Latent Reasoning: A Recurrent Depth Approach" (Geiping, Jonas, et al.). It also draws great inspiration from the yet to be published works from Jiayi Pan of UC Berkeley and the work done by the Deepseak team on Deepseak-R1-Zero. 

The current stage of this experiment is modifying the modelling.py file of huginn-125 to make it compatible with my fine tuning process, which will involve QLoRA. huginn-125 was not trained with quantizing in mind, however I am broke and would like to train it on my own machine without spending my daily budget on cloud compute.

I will not be surprised if this goes absolutely nowhere, however I wanted to try regardless for the learning experience. I am also aware my puny machine will likely take weeks to finetune even on smaller datasets. 


Currently OpenMathInstruct-1 and 2 are the datasets in mind due to their (relatively) smaller size. However given my available compute, updates to this repo will be very slow and have little scientific validity (since I can't do many trials or controls).

Provided heat death of the universe does not occur first, the model's performance will be benchmarked against MATH and GSM8K.
