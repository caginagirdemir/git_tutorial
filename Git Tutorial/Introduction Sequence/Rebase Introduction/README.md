# Rebase Introduction

Branchlar arasındaki işi birleştirmenin ikinci yolu, yeniden temellendirmedir. Yeniden temellendirme, esasen bir dizi commit alır, onları "kopyalar" ve onları başka bir yere indirir.

Bu kulağa kafa karıştırıcı gelse de, yeniden düzenlemenin avantajı, güzel bir doğrusal commit dizisi yapmak için kullanılabilmesidir.

While this sounds confusing, the advantage of rebasing is that it can be used to make a nice linear sequence of commits. The commit log / history of the repository will be a lot cleaner if only rebasing is allowed.

Let's see it in action...

Here we have two branches yet again; note that the bugFix branch is currently selected (note the asterisk)

We would like to move our work from bugFix directly onto the work from main. That way it would look like these two features were developed sequentially, when in reality they were developed in parallel.

Let's do that with the git rebase command.

<img src="pics/task4_1.png" width="230" height="250"/>

```$> git rebase main```

<img src="pics/task4_2.png" width="230" height="250"/>

Awesome! Now the work from our bugFix branch is right on top of main and we have a nice linear sequence of commits.

Note that the commit C3 still exists somewhere (it has a faded appearance in the tree), and C3' is the "copy" that we rebased onto main.

The only problem is that main hasn't been updated either, let's do that now...

Now we are checked out on the main branch. Let's go ahead and rebase onto bugFix...

<img src="pics/task4_3.png" width="230" height="250"/>

```$> git rebase bugFix```

<img src="pics/task4_4.png" width="230" height="250"/>


There! Since main was an ancestor of bugFix, git simply moved the main branch reference forward in history.
