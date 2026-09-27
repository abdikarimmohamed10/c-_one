
| Course Title | C# Programming I |

| Course Code | CA242 |

| Department | Computer Application |

| Faculty | Computer & Information Technology |

| University | Jamhuriya University of Science & Technology |

| Academic Year | 2026 |

| Semester | IV |

| Student | Abdikarim Mohamed Salad |


# ASSIGMENTS
c# programming language

# Starting Out with Visual C# (Gaddis, 6th Edition)

## Chapter 1: Introduction to Visual C#

- Object: a program component with data (properties) and operations (methods).
- Control: a visible object in a GUI (Label, Button, TextBox). A class describes a type of object.
- .NET: a collection of classes for building Windows programs. Visual Studio is the IDE.
- Main windows: Designer, Solution Explorer, Properties, Toolbox.
- Project vs Solution: a project is one application; a solution is a container for projects.
- Naming controls: start with a letter or `_`, no spaces, use camelCase (`showDayButton`).
- Code structure: Namespace ---> Class ---> Method. GUI apps are event-driven.
- Common statements:

C#
MessageBox.Show("Hello World");
answerLabel.Text = "Result";
this.Close();          // close the form


- Comments: // line and /* block */.
- Errors: syntax errors show a red wavy line; wrong statement order causes logic errors.


## Chapter 2: Processing Data

Variables and types

| Type | Use | Example |
|---|---|---|
| `string` | Text | `"Hello"` |
| `int` | Whole numbers | `40` |
| `double` | Fractions | `87.6` |
| `decimal` | Money (literal ends with `m`) | `28.75m` |


Calculations
- Operators: + - * / % . Integer division: 7 / 3 = 2 ; use (double)x / y for 2.33.
- `double` and `decimal` cannot be mixed in one operation.

Input and output
- TextBox text is a string.
 Convert with int.Parse, double.Parse, decimal.Parse.


------

- var is optional, not mandatory. Whenever the assigned value is known, var shortens the code, but it always requires an initialization value at the point of declaration.
- Numeric types (int, double, decimal) matter in calculations. Mixing types works when one side is int, but double and decimal cannot be combined directly - types need to be checked before combining them.
- int / int division can silently lose data. For example, 7 / 3 returns 2, not 2.33. Casting one operand to double fixes this.
- Everything from a TextBox is a string, even if it looks like a number - so int.Parse(), double.Parse(), or decimal.Parse() is always needed before doing math with it.
- To display a number, it must be converted back to a string with .ToString(), which can also be formatted (currency, percentage, etc.) when a cleaner display is needed.
- Exceptions are a normal part of programs, so try-catch isn't optional - it's how you keep a program from crashing when a user enters invalid input. ex.Message tells you exactly what went wrong.
- Constants (const) are for values that never change (like an interest rate), making the code easier to read and preventing accidental changes later.

