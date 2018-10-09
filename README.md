Demo feature create/update/remove feature git submodule

```
touch a.txt b.txt c.txt
git add a.txt b.txt c.txt
git commit -m 'Add a.txt b.txt c.txt'
git submodule add git@github.com:dhhiep/demo-git-sub-module-child.git my_submodule
git submodule add git@github.com:dhhiep/demo-git-sub-module-child-2.git my_submodule_2
cat my_submodule/README.md # Testing 1
cat my_submodule_2/README.md # Testing 2_1
# Update README.MD at repo demo-git-sub-module-child become "Testing 1"
# Update README.MD at repo demo-git-sub-module-child become "Testing 2_1"
cat my_submodule/README.md # Testing 1
cat my_submodule_2/README.md # Testing 2_1

```








