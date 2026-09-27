<mxfile host="app.diagrams.net" modified="2026-09-27T12:00:00.000Z" agent="Mozilla/5.0" version="22.0.7" type="device">
  <diagram name="Page-1" id="UY5lw3JXvJX1q1XJ324X">
    <mxGraphModel dx="1205" dy="602" grid="1" gridSize="10" guides="1" tooltips="1" connect="1" arrows="1" fold="1" page="1" pageScale="1" pageWidth="850" pageHeight="1100" math="0" shadow="0">
      <root>
        <mxCell id="0" />
        <mxCell id="1" parent="0" />

        <!-- Styles -->
        <UserObject label="Mode" id="modeStyle" style="rounded=1;whiteSpace=wrap;html=1;aspect=fixed;fillColor=#f9f;strokeColor=#333;" parent="1">
          <mxGeometry x="0" y="0" width="120" height="60" as="geometry" />
        </UserObject>
        <UserObject label="Action" id="actionStyle" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#9f9;strokeColor=#333;" parent="1">
          <mxGeometry x="0" y="0" width="120" height="40" as="geometry" />
        </UserObject>
        <UserObject label="Erreur" id="errorStyle" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" parent="1">
          <mxGeometry x="0" y="0" width="120" height="40" as="geometry" />
        </UserObject>
        <UserObject label="Start/End" id="startEndStyle" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#99f;strokeColor=#333;" parent="1">
          <mxGeometry x="0" y="0" width="120" height="40" as="geometry" />
        </UserObject>

        <!-- Noeuds -->
        <mxCell id="start" value="Début" style="shape=ellipse;fillColor=#99f;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="400" y="20" width="80" height="40" as="geometry" />
        </mxCell>

        <mxCell id="standardMode" value="Mode Standard&#xa;LED verte continue" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f9f;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="300" y="100" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="configMode" value="Mode Configuration&#xa;LED jaune continue" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f9f;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="300" y="250" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="maintenanceMode" value="Mode Maintenance&#xa;LED orange continue" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f9f;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="550" y="250" width="120" height="60" as="geometry" />
        </mxCell>
        <mxCell id="ecoMode" value="Mode Économique&#xa;LED bleue continue" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f9f;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="550" y="100" width="120" height="60" as="geometry" />
        </mxCell>

        <!-- Actions -->
        <mxCell id="acquisition" value="Acquisition continue&#xa;des capteurs" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#9f9;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="200" y="180" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="configAction" value="Attente commandes série&#xa;+ Mise à jour paramètres" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#9f9;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="200" y="330" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="maintenanceAction" value="Désactivation écriture&#xa;carte SD + Lecture série" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#9f9;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="450" y="330" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="ecoAction" value="Désactivation GPS&#xa;+ LOG_INTERVAL x2" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#9f9;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="450" y="180" width="120" height="40" as="geometry" />
        </mxCell>

        <!-- Erreurs -->
        <mxCell id="errRTC" value="LED rouge+bleue&#xa;Erreur RTC" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="100" y="400" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="errGPS" value="LED rouge+jaune&#xa;Erreur GPS" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="250" y="400" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="errCapteur" value="LED rouge+verte&#xa;Erreur capteur" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="400" y="400" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="errDataInco" value="LED rouge+verte (vert 2x)&#xa;Données incohérentes" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="550" y="400" width="120" height="40" as="geometry" />
        </mxCell>
        <mxCell id="errSDFull" value="LED rouge+blanche&#xa;Carte SD pleine" style="rounded=1;whiteSpace=wrap;html=1;fillColor=#f99;strokeColor=#333;" vertex="1" parent="1">
          <mxGeometry x="700" y="400" width="120" height="40" as="geometry" />
        </mxCell>

        <!-- Flèches -->
        <mxCell id="edge1" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="start" target="standardMode">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="edge2" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="standardMode" target="configMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="360" y="160" as="sourcePoint" />
            <mxPoint x="360" y="250" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge2">
            <mxGeometry x="360" y="190" width="100" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="100" height="20" as="geometry" />
              <value>Bouton rouge&#xa;pressé au démarrage</value>
            </mxCell>
          </mxCell>
        </mxCell>
        <mxCell id="edge3" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="standardMode" target="acquisition">
          <mxGeometry relative="1" as="geometry" />
        </mxCell>
        <mxCell id="edge4" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="standardMode" target="maintenanceMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="420" y="130" as="sourcePoint" />
            <mxPoint x="550" y="250" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge4">
            <mxGeometry x="485" y="170" width="80" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="80" height="20" as="geometry" />
              <value>Bouton rouge&#xa;5 secondes</value>
            </mxCell>
          </mxCell>
        </mxCell>
        <mxCell id="edge5" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="standardMode" target="ecoMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="420" y="130" as="sourcePoint" />
            <mxPoint x="550" y="100" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge5">
            <mxGeometry x="485" y="90" width="80" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="80" height="20" as="geometry" />
              <value>Bouton vert&#xa;5 secondes</value>
            </mxCell>
          </mxCell>
        </mxCell>
        <mxCell id="edge6" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="configMode" target="standardMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="360" y="310" as="sourcePoint" />
            <mxPoint x="360" y="100" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge6">
            <mxGeometry x="360" y="200" width="80" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="80" height="20" as="geometry" />
              <value>30 min sans&#xa;activité</value>
            </mxCell>
          </mxCell>
        </mxCell>
        <mxCell id="edge7" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="maintenanceMode" target="standardMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="610" y="310" as="sourcePoint" />
            <mxPoint x="420" y="100" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge7">
            <mxGeometry x="515" y="200" width="80" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="80" height="20" as="geometry" />
              <value>Bouton rouge&#xa;5 secondes</value>
            </mxCell>
          </mxCell>
        </mxCell>
        <mxCell id="edge8" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;" edge="1" parent="1" source="ecoMode" target="standardMode">
          <mxGeometry relative="1" as="geometry">
            <mxPoint x="610" y="130" as="sourcePoint" />
            <mxPoint x="420" y="100" as="targetPoint" />
          </mxGeometry>
          <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=center;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1" parent="edge8">
            <mxGeometry x="515" y="100" width="80" height="20" as="geometry" />
            <mxCell style="text;html=1;strokeColor=none;fillColor=none;align=left;verticalAlign=middle;resizable=0;points=[];autosize=1;" vertex="1">
              <mxGeometry x="0" y="0" width="80" height="20" as="geometry" />
              <value>Bouton rouge&#xa;5 secondes</value>
            </mxCell>
          </mxCell>
        </mxCell>

        <!-- Flèches vers les erreurs -->
        <mxCell id="edgeErr1" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;dashed=1;" edge="1" parent="1" source="standardMode" target="errRTC" />
        <mxCell id="edgeErr2" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;dashed=1;" edge="1" parent="1" source="standardMode" target="errGPS" />
        <mxCell id="edgeErr3" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;dashed=1;" edge="1" parent="1" source="standardMode" target="errCapteur" />
        <mxCell id="edgeErr4" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;dashed=1;" edge="1" parent="1" source="standardMode" target="errDataInco" />
        <mxCell id="edgeErr5" style="edgeStyle=none;curved=1;rounded=0;endArrow=classic;endFill=1;html=1;dashed=1;" edge="1" parent="1" source="standardMode" target="errSDFull" />
      </root>
    </mxGraphModel>
  </diagram>
</mxfile>
