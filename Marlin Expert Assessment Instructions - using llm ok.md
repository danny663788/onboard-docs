
# Marlin Expert Assessment Instructions

Version 1.0
_Last updated: January 8, 2025_
## I. Introduction

Your goal in the **Marlin Expert Assessment** within **Project Marlin** is to demonstrate you can find errors in a model's response to a coding question.

For the problem, you will be given a git repo, a prewritten prompt that asks a model to make changes to that repo, and the model's response. Your job will be to evaluate the model's response and find any errors it made.

### Summary of Your Task

- Download the provided zip of the repo and set up your workstation to view it. This represents the state of the repo **_prior_** to the conversation with the model.
- Review the prewritten user prompt to understand what is being asked of the model.
  - Make sure you have a good grasp of all requirements, so you can make sure all of them are addressed in the model's response.
- Read through the model's response and look for mistakes.
- Take the code changes the model makes as part of its response and modify the respective files in your local setup of the repo. Once you have all of the model's changes, be sure to run the tests included in the repo, or add more tests of your own to be confident the code changes are correct.
- In the task view, write down a list of all mistakes that you found in the model's response.
- Write a prompt for the next turn in this conversation. How would you go about asking for the model to fix any mistakes it made, or finish implementing any features from the first prompt that were missed?

### Important Information

- **You should only make a single submission**. Any submissions made beyond your first, will not be compensated or considered. Second attempts will be considered on a case-by-case basis.

- You have **180 minutes to complete this assessment task**, and it must be completed within a **single session**, otherwise your task will expire and prevent you from submitting.

## II. Full Task Instructions
### Step #1: How to start assessment
![](../../../../../assets/Pasted%20image%2020260125223559.png)

_Select this tile (_**_Marlin-Expert_Assessment-2_**_) on your dashboard to launch the project_

You will see:
![](../../../../../assets/Pasted%20image%2020260125223543.png)


### Step #2 :** Understanding the Interface

The application interface is a "split-screen" layout:
#### 2.1 **Left Side:** Displays the task description, a link to download the repo, the pre-written prompt, and the model's response.
#### 2.2 **Right Side:** Here you will answer two questions:
  - List the mistakes you found in the model's response, that would be blockers from merging the resulting code in a pull request. Mistakes can include anything from code mistakes, logical errors, missing features, or misinterpretations of the prompt's requirements. Format your response as a bullet pointed list.
  - Describe what you think was good about the model's response.
  - Describe any smaller, non-blocking issues that you found in the model's response.
  - Assume the previous prompt and model response was the first turn in a chat interaction with a model. How would you write the next prompt to encourage the model to complete and missing objects from the prompt and fix any errors you identified above?

### **Step #3:** Read the task description and tips for success fully

### **Step #4:** Download the provided repo and set it up for evaluation locally

- This file is the "current state" of the repo before the prompt and model response from the task.
- You are intended to take the changes the model suggests in its response to modify these files in order for you to test the model's response.

### **Step #5: ** Review the (prewritten) user prompt (block 0: user)

- Make sure you understand what is being requested.
- Keep these requests in mind as you review the response to make sure the entirety of the request is being handled.

![](../../../../../assets/Pasted%20image%2020260125223516.png)

Figure: Block 0: user - This it the prewritten user prompt

### **Step #6:** Review the model's response ( block 1: assistant)

- **Tip:** The model is a coding agent, its response will begin with a number of tool calls that allow you to see the inner workings of its process. The code files it outputs (which are at the very end of its response) are the result of its process. **_You only need to test the accuracy of the final code suggestions that the model makes._** Any mistakes the model makes before this point, as long as it corrects them, are acceptable.
- Look for any mistakes you can find in the response. Here's a list of possible mistakes to look out for:
  - Provided code that does not run
  - Test cases fail (either existing, or test cases you needed to add)
  - Missing test cases to cover newly added functionality
  - Added blocks of unnecessary or inefficient code
  - Provided solution that is far overcomplicated for what is needed
  - Model discusses code that it "added" but it is missing from the response
  - Features requested in the prompt are missing or not handled by the response
- As you go through the response, apply the model's suggested changes to the files in the repo you downloaded.
- Once all of the modifications are in place, test out the code. You can use any existing tests provided in the repo as a starting point.
- This is the longest part of the assessment, please take your time here and be diligent!

![](../../../../../assets/Pasted%20image%2020260125223459.png)

Figure: Block 1: assistant - This is the model's response

### **Step #6:** Write out a list of mistakes you found in the model's response

- Provide the mistakes in the text box, formatted as a bulleted list.
- Focus on serious mistakes, don't worry about wasting time on minor formatting or comment mistakes.

### **Step #7:** Provide a prompt for the next turn of interaction with the model

- Put yourself in the shoes of the original prompter. If the model made mistakes or did not address areas of the original prompt, how would you ask for it to make improvements?