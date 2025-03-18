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
  .red {
    color: var(--red);
  }
  .green {
    color: var(--green);
  }
  .blue {
    color: var(--blue);
  }
  .cyan {
    color: var(--cyan);
  }
  .white {
    color: var(--white);
  }
  .yellow {
    color: var(--yellow);
  }
  .pink {
    color: var(--pink);
  }
  .code-block{
    overflow-y: hidden;
    padding: 2px;
    border: 1px solid var(--pink);
    border-radius: 5px;
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
  <img class="gif rounded fragment" style="clip-path: inset(0% 0% 10% 0% round 5%)" src="https://media2.giphy.com/media/v1.Y2lkPTc5MGI3NjExeDU5d2g1bzczdHV6eHJqNnk5azhqNno5bXV1cGNpYjN6czNvbjJ6MSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/l0IylOPCNkiqOgMyA/giphy.gif">
</div>
<div class="column">
  <img class="gif rounded fragment" style="clip-path: inset(0% 0% 10% 0% round 5%)" src="https://media1.tenor.com/m/b4LEpOGvktEAAAAd/the-square-hole-square-hole.gif">
</div>

---

<img src="https://cdn-contents.anymindgroup.com/corporate/wp-uploads/2021/10/06092952/logo.png" class="rounded" style="transform: scale(0.5); margin-top: -200px">
<h2 style="position: absolute; top: 25%; left: 23%;">A bit of history</h2>

<div class="column" style="text-align: left">
<ul>
  <li>Created in 2001</li>
  <li>Open-sourced in 2004</li>
</ul>
</div>
<div class="column" style="text-align: left">
<ul>
  <li>Lightweight serde</li>
  <li>Back-bone @ Google</li>
</ul>
</div>


---

## WHY?

<div class="column">
  <img class="gif rounded fragment" src="https://media.giphy.com/media/znFOMXuHVkV36qzdbJ/giphy.gif">
</div>
<div class="column">
  <img class="gif rounded fragment" src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExcDVkNjYxcjVjZ2xhZ25ka3l4dm1hNHRqNTlrNTdmdGxzazR1ZXUyciZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/fBEMsUeGHdpsClFsxM/giphy.gif">
</div>
<div>
  <img class="gif rounded fragment" src="https://media.giphy.com/media/dvgTvNCgJxiJm8udDK/giphy.gif?cid=790b7611tiz6tafl0ww2hd66foa1sqr0duwzeyprfdg310mk&ep=v1_gifs_search&rid=giphy.gif&ct=g"/>
</div>

---

# <strong style="color: var(--green);">ANATOMY</strong>

---

<h2>
  <emph style="color: var(--blue)">IDL</emph>: <span style="font-size: 75%">interface description language</span>
</h2>

<div class="column">

<pre class="code-block" style="height: 450px">
  <code data-trim class="language-protobuf"
  >// your first .proto
package hello_proto;

syntax="proto3";

message PisaDevSubscriber {
  uint32 id = 1;
  string name = 2;
  TelegramProfile contact = 3;
}

message TelegramProfile {
  uint64 phone = 1;
  string user_name = 2;
}
  </code>
</pre>

</div>
<div class="column">
  <ul>
    <li><span class="pink">Namespace</span> and<span class="green"> version</span></li>
    <li class="no-wrap">Message as <span class="white">structed enum</span></li>
    <li class="no-wrap"><u>unique</u> field numbers</li>
    <li class="no-wrap"><span class="yellow">2^29</span> max fields</li>
    <li><span class="yellow">19000 - 19999</span> reserved</li>
    <li class="no-wrap">field type (
      <span class="cyan">optional</span> by design)</li>
  </ul>
</div>

---

## <emph>Scalar Types</emph>

<div class="third-column">
<ul class="fragment" data-fragment-index=2 style="color: var(--pink);">
  <li>string</li>
  <li>boolean</li>
  <li>bytes</li>
  <li>float</li>
  <li>double</li>
</ul>
</div>
<div class="third-column">
<ul class="fragment" data-fragment-index=3 style="color: var(--green);">
  <li>int32</li>
  <li>int64</li>
  <li>uint32</li>
  <li>uint64</li>
  <li>sint32</li>
  <li>sint64</li>
</ul>
</div>
<div class="third-column">
<ul class="fragment" data-fragment-index=4 style="color: var(--cyan);">
  <li>fixed32</li>
  <li>fixed64</li>
  <li>sfixed32</li>
  <li>sfixed64</li>
</ul>
</div>

---

## <emph>Container types</emph>
<div class="third-column">
  <h3 class="fragment" data-fragment-index="1"> ARRAYS</h3>
</div>
<div class="third-column">
  <h3 class="fragment" data-fragment-index="2">
    <span class="cyan">MAPS</span>
  </h3>
</div>
<div class="third-column">
  <h3 class="fragment" data-fragment-index="3">
    <span class="green">SUM TYPES</span>
  </h3>
</div>

<pre class="code-block" style="height: 450px">
  <code class="language-protobuf" data-noescape>
    message Channel {
      // we can nest messages
      message TelegramProfile {
        uint64 phone = 1;
        string user_name = 2;
      }
      <span class="fragment highlight" data-fragment-index="1"
      >repeated TelegramProfile subscribers = 1;</span>
      <span class="fragment highlight" data-fragment-index="2"
      >map&lt;string, boolean&gt; settings = 2;</span>
      <span class="fragment highlight" data-fragment-index="3"
      >oneof profile_picture {
        string image_url = 3; // URL of the profile picture
        bytes image_data = 4; // Raw image data
      }</span>
    }
  </code>
</pre>


---

<h2>
  <emph>ENUMERATIONS</emph>
</h2>

<pre class="code-block" style="height: 480px">
  <code class="language-protobuf" data-noescape>
    /* Message defined in other
    * .proto files can be imported
    */
    import "channel.proto"

    message ChannelInfo {
      Channel channel = 1;
      <span class="fragment" data-fragment-index="2"
      >enum ChannelType {
        CHANNEL_TYPE_UNSPECIFIED = 0; // Default value
        PUBLIC = 1; // Public channel
        PRIVATE = 2; // Private channel
        GROUP = 3; // Group channel
      }</span>
      <span class="fragment" data-fragment-index="3"
      >ChannelType channel_type = 1;</span>
    }
  </code>
</pre>

---


<div class="column">
  <h2><span class="pink">Backward</span> /
  <span class="cyan">forward  <emph>Compatibility</emph></h2></span>
<!-- <span class="yellow">Question:</span>
<p class="no-wrap">What if we want to change?</p> -->
<pre class="code-block" style="margin-top: 40px">
  <code class="language-protobuf" data-noescape>message TelegramProfile {
  uint64 phone = 1;
  string user_name = 2;
}</code>
</pre>
</div>
<div class="column fragment">
  <pre class="code-block" style="height: 420px; width: 550px;">
    <code class="language-protobuf" data-noescape>message TelegramProfile {
  // we reserve previous id
  reserved 1;
  // or even name
  reserved "phone";<br>
  // user_name is unchanged
  string user_name = 2;<br>
  oneof telephone {
    // forward compatibility
    optional uint32 numeric = 3;
    optional string alphanumeric = 4;
  }
}</code>
  </pre>
</div>

---

<h2><span class="blue">services</span></h2>

  <pre class="code-block" style="height: 400px; width: 900px;">
    <code class="language-protobuf" data-noescape>message AddMemberRequest {
  string channel_id = 1;
  TelegramProfile = 2;
}</br>
message AddMemberResponse {
    // Confirmation message
    string message = 1;
}<br>
service ChannelService{
   rpc AddMember(AddMemberRequest) returns (AddMemberResponse);
}</code>
</pre>

---

# <em class="blue">CROSS-LANGUAGE</em>
<img class="rounded" src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExOG12dDJkNzh5cWo2d3U1cGNldjVteTR3YXoxZW1sZGFuM3NuZXMyOSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/1I2NwmjvSzNS0/giphy.gif" alt=""></img>
## <span class="pink">protoc</span> to rule them all

---

<pre class="code-block" style="height: 500px; width: 900px;">
  <code class="language-bash" data-noescape># Client generation
$ protoc \
    --proto_path="channel.proto" \
    --python_out="./py-client"

$ protoc \
    --proto_path="channel.proto" \
    --java_out="./java-client"

# On-the-fly encoding:
$ echo '''
user_name: "nino"
telephone: "+39 042 1234567"
''' | protoc --encode=TelegramContanct telegram.proto > msg.bin<br>
# On-the-fly decoding:
$ cat msg.bin | protoc --decode=TelegramContanct telegram.proto</code>
</pre>

---

## <span class="red">CAVEATS</span>
<ul>
  <li>Can be loaded into memory</li>
  <li>Serialization might differ</li>
  <li>No compression</li>
  <li>❌ non-OOP languages</li>
  <li>❌ multidimensional arrays of floats</li>
</ul>

---

# About Me

<div class="column" style="margin-top: -90px;">
<h3 style="margin-top: 90px">
  <span class="blue">Anto"nino" Cangialosi</span>
</h3>
<i class="fa fa-github fa-lg"></i>
<i class="fa fa-gitlab fa-lg"></i>
<i class="fa fa-slack fa-lg">ninoCan</i><br/>
<i class="fa fa-linkedin">antonino-cangialosi</i>

</div>

<div class="column">
<span style="margin-top: 80px;">Big Data Engineer</span>
<br/>
<img class="rounded" style="background: var(--white); transform: scale(1.5); margin-top: 50px; padding: 40px" src="https://www.agilelab.it/hubfs/logo-agilelab.png">
</div>

<h2><span class="green">We are hiring!</span></h2>

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
