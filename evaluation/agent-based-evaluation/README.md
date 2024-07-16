# Agent based evaluation

This is an adaptation of the agent based evaluation published on [langgraph](https://langchain-ai.github.io/langgraph/tutorials/chatbot-simulation-evaluation/agent-simulation-evaluation/) to work with Anthropic Claude 3 hosted on Bedrock.

## Changes

1. Use of Anthropic Claude 3
2. Use of BedrockConverse API
3. Pass in human message to chatbot to start the conversation. Claude 3 requires first message to be human message.
4. Due to 3), only swap roles starting from the 2nd message for the user

## Note

The implementation is sensitive to model type and version. You might need to perform prompt engineering or change the input/output schema when using other model types and versions.