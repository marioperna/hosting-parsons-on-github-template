---
layout: default
title: JavaScript - Esercizio introduttivo n. 4
description: Crea un oggetto JavaScript con una proprietà name ed un metodo sayHi(). Chiama il metodo per mostrare un messaggio di saluto.
---

<div id="js_intro-4-sortableTrash" class="sortable-code"></div> 
<div id="js_intro-4-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_intro-4-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_intro-4-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let john = {\n" +
    "  name: &quot;John&quot;,\n" +
    "  sayHi: function() {\n" +
    "    alert(&quot;Hi buddy!&quot;);\n" +
    "  }\n" +
    "};\n" +
    "john.sayHi(); // Hi buddy!\n" +
    "name= &quot;John&quot;, #distractor\n" +
    "	sayHi= function() { #distractor\n" +
    "} #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_intro-4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_intro-4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_intro-4-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_intro-4-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

[Torna all'indice](../../../index.markdown)