## Evaluating models for prompt response

Now I am using groq cloud to evaluate different open source models
providing prompts and trying to get the exact result we want from the models for sentence constructors

We should need to evaluate the same for flash card contents, alphabet learning and comic generators 

## Models into consideration 
### Deepseek-r1-distill-llama70b

On comparing these three models for sentence constructor deepseek seems to provide the output as expected while the other models showed a minor inconsistence.
- Deepseek provided output considering the user's language level
- vocabulary table was close enough to make the students think
- provided valid evaluation and translation for the student's attempts

### Llama-3.3-70b

Llama showed expectional performance for some sentences and at sometimes provide alien characters(which might be some chinese derivates in korean which I am not aware of)
- gives high level characters which a beginner might not even be aware of
- llama captures the output format appropriately but there are inconsistency in context level

### Mixtral 8x7b-32768

Mixtral provides good vocabulary table and validates input appropriately but struggles with sentence formatting
- mixtral provides appropriate vocabulary table and good clue patterns
- but struggle in producing sentence patterns I sometimes see [Sentence] in sentence format while other models capture is somehow appropriate

## Inference
As far as we compared the three models for sentence constructor, deepseek slightly performs better than the other two in some aspect.
We can't conclude the model now as we have few other criterias to consider 
 - other prompt modules (flash card content generation, alphabet learning module etc)
 - deployment complexity
Just for now Deepseek leads