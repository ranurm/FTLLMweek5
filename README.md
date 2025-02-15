# FTLLMweek5
I fixed the following things:
1. Added correct dependencies.
2. Also tested other dependency versions to fix that one compatibility error, but that caused more errors and in the original wrong version didn't cause any functional problems so I left it how it was.
3. Implemented a bit differently rouge_score version printing, because it wasn't properly working.
4. Tried to change the model to mistralai/Mistral-7B-v0.1, EleutherAI/gpt-neo-2.7B, EleutherAI/gpt-neo-1.3B and facebook/opt-1.3b, but those models just repeated part of the input texts as output and didn't work at all. So I ended up using microsoft/phi-2.
5. Fixed configuration settings max_steps = 500, logging_steps = 50, eval_steps = 50.
6. Uploaded the model to my Hugging Face account.

I have explained each fix in the in the code separately.

## Hugging Face model
Link: https://huggingface.co/pmranu/phi-2-dialogsum-finetuned

And snapshot:
![image](https://github.com/user-attachments/assets/48ec5ef4-5ab7-447b-bc3a-674a127d0551)

## Evaluation
### Qualitative
Comparison table of each mode and human output:
![image](https://github.com/user-attachments/assets/4b708419-16e8-4e93-932a-9558e2f927c6)
Single output of finetuned model:
![image](https://github.com/user-attachments/assets/e93874ac-5f52-4527-85b3-64108980700d)

### Quantitative
Rouge results:
![image](https://github.com/user-attachments/assets/19cd909f-af2b-4173-844a-5b61d4fad510)

![image](https://github.com/user-attachments/assets/9736d3dd-631c-4f2d-8cf1-699d09353bf5)
