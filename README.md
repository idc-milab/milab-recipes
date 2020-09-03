## Cooking with git
This repository holds the communal knowledge of kitchen in the lab.

### How should I start?
1. `$ git clone git@github.com:idc-milab/milab-recipes.git`
2. `$ git checkout develop`
3. `$ git pull origin develop`
4. `$ git checkout -b your_grandpa_recipe`
5. `$ vim dessert/cake.recipe`
6. Write a nice recipe that you would like to share with everybody. Make **sure** to change the names for the branch and for the recipe
7. `$ git add dessert/cake.recipe `
8. `$ git commit -m "Added best recipe ever"`
9. `$ git push -u origin your_grandpa_recipe`
10. Now is time to got to https://github.com/idc-milab/milab-recipes/compare and ask 2 of your collaborators to check your recipe to see is expressive enough and contains clear instrcuts and list of instructions
11. At this time if you need to address comments repeat 5. to 9. and add as many commits you feel necessary
12. When you got 2 recipe reviewes that approve your recipe you should make sure you have rebased on the latest dev
13. `$ git checkout develop`
14. `$ git pull origin develop`
15. `$ git checkout your_grandpa_recipe`
16. `$ git rebase develop`
17. Fix the conflicts if any
    - here you could as well push to origin your rebased branch, but you'll get an error, try to find out the best way to solve the problem
18. `$ git checkout develop`
19. `$ git merge --no-ff your_grandpa_recipe`
20. `$ git push origin develop`
21. Thank you for collaborating with your recipe
