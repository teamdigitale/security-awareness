---
title: "Quiz"
---
<div id="surveyContainer"></div>
<div id="surveyResult"></div>

<script>
var surveyJSON = { surveyId: '173d65eb-1feb-4bbb-8103-79ae34ce2123' };
var survey = new Survey.Model(surveyJSON);

survey
    .onComplete
    .add(function (result) {
        survey.sendResult('723cc519-e005-4602-abbb-04dd3fa7aee3');
        //document
        //    .querySelector('#surveyResult')
        //    .textContent = "Result JSON:\n" + JSON.stringify(result.data, null, 3);
    });

$("#surveyContainer").Survey({ model: survey });

</script>