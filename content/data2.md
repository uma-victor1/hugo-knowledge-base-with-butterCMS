---
title: Install Hugo on Linux
---


## fields: map[site_faq_body:<header class="flex-none w-100">
<h1 class="lh-title mb3 mv0 pt3 primary-color-dark">Linux</h1>
</header>
<aside class="bt bw1 pt3 mt2 mid-gray b--mid-gray fn w-100">
<div class="f4 fw4 lh-copy">Install Hugo on Linux.</div>
</aside>
<div class="prose" id="prose">
<h2 id="editions">Editions<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#editions"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Hugo is available in two editions: standard and extended. With the extended edition you can:</p>
<ul>
<li>Encode WebP images (you can decode WebP images with both editions)</li>
<li>Transpile Sass to CSS using the embedded LibSass transpiler</li>
</ul>
<p>We recommend that you install the extended edition.</p>
<h2 id="prerequisites">Prerequisites<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#prerequisites"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Although not required in all cases, Git and Go are often used when working with Hugo.</p>
<p>Git is required to:</p>
<ul>
<li>Use the<span>&nbsp;</span><a href="https://gohugo.io/hugo-modules/">Hugo Modules</a><span>&nbsp;</span>feature</li>
<li>Build Hugo from source</li>
<li>Install a theme as a Git submodule</li>
<li>Access<span>&nbsp;</span><a href="https://gohugo.io/variables/git">commit information</a><span>&nbsp;</span>from a local Git repository</li>
<li>Host your site with services such as<span>&nbsp;</span><a href="https://aws.amazon.com/amplify/">AWS Amplify</a>,<span>&nbsp;</span><a href="https://cloudcannon.com/">CloudCannon</a>,<span>&nbsp;</span><a href="https://pages.cloudflare.com/">Cloudflare Pages</a>,<span>&nbsp;</span><a href="https://pages.github.com/">GitHub Pages</a>,<span>&nbsp;</span><a href="https://docs.gitlab.com/ee/user/project/pages/">GitLab Pages</a>, and<span>&nbsp;</span><a href="https://www.netlify.com/">Netlify</a>.</li>
</ul>
<p>Go is required to:</p>
<ul>
<li>Use the Hugo Modules feature</li>
<li>Build Hugo from source</li>
</ul>
<p>Please refer to the<span>&nbsp;</span><a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">Git</a><span>&nbsp;</span>and<span>&nbsp;</span><a href="https://go.dev/doc/install">Go</a><span>&nbsp;</span>documentation for installation instructions.</p>
<h2 id="prebuilt-binaries">Prebuilt binaries<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#prebuilt-binaries"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Prebuilt binaries are available for a variety of operating systems and architectures. Visit the<span>&nbsp;</span><a href="https://github.com/gohugoio/hugo/releases/latest">latest release</a><span>&nbsp;</span>page, and scroll down to the Assets section.</p>
<ol>
<li>Download the archive for the desired<span>&nbsp;</span><a href="https://gohugo.io/installation/linux/#editions">edition</a>, operating system, and architecture</li>
<li>Extract the archive</li>
<li>Move the executable to the desired directory</li>
<li>Add this directory to the PATH environment variable</li>
<li>Verify that you have<span>&nbsp;</span><em>execute</em><span>&nbsp;</span>permission on the file</li>
</ol>
<p>Please consult your operating system documentation if you need help setting file permissions or modifying your PATH environment variable.</p>
<p>If you do not see a prebuilt binary for the desired edition, operating system, and architecture, install Hugo using one of the methods described below.</p>
<h2 id="package-managers">Package managers<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#package-managers"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<h3 id="snap">Snap<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#snap"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p><a href="https://snapcraft.io/">Snap</a><span>&nbsp;</span>is a free and open source package manager for Linux. Available for<span>&nbsp;</span><a href="https://snapcraft.io/docs/installing-snapd">most distributions</a>, snap packages are simple to install and are automatically updated.</p>
<p>The Hugo snap package is<span>&nbsp;</span><a href="https://snapcraft.io/docs/snap-confinement">strictly confined</a>. Strictly confined snaps run in complete isolation, up to a minimal access level that&rsquo;s deemed always safe. The sites you create and build must be located within your home directory, or on removable media.</p>
<p>This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo snap install hugo
</span></span></code></pre>
</div>
<h3 id="homebrew">Homebrew<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#homebrew"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p><a href="https://brew.sh/">Homebrew</a><span>&nbsp;</span>is a free and open source package manager for macOS and Linux. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">brew install hugo
</span></span></code></pre>
</div>
<h2 id="repository-packages">Repository packages<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#repository-packages"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Most Linux distributions maintain a repository for commonly installed applications. Please note that these repositories may not contain the<span>&nbsp;</span><a href="https://github.com/gohugoio/hugo/releases/latest">latest release</a>.</p>
<h3 id="arch-linux">Arch Linux<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#arch-linux"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p>Derivatives of the<span>&nbsp;</span><a href="https://archlinux.org/">Arch Linux</a><span>&nbsp;</span>distribution of Linux include<span>&nbsp;</span><a href="https://endeavouros.com/">EndeavourOS</a>,<span>&nbsp;</span><a href="https://garudalinux.org/">Garuda Linux</a>,<span>&nbsp;</span><a href="https://manjaro.org/">Manjaro</a>, and others. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo pacman -S hugo
</span></span></code></pre>
</div>
<h3 id="debian">Debian<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#debian"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p>Derivatives of the<span>&nbsp;</span><a href="https://www.debian.org/">Debian</a><span>&nbsp;</span>distribution of Linux include<span>&nbsp;</span><a href="https://elementary.io/">elementary OS</a>,<span>&nbsp;</span><a href="https://neon.kde.org/">KDE neon</a>,<span>&nbsp;</span><a href="https://www.linuxliteos.com/">Linux Lite</a>,<span>&nbsp;</span><a href="https://linuxmint.com/">Linux Mint</a>,<span>&nbsp;</span><a href="https://mxlinux.org/">MX Linux</a>,<span>&nbsp;</span><a href="https://pop.system76.com/">Pop!_OS</a>,<span>&nbsp;</span><a href="https://ubuntu.com/">Ubuntu</a>,<span>&nbsp;</span><a href="https://zorin.com/os/">Zorin OS</a>, and others. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo apt install hugo
</span></span></code></pre>
</div>
<p>You can also download Debian packages from the<span>&nbsp;</span><a href="https://github.com/gohugoio/hugo/releases/latest">latest release</a><span>&nbsp;</span>page.</p>
<h3 id="fedora">Fedora<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#fedora"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p>Derivatives of the<span>&nbsp;</span><a href="https://getfedora.org/">Fedora</a><span>&nbsp;</span>distribution of Linux include<span>&nbsp;</span><a href="https://www.centos.org/">CentOS</a>,<span>&nbsp;</span><a href="https://www.redhat.com/">Red Hat Enterprise Linux</a>, and others. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo dnf install hugo
</span></span></code></pre>
</div>
<h3 id="opensuse">openSUSE<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#opensuse"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p>Derivatives of the<span>&nbsp;</span><a href="https://www.opensuse.org/">openSUSE</a><span>&nbsp;</span>distribution of Linux include<span>&nbsp;</span><a href="https://geckolinux.github.io/">GeckoLinux</a>,<span>&nbsp;</span><a href="https://linuxkamarada.com/">Linux Karmada</a>, and others. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo zypper install hugo
</span></span></code></pre>
</div>
<h3 id="solus">Solus<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#solus"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p>The<span>&nbsp;</span><a href="https://getsol.us/">Solus</a><span>&nbsp;</span>distribution of Linux includes Hugo in its package repository. This will install the<span>&nbsp;</span><em>standard</em><span>&nbsp;</span>edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo eopkg install hugo
</span></span></code></pre>
</div>
<h2 id="docker">Docker<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#docker"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p><a href="https://github.com/klakegg">Erlend Klakegg Bergheim</a><span>&nbsp;</span>graciously maintains<span>&nbsp;</span><a href="https://hub.docker.com/r/klakegg/hugo">Docker images</a><span>&nbsp;</span>based on images for Alpine Linux, Busybox, Debian, and Ubuntu.</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">docker pull klakegg/hugo
</span></span></code></pre>
</div>
<h2 id="build-from-source">Build from source<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/linux/#build-from-source"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>To build Hugo from source you must:</p>
<ol>
<li>Install<span>&nbsp;</span><a href="https://git-scm.com/book/en/v2/Getting-Started-Installing-Git">Git</a></li>
<li>Install<span>&nbsp;</span><a href="https://go.dev/doc/install">Go</a><span>&nbsp;</span>version 1.18 or later</li>
<li>Update your PATH environment variable as described in the<span>&nbsp;</span><a href="https://go.dev/doc/code#Command">Go documentation</a></li>
</ol>
<blockquote>
<p>The install directory is controlled by the GOPATH and GOBIN environment variables. If GOBIN is set, binaries are installed to that directory. If GOPATH is set, binaries are installed to the bin subdirectory of the first directory in the GOPATH list. Otherwise, binaries are installed to the bin subdirectory of the default GOPATH ($HOME/go or %USERPROFILE%\go).</p>
</blockquote>
<p>Then build and test:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">go install -tags extended github.com/gohugoio/hugo@latest
</span></span><span class="line"><span class="cl">hugo version
</span></span></code></pre>
</div>
</div>
<p><quillbot-extension-portal></quillbot-extension-portal></p> site_faq_description:Description on How to install Hugo on Windows site_faq_tiltle:How to install Hugo on Windows]

name: How to install Hugo on Windows

page_type: hugo_knowledge_base

published: 2023-04-12T19:33:36.893950Z

slug: how-to-install-hugo-on-windows

updated: 2023-04-12T19:33:36.893950Z

