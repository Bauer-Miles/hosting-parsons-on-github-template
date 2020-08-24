---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: UH - Carolyn Miles - Critical Thinking Parsons Problem
---
# Parsons Practice

## Practice Project
Correctly order Hello, Conversation and Goodbye by dragging the blocks to the yellow space below. Click "Get feedback" when you are done. If the blocks turn green you are correct.  Red means you need to try again by clicking "Reset problem".

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
Put the steps to critical thinking project in the correct order by dragging the blocks to the yellow space below. Click "Get feedback" when you are done. If the blocks turn green you are correct.  Red means you need to try again by clicking "Reset problem". Take a photo of your correct solution with your student ID in the photo.  Submit the photo on Blackboard.

<div id="CT-sortableTrash" class="sortable-code"></div> 
<div id="CT-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="CT-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="CT-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "Import all three starting data files\n" +
    "Verify each file import was successful\n" +
    "Combine the two store sales files into one combined sale file\n" +
    "Verify record count of combined sales file is correct\n" +
    "Identify common field to join combined sales file to the item description file\n" +
    "Join combined sales file to the item description file to create one large flat file\n" +
    "Sum sales by day by department\n" +
    "Verify one department's total manually\n" +
    "Create department report showing only required fields\n" +
    "Sum sales by day by item\n" +
    "Verify one item's total manually\n" +
    "Create item report showing only required fields\n" +
    "Verify grand totals on both reports match";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "CT-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "trashId": "CT-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#CT-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#CT-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
