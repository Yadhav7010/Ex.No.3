# Ex.No.3-Scenario-Based Report Development Utilizing Diverse Prompting Techniques for the the following Prompt Engineering types with examples - Straightforward Prompts - Tabular Format Prompting - Missing Word Prompting - Preceding Question Prompting.
### Aim: To design an AI-powered chatbot that assists customers in resolving issues related to product troubleshooting, order tracking, and general inquiries. The chatbot should handle various customer queries efficiently while maintaining a conversational and user-friendly tone. In this experiment, we will employ different prompt patterns to guide the development process of the chatbot, ranging from basic task-oriented prompts to more complex, persona-driven prompts.

### Algorithm:  1. Direct Instruction Prompts
Objective: Guide the chatbot to respond concisely to customer inquiries.
Prompt Pattern:
Prompt: "When a customer asks for the status of their order, reply with: 'Your order is currently being processed and will be delivered by [date].'"
2. Contextual Prompting
Objective: Incorporate specific context to provide detailed answers based on the user’s previous interaction.
Prompt Pattern:
Prompt: "If the customer previously mentioned that they haven’t received their order, say, 'I see that you mentioned your order hasn't arrived yet. Let me check the details for you and get back shortly.'"
3. Persona-Based Prompting
Objective: Design the chatbot to adopt a specific persona, making the interaction more engaging.
Prompt Pattern:
Prompt: "Pretend you are a friendly, helpful customer service representative. Use a conversational tone, such as 'Hey there! I’m here to help with any questions you might have. Let’s get your issue sorted!'"
4. Few-Shot Prompting
Objective: Teach the AI how to respond using a few examples, enabling it to generalize for similar situations.
Prompt Pattern:
Prompt: "Here are some examples of how to handle technical questions:
'My phone isn't charging.' → 'Have you tried using a different cable? If that doesn’t work, it may be an issue with the port.'
'The screen is flickering.' → 'It sounds like a display issue. Have you tried restarting the device?'
Now, respond to: 'My app keeps crashing.'"
5. Chain of Thought Prompting
Objective: Use a step-by-step reasoning approach for resolving more complex or technical issues.
Prompt Pattern:
Prompt: "When a customer reports their laptop overheating, guide them through the following steps:
Ask if they are using the laptop on a soft surface.
Suggest moving the laptop to a flat, hard surface for better airflow.
Ask if they’ve cleaned the vents recently.
Recommend restarting the device to see if the issue persists.
Now, solve: 'My laptop fan is making a loud noise.'"
6. Instruction with Constraints
Objective: Instruct the chatbot to provide assistance while adhering to specific constraints (e.g., response length or tone).
Prompt Pattern:
Prompt: "Respond to order inquiries in no more than 50 words and avoid using technical jargon. For example, 'Your order is on the way and should arrive by [date]. Feel free to reach out if you need anything else.'"
7. Reflective Prompting
Objective: Ensure that the chatbot reflects the user’s query back to them before providing a response, reducing misunderstandings.
Prompt Pattern:
Prompt: "When a customer asks for help, first reflect their question back to them. For example, if they ask 'How can I reset my password?' respond with 'You're asking how to reset your password, correct? Here’s how you can do it.'"
Result: The various types of Prompts are executed successfully.

## prompt and output:

# 1. Direct Instruction Prompts
Use Case: Order Status Inquiry

Scenario: Customer asks, “Has my order shipped yet?”

Refined Chatbot Response:
"Your order is currently being processed and is expected to ship by May 10. You will receive an email with tracking details once it ships. Is there anything else I can assist you with?"

Explanation:
By providing more precise information about when the order will ship (rather than just saying it's "being processed"), the chatbot sets clear expectations. It also invites further engagement by offering additional help.

Additional Scenario:
Customer asks, “How can I track my order?”

Response:
"You can track your order by visiting [tracking website], where you can enter your tracking number to get real-time updates. Let me know if you need assistance finding the number!"

# 2. Contextual Prompting
Use Case: A Customer Reports Missing Item from Order

Scenario: Customer says, “I only received part of my order.”

Refined Chatbot Response:
"I see that part of your order is missing. Let me check on the remaining items for you. Can you please provide your order number so I can investigate further?"

Explanation:
The response directly addresses the customer's concern while ensuring they are prompted to provide relevant information (order number) to move forward. The chatbot acknowledges the context of the previous statement, showing it is actively listening.

Additional Scenario:
Customer says, “I have already contacted you about my refund.”

Response:
"Thanks for letting me know. I see you've already reached out about your refund. Let me check the status for you and get back with an update shortly."

# 3. Persona-Based Prompting
Use Case: Friendly & Empathetic Interaction

Scenario: Customer starts a chat with a general inquiry about a product.

Refined Chatbot Response:
"Hey there! 😊 I’m here to help you out with anything you need! Whether it’s finding the perfect product or answering any questions you have, I’m just a message away. What can I do for you today?"

Explanation:
Using emojis and a cheerful tone, the chatbot offers an upbeat, friendly experience that feels more personal. This helps build rapport with the customer from the start.

Additional Scenario:
Customer says, “I’m so frustrated with this product!”

Response:
"I totally get how frustrating that must be! 😔 Let’s figure out what’s going wrong and get this sorted for you. Can you tell me a bit more about the issue?"

# 4. Few-Shot Prompting
Use Case: Technical Troubleshooting

Scenario: Customer says, “My headphones aren’t connecting to Bluetooth.”

Refined Chatbot Response (learned pattern):
_"Let’s try a couple of things to fix that:

Make sure Bluetooth is enabled on your device.

Forget the headphones from your Bluetooth settings and try reconnecting them.

If that doesn’t work, try restarting your phone and turning the headphones on again.
Let me know how it goes!"_

Explanation:
The chatbot uses a simple, step-by-step troubleshooting approach based on a few-shot pattern from similar tech issues, such as Bluetooth problems. It breaks down the solution into manageable steps, increasing the chances of a quick resolution.

Additional Scenario:
Customer says, “I’m getting an error message on my app.”

Response:
_"Let’s start by trying a few things:

Close and reopen the app.

Check if there’s an update available.

If the issue persists, try reinstalling the app.
If you still see the error, send me a screenshot and I’ll look into it further."_

# 5. Chain of Thought Prompting
Use Case: Troubleshooting More Complex Issues

Scenario: Customer says, “My laptop is overheating.”

Refined Chatbot Response:
_"Let’s troubleshoot step by step:

Are you using your laptop on a soft surface (like a bed or couch)? This can block the air vents.

Try placing the laptop on a flat, hard surface to help with cooling.

Have you cleaned the fans recently? Dust buildup can cause overheating.

If it’s still overheating, consider checking for any software or apps running in the background that might be using too much power.
Let me know what happens after these steps!"_

Explanation:
The chatbot methodically walks the user through potential causes of the issue and provides a structured way to narrow down the problem. This chain-of-thought approach works well for more complex technical issues where multiple factors could be at play.

Additional Scenario:
Customer says, “My printer isn’t connecting to Wi-Fi.”

Response:
_"Let’s break it down:

First, check if your Wi-Fi is working fine with other devices.

Make sure your printer is in range of the router.

Try restarting both the printer and the router.

Ensure your printer is connected to the correct Wi-Fi network.
Let me know if these steps help!"_

# 6. Instruction with Constraints
Use Case: Short, Concise Responses

Scenario: Customer asks, “When will my refund be processed?”

Refined Chatbot Response (≤50 words, no jargon):
"Your refund is being processed and should be completed by May 10. You’ll receive a confirmation email once it's done. Please reach out if you need any more information!"

Explanation:
This response adheres to the constraint of being concise (under 50 words), while still addressing the query clearly. It avoids any jargon and offers an easy-to-understand solution while maintaining a polite and helpful tone.

Additional Scenario:
Customer asks, “How do I cancel my order?”

Response:
"To cancel your order, please go to your order history and select the ‘Cancel Order’ option. If you need help with this, just let me know!"

# 7. Reflective Prompting
Use Case: Clarifying the Customer’s Request

Scenario: Customer says, “How do I return a defective item?”

Refined Chatbot Response:
_"You’re asking how to return a defective item, right? Here’s how you can do it:

Log in to your account and go to your order history.

Select the item you wish to return and click ‘Return Item.’

Follow the steps to print your return label.
Let me know if you need help with any step!"_

Explanation:
The chatbot first reflects the customer’s inquiry to confirm its understanding, then provides clear and actionable steps. This method ensures the customer feels heard and confident that the solution is tailored to their request.

Additional Scenario:
Customer says, “I need to change my shipping address.”

Response:
_"You're asking how to update your shipping address, correct? Here’s how:

Go to your account settings.

Click on ‘Shipping Address.’

Enter the new address and save the changes.
Let me know if you have any questions!"_

Conclusion:
Each of these refined examples can be adapted for various customer service situations, from simple order inquiries to more complex troubleshooting. The patterns offer flexibility for tailoring responses in a way that feels natural and empathetic, while also ensuring efficiency. Let me know if you'd like to dive into specific industry examples (e.g., e-commerce, tech support) or explore further use cases!


# Result:
 Thus the Prompts were exected succcessfully .



