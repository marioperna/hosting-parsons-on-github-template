---
layout: default
title: JS Where TO
---


## In HTML, JavaScripts must be inserted inside which HTML tags?
<div id="quiz-jswhereto-1-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-1-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-1-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "<script>\n" +
    "<javascript> #distractor\n" +
    "<js> #distractor\n" +
    "<scripting> #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-jswhereto-1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#quiz-jswhereto-1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## What is the correct file extension for JavaScript files?
<div id="quiz-jswhereto-2-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-2-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-2-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-2-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = ".js\n" +
    ".javascript #distractor\n" +
    ".jvs #distractor\n" +
    ".jsc #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-jswhereto-2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#quiz-jswhereto-2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>  


## What is a correct syntax for including a JavaScript in an HTML document?

<div id="quiz-jswhereto-3-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-3-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-3-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-3-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
    var initial = "<script src='xxx.js'> #correct\n" +
    "<script href='xxx.js'> #distractor\n" +
    "<script ref='xxx.js'> #distractor\n" +
    "<script name='xxx.js'> #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-3-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-3-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
    $("#quiz-jswhereto-3-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-jswhereto-3-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>




## What is NOT a correct syntax for writing output in JavaScript?
<div id="quiz-jswhereto-4-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-4-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-4-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-4-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "document.write('Hello World') #distractor\n" +
    "console.log('Hello World') #distractor\n" +
    "window.alert('Hello World') #distractor\n" +
    "print('Hello World') #correct";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-4-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-4-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-jswhereto-4-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-jswhereto-4-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

## alert(8); is the same as window.alert(8);. True or False?
<div id="quiz-jswhereto-5-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-5-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-5-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-5-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "True #correct\n" +
    "False #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-5-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-5-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-jswhereto-5-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-jswhereto-5-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>


## Select the correct syntax for writing 'Hello': (body'Hello'documentconsolegetElementByIdwriteprint)
<div id="quiz-jswhereto-6-sortableTrash" class="sortable-code"></div>
<div id="quiz-jswhereto-6-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="quiz-jswhereto-6-feedbackLink" value="Get Feedback" type="button" />
    <input id="quiz-jswhereto-6-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "document.write('Hello') #correct\n" +
    "console.log('Hello') #distractor\n" +
    "print('Hello') #distractor\n" +
    "body('Hello') #distractor\n" +
    "getElementById('Hello') #distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "quiz-jswhereto-6-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "trashId": "quiz-jswhereto-6-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#quiz-jswhereto-6-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#quiz-jswhereto-6-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

