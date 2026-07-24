<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>タイトル</title>

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
}

body{

font-family:"Helvetica Neue",sans-serif;
background:#000;
color:#fff;

}

/* ===== メイン画像 ===== */

.hero{

height:100vh;

background-image:url("background.jpg"); /* 後で変更 */

background-size:cover;

background-position:center;

display:flex;

align-items:center;

justify-content:center;

position:relative;

}

.hero::before{

content:"";

position:absolute;

top:0;

left:0;

width:100%;

height:100%;

background:rgba(0,0,0,.45);

}

.hero-content{

position:relative;

z-index:10;

text-align:center;

padding:20px;

}

.hero h1{

font-size:40px;

margin-bottom:20px;

letter-spacing:4px;

}

.hero p{

font-size:18px;

line-height:1.8;

max-width:500px;

margin:auto;

}

/* ===== ギャラリー ===== */

.gallery{

padding:40px 15px;

background:#111;

display:grid;

grid-template-columns:repeat(3,1fr);

gap:10px;

}

.gallery a{

display:block;

aspect-ratio:1;

overflow:hidden;

border-radius:12px;

position:relative;

}

.gallery img{

width:100%;

height:100%;

object-fit:cover;

transition:.3s;

}

.gallery a:hover img{

transform:scale(1.08);

}

.gallery span{

position:absolute;

bottom:8px;

left:8px;

background:rgba(0,0,0,.6);

padding:4px 8px;

font-size:13px;

border-radius:6px;

}

/* ===== フッター ===== */

footer{

padding:30px;

text-align:center;

background:#000;

font-size:12px;

color:#999;

}

</style>

</head>

<body>

<section class="hero">

<div class="hero-content">

<h1>タイトル</h1>

<p>

説明

</p>

</div>

</section>

<section class="gallery">

<a href="page1.html">

<img src="photo1.jpg">

<span>写真①</span>

</a>

<a href="page2.html">

<img src="photo2.jpg">

<span>写真②</span>

</a>

<a href="page3.html">

<img src="photo3.jpg">

<span>写真③</span>

</