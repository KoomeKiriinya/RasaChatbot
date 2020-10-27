## say goodbye
* goodbye
  - utter_goodbye

## bot challenge
* bot_challenge
  - utter_iamabot

## survey happy path
* greet
    - utter_greet
* affirm
    - health_form
    - form{"name": "health_form"}
    - form{"name": null}
    - utter_slots_values
    - action_reset_slots
* thankyou
    - utter_no_worries
    - utter_goodbye

## no survey
* greet
    - utter_greet
* deny
    - utter_goodbye

## survey stop
* greet
    - utter_greet
* affirm
    - health_form
    - form{"name": "health_form"}
* out_of_scope
    - utter_ask_continue
* deny
    - action_deactivate_form
    - form{"name": null}
    - action_reset_slots
    - utter_goodbye
