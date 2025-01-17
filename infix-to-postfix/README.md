<h1>
  <span class="headline">Infix to Postfix in Java Lab</span>
  <span class="subhead">Infix to Postfix</span>
</h1>

## Objective
Write a program to convert an arithmetic expression from infix to postfix notation using Java's Stack class.

## Requirements
An **infix expression** is an arithmetic expression where the operators are placed between the operands (for example, \( A + B \)). A **postfix expression** is a form where the operators come after the operands (for example, \( AB+ \)).

Your task is to write a program to convert an arithmetic expression from infix to postfix notation using Java's `Stack` class. Follow these rules for the conversion:

- **Operators and precedence rules**: 
   - \( + \) and \( - \) have the lowest precedence.
   - \( * \) and \( / \) have higher precedence.
   - \( ^ \) (exponentiation) has the highest precedence and is **right-associative**.
- **Parentheses rules**: 
   - When \( ( \) is encountered, push it onto the stack.
   - When \( ) \) is encountered, pop all operators until \( ( \) is encountered.
  
- Use the `InfixToPostfix` class in the starter code.

- The starter code includes a set of tests to help you verify your work. To run the tests, right-click on the `InfixToPostfixTest` class in the `src/test/java` directory and select **Run 'All Tests'**.

### Example inputs and expected outputs
Input: `A + B * C`  
Output: `ABC*+`

Input: `A * (B + C)`  
Output: `ABC+*`

Input: `A + B * C / (D - E)`  
Output: `ABC*DE-/+`


## Practical relevance
Humans typically write mathematical expressions in Infix format \(like A\*\(B+C\)\), but machines parse these expressions more efficiently when they are in Postfix format \(like ABC+\*\). Infix expressions like require multiple scans to evaluate, as the operations inside the parentheses must be resolved before those outside. In Postfix, the expression becomes ABC+*, allowing a compiler to evaluate it in a single scan. 
This exercise will help you:
- Understand the difference between infix and postfix expressions and why postfix is preferred for machine processing.
- Enhance your understanding of stack operations and the fundamentals of expression parsing. This knowledge is crucial for developing efficient compilers and interpreters.

