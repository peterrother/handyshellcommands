# Text in Files

Below is a list of commands for working with text in files (find/replace/etc).

## Recursive Line Count

This example is for a php codebase, but could be applied to any set of files.

```
find . \( -name "*.php" -o -name "*.tpl" -o -name "*.css" \) -type f|xargs cat|wc -l
```

## Recursive Text Replace

```
find . -type f -name '*' -print |
  while read filename
  do
    (
    sed 's/[OLD_TEXT]/[NEW_TEXT]/i;' $filename >$filename.xxxxx
    mv $filename.xxxxx $filename # replace output files with original
    )
done
```
