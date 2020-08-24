---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: UH - Carolyn Miles - Critical Thinking Parson's Problem
---
# Parsons Practice

## Practice Project
Correctly order Hello, Conversation and Goodbye by dragging the blocks to the space below. Click "Get feedback" when you are done. If the blocks turn green you are correct.  Red means you need to try again.

<div id="PP-sortableTrash" class="sortable-code"></div> 
<div id="PP-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="PP-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="PP-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "Hello\n" +
    "Conversation\n" +
    "Goodbye";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "PP-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "PP-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#PP-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#PP-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>


## Critical Thinking Project
Put the steps to making mac and cheese in the correct order by dragging them up and down in the list.  Click "Get feedback" when you are done. If the blocks turn green you are correct.  Red means you need to try again.

<div id="jlm-sortableTrash" class="sortable-code"></div> 
<div id="jlm-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="jlm-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="jlm-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "Boil water\n" +
    "Add noodles\n" +
    "Cook noodles\n" +
    "Drain noodles\n" +
    "Add milk and butter\n" +
    "Add cheese\n" +
    "Stir to combine";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "jlm-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#jlm-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#jlm-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>



