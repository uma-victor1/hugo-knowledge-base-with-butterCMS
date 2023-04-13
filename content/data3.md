---
title: Install Hugo on macOS.
---


## fields: map[site_faq_body:<header class="flex-none w-100">
<h1 class="lh-title mb3 mv0 pt3 primary-color-dark">macOS</h1>
</header>
<aside class="bt bw1 pt3 mt2 mid-gray b--mid-gray fn w-100">
<div class="f4 fw4 lh-copy">Install Hugo on macOS.</div>
</aside>
<div class="prose" id="prose">
<h2 id="editions">Editions<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#editions"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Hugo is available in two editions: standard and extended. With the extended edition you can:</p>
<ul>
<li>Encode WebP images (you can decode WebP images with both editions)</li>
<li>Transpile Sass to CSS using the embedded LibSass transpiler</li>
</ul>
<p>We recommend that you install the extended edition.</p>
<h2 id="prerequisites">Prerequisites<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#prerequisites"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
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
<h2 id="prebuilt-binaries">Prebuilt binaries<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#prebuilt-binaries"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p>Prebuilt binaries are available for a variety of operating systems and architectures. Visit the<span>&nbsp;</span><a href="https://github.com/gohugoio/hugo/releases/latest">latest release</a><span>&nbsp;</span>page, and scroll down to the Assets section.</p>
<ol>
<li>Download the archive for the desired<span>&nbsp;</span><a href="https://gohugo.io/installation/macos/#editions">edition</a>, operating system, and architecture</li>
<li>Extract the archive</li>
<li>Move the executable to the desired directory</li>
<li>Add this directory to the PATH environment variable</li>
<li>Verify that you have<span>&nbsp;</span><em>execute</em><span>&nbsp;</span>permission on the file</li>
</ol>
<p>Please consult your operating system documentation if you need help setting file permissions or modifying your PATH environment variable.</p>
<p>If you do not see a prebuilt binary for the desired edition, operating system, and architecture, install Hugo using one of the methods described below.</p>
<h2 id="package-managers">Package managers<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#package-managers"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<h3 id="homebrew">Homebrew<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#homebrew"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p><a href="https://brew.sh/">Homebrew</a><span>&nbsp;</span>is a free and open source package manager for macOS and Linux. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">brew install hugo
</span></span></code></pre>
</div>
<h3 id="macports">MacPorts<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#macports"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h3>
<p><a href="https://www.macports.org/">MacPorts</a><span>&nbsp;</span>is a free and open source package manager for macOS. This will install the extended edition of Hugo:</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">sudo port install hugo
</span></span></code></pre>
</div>
<h2 id="docker">Docker<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#docker"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
<p><a href="https://github.com/klakegg">Erlend Klakegg Bergheim</a><span>&nbsp;</span>graciously maintains<span>&nbsp;</span><a href="https://hub.docker.com/r/klakegg/hugo">Docker images</a><span>&nbsp;</span>based on images for Alpine Linux, Busybox, Debian, and Ubuntu.</p>
<div class="highlight">
<pre class="chroma" tabindex="0"><code class="language-sh" data-lang="sh"><span class="line"><span class="cl">docker pull klakegg/hugo
</span></span></code></pre>
</div>
<h2 id="build-from-source">Build from source<span>&nbsp;</span><a class="header-link" href="https://gohugo.io/installation/macos/#build-from-source"><svg class="fill-current o-60 hover-accent-color-light" height="22" viewBox="0 0 24 24" width="22" xmlns="http://www.w3.org/2000/svg"><path d="M0 0h24v24H0z" fill="none"></path><path d="M3.9 12c0-1.71 1.39-3.1 3.1-3.1h4V7H7c-2.76.0-5 2.24-5 5s2.24 5 5 5h4v-1.9H7c-1.71.0-3.1-1.39-3.1-3.1zM8 13h8v-2H8v2zm9-6h-4v1.9h4c1.71.0 3.1 1.39 3.1 3.1s-1.39 3.1-3.1 3.1h-4V17h4c2.76.0 5-2.24 5-5s-2.24-5-5-5z"></path></svg></a></h2>
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
</div> site_faq_description:This question is asked in regards to Mac users that want to get up and running with Hugo site_faq_tiltle:How do I Install Hugo on my Macbook]

name: How to install Hugo on my Macbook

page_type: hugo_knowledge_base

published: 2023-04-11T22:32:15.256870Z

slug: how-to-install-hugo-on-my-macbook

updated: 2023-04-12T17:14:39.277349Z

