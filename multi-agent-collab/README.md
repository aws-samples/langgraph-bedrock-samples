# Plan and execute agent

## Preamble

This is an adaptation of the multi collaboration agent published on [langgraph](https://langchain-ai.github.io/langgraph/tutorials/multi_agent/multi-agent-collaboration/) to work with Anthropic Claude 3 hosted on Bedrock.

## Changes

1. Use of Anthropic Claude 3
2. Use of BedrockConverse API
3. Renamed chart_generator to visualizer
4. Separate functions and prompts used for creation of researcher and visualizer
5. Updated agent_node function to filter for tool_calls and 'FINAL ANSWER' when deciding whether to update state with result
6. Updated router to pass the execution to the next agent when ToolMessage is in the last message
7. Use synchronous model invocation

## Note

The implementation is sensitive to model type and version. You might need to perform prompt engineering or change the input/output schema when using other model types and versions.
