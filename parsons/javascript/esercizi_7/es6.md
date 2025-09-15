---
layout: default
title: JavaScript - Esercizio gruppo 7 n. 6
---


<div id="js_esgroup7_6-sortableTrash" class="sortable-code"></div> 
<div id="js_esgroup7_6-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_esgroup7_6-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_esgroup7_6-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "let anno = prompt(&quot;Inserisci un anno:&quot;);\n" +
    "if ((anno % 4 === 0 &amp;&amp; anno % 100 !== 0) || (anno % 400 === 0)) {\n" +
    "  console.log(anno + &quot; è bisestile&quot;);\n" +
    "} else {\n" +
    "  console.log(anno + &quot; non è bisestile&quot;);\n" +
    "}\n" +
    "for (let i = 0; i &lt; 1; i++) { } #distractor\n" +
    "let testo = &quot;Controllo anno...&quot;; #distractor\n" +
    "console.log(testo); #distractor\n" +
    "let inutile = anno * 2; #distractor\n" +
    "if (inutile &gt; 0) { #distractor\n" +
    "  console.log(&quot;Sto pensando...&quot;); #distractor\n" +
    "} #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_esgroup7_6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_esgroup7_6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_esgroup7_6-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_esgroup7_6-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>