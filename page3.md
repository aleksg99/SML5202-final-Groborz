
<h1 style="color:mediumvioletred;">Page 3</h1>

<h2>Here is a random name caller</h2>
<button class="button" onclick="makeSentence()">Generate a sentence</button>

<p id="demo"></p>

<script>
function makeSentence() {

var person = { 
    names: [ "Brian", "Betty", "Fiona", "Freddy", "Mini", "Marvin", "Alice", "Bob", "Jane", "Arthur", "Vincent", "Amy", "He", "She" ],
    verbs: [ "speaks", "eats", "runs", "walks", "drinks" ],
    adverbs: ["slowly", "quickly", "nicely", "noisily" ]
  
};

var i;
var text = "";
for (i = 0; i < person.names.length; i++) {

  name = person.names[i];
  verb = person.verbs[Math.floor(Math.random() * person.verbs.length)];
  adv = person.adverbs[Math.floor(Math.random() * person.adverbs.length)];
  
  text += name + " " + verb + " " + adv + "<br>";
 
document.getElementById("demo").innerHTML = text;
}
}

</script>


<p>
  <a href="index.html">Home</a> <br>
  <a href="page2.html">Page 2</a>
</p>
