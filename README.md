# TwoSidedDialogueSystem

The **Two Sided Dialogue System** is a dialog system controlled by text scripts through data tables.

# The structure of the Dialogues
+ 1.Dialogue Speaker - The initiator of the dialogue, the speaker
* 2.Dialogue Text - The text of the dialog box where you can change it using modifiers (see the paragraph below)
+ 3.Delay to delete - The time until the dialog is deleted.` If the value is less than zero, the dialog will not be deleted until the [End] command is issued`

# Text Modifers
The Two Sided Dialogue System has a large number of options for changing text. Here are all of them:
```
1.<A.AnimationName> - Add text animation
```
#  
All Animation Names:
> + 1.JumpIn
> * 2.ScaleIn
> + 3.OpacityIn
> * 4.StrengthJumpIn
#  
```

2.<Static> - removes text animation
3.<Speed number> - change text speed
4.<y> change text color to yellow
5.<b> change text color to blue
6.<c> change text color to cyan
7.<g> change text color to green
8.<o> change text color to orange
9.<p> change text color to pink
10.<v> change text color to purple
11.<r> change text color to red
12.<Default> and <def> change text to default style
```
## `You can add and change additional parameters in the "DialogueTextStyle" file`

