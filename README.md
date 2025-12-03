# summary

## Multi Agent Systems
- Utilize google ADK for multi agent systems
- Sub-agents for multiple use cases like activation, appointment, billing, internet troubleshooting, mobile, outage, payments, transfers, etc.
- Each sub-agent implementation includes its corresponding prompt (agent instruction) and the definition of its tools
- Evaluation module that runs tests on the given test cases and determine success or failure based on predefined rubrics
- Beyond fixed test cases, the user simulator can generate user requests in various languages, enabling broader and more realistic testing.

## Conversational Agent Evaluation
- Evaluate conversationl agent implemented on google Dialogflow CX
- Use the simulation capability to generate diverse user experience scenarios
- Support multiple providers (to simulate users) and evaluators
- AWS integration for seemless test execution
- Test case specification: target agent, start phrase, initial params, target evaluators, success criteria, max steps, number of samples, etc.

## Iterative Learning by Active LLM Annotation (Experiments)
- Improve default NLU (simple intent classifier) though active annotation by LLM
- Identify clean/noisy samples from the classifier trained with new annotated dataset and try improving improving the model with clean set in the next step

## LLM Fine-tuning for Customized Service
- Performed fine-tuning to build an LLM that works effectively for the ‘Technician Appointment Scheduling’ use case.
- Utilized several lightweight pretrained LLM models, such as GPT-Neo 2.7B and Mistral 7B
- Tried PEFT adapter to lightly train new task-specific parameters while preserving as much of the pretrained LLM’s original performance as possible
- Generated a synthetic training dataset using the LLM to cover a wide range of desired scenarios and used it for fine-tuning

