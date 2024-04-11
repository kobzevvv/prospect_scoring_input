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

#### Historical funnel data
table structure:
— prospect_id
— is funnel start event (boolean)
— is funnel end event   (boolean)

example of dataset: 




