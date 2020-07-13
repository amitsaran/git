# Git log
    
## log all modified files in a directory
git log --name-status frontend/case | grep -E '^[A-Z]\b' | sort | uniq
git log --name-status 'frontend/*.ts' | grep -E '^[A-Z]\b' | sort | uniq

### git log for multiple authors
git log --author="amitsaran|AMITSARAN|andrew"

if pipe separated names doesn't work for multiple authors, set grep.extendedRegexp to true as below:

git config --global grep.extendedRegexp true

