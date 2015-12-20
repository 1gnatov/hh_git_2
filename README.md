```
git clone https://github.com/hhru/frontik fr_only_testing
cd fr_only_testing/
git filter-branch --subdirectory-filter  frontik/testing/ -- --all
```
создал https://github.com/1gnatov/hh_git2_fr_only_testing
```
git remote add ignatov git@github.com:1gnatov/hh_git2_fr_only_testing.git
git push -u ignatov master 
cd ..

git clone https://github.com/hhru/frontik fr_without_testing
git filter-branch --tree-filter 'rm -rf frontik/testing'
```
создал https://github.com/1gnatov/hh_git2_fr_without_testing
```
git remote add ignatov git@github.com:1gnatov/hh_git2_fr_without_testing.git
git push -u ignatov master
```
