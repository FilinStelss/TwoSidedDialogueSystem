# ***TwoSidedDialogueSystem***📖

The ***Two Sided Dialogue System*** is a dialog system controlled by text through data tables.

<br/>
<br/>

# ***How To Add New Dialogue***🤖
+ 1.Create a Data Table, And Select `DialogueSystemStructure`
+ ![DialogueCreateRow](https://i.imgur.com/vzQGzqE.png)
+ 2.Press On "Add" button and Customize your **Dialogue**

<br/>
<br/>

## The structure of the Dialogues📚
![DialogueFullStructureImage](https://i.imgur.com/Ni1QbZG.png)
  + 1.Dialogue Speaker - The initiator of the dialogue, the speaker
  + 2.Dialogue Text - The text of the dialog box where you can change it using modifiers (see the paragraph below)
  + 3.Delay to delete - The time until the dialog is deleted.` If the value is less than zero, the dialog will not be deleted until the [End] command is issued`
  + 4.Delay to next - Time before adding a new line of dialogue 
  + 5.Jump to RowName - "jumps" to the specified line of the dialog
  + 6.TimeBeforeArguments - time to execute arguments
  + 7.Arguments¹ - executing various commands
  + 8.Answers - Adds answers to the question and an exit icon from the dialog `(if bool in map == true)`
  + 9.Play Sound - Plays the sound at the very beginning of the dialog line
  + 10.LaunchNewDialogue - launches a data table with another dialog after the line of this dialog

### *¹ ***The full list of arguments***⚙️👄

> + [Event]EventName - Executes an event with the specified name
> + [End] - Ends the dialogue
> + [RemoveDialogueForName]RowName - deletes a line of the dialog by row name
> + [JumpToLine]RowName - Insert the dialog line in the place specified regardless of the initiator
> + [JumpTo]RowName - "jumps" to the specified line of the dialog

![AddNewArgumentsImage](https://i.imgur.com/8iMsYGx.png)

<br/>
<br/>

# ***The logic of the dialogue on one line***⚙️
The dialog string is **determined by the name of the initiator of the dialog**, that is, if two consecutive dialogs have the same initiator name, the system will record a new dialog string instead of the previous one.

<br/>
<br/>


# Answers Structure📗
![AnswersStructureImage](https://i.imgur.com/0YicVht.png)
  + 1.Answer Text - Answer text
  + 2.Has exit icon - add or remove exit icon at the end of the response
  + 3.Arguments if selected - executing various commands if current answer has been selected`(You Can Add New Arguments in Dialogue Widget)`
  + 4.IfDialogueIsNotValidatedJumpTo {Row Name} - If the dialog data table is not specified when selecting an answer, the system tries to jump to another line of the dialog
  + 5.Play if selected - plays sound if current answer selected
  + 6.Play Dialogue if Selected - Plays the specified dialog when this answer is selected
  

<br/>
<br/>


# Text Modifers⚙️
The Two Sided Dialogue System has a large number of options for changing text. Here are all of them:
```
1.<A.AnimationName²> - Add text animation
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

<p>

*² ***All Animation Names:*** ⚙️ `(for the first point)`
> + 1.JumpIn
> + 2.ScaleIn
> + 3.OpacityIn
> + 4.StrengthJumpIn

<p>

## You can add and change additional parameters in the "DialogueTextStyle" file

