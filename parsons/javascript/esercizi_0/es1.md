---
layout: default
title: JavaScript - Esercizio introduttivo n. 1
description: Crea una pagina HTML che mostra un messaggio “Hello, world!” mediante un alert contenuto in uno script interno.
---

<div id="js_intro-1-sortableTrash" class="sortable-code"></div> 
<div id="js_intro-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_intro-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_intro-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "&lt;!DOCTYPE HTML&gt;\n" +
    "&lt;html&gt;\n" +
    "&lt;body&gt;\n" +
    "  &lt;p&gt;Before the script...&lt;/p&gt;\n" +
    "  &lt;script&gt;\n" +
    "    alert(&#039;Hello, world!&#039;);\n" +
    "  &lt;/script&gt;\n" +
    "  &lt;p&gt;...After the script.&lt;/p&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_intro-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_intro-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_intro-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>