<div class="col-md-6">
    
<h2 id="giti-yükleyin">Git’i Yükleyin</h2>
<p>GitHub, en yaygın depo eylemleri için grafiksel bir kullanıcı arabirimi ve Git’in gelişmiş senaryolar için otomatik olarak güncellenen bir komut satırı sürümü içeren masaüstü istemcileri sağlar.</p>

<h3 id="github-masaüstü">GitHub Masaüstü</h3>
<p>https://desktop.github.com/</p>

<p>Linux ve POSIX sistemleri için Git dağıtımlarını resmi Git SCM web sitesinde bulabilirsiniz.</p>

<h3 id="tüm-platformlar-için-git">Tüm platformlar için Git</h3>
<p>https://git-scm.com</p>

<h2 id="takım-yapılandırna">Takım yapılandırna</h2>
<p>Tüm yerel depolar için kullanıcı bilgilerini yapılandırın</p>

<p><code class="language-plaintext highlighter-rouge">$ git config --global user.name "[name]"</code></p>

<p>Tüm yerel depolar için kullanıcı bilgilerini yapılandırın</p>

<p><code class="language-plaintext highlighter-rouge">$ git config --global user.email "[email address]"</code></p>

<p>Tüm yerel depolar için eposta bilgilerini yapılandırın</p>

<h2 id="create-repositories">Create repositories</h2>
<p>Yeni bir depo başlatın veya mevcut bir URL’den bir tane edinin</p>

<p><code class="language-plaintext highlighter-rouge">$ git init [project-name]</code></p>

<p>Belirtilen adla yeni bir yerel depo oluşturur</p>

<p><code class="language-plaintext highlighter-rouge">$ git clone [url]</code></p>

<p>Bir projeyi ve tüm sürüm geçmişini indirin</p>


</div>

<div class="col-md-6">
    
<h2 id="değişiklik-yapmak">Değişiklik yapmak</h2>
<p>Düzenlemeleri inceleyin ve bir işlem gerçekleştirin</p>

<p><code class="language-plaintext highlighter-rouge">$ git status</code></p>

<p>Taahhüt edilecek tüm yeni veya değiştirilmiş dosyaları listeler</p>

<p><code class="language-plaintext highlighter-rouge">$ git diff</code></p>

<p>Henüz aşamalandırılmamış dosya farklarını gösterir</p>

<p><code class="language-plaintext highlighter-rouge">$ git add [file]</code></p>

<p>Sürüm hazırlığı için dosyanın anlık görüntüsünü al.</p>

<p><code class="language-plaintext highlighter-rouge">$ git diff --staged</code></p>

<p>Hazırlama ve son dosya sürümü arasındaki dosya farklarını gösterir.</p>

<p><code class="language-plaintext highlighter-rouge">$ git reset [file]</code></p>

<p>Dosyayı dizinden kaldırır ama içeriği korur.</p>

<p><code class="language-plaintext highlighter-rouge">$ git commit -m"[descriptive message]"</code></p>

<p>Sürüm geçmişinde dosya anlık görüntülerini kalıcı olarak kaydeder</p>

<h2 id="grup-değişiklikleri">Grup değişiklikleri</h2>
<p>Bir dizi taahhüt adı verin ve daha önce tamamlanmış olan çabaları birleştirin</p>

<p><code class="language-plaintext highlighter-rouge">$ git branch</code></p>

<p>Geçerli depodaki tüm yerel dalları listeler</p>

<p><code class="language-plaintext highlighter-rouge">$ git branch [branch-name]</code></p>

<p>Yeni bir dal oluştur</p>

<p><code class="language-plaintext highlighter-rouge">$ git checkout [branch-name]</code></p>

<p>Belirtilen dala geçer ve çalışma dizinini günceller</p>

<p><code class="language-plaintext highlighter-rouge">$ git merge [branch-name]</code></p>

<p>Belirtilen dalın geçmişini mevcut dalla birleştirir</p>

<p><code class="language-plaintext highlighter-rouge">$ git branch -d [branch-name]</code></p>

<p>Belirtilen dalı siler</p>

</div>
<div class="clearfix"></div>

<div class="col-md-6">
    
<h2 id="dosya-yenileme">Dosya Yenileme</h2>
<p>Sürümlü dosyaları taşıma ve silme</p>

<p><code class="language-plaintext highlighter-rouge">$ git rm [file]</code></p>

<p>Dosyayı çalışma dizininden siler ve dizini günceller</p>

<p><code class="language-plaintext highlighter-rouge">$ git rm --cached [file]</code></p>

<p>Dosyayı sürüm kontrolünden kaldırır ancak dosyayı yerel olarak korur</p>

<p><code class="language-plaintext highlighter-rouge">$ git mv [file-original] [file-renamed]</code></p>

<p>Dosya adını değiştirir ve işleme için hazırlayın</p>

<h2 id="i̇zlemeyi-bastır">İzlemeyi bastır</h2>
<p>Geçici dosyaları ve yolları hariç tut</p>

<div class="language-plaintext highlighter-rouge"><div class="highlight"><pre class="highlight"><code>*.log
build/
temp-*
</code></pre></div></div>

<p><code class="language-plaintext highlighter-rouge">.Gitignore</code> adlı bir metin dosyası, belirtilen kalıplarla eşleşen dosya ve yolların yanlışlıkla sürümlendirilmesini bastırır.</p>

<p><code class="language-plaintext highlighter-rouge">$ git ls-files --others --ignored --exclude-standard</code></p>

<p>Bu projedeki yok sayılan tüm dosyaları listeler</p>

<h2 id="parçaları-kaydet">Parçaları kaydet</h2>
<p>Eksik değişiklikleri sakla ve geri yükle</p>

<p><code class="language-plaintext highlighter-rouge">$ git stash</code></p>

<p>Değiştirilmiş tüm sürüm dosyalarını geçici olarak kaydedin</p>

<p><code class="language-plaintext highlighter-rouge">$ git stash pop</code></p>

<p>En son saklanan dosyaları geri yükler</p>

<p><code class="language-plaintext highlighter-rouge">$ git stash list</code></p>

<p>Önbelleğe alınmış tüm değişiklikleri listeler</p>

<p><code class="language-plaintext highlighter-rouge">$ git stash drop</code></p>

<p>En son saklanan değişiklikleri atar</p>

</div>

<div class="col-md-6">
    
<h2 id="geçmişi-incele">Geçmişi incele</h2>
<p>Proje dosyalarının gelişimini izlemek ve incelemek</p>

<p><code class="language-plaintext highlighter-rouge">$ git log</code></p>

<p>Geçerli dalın sürüm geçmişini listeler</p>

<p><code class="language-plaintext highlighter-rouge">$ git log --follow [file]</code></p>

<p>Yeniden adlandırmalar dahil, dosyanın sürüm geçmişini listeler</p>

<p><code class="language-plaintext highlighter-rouge">$ git diff [first-branch]...[second-branch]</code></p>

<p>İki dal arasındaki içerik farklarını gösterir</p>

<p><code class="language-plaintext highlighter-rouge">$ git show [commit]</code></p>

<p>Belirtilen taahhüdün meta verilerini ve içerik değişikliklerini göster</p>

<h2 id="tekrarlama-işlemleri">Tekrarlama işlemleri</h2>
<p>Hataları temizle ve değiştirme geçmişini yaz</p>

<p><code class="language-plaintext highlighter-rouge">$ git reset [commit]</code></p>

<p>Değişiklikleri yerel olarak koruyarak, <code class="language-plaintext highlighter-rouge">[taahhüt]</code> sonrasında verilen tüm taahhütleri geri alır.</p>

<p><code class="language-plaintext highlighter-rouge">$ git reset --hard [commit]</code></p>

<p>Tüm geçmişi iptal eder ve belirtilen taahhütte yapılan değişiklikleri geri alır</p>

<h2 id="değişiklikleri-eşle">Değişiklikleri eşle</h2>
<p>Bir uzaktan (URL) kaydedin ve depo geçmişini değiştirin</p>

<p><code class="language-plaintext highlighter-rouge">$ git fetch [remote]</code></p>

<p>Tüm geçmişi uzak depodan indirir</p>

<p><code class="language-plaintext highlighter-rouge">$ git merge [remote]/[branch]</code></p>

<p>Uzak dalı geçerli yerel dalla birleştirir</p>

<p><code class="language-plaintext highlighter-rouge">$ git push [remote] [branch]</code></p>

<p>Tüm yerel dal işlemlerini GitHub’a yükler</p>

<p><code class="language-plaintext highlighter-rouge">$ git pull</code></p>

<p>Yer imi geçmişini indirir ve değişiklikleri içerir</p>

</div>
