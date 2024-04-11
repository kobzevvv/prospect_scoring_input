# This repo is for standartised input for prospect scoring

## usecase
Data from merketing events and other source

### marketing events as features to score
marketing channel, campaign, refferer or whatever

### visited page as features
page category, some part of page path and exactly the page (for populer page)

## standard input 
### sise
scoring should handle with 20k — 100k uniq features

### format
#### prospect with features array
table strucure:
— prospect_id
— features list (comma separated)

example https://docs.google.com/spreadsheets/d/1QMH8kIB26srrJSox4Gl29Vm0X6ywrhJlsCRz5Jb5Uec/edit#gid=2059325635

#### historical funnel data
table structure:
— prospect_id
— funnel start event (boolean)
— funnel end event   (boolean)



