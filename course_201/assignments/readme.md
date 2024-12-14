 **1. Messages**
- **Purpose:** Messages are the input format for the conversation. They represent a structured sequence of the dialogue between the user and the AI.
- **Functionality in Gemini API:** 
  - Each message includes a `role` (e.g., `user`, `assistant`, or `system`) and `content`. 
  - The `system` role can set the context, rules, or behavior for the AI.
  - The `user` role contains the input or query.
  - The `assistant` role holds the AI's response in a conversational thread.
 **2. Model**
- **Purpose:** Determines which version or type of the AI model will be used for processing the request.
- **Functionality in Gemini API:**
  - The model parameter specifies the exact version of Gemini to use (e.g., `gemini-1.5-flash`).As i used while making chatbot.
  - 
    ![Screenshot 2024-12-12 232750](https://github.com/user-attachments/assets/7c311818-9fad-477a-94a0-1b99c99a2aae)

  - Advanced models may offer better performance, reasoning, or response quality at the cost of higher resource usage.

 **3. Max Completion Tokens**
- **Purpose:** Sets the limit on the number of tokens (words or parts of words) in the generated response.
- **Functionality in Gemini API:**
  - Defines the maximum size of the response, ensuring it doesn't exceed a specified length.
  - Prevents excessive usage or responses too long for practical use.
  - Balances brevity and informativeness.

 **4. n**
- **Purpose:** Controls the number of response completions to generate per request.
- **Functionality in Gemini API:**
  - If `n` is set to 3, for example, Gemini API will generate three different responses for the same query.
  - Useful for comparing outputs or when a range of suggestions is needed.
 **5. Stream**
- **Purpose:** Enables or disables real-time streaming of the response.
- **Functionality in Gemini API:**
  - When `stream` is `true`, the response is delivered incrementally (token by token) in real-time.
  - Useful for scenarios where latency matters, like chatbots, where users prefer seeing the response appear as it's generated.
 **6. Temperature**
- **Purpose:** Controls the randomness or creativity of the AI's responses.
- **Functionality in Gemini API:**
  - A higher value (e.g., `0.8`) makes the output more diverse and creative.
  - A lower value (e.g., `0.2`) ensures focused and deterministic outputs, suitable for tasks requiring precision or accuracy.
**7. Top_p**
- **Purpose:** Implements nucleus sampling, controlling the probability distribution of token selection.
- **Functionality in Gemini API:**
  - If `top_p` is set to `0.9`, the API considers only the most probable tokens that cumulatively add up to 90% probability.
  - Balances randomness and coherence by dynamically narrowing the selection scope.

**8. Tools**
- **Purpose:** Specifies auxiliary capabilities or plugins that the AI can use to enhance functionality.
- **Functionality in Gemini API:**
  - Tools could include APIs for accessing external systems like calculators, browsers, or databases.
  - When tools are enabled, the AI can perform tasks beyond standard text-based responses, such as looking up live data or performing computations.



