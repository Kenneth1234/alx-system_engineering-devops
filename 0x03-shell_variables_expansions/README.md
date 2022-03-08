0x03. Shell, init files, variables and expansions

Tasks:

- ' alias ls="rm *" 'creates an alias named ls with value rm *
Hello you - ' echo "hello $USER" ' prints hello user, where user is the current Linux user.
The path to success is to take massive, determined action - 'export PATH=$PATH:/action' Adds /action to the PATH. /action is the last directory the shell looks into when looking for a program.
If the path be beautiful, let us not ask where it leads - ' echo $((` echo $PATH | tr ':' '\n' | wc -l ' counts the number of directories in the PATH.
Global variables - ' printenv ' lists environment variables.
Local variables - ' set ' lists all local variables and environment variables, and functions.
Local variable - ' BEST="School" ' creates a variable named BEST with value School.
Global variable - ' export BEST="School" ' creates a new global variable.
Every addition to true knowledge is an addition to human power - ' echo $((128 + $TRUEKNOWLEDGE))' prints the result of the addition of 128 with the value stored in the environment variable TRUEKNOWLEDGE, followed by a new line.
Divide and rule - ' echo $(($POWER / $DIVIDE))' prints the result of POWER divided by DIVIDE, followed by a new line.
Love is anterior to life, posterior to death, initial of creation, and the exponent of breath - ' echo $(($BREATH ** $LOVE)) ' displays the result of BREATH to the power LOVE.
There are 10 types of people in the world -- Those who understand binary, and those who don't - ' echo $((2#$BINARY)) ' converts a number from base 2 stored in the environment variable BINARY to base 10.
Combination - ' echo {a..z}{a..z} | tr ' ' '\n' | grep -v "oo" ' rints all possible combinations of two letters, except oo.
Letters are lower cases, from a to z

One combination per line

The output should be alpha ordered, starting with aa

Do not print oo

Your script file should contain maximum 64 characters

Floats - ' printf "%.2f\n" $NUM ' prints a number stored in the environment variable NUM with two decimal places, followed by a new line.
Decimal to Hexadecimal - ' printf "%x\n" $DECIMAL' converts a number stored in the environment variable DECIMAL to base 16, followed by a new line.
Everyone is a proponent of strong encryption - ' tr 'A-Za-z' 'N-ZA-Mn-za-m' ' encodes and decodes text using the rot13 encryption. Assuming ASCII.
The eggs of the brood need to be an odd number - ' paste -d, - - | cut -d, -f1 ' prints every other line from the input, starting with the first line.
I'm an instant star. Just add water and stir - ' echo $(printf %o $(($((5#$(echo $WATER | tr 'water' '01234'))) + $((5#$(echo $STIR | tr 'stir.' '01234'))))) | tr '01234567' 'bestchol') 'adds the two numbers stored in the environment variables WATER and STIR and prints the result.
WATER is in base water

STIR is in base stir.

The result should be in base bestchol
