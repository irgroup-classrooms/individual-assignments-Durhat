# Analysis of "lotr.scripts.csv"

## Total number of lines and unique words used in dialogs:

### Command:

wc -l cleaned_lotr_scripts.csv
cut -d ',' -f3 cleaned_lotr_scripts.csv | tr -s '[:space:]' '\n' | tr -d '[:punct:]' | sort | uniq -c | wc -l

### Result:

2391
3448

## Distribution of unique words on the three films:

### Command:

cut -d ',' -f4 cleaned_lotr_scripts.csv | sort | uniq -c

### Result:

349 The Fellowship of the Ring
602 The Return of the King
680 The Two Towers

## Top 5 characters in "char" column::

### Command:

cut -d ',' -f2 cleaned_lotr_scripts.csv | sort | uniq -c | sort -nr | head -5

### Result:

226 FRODO
217 SAM
204 GANDALF
187 ARAGORN
163 PIPPIN

## Top 5 characters in the dialogs:

### Command:

awk -F ',' '{print $2, NF-3}' cleaned_lotr_scripts.csv | sort | uniq -c | sort -nr | head -5

### Result:

169 FRODO 1
146 SAM 1
128 ARAGORN 1
122 PIPPIN 1
122 GANDALF 1
