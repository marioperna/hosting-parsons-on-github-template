---
layout: default
title: JavaScript - Introduzione
---


## DOMANDA 1: JAVA è la forma contratta di JavaScript ?
<div id="quiz-intro-1-sortableTrash" class="sortable-code"></div> 
<div id="quiz-intro-1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="quiz-intro-1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="quiz-intro-1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "false\n" +
    "true #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-intro-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-intro-1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-intro-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#quiz-intro-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



## Chi ha creato JavaScript ?
<div id="quiz-intro-2-sortableTrash" class="sortable-code"></div>
<div id="quiz-intro-2-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-intro-2-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-intro-2-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "Brendan Eich\n" +
    "James Gosling #distractor\n" +
    "Dennis Ritchie #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-intro-2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-intro-2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-intro-2-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-intro-2-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

## Select the correct JavaScript method for finding the specified HTML element --> document._______('demo').innerHTML

<div id="quiz-intro-3-sortableTrash" class="sortable-code"></div>
<div id="quiz-intro-3-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-intro-3-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-intro-3-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "getElementById #correct\n" +
    "getElementByClassName #distractor\n" +
    "getElementByName #distractor\n" +
    "getElementByTagName #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-intro-3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-intro-3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-intro-3-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-intro-3-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

