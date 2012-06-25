---
layout: page
title: "who's who"
comments: false
sharing: false
footer: true
people: 
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Anne Beaubien", "Bride"], 
      ["Birth place", "Missouri, USA"],
      ["Current location", "California, USA"],
      ["Favorite drink", "Sangria Smoothie"],
      ["Favorite past-times", "cycling, cooking, gardening, traveling"],
      ["About", "Anne loves cooking for Chris and spends most of her time coming up with new recipes for her website WaffleHearts.com, which are of course taste tested by Chris."]
    ]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Christopher Campbell Jensen", "Groom"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "California, USA "],
      ["Favorite drink", "Midori Sour"],
      ["Favorite past times", "programming, traveling, exercise"],
      ["About", "Chris is really enjoying the sunny california coast while working at Apple Inc, helping to develop all of those very secret devices. You know you have one."]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Margaret S. Beaubien", "Mother of the Bride"],
      ["Birthplace", "Arizona, USA"],
      ["Current location", "Virginia, USA"],
      ["Favorite drink", ""],
      ["Favorite past times", ""],
      ["About", "Margaret is a Captain in the US Navy and we can't tell you what she does or she would have to kill you."]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Joan Jensen", "Mother of the Groom"],
      ["Birthplace", "Newcastle, England"],
      ["Current location", "Vestby, Norway"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", "Joan works for VPS, the only central securities depository in Norway. Perks of her job include frequent flier miles and relaxing at the company’s French Apartment."]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Jennifer Walker", "Maid of Honor"],
      ["Birthplace", "Arizona, USA"],
      ["Current location", "Washington DC, USA"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", "Jennifer and Anne have been best friends since they were 7 "]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Øyvind Rassmussen", "Best Man"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "Bergen, Norway"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Katie Velazco", "Bridesmaid"],
      ["Birthplace", "Georgia, USA"],
      ["Current location", "Maryland, USA"],
      ["Favorite drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Steven Jensen", "Groomsman"],
      ["Birthplace", "Oslo, Norway"],
      ["Current location", "London, England"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "test.jpg"], 
      ["Name", "Amy Jizmagian", "Bridesmaid"],
      ["Birthplace", "California, USA"],
      ["Current location", "California, USA"],
      ["Favorite Drink", ""],
      ["Favorite past times", ""],
      ["About", ""]
	]
  - [
      ["Photo", "test.jpg"], 
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
				<img src="{{detail[1]}}" height="200px" width="200px"/>
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