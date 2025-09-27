Shell, init files, variables and expansions

By: Julien Barbier
Weight: 1
Project Duration: Sep 13, 2025 → Sep 26, 2025

📚 Resources

Read or watch:

Expansions

Shell Arithmetic

Variables

Shell initialization files

The alias Command

Technical Writing basics

Man or help:
printenv, set, unset, export, alias, unalias, ., source, printf

🎯 Learning Objectives

By the end of this project, you should be able to explain (without Google):

General

What happens when you type:

ls -l *.txt


→ The shell expands *.txt (globbing), then executes /bin/ls with arguments.

Shell Initialization Files

/etc/profile and /etc/profile.d → System-wide login shell configs

~/.bashrc → User-specific non-login shell config

Variables

Local vs Global variables

Reserved variables (HOME, PATH, PS1)

Special parameters ($?, $#, $*, $@)

Create, update, delete shell variables

Expansions

Word, pathname, arithmetic, variable, and command expansions

Quotes: single ' ' vs double " "

Command substitution: `cmd` or $(cmd)

Shell Arithmetic

$((expression)) syntax

Operators: + - * / % **

Aliases

Create: alias name='command'

List: alias

Disable: \command or unalias name

Other Help Pages

Execute commands from a file: . file or source file

⚙️ Requirements

Editors: vi, vim, emacs

Scripts tested on Ubuntu 20.04 LTS

Each script = 2 lines only

Files must end with a newline

First line = #!/bin/bash

README.md must describe each script

Forbidden: &&, ||, ;, bc, sed, awk

All files executable

📂 Project Tasks & Solutions
0. Alias

File: 0-alias
Create alias ls='rm *'

#!/bin/bash
alias ls='rm *'

1. Hello you

File: 1-hello_you
Print: hello <current_user>

#!/bin/bash
echo "hello $USER"

2. The path to success

File: 2-path
Add /action to the end of PATH.

#!/bin/bash
export PATH="$PATH:/action"

3. Count directories in PATH

File: 3-paths

#!/bin/bash
echo $PATH | tr ':' '\n' | wc -l

4. Global variables

File: 4-global_variables

#!/bin/bash
printenv

5. Local variables

File: 5-local_variables

#!/bin/bash
set

6. Create local variable

File: 6-create_local_variable

#!/bin/bash
BEST="School"

7. Create global variable

File: 7-create_global_variable

#!/bin/bash
export BEST="School"

8. True knowledge

File: 8-true_knowledge

#!/bin/bash
echo $((TRUEKNOWLEDGE+128))

9. Divide and rule

File: 9-divide_and_rule

#!/bin/bash
echo $((POWER/DIVIDE))

10. Exponent of breath

File: 10-love_exponent_breath

#!/bin/bash
echo $((BREATH**LOVE))

11. Binary to Decimal

File: 11-binary_to_decimal

#!/bin/bash
echo $((2#$BINARY))

12. Combinations

File: 12-combinations

#!/bin/bash
echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo"

13. Floats

File: 13-print_float

#!/bin/bash
printf "%.2f\n" $NUM

14. Decimal to Hexadecimal

File: 14-decimal_to_hexadecimal

#!/bin/bash
printf "%x\n" $DECIMAL

15. ROT13 Encryption

File: 15-rot13

#!/bin/bash
tr 'A-Za-z' 'N-ZA-Mn-za-m'

16. Odd lines

File: 16-odd

#!/bin/bash
sed -n 'p;n'

17. Water and Stir (Base conversions)

File: 17-water_and_stir

#!/bin/bash
echo $(( $(echo $WATER | tr water 01234) + $(echo $STIR | tr stir. 01234) )) | tr 0123456789 bestchol

🔑 Extra Techniques Learned

Using tr for text transformation and encoding

Using printf for formatting (hex, float, etc.)

Understanding base conversion in bash (2#, printf %x)

Using brace expansion {a..z}

Using pipes to chain commands efficiently

How to disable an alias temporarily with \command

✅ Conclusion

This project teaches core Bash fundamentals: environment vs local variables, expansions, arithmetic, aliases, initialization files, and simple scripting.
It strengthens your ability to understand what happens inside the shell when you type commands.

👉 Repo: alu-shell
👉 Directory: init_files_variables_and_expansions
