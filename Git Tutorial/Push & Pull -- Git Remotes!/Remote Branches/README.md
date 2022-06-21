# Remote Branches

Artık git klonu çalışırken gördüğümüze göre, gerçekte neyin değiştiğine geçelim.

Fark etmiş olabileceğiniz ilk şey, yerel repomuzda o/main adlı yeni bir dalın ortaya çıkmasıdır. Bu tip branch bir remote branch olarak isimlendirilir, remote branchler spesifik özelliklere sahiptir çünkü onlar benzersiz bir amaca hizmet eder. Fark etmiş olabileceğiniz ilk şey, yerel repomuzdaki o/main adlı yeni bir dalın ortaya çıkmasıdır.

Remote branchler uzak repoların durumunu yansıtır (bu uzak repolar hakkında son konuştuğumuzdan beri). Onlar lokal çalışma ve halka açık çalışma arasındaki farkları anlamamıza yardımcı olur -- çalışmamızı paylaşmaya başlamadan önce dikkate almamız gereken kritik bir adım.

Remote branchler, onları kontrol ettiğinizde, müstakil HEAD moduna geçmeniz gibi özel bir özelliğe sahiptir. Git bunu bilerek yapıyor çünkü bu dallarda doğrudan çaışamazsınız; başka bir yerde çalışmanız ve ardından çalışmanızı remote çalışma ile paylaşmanız gerekir (bundan sonra uzak şubeleriniz güncellenir.)

Açık olmak gerekirse: Remote branchler sizin lokal reponuzdadır, remote repo da değildir.

o/ nedir?

Remote branchlarda önde gelen o/ nin ne için olduğunu merak ediyor olabilirsiniz. Pekala, remote branchlerinde (gerekli) bir adlandırma kuralı vardır -- bunlar şu formatta gösterilir:

remote name / branch name 



Gerçek git kullanımında remote adı origin olacaktır!


<img src="pics/task2_1.png" width="220" height="250"/>

``` 
$>git checkout o/main
$>git commit
```

<img src="pics/task2_2.png" width="220" height="250"/>



