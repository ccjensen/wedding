---
layout: page
title: "who's who"
comments: false
sharing: false
footer: true
people: 
  - [
      ["Photo", "anne.jpg"], 
      ["Name", "Anne Beaubien", "Bride"], 
      ["Birth place", "Missouri, USA"],
      ["Current location", "California, USA"],
      ["Favorite drink", "Sangria Smoothie"],
      ["Favorite past-times", "cycling, cooking, gardening, traveling"],
      ["About", "Having grown up in a military family, Anne has rarely spent more than 2 years in the some place. Fortunately she loves to travel, and was lucky enough to find herself a foreigner who shares the same passion.
	  Anne loves cooking for Chris and spends most of her time coming up with new recipes for her website WaffleHearts.com, which are of course taste tested by Chris."]
    ]
  - [
      ["Photo", "chris.jpg"], 
      ["Name", "Christopher Campbell Jensen", "Groom"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "California, USA "],
      ["Favorite drink", "Midori Sour"],
      ["Favorite past times", "programming, traveling, exercise"],
      ["About", "Being half English and half Norwegian with family spread across the two countries involved a lot of travelling forth and back for Christopher. Therefore it surprised no one that as soon as he reached adulthood he spent the next ten years seeing different parts of the world. Currently Christopher is really enjoying the sunny california coast while working at Apple Inc, helping to develop all of those very secret devices. You know you have one."]
	]
  - [
      ["Photo", "margaret.jpg"], 
      ["Name", "Margaret S. Beaubien", "Mother of the Bride"],
      ["Birthplace", "Arizona, USA"],
      ["Current location", "Virginia, USA"],
      ["Favorite drink", "Margarita"],
      ["Favorite past times", "reading, traveling, taking pictures, having tea with her daughter (Anne)"],
      ["About", "Margaret is a single parent with two great kids. Her love of caring for others lead her to a career in nursing where she eventually joined the Navy Nurse Corps. After becoming a captain, Margaret moved on to serve as the Chief Medical Information Officer and quite recently became the first Naval Officer and nurse to serve as the Deputy Chief Information Officer for the Military Health System."]
	]
  - [
      ["Photo", "joan.jpg"], 
      ["Name", "Joan Jensen", "Mother of the Groom"],
      ["Birthplace", "Corbridge, England"],
      ["Current location", "Vestby, Norway"],
      ["Favorite Drink", "Wine: a glass of Italian red Barolo or Ripasso and on lazy, warm summer days rosé from Provence or a glass of sparkling"],
      ["Favorite past times", "Theatre visits, jazz music, gardening and should be golf BUT at the moment the golf bag is collecting dust."],
      ["About", "Joan is a single parent for two great yet very different brothers. She currently works for VPS, the only central securities depository in Norway, where she primarily helps develop international data exchange standards used by a lot of the European countries. Perks of her job include frequent flier miles and relaxing at the company’s French apartment."]
	]
  - [
      ["Photo", "jennifer.jpg"], 
      ["Name", "Jennifer Walker", "Maid of Honor"],
      ["Birthplace", "Arizona, USA"],
      ["Current location", "Washington DC, USA"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", "Jennifer and Anne have been best friends since they were 7"]
	]
  - [
      ["Photo", "oyvind.jpg"], 
      ["Name", "Øyvind Rassmussen", "Best Man"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "Bergen, Norway"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "katie.jpg"], 
      ["Name", "Katie Velazco", "Bridesmaid"],
      ["Birthplace", "Georgia, USA"],
      ["Current location", "Maryland, USA"],
      ["Favorite drink", "Peruvian Chicha Morada! Her dad is from Peru (though never taught her Spanish and only took her to the country once when she was 12) so drinking this spiced fruit juice made from dried purple corn is about the extent of her 1/2 heritage"],
      ["Favorite past times", "Katie loves museums and reading about archaeology. She also enjoys being outdoors, taking walks, buying tech gadgets (and everything else) off Amazon, and playing RPGs while her girlfriend cheers her on and eats popcorn"],
      ["About", "Katie actually introduced Anne and Chris! Though it was technically really an online dorm forum & a beautiful thing you might have heard of called an iPhone that brought them together"]
	]
  - [
      ["Photo", "steven.jpg"], 
      ["Name", "Steven Jensen", "Groomsman"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "London, England"],
      ["Favorite Drink", "Why choose one!? Old Fashion, Pisco Sour, English bitter, Bordeaux reds…the list is endless!"],
      ["Favorite past times", "Golf, Countryside walks with the dog, Skiing, Seeing the world"],
      ["About", "Steven, big brother of the Groom, used to allocate plenty time to provide his little brother daily teasing sessions when they were younger. However in recent years, he has replaced teasing with telephone calls across the Atlantic asking Christopher for urgent help with his Apple gadgets! Steven shares a flat in Notting Hill with his girlfriend Aislinn and their dog Asterix. He has been living and working as a banker in London since 2005."]
	]
  - [
      ["Photo", "amy.jpg"], 
      ["Name", "Amy Jizmagian", "Bridesmaid"],
      ["Birthplace", "California, USA"],
      ["Current location", "California, USA"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "michael.jpg"], 
      ["Name", "Michael Beaubien", "Groomsman"],
      ["Birthplace", "Missouri, USA"],
      ["Current location", ""],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
---
{% for person in page.people %}
<div class="who">
	{% for detail in person %}
		{% if detail[0] == "Name" %}
			<h2>{{detail[1]}} ({{detail[2]}})</h2>			
		{% elsif detail[0] == "Photo" %}
			<div class="picture">
				<img src="../images/{{detail[1]}}" height="200px" width="200px"/>
			</div>
		{% else %}			
			<p>
				<span class="category">{{detail[0]}}: </span>{{detail[1]}}
			</p>
		{% endif %}
	{% endfor %}
</div>
<hr/>
{% endfor %}