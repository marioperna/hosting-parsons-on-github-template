---
layout: default
title: JavaScript - Esercizio introduttivo n. 3
description: Crea un programma che dichiari una costante e la stampi in console. 
---


<div id="js_intro-3-sortableTrash" class="sortable-code"></div> 
<div id="js_intro-3-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="js_intro-3-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="js_intro-3-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "const myBirthday = &#039;18.04.1982&#039;;\n" +
    "console.log(&quot;My Birthday is:&quot;, myBirthday);\n" +
    "myBirthday = &#039;01.01.2001&#039;; #distractor\n" +
    "console.log(&quot;My Birthday is:&quot;-&gt;myBirthday); #distractor\n" +
    "console.log(&quot;My Birthday is:&quot;.myBirthday); #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "js_intro-3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "js_intro-3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#js_intro-3-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#js_intro-3-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>