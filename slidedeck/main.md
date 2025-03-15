<style>
  :root {
    --r-background-color: rgb(33, 34, 44);
    --grey: rgb(65, 69, 88);
    --white: rgb(248, 248, 242);
    --blue: rgb(106, 154, 224);
    --cyan: rgb(128, 255, 234);
    --green: rgb(138, 255, 128);
    --r-heading-color: rgb(255, 202, 128);
    --pink: rgb(255, 128, 191);
    --r-main-color: rgb(149, 128, 255);
    --red: rgb(255, 149, 128);
    --yellow: rgb(255, 255, 128);
     #FF80BF;
  }
  .no-wrap {
    white-space: nowrap;
  }
  .larger {
    font-size: larger;
  }
  .small {
    font-size: 90%;
  }
  .small-column {
    float: left;
    width: 25%;
  }
  .third-column {
    float: left;
    width: 33%;
  }
  .column {
    float: left;
    width: 50%;
  }
  .large-column {
    float: left;
    width: 75%;
  }
  h1 {
    font-weight: 100;
  }
  img {
    loading: lazy;
  }
  .gif {
    height: 240px;
    width: 360px;
  }
  li {
    line-height: 2em;
  }
  emph {
    color: var(--red);
  }
  .lc {
    text-transform: lowercase;
  }
  .tips {
    padding: 0; /* Reset padding for the list */
    margin: 0;
  }
  .tips li {
    list-style: none; /* Remove default bullets */
    position: relative; /* Allow positioning of the pseudo-element */
    padding-left: 75px; /* Space for "TIP:" */
  }
  .tips li::before {
    content: "TIP:"; /* Add the "TIP:" text */
    position: absolute;
    left: 0;
    font-style: italic; /* Style as emphasized text */
    font-weight: bold;
    color:var(--green)
  }
  .rounded {
    border-radius: 5%;
  }
  .repo {
    padding: 0; /* Reset padding for the list */
    margin: 0;
  }
  .repo li {
    list-style: none; /* Remove default bullets */
    position: relative; /* Allow positioning of the pseudo-element */
    padding-left: 75px; /* Space for "TIP:" */
  }
  .repo li::before {
    content: "REPO:"; /* Add the "TIP:" text */
    position: absolute;
    margin-left: -30px;
    left: 0;
    font-style: italic; /* Style as emphasized text */
    font-weight: bold;
    color:var(--pink)
  }
  .sd {
    padding: 0; /* Reset padding for the list */
    margin: 0;
  }
  .sd li {
    list-style: none; /* Remove default bullets */
    position: relative; /* Allow positioning of the pseudo-element */
    padding-left: 75px; /* Space for "TIP:" */
  }
  .sd li::before {
    content: "SLIDES:"; /* Add the "TIP:" text */
    position: absolute;
    margin-left: -30px;
    left: 0;
    font-style: italic; /* Style as emphasized text */
    font-weight: bold;
    color:var(--green)
  }
  .r-stack {
    display: grid;
    grid-template-rows: 100%;
  }
</style>


<h1><emph style="color: var(--r-main-color)">ProtoBuf</emph></h1>
<h1><emph style="color: var(--r-main-color)">from scratch</emph></h1>
<h2><em style="color: var(--green)">the API game-changer</em></h1>

---

## <emph>Question:</emph> How many of you work with APIs?

---

## <emph>XML</emph> and <emph>JSON</emph>: down-sides

<div class="column">
  <img class="gif rounded" src="">
</div>
<div class="column">
  <img class="gif rounded" src="">
</div>

---

## Protobuf: a bit of history

---

<div class="column">
<img class="gif rounded" src="">
</div>
<div class="column">
<img class="gif rounded" src="">
</div>
<div>
<img class="gif rounded" src=""/>
</div>

---

# <strong style="color: var(--r-main-color);">ANATOMY</strong>

---

## <empth>Messages</empth> as

<div class="column">
<img src="https://miro.medium.com/v2/resize:fit:487/1*_te2Z2DGMmbwu3plPjlB8g.jpeg" class="gif rounded">
</div>
<div class="column">
<ul>
  <li>Different <emph>layers</emph></li>
  <li>Opaque <emph>jargon</emph></li>
  <li class="no-wrap"><emph>Not everything</emph> is testable</li>
  <li class="no-wrap"><emph>Mutability</emph> creates <emph>side-effects</emph></li>
</ul>
</div>

---

## <emph>Basic types</emph>

<div class="third-column">
<ul class="fragment" data-fragment-index=2 style="color: var(--pink);">
  <li>finer detail</li>
  <li>isolation</li>
  <li>faster</li>
  <li>brittle</li>
</ul>
</div>
<div class="third-column">
<ul class="fragment" data-fragment-index=3 style="color: var(--green);">
  <li>interfaces</li>
  <li>behavioural</li>
  <li>fast/slow</li>
  <li>durable</li>
</ul>
</div>
<div class="third-column">
<ul class="fragment" data-fragment-index=4 style="color: var(--cyan);">
  <li>processes</li>
  <li>enseble</li>
  <li>slow</li>
  <li>error-prone</li>
</ul>
</div>

---

## <emph>Container types</emph>

---


<div class="third-column"><img style="height:180px;" style="height: 240px;" src="slidedeck/assets/test-shapes/reverse-pyramid.svg"></div>
<div class="third-column"><img style="height:180px;" src="slidedeck/assets/test-shapes/pyramid.svg"></div>
<div class="third-column"><img style="height:180px;" src="slidedeck/assets/test-shapes/diamond.svg"></div>
<div>

## Backward/Forward <emph>Compatibility</emph>

---

# <em>CROSS-LANGUAGE</em>

---

## <span style="color: var(--green);">protoc</span> to rule them all
<img src="" style="rounded gif" />

---

```
class TestSuite:

  func testCase {
    # Arrange
    under_test = greet
    expected = "Hello, World!"

    # Act
    actual = under_test()

    # Assert
    assert actual == expected
  }

```

---

# About Me

<div class="column" style="margin-top: -90px;">
<h3 style="margin-top: 130px">Anto"nino" Cangialosi</h3>
Big Data Engineer<br/>
<img style="width: 160px;" src="https://www.agilelab.it/hubfs/logo-agilelab.png">
<br>
<i class="fa fa-github fa-lg"> </i>
<i class="fa fa-gitlab fa-lg"> </i>
<i class="fa fa-slack fa-lg">ninoCan</i><br/>
<i class="fa fa-linkedin">antonino-cangialosi</i>

</div>

<div class="column">
<img style="width: 160px" src="https://images.credly.com/size/340x340/images/8b8ed108-e77d-4396-ac59-2504583b9d54/cka_from_cncfsite__281_29.png">
<img style="width: 140px" src="https://images.credly.com/size/340x340/images/2d613ff8-8879-430b-b2d8-925fa29785e8/image.png">
<img style="width: 130px" src="https://images.credly.com/size/340x340/images/f28f1d88-428a-47f6-95b5-7da1dd6c1000/KCNA_badge.png">
<img style="width: 190px" src="https://www.datacamp.com/statement-of-accomplishment/badge/track/86369ef15d2722bc789beeb26e9a5f28c68558d7.png">
<img style="width: 190px" src="https://www.datacamp.com/statement-of-accomplishment/badge/track/e265d97f60368099e8c955bf28b08b306f00a506.png">
</div>


---

# Thank you!

<ul class="repo small">
  <li class="no-wrap small">https://www.github.io/ninocan/talk-protobuf-from-scratch/</li>
</ul>
<ul class="small sd">
  <li class="small">https://ninocan.github.io/talk-protobuf-from-scratch/</li>
</ul>

<div class="column">
<iframe src="https://ninocan.github.io/talk-protobuf-from-scratch" width="100%" height="360" frameborder="0" scrolling="no"></iframe>
  <embed
    class="rounded"
    src="https://github.com/ninoCan/">
  </embed>
</div>
<div class="column"><img class="rounded" src="slidedeck/assets/qr-code.svg" style="height: 360px; margin-top: -1px;"></img></div>
