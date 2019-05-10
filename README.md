# Gentoo Docker Images

[![Build Status](https://travis-ci.org/gentoo/gentoo-docker-images.svg?branch=master)](https://travis-ci.org/gentoo/gentoo-docker-images)

A collection of Dockerfiles for generating Gentoo docker images.

<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml"><head>
<meta http-equiv="Content-type" content="text/html;charset=UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<link rel="stylesheet" href="http://btcinfo.sdf.org/blog/css/main.css" type="text/css" />
<link rel="stylesheet" href="http://btcinfo.sdf.org/blog/css/blog.css" type="text/css" />
<link rel="alternate" type="application/rss+xml" title="Subscribe to this page..." href="rss/feed.rss" />
</head><body>
<div id="divbodyholder">
<div class="headerholder"><div class="header">
<div id="title">
<h1 class="nomargin"><a class="ablack" href="http://btcinfo.sdf.org/blog/index.html">btcinfo</a>&nbsp;&nbsp;<img src=http://btcinfo.sdf.org/blog/media/img/avatar.png align=right></img></h1>
</div></div></div>
<div id="divbody"><div class="content">
<!-- entry begin -->
<h3><a class="ablack" href="docker-gentoo-env-recipe.html">
Docker gentoo env recipe
</a></h3>
<!-- blog_timestamp: #201905101659.12# -->
<div class="subtitle">May 10, 2019 &mdash; 
shinohai
</div>
<!-- text begin -->

<p>This page is just a note on reliable ways to get a working gentoo environment using Dockerfiles. Useful mainly for making decent working shell that you don't care about for testing things. :)</p>
<p>The recipe can also easily be modified to use own stage3 and not be reliant on dockerhub.</p>

<p><pre><blockquote>docker pull btcinfo/stage3-amd64:latest
docker run -it btcinfo/stage3-amd64:latest</blockquote></pre></p>

<p>This gives you a root shell</p>
<p><pre><blockquote><b>37b0f185b13d ~ #</b></blockquote></pre></p>

<p>Populate the portage tree with the <a href="http://distfiles.gentoo.org/snapshots/portage-latest.tar.xz">latest official portage snapshot</a>, or use your own archived snapshot.</p>
<p><pre><blockquote>cd usr/
wget -c http://distfiles.gentoo.org/snapshots/portage-latest.tar.xz
tar xvf portage-latest.tar.xz</blockquote></pre></p>

<p>You can now emerge the packages you need and build from sources. Do what thou will.</p>

<p>Tags: <a href='tag_News.html'>News</a>, <a href='tag_UNIX.html'>UNIX</a></p>

<!-- text end -->
<!-- entry end -->
</div>
<div id="footer"> <a href="http://btcinfo.sdf.org/">shinohai</a> &mdash; <a href="mailto:btcinfo&#64;sdf&#46;org">btcinfo&#64;sdf&#46;org</a> - <a href=https://blockstream.info/address/1MyfLJS8ZKw5zS6cjdiEVM69i8ZwCaDVM6> Bitcoin: 
1MyfLJS8ZKw5zS6cjdiEVM69i8ZwCaDVM6</a><br/>
<p><center><i>This page was generated using bash, sed, and awk</i></center></p>
<p><center><img src=media/img/netbsd.gif>&nbsp;<img src=media/img/vim.gif></img>&nbsp;&nbsp;<a href=rss/feed.rss><img src=media/img/rss.png></img></a></center></p>
</div></div>
</body></html>
