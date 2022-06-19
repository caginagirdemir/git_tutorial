# Git Branches

Git'teki branchler inanılmaz derecede hafiftir. Onlar sadece belirli bir committin pointerını taşır - başka bir şey değil. Bir çok Git meraklısının şunu söylemesinin nedeni budur: 

Branch early, and branch often

Çok sayıda branch yapmak depolama/bellek yükü yapmadığından, büyük branchlar yerine onları mantıklı bir şekilde küçük branchlara bölmek daha kolaydır.

Branchları ve commitleri karşılaştırmaya başladığımızda, bu iki özelliğin nasıl birleştiğini göreceğiz.

Burada newImage adında yeni bir dal oluşturacağız.

<img src="pics/task2.png" width="220" height="250"/>

```$> git branch newImage```

<img src="pics/task2_2.png" width="220" height="250"/>

```$> git commit```

<img src="pics/task2_3.png" width="220" height="250"/>

Ama Hayır! main branch taşındı ama newImage branch taşınmadı! Bunun nedeni yeni branch üzerinde olmamamızdı, yıldız işareti main branch üzerindeydi.

```$> git checkout newImage``` (branch değişikliği.)

```$> git commit```

<img src="pics/task2_4.png" width="220" height="250"/>


Bu arada, burada bir kısayol var: eğer yeni bir şube oluşturmak ve aynı zamanda ona checkout olmak istiyorsanız kısaca şöyle yapabilirsiniz:

```$> git checkout -b [yourbranchname]```

