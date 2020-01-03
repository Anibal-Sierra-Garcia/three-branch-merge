# three-branch-merge
Practice with remote repos and merge conflicts
There are two files in all the commits: Greeting.java and Readme.md. 

The content of Greeting.java is always of the form

public class Greeting.java {
  public static void main(String[] args) {
    System.out.println(text);
  }
}
where text is Hello something. The precise text also gives name to the commits, and then we have the following diagram:


                   branch inclusive: Hello everybody! ------------------------------------\
                                     /                                                     \
                                    /                                                       \
                                   /                                                         \      
    master --> Initial commit --- Hello World ----- Hello World! ---- Hello guys! ---- Hello everybody! ---- README.md
                                   \                                   /
                                    \                                 /
                                     \                               /
                   branch informal: Hello guys!   ----------------- /
                          
                          
time --------------------------------->                        
                          
                          
1. Initially we have master branch, that we fork into two branches inclusive and informal. 

2. Then we make the commit "Hello World!" (notice the !), and make commits "Hello everybody!" in the inclusive branch
and "Hello guys!" in informal. 

3. As we made commit "Hello World!", the merge of informal is not a fast-forward and it will produce a conflict, that we solve choosing in favor of informal text "Hello guys!", which then appears in master.

4. Now we do the same with inclusive, which also produces conflict and we choose "Hello everybody!" to appear in the end.

5. Finally we write this README.md, which involves three commits.
