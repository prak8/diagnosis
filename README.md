# Diagnosis System Chatbot

## Project Information

AIT 526
Final Project
Author: Team 1 - Alice Chen, Hrishikesh Karambelkar, Prakriti Panday, Sean Park


## Description of the problem to be solved 

The objective of this project attempts to simplify medical diagnosis, interpret the content, provide a score reflecting the severity of the diagnosis and define complex terms typically used in medical jargon. The main system entails a chatbot with multiple components integrated into it's script including a API connection to a medical library and a sentiment analyzer. Both these systems reflect the two main services offered by the chatbot, medical term definitions and diagnosis interpretation. The medical term utlizes an API key to connect to UMLS, a medical library. This connection extracts definitions that chatbot user may be interested in. The next component includes scoring the sentiment of the diagnosis using the Vader librar, which the user can comprehend either as a severe or non-severe diagnosis.

## An actual example of program output and usage

Figure A shows the output when asked to define medical terms


Figure B shows the output when asked to interpret the diagnosis

## Algorithm

* Input of the user's name to personalize the interaction
* Choose from 3 options: 1. Define medical term 2. Interpret diagnosis 3. Exit
* If 1. Enter one medical word, connect via API key to ULMS library, search the target word, extract the definition, and return as output to user.
* If 2. Enter complex diagnosis, tokenize it. Word spot to the provided script, apply to a modified sentiment analyzer with boosted scores to coordinate with the      medical jargon, scale the compound sentiment scores into severity catogories and finally return an output summarizing score and comprehensible interpretation. 

A flow diagram of the Diagnosis system chatbot

![Untitled Document-2](https://user-images.githubusercontent.com/90986120/144150961-c564bbb1-cb39-4833-9735-84ccec26ee8e.png)
