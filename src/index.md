---
title: small cypress
layout: layout\base.njk
---

<html>
<head>
<style>
.container {
  display: grid;
  grid-template-areas:
    "menu content";
  grid-template-columns: 1fr 3fr;
  gap: 5px;
  background-color: #a6e6db;
  padding: 3px;
}
.container > div {
  background-color: #a6e6db;
  padding: 10px;
}
.container > div.menu {
  grid-area: menu;
  background-color:#ebf9f7;
  border: double
  ;
}
.container > div.content {
  grid-area: content;
}
</style>
</head>
<body>
<div class="container">
  <div class="menu"><a href="#">Link 1</a><br><a href="#">Link 2</a><br><a href="#">Link 3</a></div>
  <div class="content"><h3>howdy</h3><p>
  I'm small cypress and this is my anonymized home on the web. </p></div>
</div>

</body>
</html>