# Building-an-Agent_With-LangGraph
Key concepts¶
LangGraph applications are built around a graph structure. As the developer, you define an application graph that models the state transitions for your application. Your app will define a state schema, and an instance of that schema is propagated through the graph.

Each node in the graph represents an action or step that can be taken. Nodes will make changes to the state in some way through code that you define. These changes can be the result of invoking an LLM, by calling an API, or executing any logic that the node defines.

Each edge in the graph represents a transition between states, defining the flow of the program. Edge transitions can be fixed, for example if you define a text-only chatbot where output is always displayed to a user, you may always transition from chatbot -> user. The transitions can also be conditional, allowing you to add branching (like an if-else statement) or looping (like for or while loops).

LangGraph is highly extensible and provides a number of features that are not part of this tutorial, such as memory, persistance and streaming. To better understand the key concepts and philophies behind LangGraph, check out their Conceptual guides and High-level overview.
