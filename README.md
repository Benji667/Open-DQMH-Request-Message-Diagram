# Open DQMH Request Message Diagram

Adds a right-click shortcut to DQMH Module **Request**, **Request and Wait for Reply** and **Round Trip Broadcast** methods on the block diagram allowing the developer to quickly point to the case frame of the Message Handling Loop, of the DQMH Module Main VI, where the Request is handled.

When writing code using DQMH Framework, the way you communicate between actors is by way of messages. Each DQMH Module has a set of methods which collects the inputs for the message and transports it using user event, but the Public API VIs (which is often what you see on the block diagram) is not what gets executed by the actor that receives the message. The actual logic that executes when the message is received resides in the Message Handling Loop (MHL) of the DQMH Module Main VI which reads the message causes the corresponding subdiagram of the Case structure to execute. 
