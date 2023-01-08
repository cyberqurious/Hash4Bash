# Conditional Constructs

### 1. if: **consequent-commands** will only run when **test-commands** returns status **0** i.e **True**.
  
```
if test-commands; then
  consequent-commands;
[elif more-test-commands; then
  more-consequents;]
[else alternate-consequents;]
fi
```

```
Syntex:
if [[ $VAR -gt xx ]]; then
  echo "Success!"
fi
```

```
eg. 
1. if (( "${1}" % x == 0 )) # Integer
2. if [ $(expr $1 % x) -eq 0 ]; # Integer
3. if (( "$1" % 3 == 0 )); # Integer

```

2. 

