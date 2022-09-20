# Feedback po wydarzeniu

<!-- The following div will be populated only when JS is enabled -->
<div id="language-switch">
</div>

<div style="text-align: center" id="feedback-form">
	<p style="text-align: left;" id="prompt">Pomóż nam i zostaw feedback :)</p>
    <form action="https://awfeedback.dev2.szostek.net/thanks" method="post" accept-charset="UTF-8">
	  <h2 id="score">Ogólna ocena wydarzenia</h2>
	  <div id="feedback-points">
		<div class="wrap">
          <input type="radio" id="1" name="score" value="1">
          <label for="1">1</label>
	    </div>
		<div class="wrap">
          <input type="radio" id="2" name="score" value="2">
          <label for="2">2</label>
	    </div>
		<div class="wrap">
          <input type="radio" id="3" name="score" value="3">
          <label for="3">3</label>
	    </div>
		<div class="wrap">
          <input type="radio" id="4" name="score" value="4">
          <label for="4">4</label>
	    </div>
		<div class="wrap">
          <input type="radio" id="5" name="score" value="5">
          <label for="5">5</label>
	    </div>
		<div class="wrap">
          <input type="radio" id="6" name="score" value="6">
          <label for="6">6</label>
	    </div>
	  </div>
      <h2><label for="good" id="q1">Co poszło dobrze?</label><br></h2>
      <textarea id="good" name="good" rows="10" style="width: 90%"></textarea><br>
      <h2><label for="bad" id="q2">Co można poprawić?</label><br></h2>
      <textarea id="bad" name="bad" rows="10" style="width: 90%"></textarea><br>
      <input id="feedback-submit-button" type="submit" value="send">
    </form>
<div>

<script>

	const englishTranslation = {
		"feedback-po-wydarzeniu": "Event feedback",
		"prompt": "We would love some feedback from you :)",
		"score": "How did you like it overall?",
		"q1": "What went well?",
		"q2": "What can be improved?",
		"language-switch": "<div id=\"language-switch\"> Przełącz na: <img class=\"lang-icon\" src=\"/assets/flag-pl.svg\" onclick=\"translateFormToPolish()\"> </div>"
	}

	function populatePolishTranslation() {
		for(var id in englishTranslation){
			polishTranslation[id] = document.getElementById(id).innerHTML
		}
	}

	function translateFormToEnglish(){
		for(var id in englishTranslation){
			translateElementById(id, englishTranslation[id])
		}
	}

	function translateFormToPolish(){
		for(var id in polishTranslation){
			translateElementById(id, polishTranslation[id])
		}
	}

	function translateElementById(id, newInnerHTML) {
		element = document.getElementById(id)
		element.innerHTML = newInnerHTML
	}

	var polishTranslation = {}

	// show the language switch only if JS is enabled
	translateElementById("language-switch", "Switch to: <img class=\"lang-icon\" src=\"/assets/flag-uk.svg\" onclick=\"translateFormToEnglish()\">")
	
	populatePolishTranslation()

</script>
