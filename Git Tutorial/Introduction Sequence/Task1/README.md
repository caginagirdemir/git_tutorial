# Git Commits

Git deposundaki bir commit, dizinizdeki tüm (sadece izlenenler) dosyaların anlık görüntüsünü kaydeder. Devasa bir kopyala ve yapıştır gibi, ama daha da iyisi!

Git, commitleri olabildiğinde hafif tutmak istiyor, bu nedenle her commit tüm dizini körü körüne kopyalamaz. (Mümkün olduğunda) bir committi bir dizi değişiklik veya bir "delta" olarak havuzun bir sürümünden diğerine sıkıştırabilir.

Git also maintains a history of which commits were made when. That's why most commits have ancestor commits above them -- we designate this with arrows in our visualization. Maintaining history is great for everyone working on the project!

It's a lot to take in, but for now you can think of commits as snapshots of the project. Commits are very lightweight and switching between them is wicked fast!

Let's see what this looks like in practice. On the right we have a visualization of a (small) git repository. There are two commits right now -- the first initial commit, C0, and one commit after that C1 that might have some meaningful changes.

Hit the button below to make a new commit.

<img src="task1_1.png" width="250" height="250"/> <img src="task1_1.png" width="250" height="250"/>
