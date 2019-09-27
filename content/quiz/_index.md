---
title: "Quiz"
---
<div id="surveyContainer"></div>

<script>
var surveyJSON = { surveyId: '173d65eb-1feb-4bbb-8103-79ae34ce2123'}

function sendDataToServer(survey) {
    survey.sendResult('723cc519-e005-4602-abbb-04dd3fa7aee3');
}

var survey = new Survey.Model(surveyJSON);
$("#surveyContainer").Survey({
    model: survey,
    onComplete: sendDataToServer
});
</script>