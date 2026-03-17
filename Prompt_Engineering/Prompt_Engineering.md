Prompt Engineering Techniques:
Prompt engineering involves carefully designing input text to achieve improved outcomes from language models. An optimized prompt enables more accurate and refined results from LLMs.

3 C’s Prompt Template:

Context: 
Define clear context for the model, such as specifying roles and responsibilities. This helps the language model understand the situation or task it is being asked to address.

    Example:
    	Quality Analyst:  To design a test case for an user story 
    o	Behave like a Quality analyst and design test cases for Insurance login page

Role:
The role component plays a crucial part in prompt engineering by enabling the model to adopt the intended persona or perspective based on the input text. By specifying a clear role, the model is guided to generate responses that align closely with the desired viewpoint or expertise.
In addition, defining the role allows language models to understand their responsibilities within the context of the prompt. This helps them to use a suitable tone and approach, ensuring the output is relevant and tailored to the task at hand.

Constraints:
 Include constraints in the prompt to make it more specific. Constraints guide the model to focus on aspects or requirements of the task.

    Example:
    	Test Case Design: Include negative scenarios or browser compatibility

Clarity:
Provide clear instructions regarding the output format of the LLM response. This ensures the results are structured and meet the user's expectations.

    Example:
    	Provide test cases in a table with below provided columns
    o	Test Case ID,
    o	 Test Steps, 
    o	Description about Test Cases, 
    o	Expected Results


Types of Prompting:

Single Shot Prompting:
 
Providing instructions to models without any example to generate response

    Example1: Design test case for Banking Fraud Detection login page.

    Example 2: 
    Context: Behave like a Quality Analyst working on Banking Fraud Detection Application Instructions: Design test cases for valid login, invalid login and forget password
    Constraints: Include negative scenarios and browser compatibility (Edge and Chrome)
    Output: Provide test cases in a table with columns – Test Case ID, Description, Test Steps and Expected Results

Note: Both examples are single-shot prompts, but Example 2 is more optimized. It provides clear context and instructions for better responses, while Example 1 can cause the model to hallucinate and waste tokens and time.
Tokens:

Few Shot Prompting: 

Provide instructions to the model with one or more examples to generate response in a desired output format.

    Example: Behave like a Quality Analyst working on Banking Fraud Detection Application. Design Test cases for login page and below are example test cases.
    1.	TC1: Test case for valid login (steps and expected results)
    2.	TC2: Test Case for invalid login (same structure)


Chain of Thoughts Prompting:

Prompting AI to explain reasoning step by step. Useful for getting more detailed responses.

    Example:
    Input: Behave like a Test Automation Engineer working on playwright automation tool- python. What is the reason for the below error.
    Error: error description
    Output: list of possibilities of causing error.

Iterative Prompts:

Iterative prompting refers to breaking down tasks into multiple steps, with each prompt targeting a specific aspect of the overall objective. After each prompt, the outcome is thoroughly assessed and, if needed, modified before progressing to the next phase. This approach promotes greater accuracy and dependability by enabling ongoing refinement and verification throughout the process.