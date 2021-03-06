---
# Front matter (even empty) required for Jekyll to process
---

#### Map Name: Dominica

#### JavaScript Alias: maps/dominica


<div class="code-wrapper">
<ul class='code-tabs'>
    <li class='active'>
        <a data-toggle='new-json'>New JSON Format</a>
    </li>
    <li>
        <a data-toggle='old-json'>Old JSON Format</a>
    </li>
    <li>
        <a data-toggle='old-xml'>Old XML Format</a>
    </li>
</ul>
<div class='tab-content'>
    <pre class='plain-code'></pre>
    <div class='tab new-json-tab active'>
<pre><code class="language-javascript">
{
    "map": {
        "showshadow": "0",
        "showlabels": "0",
        "showmarkerlabels": "1",
        "fillcolor": "F1f1f1",
        "bordercolor": "CCCCCC",
        "basefont": "Verdana",
        "basefontsize": "10",
        "markerbordercolor": "000000",
        "markerbgcolor": "FF5904",
        "markerradius": "6",
        "usehovercolor": "0",
        "hoveronempty": "0",
        "showmarkertooltip": "1",
        "canvasBorderColor": "375277",
        "canvasBorderAlpha": "0"
    },
    "markers": {
        "shapes": [
            {
                "id": "myCustomShape",
                "type": "circle",
                "fillcolor": "FFFFFF,333333",
                "fillpattern": "radial",
                "showborder": "0",
                "radius": "4"
            },
            {
                "id": "newCustomShape",
                "type": "circle",
                "fillcolor": "FFFFFF,000099",
                "fillpattern": "radial",
                "showborder": "0",
                "radius": "3"
            }
        ],
        "items": [
            {
                "id": "RO",
                "shapeid": "myCustomShape",
                "x": "56.89",
                "y": "208.27",
                "label": "Roseau",
                "labelpos": "left"
            },
            {
                "id": "01",
                "shapeid": "newCustomShape",
                "x": "13.95",
                "y": "39.72",
                "label": "Portsmouth",
                "labelpos": "right"
            },
            {
                "id": "02",
                "shapeid": "newCustomShape",
                "x": "109.5",
                "y": "65.48",
                "label": "Marigot"
            },
            {
                "id": "03",
                "shapeid": "newCustomShape",
                "x": "36.5",
                "y": "151.37",
                "label": "Saint Joseph"
            },
            {
                "id": "04",
                "shapeid": "newCustomShape",
                "x": "135.27",
                "y": "190.02",
                "label": "La Plaine",
                "labelpos": "left"
            },
            {
                "id": "05",
                "shapeid": "newCustomShape",
                "x": "98.76",
                "y": "241.55",
                "label": "Berekua"
            }
        ]
    }
}
</code></pre>


<p class='text-success'>New JSON format for map marker data.</p>

    </div>
    <div class='tab old-json-tab'>
<pre><code class="language-javascript">
{
    "map": {},
    "markers": {
        "shapes": [
            {
                "id": "myCustomShape",
                "type": "circle",
                "fillcolor": "FFFFFF,333333",
                "fillpattern": "radial",
                "showborder": "0",
                "radius": "4"
            },
            {
                "id": "newCustomShape",
                "type": "circle",
                "fillcolor": "FFFFFF,000099",
                "fillpattern": "radial",
                "showborder": "0",
                "radius": "3"
            }
        ],
        "definition": [
            {
                "id": "RO",
                "x": "56.89",
                "y": "208.27",
                "label": "Roseau",
                "labelpos": "left"
            },
            {
                "id": "01",
                "x": "13.95",
                "y": "39.72",
                "label": "Portsmouth",
                "labelpos": "right"
            },
            {
                "id": "02",
                "x": "109.5",
                "y": "65.48",
                "label": "Marigot"
            },
            {
                "id": "03",
                "x": "36.5",
                "y": "151.37",
                "label": "Saint Joseph"
            },
            {
                "id": "04",
                "x": "135.27",
                "y": "190.02",
                "label": "La Plaine",
                "labelpos": "left"
            },
            {
                "id": "05",
                "x": "98.76",
                "y": "241.55",
                "label": "Berekua"
            }
        ],
        "application": [
            {
                "id": "RO",
                "shapeid": "myCustomShape"
            },
            {
                "id": "01",
                "shapeid": "newCustomShape"
            },
            {
                "id": "02",
                "shapeid": "newCustomShape"
            },
            {
                "id": "03",
                "shapeid": "newCustomShape"
            },
            {
                "id": "04",
                "shapeid": "newCustomShape"
            },
            {
                "id": "05",
                "shapeid": "newCustomShape"
            }
        ]
    }
}
</code></pre>


<p class='text-success'>Old JSON format for map marker data, using separate application and definition blocks.</p>

    </div>
    <div class='tab old-xml-tab'>
<pre><code class="language-html">
<map>
	<markers>
	   <shapes>
	       <shape id='myCustomShape' type='circle' fillColor='FFFFFF,333333' fillPattern='radial' showBorder='0' radius='4'/>
		   <shape id='newCustomShape' type='circle' fillColor='FFFFFF,000099' fillPattern='radial' showBorder='0' radius='3'/>
		</shapes>
		<definition>
			<marker id='RO' x='56.89' y='208.27' label='Roseau' labelpos='left'  />
			<marker id='01' x='13.95' y='39.72' label='Portsmouth' labelPos='right'  />
			<marker id='02' x='109.5' y='65.48' label='Marigot'  />
			<marker id='03' x='36.5' y='151.37' label='Saint Joseph'  />
			<marker id='04' x='135.27' y='190.02' label='La Plaine' labelPos='left' />
			<marker id='05' x='98.76' y='241.55' label='Berekua'  />

		</definition>
		<application>
			<marker id='RO' shapeId='myCustomShape'  />
			<marker id='01' shapeId='newCustomShape'  />
			<marker id='02' shapeId='newCustomShape'  />
			<marker id='03' shapeId='newCustomShape'  />
			<marker id='04' shapeId='newCustomShape'  />
			<marker id='05' shapeId='newCustomShape'  />

		</application>
	</markers>
</map>
</code></pre>

<p class='text-success'>Old XML format for map marker data, using separate application and definition blocks.</p>

</div>
</div>
</div>
