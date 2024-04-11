# This repo is for standartised input for prospect scoring

## usecase
1. Take data from marketing events and other sources and score prospects by chance of won
2. understend what features are the most important to make portret of Ideal Customer Profile (ICP)

![Screenshot 2024-04-11 at 00 09 01](https://github.com/kobzevvv/prospects_scoring_input_output/assets/24790956/d5f5e1bb-39e4-43c3-a173-0986cc4a281b)



### marketing events as features to score
marketing channel, campaign, refferer or whatever

### visited page as features
page category, some part of page path and exactly the page (for populer page)

## standard input 
### size
scoring should handle with 20k — 100k uniq features

### format
![Screenshot 2024-04-10 at 23 51 56](https://github.com/kobzevvv/prospect_scoring_input/assets/24790956/1deaa4f3-7b7f-4d06-81ab-b43ee863bd86)


#### prospect with features array
table structure:
— prospect_id
— features list (comma separated)

example https://docs.google.com/spreadsheets/d/1QMH8kIB26srrJSox4Gl29Vm0X6ywrhJlsCRz5Jb5Uec/edit#gid=2059325635

Important: 
Features shouldn't be an outcome of the goal completion event (for example: agreement amount)

#### Historical funnel data
table structure:
— prospect_id
— is proving started (boolean)
— is funnel end event   (boolean)

Question: Why so many columns if it could be just "prospect_id" with goal completion? 
Answer: BC it's straightforward to make a mistake here. With explicit fields it should be less often problems like these: 
- wrong sampling (when we have additional subset of prospects that not a part of funnel, we do this via: "is proving started" (boolean)
- causation missing. when goal completion were before the "is proving started" event


example of dataset: https://docs.google.com/spreadsheets/d/1PY3ee3V6hUlAyhj2kZz8-xiU8V5iyvnLECbtse-zRsQ/edit?usp=drive_link




