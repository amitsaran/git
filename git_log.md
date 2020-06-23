# Git log
    
## log all modified files in a directory
git log --name-status frontend/case | grep -E '^[A-Z]\b' | sort | uniq
git log --name-status 'frontend/*.ts' | grep -E '^[A-Z]\b' | sort | uniq

