# Clone Intro

Uzak depolar aslında o kadar karmaşık değildir. Günümüzün bulut dünyasında git remotes hakkında bir çok büyü olduğunu düşünmek kolaydır, fakat onlar aslında repositylerinizin uzak bilsayardaki kopyalarıdır. Siz tipik bir şekilde internet aracılığıyla commitlerinizi ileri ve geri transfer etmenize izin veren  diğer bilgisayarla konuşabilirsiniz.

Söyleniyorki, remote repolar bir sürü harika özelliği vardır:

- İlk ve hepsinden önemli, remoteler harika bir backup olarak hizmet eder! Local git repolar (bildiğiniz gibi) dosyaları önceki duruma restore edebilir, fakat tüm bu bilgiyi local bir şekilde saklar.Git repositorinizi diğer bilgisayara kopyalayarak,  tüm verilerinizi kaybedebilir ve yine de left off yaptığınız yerden pick up yapabilirsiniz.

- Daha önemlisi, remoteler kodları sosyal yapar! Şimdi projenizin kopyasını başka bir yerde barındırarak, arkadaşlarınız projenize çok kolay bir şekilde (veya son değişikliklerinize pull in yaparak) katkı yapabilir

Remote repolar hakkındaki etkinliği görselleştiren websitelerini kullanmak oldukça popüler haldedir (GitHub gibi), fakat remote repolar her zaman böyle araçlar için belkemiği görevi görür. Bu yüzden onları anlamak önemlidir!

Bu noktaya kadar, Git Branching öğrenme local repository çalışmalarına (branching, merging, rebaseing, etc) temellerine odaklanmıştır. Ancak şimdi biz remote repository çalışmalarını öğrenmek istiyoruz, bu dersler için ortamı  kuracak komutlara ihtiyacımız var. Git clone bu komut olacak.

Teknik olarak, git clone gerçek dünyada remote repositorylerin lokal kopyalarını oluşturmak için kullanacağımız komuttur (github dan örneğin). Git Branching öğrende bu komutu biraz farklı kullanıyoruz -- git klonu gerçekte local repodan uzakta remote bir repo oluşturur. Elbette teknik olarak gerçek komutun zıt anlamıdır, fakat bu cloning ve remote repository çalışması arasında bir bağlantı inşaa etmemize yardımcı olur, bu yüzden şimdilik onunla çalışalım.


<img src="pics/task1_1.png" width="220" height="250"/>

```
$> git clone 
```

<img src="pics/task1_2.png" width="220" height="250"/>

İşte orada! Şimdi projemizin remote reposu var. Ayrıcımı belirgin hale getirmek için bazı görsel değişiklikler dışında oldukça benzer görünüyor -- sonraki seviyelerde bu repolarla nasıl paylaştığımızı göreceksiniz.
