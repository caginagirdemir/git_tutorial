# Remote Branches

Artık git klonu çalışırken gördüğümüze göre, gerçekte neyin değiştiğine geçelim.

Fark etmiş olabileceğiniz ilk şey, yerel repomuzda o/main adlı yeni bir dalın ortaya çıkmasıdır. Bu tip branch bir remote branch olarak isimlendirilir, remote branchler spesifik özelliklere sahiptir çünkü onlar benzersiz bir amaca hizmet eder. Fark etmiş olabileceğiniz ilk şey, yerel repomuzdaki o/main adlı yeni bir dalın ortaya çıkmasıdır.

Remote branchler uzak repoların durumunu yansıtır (bu uzak repolar hakkında son konuştuğumuzdan beri). Onlar lokal çalışma ve halka açık çalışma arasındaki farkları anlamamıza yardımcı olur -- çalışmamızı paylaşmaya başlamadan önce dikkate almamız gereken kritik bir adım.

Remote branchler, onları kontrol ettiğinizde, müstakil HEAD moduna geçmeniz gibi özel bir özelliğe sahiptir. Git bunu bilerek

Remote branches have the special property that when you check them out, you are put into detached HEAD mode. Git does this on purpose because you can't work on these branches directly; you have to work elsewhere and then share your work with the remote (after which your remote branches will be updated).

To be clear: Remote branches are on your local repository, not on the remote repository.

What is o/?

You may be wondering what the leading o/ is for on these remote branches. Well, remote branches also have a (required) naming convention -- they are displayed in the format of:

remote name / branch name

Hence, if you look at a branch named o/main, the branch name is main and the name of the remote is o.

Most developers actually name their main remote origin, not o. This is so common that git actually sets up your remote to be named origin when you git clone a repository.

Unfortunately the full name of origin does not fit in our UI, so we use o as shorthand :( Just remember when you're using real git, your remote is probably going to be named origin!

That's a lot to take in, so let's see all this in action.


Lets check out a remote branch and see what happens.

<img src="pics/task2_1.png" width="220" height="250"/>

``` 
$>git checkout o/main
$>git commit
```

<img src="pics/task2_2.png" width="220" height="250"/>



As you can see, git put us into detached HEAD mode and then did not update o/main when we added a new commit. This is because o/main will only update when the remote updates.

To finish this level, commit once off of main and once after checking out o/main. This will help drive home how remote branches behave differently, and they only update to reflect the state of the remote.
