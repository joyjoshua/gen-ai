What is an Agent?
1. And this is what an Agent is: an AI model capable of reasoning, planning, and interacting with its environment.
2. Let's assume Alfred is an AI agent, and we ask him to get us coffee

    Before fulfilling the order, Alfred engages in reasoning and planning, figuring out the steps and tools he needs to:
    Go to the kitchen
    Use the coffee machine
    Brew the coffee
    Bring the coffee back

Official definition of Agents
An Agent is a system that leverages an AI model to interact with its environment in order to achieve a user-defined objective. It combines reasoning, planning, and the execution of actions (often via external tools) to fulfill tasks.

Agents is split into 2 parts
1. The Brain (AI Model)
    This is where all the thinking happens. The AI model handles reasoning and planning. It decides which Actions to take based on the situation.
2. The Body (Capabilities and Tools)
    This part represents everything the Agent is equipped to do.
    The scope of possible actions depends on what the agent has been equipped with. For example, because humans lack wings, they can’t perform the “fly” Action, but they can execute Actions like “walk”, “run” ,“jump”, “grab”, and so on.

Spectrum of Agents
![agent spectrum](/media/image.png)

1. The Brain aka LLM
    a. LLM takes in input as a text, reasons and plans and returns back output in text

2. The Body (Capabilities and Tools)
    a. to enhance the functionality of an agent, where if I want GPT to create an image by giving a description it will gladly do so, but using LLM it's not possible, so devs in hugging face or open ai etc, implemented additional functionality (called Tools), that the LLM can use to create images.

Tasks the Agent can do
1. "An Agent can perform any task we implement via Tools to complete Actions."
    a. For example, if I write an Agent to act as my personal assistant (like Siri) on my computer, and I ask it to “send an email to my Manager asking to delay today’s meeting”, I can give it some code to send emails. This will be a new Tool the Agent can use whenever it needs to send an email. We can write it in Python:

    def send_message_to(recipient, message):
    """Useful to send an e-mail message to a recipient"""
    ...
2. LLMs will use these tools to run whenever required to fulfill it's user's needs
    send_message_to("Manager", "Can we postpone today's meeting?")

The design of the Tools is very important and has a great impact on the quality of your Agent. Some tasks will require very specific Tools to be crafted, while others may be solved with general purpose tools like “web_search”.

Note: 'Note that Actions are not the same as Tools. An Action, for instance, can involve the use of multiple Tools to complete.'

Real world examples
1. Personal Virtual Assistants (Siri, Alexa etc)
2. Customer Service Chatbots
3.  AI Non-Playable Character in a video game


Summary
To summarize, an Agent is a system that uses an AI Model (typically an LLM) as its core reasoning engine, to:

1. Understand natural language: Interpret and respond to human instructions in a meaningful way.
2. Reason and plan: Analyze information, make decisions, and devise strategies to solve problems.
3. Interact with its environment: Gather information, take actions, and observe the results of those actions.