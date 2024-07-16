# Plan and execute agent

## Preamble

This is an adaptation of the plan and execute agent published on [langgraph](https://langchain-ai.github.io/langgraph/tutorials/plan-and-execute/plan-and-execute/) to work with Anthropic Claude 3 hosted on Bedrock.

## Changes

1. Use of Anthropic Claude 3
2. Use of BedrockConverse API
3. Execution step prompt template
4. Use synchronous model invocation

## Note

The implementation is sensitive to model type and version. You might need to perform prompt engineering or change the input/output schema when using other model types and versions.
