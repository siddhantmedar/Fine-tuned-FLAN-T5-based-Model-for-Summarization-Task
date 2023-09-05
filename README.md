## Model Details

## Repository<br>
[medarsiddhant/flan-t5-xxl-sharded-fp16-model](https://huggingface.co/medarsiddhant/flan-t5-xxl-sharded-fp16-model)<br>

## Dataset<br>
[samsum](https://huggingface.co/datasets/samsum)<br>

## Trained for epochs<br>
7<br>

## Finetuned from Model<br>
[philschmid/flan-t5-xxl-sharded-fp16](philschmid/flan-t5-xxl-sharded-fp16) [sharded version of flan-t5-xxl]<br>

## Original Base Model<br>
[google/flan-t5-xxl](https://huggingface.co/google/flan-t5-xxl))<br>

## Downstream Use<br>
Summarization<br>

## Finetuning Method<br>
PEFT(LoRA), bitsanbytes LLM.int8() to quantize out frozen LLM weights to int8. This allows us to reduce the needed memory for FLAN-T5 XXL ~4x.<br>

## Results:
#### Rogue1: 50.539160%<br>
#### Rouge2: 25.023891%<br>
#### RougeL: 41.633410%<br>
#### RougeLsum: 41.650940%<br>

## Example<br>
#### input sentence: Richie: Pogba<br>
#### Clay: Pogboom<br>
#### Richie: what a s strike yoh!<br>
#### Clay: was off the seat the moment he chopped the ball back to his right foot<br>
#### Richie: me too dude<br>
#### Clay: hope his form lasts<br>
#### Richie: This season he's more mature<br>
#### Clay: Yeah, Jose has his trust in him<br>
#### Richie: everyone does<br>
#### Clay: yeah, he really deserved to score after his first 60 minutes<br>
#### Richie: reward<br>
#### Clay: yeah man<br>
#### Richie: cool then <br>
#### Clay: cool<br>
------------------------------------------------------------
## Summary<br>
#### Richie and Clay are excited about Pog

## Hardware Type<br>
#### RunPod Pytorch 2.0.1 (1 x RTX A6000, 16 vCPU 62 GB RAM, cuda11.8.0-devel)<br>
## Hours used
#### ~18
![image](https://github.com/siddhantmedar/PEFT-FLAN-T5-XXL-Sharded-FP16-Model/assets/15628564/064affec-6a5b-4bee-a991-4022efcb17c7)
