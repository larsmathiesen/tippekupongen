---
layout: page
title: Uke 32 - 2016
subtitle: 8. august - 14. august
---

{% for it in site.data.2016_32_1 %}
<div class="col-md-12">
	<p>{{it[0]}} - {{it[1].dato}}</p>
<div class="col-md-12">
Full tid
<table>
		<tr>
			<th>#</th>
			<th>Lag</th>
			<th>Pause</th>
			<th>Resultat</th>
			
		</tr>
		{% for match in it[1].Matches %}
			<tr>
				<td>{{match[0]}}</td>
				<td>{{match[1].Hometeam}} -  {{match[1].Awayteam}}</td>
				<td>{{match[1].PauseResult}} B</td>
				<td>{{match[1].Result}}  H</td>
				
			</tr>
		{% endfor %}
	</table>
</div>

</div>

{% endfor %}