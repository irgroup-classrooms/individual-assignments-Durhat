# Command Line Commands
|**Command**|**Purpose**|
|---|---|
|**pwd** (Print Working Directory)|shows current directory|
||
|**cd** (Change Directory)|changes directory to what's putted behind it|
|***cd** flags*|
|cd .|current directory|
|cd ..|parent directory (directory above current)|
|cd ~|home directory|
|cd -|previous directory|
||
|**ls** (List Directories)|Shows all files/contents within current directory (or other directories by putter path after it)|
|***ls** flags*|
|ls -a|Shows hidden files (files starting with ".".|
|ls -l|Shows detailed list of files in a long format.|
|ls -la|-a and -l combined|
|ls -R|Recursively list directory contents
(lists ALL files going down the path of current directory)|
|ls -r|reverses sorting order|
|ls -t|sorts by midification time, newest first|
||
|**touch**|creates new file (*touch text.txt*)|
||
|**file**|shows file type|
||
|**cat**|shows file content|
||
|**less**|reduces content of files by displaying them in a paged manner with navigation commands|
|***less** navigation commands*|
|q|Quit and go back to shell|
|*arrow keys*|Page up, Page down, Up and Down|
|g|Moves to beginn of a text file|
|G|Moves to end of a text file|
|/search|Like cmnd/ctrl + F: Search inside the text|
|h|Help for how to use *less*|
||
|**history**|Shows history of commands that were used|
|**ctrl + R**|Browse through recent used commands by pressing ctrl + R repetedly. It also autofills recent used commands when typing in.|
|**!!**|Automatically runs last used command|
|**clear**|Clears shell completely|
||
|***Tab key***|Press Tab key for auto-completion for files, commands, directories etc.|
||
|**cp** (Copy)|Copy files or directories.|
|***cp** wildcards*|
|*|Represents all single characters or strings (e.g. cp *.jpg /home/pete/Pictures *copies all files with .jpg ending in that specific directory*)|
|?|Represents one character|
|[]|Represents every character within the brackets.|
|-i|Asks if you really want to run that command by putting it right after the command.|
||
|**mv** (Move)|Moves or renames file. *Rename (files or directories)*: mv oldfile newfile *Move*: mv file (or secondfile) /directory1/directory2|
||
|**mkdir** (Make Directory)|Creates one or multiple directories (e.g. mkdir directory1 directory2|
|*mkdir -p*|Creates subdirectories at the same time (mkdir -p directory1/sub1/sub2/)|
||
|**rm** (Remove)|Deletes file **immediately** without trash can (except write-protected files).|
|*rm -f*|Forces to delete files, also write-protected ones|
|*rm -r*|-r is needed to also be able to delete directories|
|*rmdir*|Deletes directory|
||
|**find**|Search for files: find [path] [searchcriterias] [action] (e.g. find . -name "file.txt")|
|*actions for **find***|
|-iname|Case-insensitive search|
|-type|Search for files (-type f) or directories (-type d)|
|-size|Search by size; k (kilobytes), M (megabytes), or G (gigabytes) (e.g. find . -size +10M)|
|-mtime|Search by modification Date|
|Combined Search Criteria|e.g. find . -name "*.txt" -size +1M|
|-exec|Perform actions when attached to search-command (example for deleting all .log files in current directory: find . -name "*.log" -exec rm {}(each found file) \\;(ends command))|
||
|**man**|Opens manual for any command attached to it|
||
|**alias**|Creates alies by using following pattern: alias [the alias]='[original command]'|
||
|**exit**|Exits shell|










