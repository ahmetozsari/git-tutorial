# git-tutorial
Git kodları kullanım
Git’i Yükleyin
GitHub, en yaygın depo eylemleri için grafiksel bir kullanıcı arabirimi ve Git’in gelişmiş senaryolar için otomatik olarak güncellenen bir komut satırı sürümü içeren masaüstü istemcileri sağlar.

GitHub Masaüstü
https://desktop.github.com/

Linux ve POSIX sistemleri için Git dağıtımlarını resmi Git SCM web sitesinde bulabilirsiniz.

Tüm platformlar için Git
https://git-scm.com

Takım yapılandırna
Tüm yerel depolar için kullanıcı bilgilerini yapılandırın

$ git config --global user.name "[name]"

Tüm yerel depolar için kullanıcı bilgilerini yapılandırın

$ git config --global user.email "[email address]"

Tüm yerel depolar için eposta bilgilerini yapılandırın

Create repositories
Yeni bir depo başlatın veya mevcut bir URL’den bir tane edinin

$ git init [project-name]

Belirtilen adla yeni bir yerel depo oluşturur

$ git clone [url]

Bir projeyi ve tüm sürüm geçmişini indirin

Değişiklik yapmak
Düzenlemeleri inceleyin ve bir işlem gerçekleştirin

$ git status

Taahhüt edilecek tüm yeni veya değiştirilmiş dosyaları listeler

$ git diff

Henüz aşamalandırılmamış dosya farklarını gösterir

$ git add [file]

Sürüm hazırlığı için dosyanın anlık görüntüsünü al.

$ git diff --staged

Hazırlama ve son dosya sürümü arasındaki dosya farklarını gösterir.

$ git reset [file]

Dosyayı dizinden kaldırır ama içeriği korur.

$ git commit -m"[descriptive message]"

Sürüm geçmişinde dosya anlık görüntülerini kalıcı olarak kaydeder

Grup değişiklikleri
Bir dizi taahhüt adı verin ve daha önce tamamlanmış olan çabaları birleştirin

$ git branch

Geçerli depodaki tüm yerel dalları listeler

$ git branch [branch-name]

Yeni bir dal oluştur

$ git checkout [branch-name]

Belirtilen dala geçer ve çalışma dizinini günceller

$ git merge [branch-name]

Belirtilen dalın geçmişini mevcut dalla birleştirir

$ git branch -d [branch-name]

Belirtilen dalı siler

Dosya Yenileme
Sürümlü dosyaları taşıma ve silme

$ git rm [file]

Dosyayı çalışma dizininden siler ve dizini günceller

$ git rm --cached [file]

Dosyayı sürüm kontrolünden kaldırır ancak dosyayı yerel olarak korur

$ git mv [file-original] [file-renamed]

Dosya adını değiştirir ve işleme için hazırlayın

İzlemeyi bastır
Geçici dosyaları ve yolları hariç tut

*.log
build/
temp-*
.Gitignore adlı bir metin dosyası, belirtilen kalıplarla eşleşen dosya ve yolların yanlışlıkla sürümlendirilmesini bastırır.

$ git ls-files --others --ignored --exclude-standard

Bu projedeki yok sayılan tüm dosyaları listeler

Parçaları kaydet
Eksik değişiklikleri sakla ve geri yükle

$ git stash

Değiştirilmiş tüm sürüm dosyalarını geçici olarak kaydedin

$ git stash pop

En son saklanan dosyaları geri yükler

$ git stash list

Önbelleğe alınmış tüm değişiklikleri listeler

$ git stash drop

En son saklanan değişiklikleri atar

Geçmişi incele
Proje dosyalarının gelişimini izlemek ve incelemek

$ git log

Geçerli dalın sürüm geçmişini listeler

$ git log --follow [file]

Yeniden adlandırmalar dahil, dosyanın sürüm geçmişini listeler

$ git diff [first-branch]...[second-branch]

İki dal arasındaki içerik farklarını gösterir

$ git show [commit]

Belirtilen taahhüdün meta verilerini ve içerik değişikliklerini göster

Tekrarlama işlemleri
Hataları temizle ve değiştirme geçmişini yaz

$ git reset [commit]

Değişiklikleri yerel olarak koruyarak, [taahhüt] sonrasında verilen tüm taahhütleri geri alır.

$ git reset --hard [commit]

Tüm geçmişi iptal eder ve belirtilen taahhütte yapılan değişiklikleri geri alır

Değişiklikleri eşle
Bir uzaktan (URL) kaydedin ve depo geçmişini değiştirin

$ git fetch [remote]

Tüm geçmişi uzak depodan indirir

$ git merge [remote]/[branch]

Uzak dalı geçerli yerel dalla birleştirir

$ git push [remote] [branch]

Tüm yerel dal işlemlerini GitHub’a yükler

$ git pull

Yer imi geçmişini indirir ve değişiklikleri içerir
