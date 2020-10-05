# Nano Cheat Sheet

:grey_question: GNU nano is a text editor for Unix-like computing systems or operating environments using a **command line interface**. It's written on **C** language.

## Contents

- [File Operations](#file-operations)
- [Edit Operations](#edit-operations)
- [Searching and Inserting Operations](#searching-and-inserting-operations)
- [Deleting Operations](#deleting-operations)
- [Special Operations](#special-operations)
- [Moving in File Operations](#moving-in-file-operations)
- [Special Operations in File](#special-operations-in-file)
- [Information Operations](#information-operations)
- [Other Operations](#other-operations)

</br>

### File Operations

|  Commands  | Descriptions                          |
| :--------: | ------------------------------------- |
| `CTRL + S` | Saving changes on current file.       |
| `CTRL + O` | Saves as operation on current file.   |
| `CTRL + R` | Inserting whole file in current file. |
| `CTRL + X` | Closing current file.                 |

</br>

### Edit Operations

|  Commands  | Descriptions                                                       |
| :--------: | ------------------------------------------------------------------ |
| `CTRL + K` | Copy and cut whole active cursor line.                             |
| `CTRL + M` | Adding a blank line on active cursor line.                         |
| `ALT + 6`  | Copy whole whole active cursor line.                               |
| `CTRL + U` | Pasting copied text.                                               |
| `ALT + T`  | Copy and cut operation between current cursor line to end of file. |
| `ALT + 3`  | Comment and uncomment on active cursor line.                       |
| `CTRL + ]` | Completes current word.                                            |
| `ALT + U`  | Undo last operation.                                               |
| `ALT + E`  | Redo last undo operation.                                          |

</br>

### Searching and Inserting Operations

|  Commands  | Descriptions                                 |
| :--------: | -------------------------------------------- |
| `CTRL + Q` | Backward search operation with entered text. |
| `CTRL + W` | Forward search operation with entered text.  |
| `ALT + Q`  | Finds next occurrence backward search.       |
| `ALT + W`  | Finds next occurrence forward search.        |
| `ALT + R`  | Replacing operation session.                 |

</br>

### Deleting Operations

|     Commands      | Descriptions                      |
| :---------------: | --------------------------------- |
|    `CTRL + H`     | Deletes character before cursor.  |
|    `CTRL + D`     | Deletes character under cursor.   |
| `ALT + Backspace` | Deletes word to the left.         |
|   `CTRL + Del`    | Deletes word to the right.        |
|    `ALT + Del`    | Deletes whole current line.       |
|     `ALT + T`     | Deletes whole after current line. |

</br>

### Special Operations

:warning: If you set up correct configuration, these commands fine executing.

|  Commands  | Descriptions                     |
| :--------: | -------------------------------- |
| `CTRL + T` | Runs commands.                   |
| `CTRL + J` | :question:                       |
| `ALT + J`  | :question:                       |
| `ALT + B`  | Syntax checking.                 |
| `ALT + F`  | Runs a formatter/fixer/arranger. |
| `ALT + :`  | Starts/stops recording of macro. |
| `ALT + ;`  | Replays macro.                   |

</br>

### Moving in File Operations

|         Commands         | Descriptions                        |
| :----------------------: | ----------------------------------- |
|        `CTRL + B`        | Cursor goes one character backward. |
|        `CTRL + F`        | Cursor goes one character forward.  |
| `CTRL + ←` or `CTRL + 2` | Cursor goes one word backward.      |
|        `CTRL + →`        | Cursor goes one word forward.       |
|        `CTRL + A`        | Cursor goes start of line.          |
|        `CTRL + E`        | Cursor goes end of line.            |
|        `CTRL + P`        | Cursor goes one line up.            |
|        `CTRL + N`        | Cursor goes one line down.          |
|        `CTRL + ↑`        | Cursor goes one block previous.     |
|        `CTRL + ↓`        | Cursor goes one block next.         |
|        `CTRL + Y`        | Cursor goes one page up.            |
|        `CTRL + V`        | Cursor goes one page down.          |
|        `ALT + \`         | Goes top of buffer.                 |
|        `ALT + /`         | Goes end of buffer.                 |
|  `ALT + 9 veya ALT + 7`  | Cursor goes up start of line.       |
|        `ALT + 8`         | Cursor goes down start of line.     |
|        `ALT + 0`         | Cursor goes down blank line.        |

</br>

### Special Operations in File

|         Commands          | Descriptions              |
| :-----------------------: | ------------------------- |
| `Alt + G` veya `CTRL + 7` | Cursor goes entred line.  |
|         `Alt + ]`         | Cursor goes left bracked. |
|         `Alt + ↑`         | Screen slides up.         |
|         `Alt + ↓`         | Screen slides down.       |
|         `Alt + <`         | :question:                |
|         `Alt + >`         | :question:                |
|         `Alt + S`         | :question:                |
|         `Alt + L`         | :question:                |
|         `Alt + Z`         | :question:                |

</br>

### Information Operations

|  Commands  | Descriptions                               |
| :--------: | ------------------------------------------ |
| `Ctrl + C` | Reports cursor position.                   |
| `Alt + D`  | Reports word/line/char count current file. |
| `Ctrl + G` | Shows help page.                           |
| `ALT + Y`  | Colourful syntax enables/disables.         |
| `ALT + X`  | Help mode enables/disables.                |
| `ALT + M`  | Mouse support mode enables/disables.       |
| `ALT + C`  | Constant cursor mode enables/disables.     |

</br>

### Other Operations

|   Commands    | Descriptions                                        |
| :-----------: | --------------------------------------------------- |
|   `Alt + i`   | Makes automatically whitespace.                     |
|   `Alt + J`   | Rearranges words which is sorted with 1 line space. |
|   `Alt + O`   | Turns Tab characters to whitespace characters.      |
|   `Alt + A`   | The mark operation enables/disables.                |
|     `Tab`     | Indents marked region.                              |
| `Shift + Tab` | Unindents marked region.                            |
|   `Alt + N`   | Shows line numbers.                                 |
|   `Alt + P`   | Shows whitespace with (.) dot.                      |
|   `Alt + V`   | Enters next keystorke verbatim.                     |
|  `Ctrl + L`   | Refreshs current nano.                              |
|  `Ctrl + Z`   | Suspends nano editor.                               |

</br>

:pray: If you know description replacing with :question: mark or add new command in Cheat Sheet just open a [request][request-link] or contact me on [linkedin][linkedin-link].

[request-link]: https://github.com/uysalserkan/Cheat-Sheets/pulls
[linkedin-link]: https://linkedin.com/in/uysalserkan
