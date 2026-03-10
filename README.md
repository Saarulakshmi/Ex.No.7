# Exno.7-Develop a prompt-based application tailored to their personal needs, fostering creativity and practical problem-solving skills while leveraging the capabilities of large language models.

# Date: 01.03.2026
# Register no: 212223050040
# Aim:
To develop a prompt-based application using ChatGPT - To demonstrate how to create a prompt-based application to organize daily tasks, showing the progression from simple to more advanced prompt designs and their corresponding outputs.

## AI Tools Required: 
- ChatGPT
- Google Gemini (optional)
- Claude AI (optional)

## Objective
To understand how LLMs interact with user prompts.
To build a simple application that processes user input and generates meaningful output.
To explore customization of prompts for personal or real-world use cases.

# Explanation: 
Prompt:
"Design a personal productivity assistant that can help manage daily tasks, schedule reminders, suggest wellness tips, and answer general queries. The assistant should interact using natural language and be adaptable to the user’s changing preferences over time."
Procedure:
1. Define the core requirements of a personal productivity assistant.
2. Identify and construct appropriate prompts for each task using an LLM (e.g., ChatGPT).
3. Simulate natural user interaction through a simple interface or command-line system.
4. Collect feedback or inputs from users and adapt responses accordingly.
5. (Optional) Integrate basic memory to simulate preference adaptation.
EXPECTED OUTPUT: - (attached the drive link)
Output (Example Response by LLM):
Personal Productivity Assistant Features:
1. Daily Task Manager:
o Accept tasks via natural language (e.g., "Remind me to call mom at 6 PM").
o Organize tasks by priority and deadline.
o Provide daily summaries and pending items.
2. Smart Scheduler:
o Schedule events and set reminders using contextual understanding.
o Notify user of overlapping appointments or free time slots.
3. Wellness Tips Generator:
o Suggest daily wellness advice (hydration, exercise, screen-time breaks).
o Adapt suggestions based on past user preferences and responses.

## Concept
A prompt-based application takes natural language input from the user, sends it to an AI model (like GPT), and returns a useful response.
This encourages:
Creative thinking
Logical problem solving
Personal customization (education, productivity, lifestyle, etc.)

## Example Application: Personal Task Assistant
How it works
User enters a prompt such as
“Create my study plan for tomorrow.”
The application sends this to the LLM.
The model generates a clear, personalized output.
The user can refine the prompt to get better results.

# INTRODUCTION

Large Language Models (LLMs) such as ChatGPT can be used to build intelligent prompt-based applications that assist users in performing daily tasks. By designing structured prompts, users can guide the AI model to produce meaningful, organized, and context-aware responses.

This experiment demonstrates how prompt engineering can be used to create small AI-assisted applications for productivity and daily management.

# APPLICATION SCENARIOS

The following prompt-based applications were designed:

1. Study Time Scheduler
2. Project Task Breakdown
3. Personal Budget Manager
4. Travel Itinerary Planner
5. Daily Productivity Assistant

# PROMPT PROGRESSION

## 1. Simple Prompt

Prompt:

Create a list of tasks for today.

### Output

- Attend college lecture
- Complete assignment
- Study programming
- Exercise
- Review notes

Observation:  
Simple prompts produce basic responses but lack structure and prioritization.

# 2. Structured Prompt

Prompt:

Create a structured daily schedule for a student including study time, exercise, meals, and relaxation.

### Output

Morning

- 7:00 AM – Wake up
- 8:00 AM – Breakfast
- 9:00 AM – College lectures

Afternoon

- 1:00 PM – Lunch
- 2:00 PM – Assignment work
- 4:00 PM – Study session

Evening

- 6:00 PM – Exercise
- 7:30 PM – Dinner

Night

- 9:00 PM – Revision
- 10:30 PM – Sleep

Observation:  
Structured prompts generate more organized and useful outputs.

# 3. Advanced Prompt – Study Time Scheduler

Prompt:

Act as a study planner. Create a weekly study schedule for an engineering student preparing for exams, including subject revision, practice problems, and short breaks.

### Output

Monday
- 9 AM – Mathematics revision
- 11 AM – Break
- 12 PM – Electronics problem solving

Tuesday
- 9 AM – Programming practice
- 11 AM – Break
- 12 PM – Control Systems revision

Wednesday
- 9 AM – Power Systems study
- 11 AM – Break
- 12 PM – Previous year question practice

Observation:  
Role-based prompts improve relevance and task-specific outputs.

# 4. Prompt-Based Application – Project Task Breakdown

Prompt:

Break down a final year engineering project into manageable tasks including planning, development, testing, and documentation.

### Output

Project Development Stages

1. Planning Phase
   - Define project objective
   - Conduct literature survey
   - Create project timeline

2. Development Phase
   - Design system architecture
   - Develop modules
   - Integrate components

3. Testing Phase
   - Perform unit testing
   - Validate results
   - Fix errors

4. Documentation Phase
   - Prepare report
   - Create presentation
   - Final review

# 5. Prompt-Based Application – Personal Budget Manager

Prompt:

Act as a financial assistant and create a simple monthly budget plan for a student.

### Output

Monthly Budget Plan

Income:
- Allowance: ₹5000

Expenses:
- Food: ₹2000
- Transport: ₹1000
- Study materials: ₹800
- Entertainment: ₹500
- Savings: ₹700

Recommendation:
Try to save at least 10–15% of your monthly allowance.

# 6. Prompt-Based Application – Travel Itinerary Planner

Prompt:

Create a 3-day travel itinerary for visiting Chennai including major tourist attractions, food suggestions, and transportation tips.

### Output

Day 1
- Visit Marina Beach
- Explore Kapaleeshwarar Temple
- Try South Indian meals

Day 2
- Visit Mahabalipuram
- Explore Shore Temple
- Local seafood dinner

Day 3
- Visit Government Museum
- Shopping at T Nagar
- Cultural performance in evening

# PERSONAL PRODUCTIVITY ASSISTANT FEATURES

1. Daily Task Manager
   - Accept tasks using natural language
   - Organize tasks based on priority

2. Smart Scheduler
   - Automatically schedule events
   - Detect conflicts in schedule

3. Wellness Tips Generator
   - Suggest hydration reminders
   - Encourage short breaks

4. Personalized Recommendations
   - Adapt responses based on user preferences

# ANALYSIS

The experiment shows that prompt engineering significantly improves AI responses.

| Prompt Type | Quality | Structure | Usefulness |
|--------------|--------|----------|-----------|
| Simple Prompt | Basic | Low | Moderate |
| Structured Prompt | Good | Medium | Good |
| Role-Based Prompt | High | High | Excellent |

Key Findings:

- Clear prompts produce better results.
- Role-based prompts generate more realistic responses.
- Detailed prompts help AI produce practical solutions.

# CONCLUSION

Prompt-based applications demonstrate how large language models can assist users in everyday activities such as scheduling tasks, managing budgets, planning travel, and organizing projects. By refining prompts, users can obtain more structured, accurate, and useful outputs.


## Sample Code (Python – simple console app)
```
import openai

openai.api_key = "YOUR_API_KEY"

while True:
    user_prompt = input("Enter your request: ")

    if user_prompt.lower() in ["exit", "quit"]:
        break

    response = openai.ChatCompletion.create(
        model="gpt-3.5-turbo",
        messages=[{"role": "user", "content": user_prompt}]
    )

    print("AI:", response.choices[0].message["content"])
```
## Output Example

Input:
“Generate a weekly workout plan for me.”

Output:
A structured workout plan with daily exercises.

# Result: 
The lab exercise resulted in the creation of a prototype concept for a personal assistant powered by large language models. Students were able to:
 Understand how to tailor LLM prompts to real-life applications.
 Foster creativity by designing features suited to their personal or academic lives.
 Learn prompt engineering techniques for optimal interaction with AI tools.
 Experience the versatility and utility of generative AI in solving everyday problems.
