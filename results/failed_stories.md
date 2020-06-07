## happy path 1 (C:\Users\mrira\AppData\Local\Temp\tmpjo_gitfz\96188083e3664774b8e13079557ab708_conversation_tests.md)
* greet: hello there!
    - utter_greet   <!-- predicted: utter_goodbye -->
* mood_great: amazing   <!-- predicted: greet: amazing -->
    - utter_happy   <!-- predicted: utter_goodbye -->


## happy path 2 (C:\Users\mrira\AppData\Local\Temp\tmpjo_gitfz\96188083e3664774b8e13079557ab708_conversation_tests.md)
* greet: hello there!
    - utter_greet   <!-- predicted: utter_goodbye -->
* mood_great: amazing   <!-- predicted: greet: amazing -->
    - utter_happy   <!-- predicted: utter_goodbye -->
* goodbye: bye-bye!
    - utter_goodbye


## sad path 1 (C:\Users\mrira\AppData\Local\Temp\tmpjo_gitfz\96188083e3664774b8e13079557ab708_conversation_tests.md)
* greet: hello
    - utter_greet   <!-- predicted: utter_goodbye -->
* mood_unhappy: not good   <!-- predicted: greet: not good -->
    - utter_cheer_up   <!-- predicted: utter_goodbye -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* affirm: yes   <!-- predicted: goodbye: yes -->
    - utter_happy   <!-- predicted: utter_goodbye -->


## sad path 2 (C:\Users\mrira\AppData\Local\Temp\tmpjo_gitfz\96188083e3664774b8e13079557ab708_conversation_tests.md)
* greet: hello
    - utter_greet   <!-- predicted: utter_goodbye -->
* mood_unhappy: not good   <!-- predicted: greet: not good -->
    - utter_cheer_up   <!-- predicted: utter_goodbye -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: not really   <!-- predicted: bot_challenge: not really -->
    - utter_goodbye   <!-- predicted: utter_iamabot -->


## sad path 3 (C:\Users\mrira\AppData\Local\Temp\tmpjo_gitfz\96188083e3664774b8e13079557ab708_conversation_tests.md)
* greet: hi
    - utter_greet   <!-- predicted: utter_goodbye -->
* mood_unhappy: very terrible   <!-- predicted: goodbye: very terrible -->
    - utter_cheer_up   <!-- predicted: utter_goodbye -->
    - utter_did_that_help   <!-- predicted: action_listen -->
* deny: no   <!-- predicted: greet: no -->
    - utter_goodbye


