Demo feature create/update/remove feature git submodule

```
touch a.txt b.txt c.txt
git add a.txt b.txt c.txt
git commit -m 'Add a.txt b.txt c.txt'
git submodule add git@github.com:dhhiep/demo-git-sub-module-child.git my_submodule
git submodule add git@github.com:dhhiep/demo-git-sub-module-child-2.git my_submodule_2
cat my_submodule/README.md # Testing 1_1
cat my_submodule_2/README.md # Testing 2_1

# Update README.MD at repo demo-git-sub-module-child become "Testing 1_2"
# Update README.MD at repo demo-git-sub-module-child become "Testing 2_2"
cat my_submodule/README.md # Still `Testing 1_1`
cat my_submodule_2/README.md # Still `Testing 2_1`
git submodule update --remote
cat my_submodule/README.md # New content `Testing 1_2`
cat my_submodule_2/README.md # New content `Testing 2_2`

# README.md in demo-git-sub-module-child branch 'xxx' have content xxx
git config -f .gitmodules submodule.my_submodule.branch xxx
git submodule update --remote
cat my_submodule/README.md # New content `xxx`
cat my_submodule_2/README.md # `Testing 2_2`
```








