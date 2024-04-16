# TwoSidedDialogueSystem

The **Two Sided Dialogue System** is a dialog system controlled by text scripts through data tables.

# The structure of the Dialogues
+ 1.Dialogue Speaker - The initiator of the dialogue, the speaker
+ 2.Dialogue Text - The text of the dialog box where you can change it using modifiers (see the paragraph below)
+ 3.Delay to delete - The time until the dialog is deleted.` If the value is less than zero, the dialog will not be deleted until the [End] command is issued`
+ 4.Delay to next - Time before adding a new dialog
+ 5.Jump to - "jumps" to the specified line of the dialog
+ 6.TimeBeforeArguments - time to execute arguments
+ 7.Arguments - executing various commands
+ 8.Answers - Adds answers to the question and an exit icon from the dialog `(if bool in map == true)`\
+ 9.Play Sound - Plays the sound at the very beginning of the dialog line
+ 10.LaunchNewDialogue - launches a data table with another dialog after the line of this dialog

#### __the full list of arguments__
  + >[Event]EventName - Executes an event with the specified name
  + >[End] - Ends the dialogue
  + >[RemoveDialogueForName]RowName - deletes a line of the dialog by row name
  + >[JumpToLine]RowName - Insert the dialog line in the place specified regardless of the initiator

# Text Modifers
The Two Sided Dialogue System has a large number of options for changing text. Here are all of them:
```
1.<A.AnimationName> - Add text animation
```

<p>

__All Animation Names:__
> + 1.JumpIn
> * 2.ScaleIn
> + 3.OpacityIn
> * 4.StrengthJumpIn

<p>
  
```
2.[<Static>] - removes text animation
3.<Speed 0.02> - change text speed
4.<y> - change text color to yellow
5.<b> - change text color to blue
6.<c> - change text color to cyan
7.<g> - change text color to green
8.<o> - change text color to orange
9.<pin> - change text color to pink
10.<pur> - change text color to purple
11.<r> - change text color to red
12.<Default> - and <def> change text to default style
```

## `You can add and change additional parameters in the "DialogueTextStyle" file`

