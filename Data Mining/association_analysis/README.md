# Association Analysis

#### Dependencies:
<i>
Python 3.6.1
<br>Pandas 0.20.1
<br>Itertools
</i>

#### Execution in command line: 

```bash
python3 Association.py [filename] [support percent] [confidence percent]
```
The program is tested with the included file <i>associationrulestestdata.txt</i>. 
Please feel free to use this program with any other files, or modify it as per your own needs.

#### Example:

```bash
python3 Association.py associationruletestdata.txt 50 70
```

#### Querying:
Type in query as per given format. Type "exit" to quit program.

#### Query format examples:
```
asso_rule.template1("RULE", "ANY", ['G59_Up'])
asso_rule.template1("RULE", "NONE", ['G59_Up'])
asso_rule.template1("RULE", 1, ['G59_Up', 'G10_Down'])
asso_rule.template1("BODY", "ANY", ['G59_Up'])
asso_rule.template1("BODY", "NONE", ['G59_Up'])
asso_rule.template1("BODY", 1, ['G59_Up', 'G10_Down'])
asso_rule.template1("HEAD", "ANY", ['G59_Up'])
asso_rule.template1("HEAD", "NONE", ['G59_Up'])
asso_rule.template1("HEAD", 1, ['G59_Up', 'G10_Down'])
asso_rule.template2("RULE", 3)
asso_rule.template2("BODY", 2)
asso_rule.template2("HEAD", 1)
asso_rule.template3("1or1", "BODY", "ANY", ['G10_Down'], "HEAD", 1, ['G59_Up'])
asso_rule.template3("1and1", "BODY", "ANY", ['G10_Down'], "HEAD", 1, ['G59_Up'])
asso_rule.template3("1or2", "BODY", "ANY", ['G10_Down'], "HEAD", 2)
asso_rule.template3("1and2", "BODY", "ANY", ['G10_Down'], "HEAD", 2)
asso_rule.template3("2or2", "BODY", 1, "HEAD", 2)
asso_rule.template3("2and2", "BODY", 1, "HEAD", 2)
```

#### Notes:
"Up" and "Down" should be entered in sentence case and not in "UPPER" or "lower" case.
