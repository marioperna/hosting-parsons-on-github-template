---
layout: default
title: HTML - Esercizio Gruppo 0 n. 1
description: Crea una struttura HTML di base
---

<div id="html_intro-1-sortableTrash" class="sortable-code"></div>
<div id="html_intro-1-sortable" class="sortable-code"></div>
<div style="clear:both;"></div>
<p>
    <input id="html_intro-1-feedbackLink" value="Get Feedback" type="button" />
    <input id="html_intro-1-newInstanceLink" value="Reset Problem" type="button" />
</p>
<script type="text/javascript">
(function(){
  var initial = "&lt;!DOCTYPE html&gt;\n" +
    "&lt;html lang=&#039;en&#039;&gt;\n" +
    "&lt;head&gt;\n" +
    "  &lt;meta charset=&#039;UTF-8&#039;&gt;\n" +
    "  &lt;meta name=&#039;viewport&#039; content=&#039;width=device-width, initial-scale=1.0&#039;&gt;\n" +
    "  &lt;meta http-equiv=&#039;X-UA-Compatible&#039 content=&#039;ie=edge&#039;&gt;\n" +
    "  &lt;title&gt;Document&lt;/title&gt;\n" +
    "&lt;/head&gt;\n" +
    "&lt;body&gt;\n" +
    "  &lt;h1&gt;My First Heading&lt;/h1&gt;\n" +
    "  &lt;p&gt;My first paragraph.&lt;/p&gt;\n" +
    "&lt;/body&gt;\n" +
    "&lt;/html&gt;";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "html_intro-1-sortable",
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
  $("#html_intro-1-newInstanceLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.shuffleLines();
  });
  $("#html_intro-1-feedbackLink").click(function(event){
      event.preventDefault();
      parsonsPuzzle.getFeedback();
  });
})();
</script>

[Torna all'indice](../../../index.markdown)