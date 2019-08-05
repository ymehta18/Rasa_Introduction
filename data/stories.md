## happy path
* greet
  - utter_greet
* inform{"name"="Bob"}
  - slot{"name":"Bob"}
  - utter_tell
* mood_great
  - utter_happy

## sad path 1
* greet
  - utter_greet
* inform{"name"="Bob"}
  - slot{"name":"Bob"}
  - utter_tell
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* affirm
  - utter_happy

## sad path 2
* greet
  - utter_greet
- utter_ask
* inform{"name"="Bob"}
  - slot{"name":"Bob"}
  - utter_tell
* mood_unhappy
  - utter_cheer_up
  - utter_did_that_help
* deny
  - utter_goodbye

## say goodbye
* goodbye
  - utter_goodbye

## story ask_name
  - utter_ask
* inform{"name"="Bob"}
  - slot{"name":"Bob"}
  - utter_tell
* goodbye
  - utter_goodbye

## story hello
* greet
  - utter_greet

## story time
* ask_time
  - utter_time

