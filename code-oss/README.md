# How to use this


## backup

**Extension**
```markdown
# 1.export from current env

code --list-extensions > extension.txt

# 2. improt single extension info 

code --install-extension

# 3. checkout help

code -h
 

```


## recover


```markdown
# 1. recover from file with script

## with fish
while read ext
  codium --install-extension $ext
end < .extension

## with window PowerShell
Get-Content ./extension.txt | ForEach-Object {
  codium --install-extension $_
}

```