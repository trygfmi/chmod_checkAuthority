<!-- wp:heading -->
<h2 class="wp-block-heading">前書き</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>このリポジトリは、chmodコマンドを実行してファイルの権限を変更した場合の挙動を検証します</p>
<!-- /wp:paragraph -->

<!-- wp:heading -->
<h2 class="wp-block-heading">インストールする必要のあるコマンド</h2>
<!-- /wp:heading -->

<!-- wp:list {"ordered":true} -->
<ol class="wp-block-list"><!-- wp:list-item -->
<li>git</li>
<!-- /wp:list-item --></ol>
<!-- /wp:list -->

<!-- wp:heading -->
<h2 class="wp-block-heading">クイックスタート</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>上記のコマンドをインストール済みの方は、以下のコマンドを実行してリポジトリからダウンロード後、ディレクトリを移動し、chmodを実行して権限が変更されたshell scriptを実行してみてください</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">ubuntu</h3>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>出力結果</summary><!-- wp:code {"style":{"color":{"background":"#ffeeee"}}} -->
<pre class="wp-block-code has-background" style="background-color:#ffeeee"><code>hello chmod command world
bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre>
<!-- /wp:code --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">macos</h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">MacPorts</h4>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>source ~/bashrc_folder/macports_alias
git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>出力結果</summary><!-- wp:code {"style":{"color":{"background":"#ffeeee"}}} -->
<pre class="wp-block-code has-background" style="background-color:#ffeeee"><code>hello chmod command world
bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre>
<!-- /wp:code --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">windows</h3>
<!-- /wp:heading -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">WSL2</h4>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>出力結果</summary><!-- wp:code {"style":{"color":{"background":"#ffeeee"}}} -->
<pre class="wp-block-code has-background" style="background-color:#ffeeee"><code>hello chmod command world
bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre>
<!-- /wp:code --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">MSYS2 MINGW64</h4>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>不可</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>出力結果</summary><!-- wp:code {"style":{"color":{"background":"#ffeeee"}}} -->
<pre class="wp-block-code has-background" style="background-color:#ffeeee"><code>不可</code></pre>
<!-- /wp:code --></details>
<!-- /wp:details -->

<!-- wp:heading -->
<h2 class="wp-block-heading">実行手順</h2>
<!-- /wp:heading -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">ubuntu</h3>
<!-- /wp:heading -->

<!-- wp:details -->
<details class="wp-block-details"><summary>クリックして詳細を開く</summary><!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">事前確認</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のコマンドを端末に打ち込んでcommand not foundが出なければokです</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git --version</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">preinstall</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>端末でcommand not foundが出たコマンドを以下のコマンドでインストールしてください</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>sudo apt install git</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">コマンド</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のshell scriptを実行することで詳細のような文字列が出力されるはずです</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>詳細</summary><!-- wp:paragraph -->
<p><pre class="wp-block-code has-24292-eff-color has-text-color has-background has-1-125-rem-font-size" style="background-color:#ffeeee"><code>hello chmod command world<br>bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre></p>
<!-- /wp:paragraph --></details>
<!-- /wp:details --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">macos</h3>
<!-- /wp:heading -->

<!-- wp:details -->
<details class="wp-block-details"><summary>クリックして詳細を開く</summary><!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">事前確認</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のコマンドをターミナルに打ち込んでcommand not foundが出なければokです</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>source ~/bashrc_folder/macports_alias
git --version</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>※macosはMacPortsパッケージマネージャを使用してコマンドを管理します。もしインストールしていない方は以下のリンクからMacPortsのインストール手順をご覧ください</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>またコマンドに別名を設定して既存の環境と競合しないでコマンドを呼び出せるようにします。</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p>初めてこのブログを利用する方は、以下の2つの記事を参考に環境構築してください</p>
<!-- /wp:paragraph -->

<!-- wp:embed {"url":"https://ss523971.stars.ne.jp/todo/how-to-install-macports/","type":"wp-embed","providerNameSlug":"todo"} -->
<figure class="wp-block-embed is-type-wp-embed is-provider-todo wp-block-embed-todo"><div class="wp-block-embed__wrapper">
https://ss523971.stars.ne.jp/todo/how-to-install-macports/
</div></figure>
<!-- /wp:embed -->

<!-- wp:embed {"url":"https://ss523971.stars.ne.jp/todo/how-to-setup-macports-alias","type":"wp-embed","providerNameSlug":"todo"} -->
<figure class="wp-block-embed is-type-wp-embed is-provider-todo wp-block-embed-todo"><div class="wp-block-embed__wrapper">
https://ss523971.stars.ne.jp/todo/how-to-setup-macports-alias
</div></figure>
<!-- /wp:embed -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">preinstall</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>ターミナルでcommand not foundが出たコマンドを以下のコマンドでインストールしてエイリアスを設定してください</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>sudo port install git
echo 'alias git="/opt/local/bin/git"' &gt;&gt; ~/bashrc_folder/macports_alias</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">コマンド</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のshell scriptを実行することで詳細のような文字列が出力されるはずです</p>
<!-- /wp:paragraph -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>source ~/bashrc_folder/macports_alias
git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>詳細</summary><!-- wp:paragraph -->
<p><pre class="wp-block-code has-24292-eff-color has-text-color has-background has-1-125-rem-font-size" style="background-color:#ffeeee"><code>hello chmod command world<br>bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre></p>
<!-- /wp:paragraph --></details>
<!-- /wp:details --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":3} -->
<h3 class="wp-block-heading">windows</h3>
<!-- /wp:heading -->

<!-- wp:details -->
<details class="wp-block-details"><summary>クリックして詳細を開く</summary><!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading">事前確認</h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のコマンドをプロンプトに打ち込んでcommand not foundが出なければokです</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">WSL2</h5>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git --version</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">MSYS2 MINGW64</h5>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>不可</code></pre>
<!-- /wp:code -->

<!-- wp:paragraph -->
<p>※windowsはWSL2とMSYS2 MINGW64で確認しています。可能な限りWSL2をインストールしていただいて、もし設定できなかった場合はMSYS2をインストールすることで実行できますが、所々WSL2でしか実行できないコマンドが出てくるかもしれません。WSL2とMSYS2のインストール方法は下記の記事を参考にしてください</p>
<!-- /wp:paragraph -->

<!-- wp:embed {"url":"https://ss523971.stars.ne.jp/todo/how-to-install-wsl2","type":"wp-embed","providerNameSlug":"todo"} -->
<figure class="wp-block-embed is-type-wp-embed is-provider-todo wp-block-embed-todo"><div class="wp-block-embed__wrapper">
https://ss523971.stars.ne.jp/todo/how-to-install-wsl2
</div></figure>
<!-- /wp:embed -->

<!-- wp:embed {"url":"https://ss523971.stars.ne.jp/todo/how-to-install-msys2","type":"wp-embed","providerNameSlug":"todo"} -->
<figure class="wp-block-embed is-type-wp-embed is-provider-todo wp-block-embed-todo"><div class="wp-block-embed__wrapper">
https://ss523971.stars.ne.jp/todo/how-to-install-msys2
</div></figure>
<!-- /wp:embed -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading"><strong>preinstall</strong></h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>プロンプトでcommand not foundが出たコマンドを以下のコマンドでインストールしてください</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">WSL2</h5>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>sudo apt install git</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">MSYS2 MINGW64</h5>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>pacman --sync git</code></pre>
<!-- /wp:code -->

<!-- wp:heading {"level":4} -->
<h4 class="wp-block-heading"><strong>コマンド</strong></h4>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>以下のshell scriptを実行することで詳細のような文字列が出力されるはずです</p>
<!-- /wp:paragraph -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">WSL2</h5>
<!-- /wp:heading -->

<!-- wp:code {"className":"has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"} -->
<pre class="wp-block-code has-24292-eff-color has-cyan-bluish-gray-background-color has-text-color has-background has-1-125-rem-font-size"><code>git clone https://github.com/trygfmi/chmod_checkAuthority
cd chmod_checkAuthority
ls -l
cat ./start_chmod_checkAuthority.sh
chmod 755 ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rwxr-xr-x 755
chmod -x ./start_chmod_checkAuthority.sh
./start_chmod_checkAuthority.sh #rw-r-xr-x 655</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>詳細</summary><!-- wp:paragraph -->
<p><pre class="wp-block-code has-24292-eff-color has-text-color has-background has-1-125-rem-font-size" style="background-color:#ffeeee"><code>hello chmod command world<br>bash: ./start_chmod_checkAuthority.sh: Permission denied</code></pre></p>
<!-- /wp:paragraph --></details>
<!-- /wp:details -->

<!-- wp:heading {"level":5} -->
<h5 class="wp-block-heading">MSYS2 MINGW64</h5>
<!-- /wp:heading -->

<!-- wp:code {"backgroundColor":"cyan-bluish-gray"} -->
<pre class="wp-block-code has-cyan-bluish-gray-background-color has-background"><code>不可</code></pre>
<!-- /wp:code -->

<!-- wp:details -->
<details class="wp-block-details"><summary>詳細</summary><!-- wp:paragraph -->
<p><pre class="wp-block-code has-24292-eff-color has-text-color has-background has-1-125-rem-font-size" style="background-color:#ffeeee"><code>不可</code></pre></p>
<!-- /wp:paragraph --></details>
<!-- /wp:details --></details>
<!-- /wp:details -->

<!-- wp:heading -->
<h2 class="wp-block-heading">後書き</h2>
<!-- /wp:heading -->

<!-- wp:paragraph -->
<p>chmod 754やchmod 751など色々試してみてください</p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->

<!-- wp:paragraph -->
<p></p>
<!-- /wp:paragraph -->