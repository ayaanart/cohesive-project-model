# Cohesive Project Model Manual
file: `manual.md`

## README
**This file's purpose:** explain how to use the Cohesive Project Model.

**What it is NOT:**
- List of benefits and weaknesses.
- Reasoning of decisions.
- Guide to help you decide if you should use this model.
- Summary/overview of the model.
> There are other files in the project folder that do this. Check the `README.md` file in the project folder for guidance.

This document uses many terms that are created for this model.
A created term is surrounded by asterisks and has a capital letter at the start of each word.
For example: *Jot Mode*.
You can find every term created for this project in `## Term Index`.
The terms in `## Term Index` are organized in alphabetic order with a definition next to them,
or a heading that explains the term.

The `## Term Index` lists only the root term, but you can add affixes with a hyphen outside the asterisks.
For example: *Jot Mode*-ing.

## Term Index
// TODO: Leave this for the last. Note: this is how I plan to structure the terms:
- Term
    - Def/heading
- Other Term
    - That terms def/heading
...keep going alphabetically

---

## *Mode*
*Mode*-s are a group of actions that contribute to a single aim which is designed to help finish the project.
Every *Mode* has a unique aim compared to any other *Mode*.
An individual is only in one *Mode* at a time,
but multiple people can be in different *Mode*-s at the same time.

## *Mode* Selection
- If *Prerequisite Mode* has never been entered for this project, then enter *Prerequisite Mode*.

- If *Prerequisite Mode* has been entered for this project, then enter *Selode Mode*.

Once you enter a *Mode* you exit the *Mode* once you complete the actions of that *Mode*,
or you need to enter another *Mode* to get something done. // TODO: figure out a better way to explain this

## Leaving *Mode*-s Unfinshed
On the file, or work you are leaving halfway write a TODO block at the end or in a reasonable spot.
Example:
```
<your-work-about-your-story-structure>

/*
TODO:
- Decide whoses prespective the story is in
- Decide how to start the story
*/
```
You do not need to follow a code like TODO block; you can keep the TODO in any style you want,
but you want to keep it concise, this is not your plan.

---

## *Jot Mode*

**Aim:** Quickly capture Head Idea(s) before they are forgotten.

**Actions:**
1. Jot your *Head Idea*(s) on your *Jot Pad*, which you decided on in *Prerequisite Mode*.
The style of jotting is up to you; you could write, draw or anything else,
but choose a style that is quick, and helps you recall easily.
You do not want a complete neat descriptions,
but rather something non-time consuming and can help you remember your *Head Idea*.

2. Store your *Jot Pad* in the place it belongs, which you decided on in *Prerequisite Mode*.

**Edge Cases:**
- If your *Jot Pad* is unavailable:
    - jot in something that you will use/see later.

- If you can not store your *Jot Pad* in the correct place:
    - store it in a reasonable place where you will see it later (like on your desk, not in a random drawer).

### Example
You are implementing an enemy for your video game but you are interrupted and need to attend to something else,
but then you just get a brainwave for a new enemy that you have not written anywhere,
so you quickly jot down
"enemy with the same attack that is slow or fast. The slow = parry and fast = dodge. Attack itself same, you watch the speed.",
in your sketchbook and then attend to the thing you have to do.


## *Brainstorm Mode*

**Aim:** Produce 1 solution and/or idea about something specific.

**Actions:**
1. Create a folder in `/brainstorm/raw/`.
The folder name should be the date you created this folder, and should use this format: YYYY-MM-DD.
Then followed by 2 keywords about what you are brainstorming separated with a hyphen.
Example:  `2026-09-15-peashooter-attack`
The keyword's job is to just jog your memory when you view the file name;
it does not have to represent your entire brainstorm.

2. Inside the folder you just created, create a file called `context.md`,
and inside `context.md` explain the context for your brainstorming, following this template:
```
# Folder Name in Title Case but Replace Date with the Word: "Brainstorm"
file: `context.md`

> current state: in-progress
> tags: <tags-separate-with-commas> /* used for finding this brainstorm:
e.g. find a brainstorm about a specific enemy, search all files for that enemy name in the tag section.
There should be around 3 tags */

## Aim
// what you are trying to brainstorm

## Reason
// the reason you are brainstorming, which would be the issue that caused you to need to brainstorm
```
Your current state is the current state of this brainstorming and will always be `in-progress` at step 2.
The file should be <80 words.
Do not spend too much time and effort on this file (e.g. trying to fix grammar),
instead make the file good enough that a person reading this can understand what you are brainstorming and why.
Make sure not to brainstorm too much at once, keep your aim scoped.
For example: Improve an enemy's AI to make it feel more fair, not brainstorm your entire game at once,
but do not let that scope trick you, sometimes the best solution for your aim can be not where you expected.
Taking the AI example, maybe the solution was to improve the terrain of your game to make it feel more fair.
Do not be shortsighted.

3. Begin brainstorming with any method of your choosing until you find the solution you want to continue with,
and then update the current state in `brainstorm/raw/<folder-name>/context.md` to `finished`.
Now you can no longer continue brainstorming in this folder,
and if you want to brainstorm again on the same aim you have to create a new folder.
While brainstorming can have many ideas, but you must select the 1 idea you want to use.
You often need *Learn Mode* during this step.
Remember if later you do not like the idea you selected, you can always brainstorm again.

4. Keep what you produced during the brainstorming session in the folder you created in step 1.
You can keep multiple files, with each attempt of brainstorming having their own file.
Name the file(s) `attempt-#` with # being a number that shows which attempt it was.
The first attempt will be `attempt-1` while the 5th attempt will be `attempt-5`.

5. Create a file in `/brainstorm/polished/`.
Name the file the same name you named the folder in step 1 followed by a `.md` extension.
Describe the result of your brainstorming and context in this file, following this format:
```
# <folder-name-in-title-case-but-replace-date-with-the-word:-"brainstorm">
file: `<name-of-folder-in-step-1>.md`

## Aim
// Explain the aim of this brainstorming.

## Reason
// explain the reason for brainstorming, which would be the issue that caused the need for brainstorming.

## Result
// explain the result of your brainstorming (your solution(s)) and why they work
```
This file's word count is not strict, so use how many words you need to communicate the idea.
Your word count will have to vary depending on the complexity of the idea.
This file does not need to be anywhere near perfect as it is not your official documentation.
It needs to convey the results of the brainstorm in a way that a person does not need to open anything in the `/brainstorm/raw`.
It does not need perfect grammar; it needs to be not painful to understand.
Do not spend long on this.

**Edge Cases:**
- You want to name a folder with a name that is already taken (very unlikely).
  	 - Change the keywords so that the name is different.

- You just started step 4 or 5 but want to go back to step 3.
    - You can go back track to step 3, just add `-INCOMPLETE` to the file name of the file you made in step 5 if you made a file,
    and change the current state in context.md back to `in-progress`.

- In step 4 you are unable to keep your brainstorming in `/brainstorming/raw` for whatever reason.
    - Still create the file, but for the file name swap `attempt` to `attempt-meta`, and instead of keeping what you brainstormed follow this format:
    ```
    # <folder-name-in-title-case-but-replace-date-with-the-word:-"brainstorm">
	file: `attempt-?-<#>.md`
    
    ## README
    You can access the actual brainstorm <say-where-can-access-it> /*
    if you can not access it anywhere change the line to: 
    "You can not access the brainstorm anywhere because <say-your-reason>.
    And end this heading with that. 
    You do not need to below line if you can not access the brainstorm anywhere.
    */

    The actual brainstorm was unable to be shown here because <state-your-reason>.
    
    ## Process
    The brainstorm used the process
    <explain-what-brainstorming-process-you-used.-Make-sure-it-flows-grammaticaly-with-the-sentence>
    
    ## Description
    <list-of-adjectives-and/or-adjectival-phrases-describing-the-actuall-brainstorm> // Do not describe the result.
    ```
    This file should be >80 words. Do not spend long on this.
    Note: If you did your brainstorming physically you can just upload a photo.

### Example
You want to brainstorm a unique character design for a rich man for a short story you are making.
You take out your notebook and pen and start brainstorming.
You decide on dressing him in complete purple, top to bottom.
Pant is purple; hat is purple, cane is purple, everything is purple.
You upload the photo to `/brainstorm/raw/` and you name the file attempt-1.png.
The entire process took around 30mins, with the actual brainstorming taking 20mins.
The other things only took 10mins all together
(which shows that you are not trying to make it perfect and you are not spending too much time polishing files).

## *Prerequisite Mode*

**Aim:** Complete the essential tasks required before entering any other *Mode.

**Actions:**
- In `/` create the *Goal File*.
- In `/` create the *Scope File*.
- In `/` create the *Jot File*.
Note: While we keep goal and scope in different files they both contribute to your goal.

**Edge Cases:**
- You want to change your goal, scope, or *Jot Pad*-(s)
	- Go ahead and enter *Prerequisite Mode* again and change what you want.
	Note: that you should not really being changing these often,
	especially your goal.
	If you keep changing your goal and scope then it becomes less guideness and more what the vibe is right now.
	If you keep changing your *Jot Pad*-(s) then you may not be able to remember it when you need it.

### Example
You get an urge to create a story that your little sister will enjoy.
When you felt this urge you instantly thought of how your little sister really loves mystery stories.
You enter *Prerequisite Mode*, and create the 3 needed files.
When creating the files you thought for a bit before deciding.
For your goal you made it: creating a story that your little sister will enjoy.
For your scope you decided on making it between 3000-5000 words as you did not want to take too long.
For your *Jot Pad* you decided on making it your sketchbook.
Notice how for your goal you did not make it creating a mystery story your sister will like.
It being a mystery story is just because your sister likes it, it is not your goal.
If the mystery story was part of your goal then you would do a mystery story even if your sister did not like it.

## *Selode Mode*

**Aim**: Decide which will be the best *Mode* for you to enter based on the current state of the project.

// TODO

---

