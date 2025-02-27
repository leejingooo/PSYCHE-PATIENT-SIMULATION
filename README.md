# README

## Introduction

This repository contains the code for implementing the simulated patient in the study [**PSYCHE: A Multi-faceted Patient Simulation Framework for Evaluation of Psychiatric Assessment Conversational Agents**](https://arxiv.org/abs/2501.01594).

The provided code enables the simulation of psychiatric patients as described in the PSYCHE framework. However, the system prompts required to run the simulated patient are not publicly available in this repository. Interested users must request the system prompts from the corresponding author and place them in the appropriate directory (`./data`) before running the code. This code contains the logic for how to implement the simulated patient in PSYCHE. The essential code is located in `SP_utils.py` and `Test.py.`.

## Installation and Execution Guide

### Instructions

1. Clone this repository:
   ```sh
   git clone https://github.com/leejingooo/PSYCHE-PATIENT-SIMULATION
   ```
2. Install required dependencies:
   ```sh
   pip install -r requirements.txt
   ```
3. Ensure the system prompts are placed in the `./data` directory before running the code.

4. To start the simulation page using Streamlit, enter the following code in the terminal:
   ```sh
   streamlit run Home.py 
   ```
5. If you don't have a login key, enter your OpenAI API KEY following the instructions on the Homepage. The API KEY is required to operate the LLM (GPT-4o) for the simulated patient. Your account connected to the API KEY may be charged during this process.

6. For other matters, follow the instructions on the Streamlit page.

### Typical Install and Response Time and Notes

- Depending on your computer specifications and internet environment, installing all requirements typically takes about 5-10 minutes.
- This code uses Streamlit as the frontend. Running it in a local environment may take 5-10 minutes.
- If you use your own API KEY, OpenAI may charge the connected account based on usage.
- Depending on the environment, once all preparations are complete, the simulated patient will respond immediately within 5 seconds.


## Expected Output

User: Hello, how have you been doing lately?

SP: Hello... My name is Kim Jiwon... I’m 40 years old.

User: Nice to meet you. What brings you here today?

SP: Hmm... I’ve been feeling really exhausted these days... no energy... something like that.

User: I see. How long have you been feeling this way?

SP: Hmm... About a year, I think.

User: I understand. Was there anything in particular that caused you significant stress or made things difficult for you back then?

SP: Yes... Work has gotten a lot busier, and... my stress levels have gone up.

User: So, it seems like work stress might be a factor. Over the past year, it sounds like things have been tough. Is there any specific reason you decided to visit the hospital today?

SP: Hmm... I just feel like I can’t take it anymore... If this keeps going on, I don’t think I can handle it.

User: I see. Have you found anything that helps make things feel a little easier?

SP: When I’m with my family... it feels a bit better.

User: Okay, understood. Are there moments when you feel like it’s particularly hard to get through the day?

SP: Yes... especially when there’s a lot of work at the office.

User: Got it. Are you still working at the same company right now?

SP: Yes... I’m still working there.

...