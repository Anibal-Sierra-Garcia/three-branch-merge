# three-branch-merge
Practice with remote repos and merge conflicts


                         inclusive: Hello everybody! ------------------------------------\
                                     /                                                    \
                                    /                                                      \
                                   /                                                        \      
    master --> Initial commit --- Hello World ----- Hello World! ---- Hello guys! ---- Hello everybody! ---- README.md
                                   \                                   /
                                    \                                 /
                                     \                               /
                          informal: Hello guys!   ----------------- /
                          
                          
time --------------------------------->                        
                          
1. Initially we have master branch, that we fork into two branches inclusive and informal. 

2. Then we make the commit "Hello World!" (notice the !), and make commits "Hello everybody!" in the inclusive branch
and "Hello guys!" in informal. 

3. As we made commit "Hello World!", the merge of informal is not a fast-forward and it will produce a conflict, that we solve choosing in favor of informal text "Hello guys!", which then appears in master.

4. Now we do the same with inclusive, which also produces conflict and we choose "Hello everybody!" to appear in the end.

5. Finally we write this README.md.
