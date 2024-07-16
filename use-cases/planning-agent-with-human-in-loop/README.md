# Plan and execute agent with human in the loop

## Preamble

An example of a credit card company that interfaces with customers through a chatbot agent.

## Functionality

The chatbot has at its disposal 3 tools

1. Customer info retriever - retrieve information including name, address, registration date etc.
2. Delivery duration retriever  - retrieve duration estimates based on address
3. Delivery date calculator - calculate date of delivery based on duration and registration date

The chatbot will plan/replan its workflow at every step while using the tools to complete the task. It will also direct the question to a human if the request falls beyond its jurisdiction.
