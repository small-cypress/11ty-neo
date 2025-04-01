---
title: about
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
.p1 {
  font-family: var(--sans-font);
}

</style>
</head>
<body>
<div class="container">
  <div class="menu"><a href="https://cedar-crown-0f4.notion.site/small-cypress-link-bucket-19d9ca30d69c8051b4f8d06e531764c3?pvs=74">link bucket</a><br><a href="https://www.are.na/small-cypress/index">are.na</a><br><a href="https://indieweb.social/@small_cypress">fediverse</a></div>
  <div class="content"><h3>howdy</h3><p>
  I'm small cypress and this is my anonymized home on the web. </p>
<p>I am learning in public and making mistakes!</div>



</div>

</body>
</html>