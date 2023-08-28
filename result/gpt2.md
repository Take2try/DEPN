# The privacy Number leakage risk of GPT2

|Model|EpochTraining Time|Validation PPL|Exposure|
|----|----|----|----|----|
|GPT2|10|24h|8.40|12.1|

we trained GPT2 on Enorn Dataset for 10 epochs with 4 A6000 GPUs, which spent 24 hours. The validation perplexity of this model is 8.40, and the averge exposure of memorized Telephone Numbers is 12.1.

# The privacy Number leakage risk of privacy erased GPT2

|Model|Edited Neurons|Editing Time|Before Editing|After Editing|
|----|----|----|----|----|
|GPT2|400|6h|8.62|9.5|

We used DEPN to aid the GPT2 in privacy leakage risk, which edited 400 privacy neurons and spent 6h on one A6000 GPU. The validation perplexity of new model is 8.40, and the averge exposure of memorized Telephone Numbers becomes to 12.1. The privacy erased GPT2`s performance droped a little and the privacy leakage risk reduction is significant.

- The result shows the DEPN framework strikes a balance between performance and privacy protection on GPT2.
