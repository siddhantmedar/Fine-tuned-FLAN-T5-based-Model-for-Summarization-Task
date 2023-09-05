PEFT FLAN T5-XXL Sharded FP16 Model
## HF Link

## Model Details
Repository: [medarsiddhant/flan-t5-xxl-sharded-fp16-model](https://huggingface.co/medarsiddhant/flan-t5-xxl-sharded-fp16-model)
Dataset: [samsum](https://huggingface.co/datasets/samsum)
Trained for epochs: 7
Finetuned from Model : [philschmid/flan-t5-xxl-sharded-fp16](philschmid/flan-t5-xxl-sharded-fp16) [sharded version of flan-t5-xxl]
Original Base Model : [google/flan-t5-xxl](https://huggingface.co/google/flan-t5-xxl))
Downstream Use : Summarization
Finetuning Method: PEFT(LoRA), bitsanbytes LLM.int8() to quantize out frozen LLM weights to int8. This allows us to reduce the needed memory for FLAN-T5 XXL ~4x.
Results:
Rogue1: 50.539160%
rouge2: 25.023891%
rougeL: 41.633410%
rougeLsum: 41.650940%

Example:
input sentence: Richie: Pogba
Clay: Pogboom
Richie: what a s strike yoh!
Clay: was off the seat the moment he chopped the ball back to his right foot
Richie: me too dude
Clay: hope his form lasts
Richie: This season he's more mature
Clay: Yeah, Jose has his trust in him
Richie: everyone does
Clay: yeah, he really deserved to score after his first 60 minutes
Richie: reward
Clay: yeah man
Richie: cool then 
Clay: cool
------------------------------------------------------------
summary:
Richie and Clay are excited about Pog

Hardware Type: RunPod Pytorch 2.0.1 (1 x RTX A6000, 16 vCPU 62 GB RAM, cuda11.8.0-devel)
Hours used: ~18
