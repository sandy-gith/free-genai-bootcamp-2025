## Business requirements

For a Korean Language Learning School to extend the language offering and also augment the learning experience for students between instructor-led classes.

The school has an existing learning portal and learning record store. 
You've been tasked to:
- build a collection of learning apps using various different use-cases of AI
- Maintain the learning experience the learning portal using AI developer tools
- Extend the platform to support various different languages

The User can choose their own level and improve from there with the study activites

The user should able to resume any activity from exactly where they left, so that they don't need to start over for a word or sentence  and even alphabets.

The study activites should be more interesting and entertaining wanting the students to spend a little more time each day, so we are making it more like a interaction everywhere and also enabling learning through flash cards, conversations, songs of their choice, and visual novels(or comics)

## Functional Requirements

We should be able to host the choice of LLM in the business's local environment or in their own infrastructure to according to their compliance policy. So there will be a need to set up a internal Vector database with pretrained LLM 

## Data Strategy

The students current state like levels and every conversation will be stored in a Database to enable the user revisit and continue conversations at any point of time.

Also for LLM we should enable RAG either with open internet or a internally hosted vector database.

## Model Selection and Deployment

The Business prefer self hosted LLMs, which can be either in their local infrastructure or cloud like AWS
The Open Souce LLM models are actually preferred to reduce the cost and external dependencies

We are still exploring on the number of models to use, since the business also choose to provide listening and speech experience to the students. 
- We might need a speech to text model as well as a text to text model
- Or we can go for a text to text model, with speech to text generator available in market as a layer

For now the open source models in consideration are
- Llama-3.3-70B
- Llama-3.1-Nemotron-70B
- DeepSeek-R1