+++
title = "Spezifikation"
weight = 2
+++

### Programm

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Schlüsselwort</td>
    <td colspan="2">PROGRAM</td>
  </tr>
  <tr>
    <td rowspan="3">Adresse</td>
    <td colspan="2">NAME</td>
  </tr>
  <tr>
    <td colspan="2">TYPE</td>
  </tr>
  <tr>
    <td colspan="2">COMM</td>
  </tr>
  <tr>
    <td rowspan="4">Werte</td>
    <td>PROGRAM:NAME</td>
    <td>String</td>
  </tr>
  <tr>
    <td rowspan="2">PROGRAM:UNIT</td>
    <td>MM</td>
  </tr>
  <tr>
    <td>INCH</td>
  </tr>
  <tr>
    <td>PROGRAM:COMM</td>
    <td>String</td>
  </tr>
    <tr>
    <td rowspan="3">Beispiel</td>
    <td colspan="2">PROGRAM:COMM=Links</td>
  </tr>
  <tr>
    <td colspan="2">PROGRAM:UNIT=MM</td>
  </tr>
  <tr>
    <td colspan="2">PROGRAM:NAME=5544</td>
  </tr>
</tbody>
</table>


### Interpolation

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Schlüsselwort</td>
    <td><b>INTERPO</B></td>
  </tr>
  <tr>
    <td rowspan="6">Werte</td>
    <td>RAPID</td>
  </tr>
  <tr>
    <td>WORK</td>
  </tr>

  <tr>
    <td>ARC,CW</td>
  </tr>

  <tr>
    <td>ARC,CCW</td>
  </tr>

  <tr>
    <td>ARC,CW,CENTER</td>
  </tr>

  <tr>
    <td>ARC,CCW,CENTER</td>
  </tr>

  <tr>
    <td>Beispiel</td>
    <td>INTERPO=ARC,CCW</td>
  </tr>
</tbody>
</table>

### Kreismittelpunkt

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Schlüsselwort</td>
    <td>CENTER</td>
  </tr>
  <tr>
    <td>Adresse</td>
    <td>Achse</td>
  </tr>
  <tr>
    <td>Wert</td>
    <td>Position</td>
  </tr>
    <tr>
    <td>Beispiel</td>
    <td>CENTER:X=20</td>
  </tr>
</tbody>
</table>

### Bewegung

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Schlüsselwort</td>
    <td>GOTO</td>
</tr>
<tr>
    <td>Adresse</td>
    <td>Achse</td>
  </tr>
  <tr>
    <td>Wert</td>
    <td>Position</td>
  </tr>
<tr>
    <td>Beispiel</td>
    <td>GOTO:X=-22-543</td>
  </tr>
</tbody>
</table>

### Arbeitsebene

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>WORKPLANE</td>
    </tr>
      <tr>
        <td rowspan="3">Werte</td>
        <td>XY+Z</td>
    </tr>
  <tr>
        <td>XZ+Y</td>
    </tr>
  <tr>
        <td>YZ+X</td>
    </tr>
    </tbody>
</table>


### Radiuskompensation

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>COMPENSATION</td>
    </tr>
    <tr>
        <td rowspan="3">Werte</td>
        <td>LEFT</td>
    </tr>
    <tr>
        <td>RIGHT</td>
    </tr>
    <tr>
        <td>OFF</td>
    </tr>
  <tr>
    <td>Beispiel</td>
    <td>COMPENSATOIN=OFF</td>
  </tr>
    </tbody>
</table>


### Offset

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>OFFSET</td>
    </tr>
  <tr>
    <td>Wert</td>
    <td>Offsetnummer</td>
  </tr>
    <tr>
        <td rowspan="2">Adresse</td>
        <td>LEN</td>
    </tr>
     <tr>
        <td>DIAM</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>OFFSET:LEN=10</td>
    </tr>
    </tbody>
</table>


 ### Werkzeugaufruf

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>TOOL_CALL</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Werkzeugnummer</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>TOOL_CALL=12</td>
    </tr>
    </tbody>
</table>


### Drehzahl

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>RPM</td>
    </tr>
  <tr>
    <td>Beispiel</td>
    <td>RPM=1200</td>
  </tr>
    </tbody>
</table>


### Maschinenbefehle

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>FUNCTION_MACHINE</td>
    </tr>
    <tr>
        <td>Wert</td>
        <td>M-Code Nummer</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>FUNCTION_MACHINE=56</td>
    </tr>
    </tbody>
</table>



### Kommentar

<table id="myTable">
    <tbody>
        <tr>
            <td class="column1">Schlüsselwort</td>
            <td>COMM</td>
        </tr>
        <tr>
            <td>Beispiel</td>
            <td>COMM=PLANFRAESEN</td>
        </tr>
    </tbody>
</table>


### Bearbeitungszyklen

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td colspan="2">CYCLE</td>
    </tr>
    <tr>
        <td rowspan="6">Werte</td>
        <td>Bohren</td>
        <td>DRILL</td>
    </tr>
    <tr>
        <td>Bohren mir Verweilzeit</td>
        <td>DRILL,DELAY</td>
    </tr>
    <tr>
        <td>Tieflochbohren</td>
        <td>DRILL,DEEP_HOLE</td>
    </tr>
    <tr>
        <td>Gewindeschneiden</td>
        <td>TAP</td>
    </tr>
    <tr>
        <td>Reiben</td>
        <td>REAM</td>
    </tr>
    <tr>
        <td>Stopp</td>
        <td>STOP</td>
    </tr>
        <td class="column1">Beispiel</td>
        <td colspan="2">CYCLE=DRILL,DEEP_HOLE</td>
    </tbody>
</table>


### Nullpunkt

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>ORIGIN</td>
    </tr>
    <tr>
        <td>Wert</td>
        <td>Nullpunknummer</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>ORIGIN=1</td>
    </tr>
    </tbody>
</table>


### Vorschub

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>FEEDRATE</td>
    </tr>
    <tr>
        <td>Wert</td>
        <td>Vorschubwert</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>FEEDRATE=200</td>
    </tr>
    </tbody>
</table>

### Vorschubart

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td>FEEDRATE_TYPE</td>
    </tr>
    <tr>
        <td rowspan="3">Wert</td>
         <td>MIN</td>
    </tr>
    <tr>
        <td>RPM</td>
    </tr>
        <tr>
        <td>FZ</td>
    </tr>
    <tr>
        <td>Beispiel</td>
        <td>FEEDRATE_TYPE=MIN</td>
    </tr>
    </tbody>
</table>

 ### Nullpunktverschiebung


<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td colspan="2">MATRIX</td>
    </tr>
    <tr>
        <td rowspan="3">Adresse</td>
        <td>Verschiebung in X</td>
        <td>SHIFT_X</td>
    </tr>
    <tr>
        <td>Verschiebung in Y</td>
        <td>SHIFT_Y</td>
    </tr>
    <tr>
        <td>Verschiebung in Z</td>
        <td>SHIFT_Z</td>
    </tr>
    <tr>
        <td class="column1">Beispiel</td>
        <td colspan="2">MATRIX:SHIFT_X=33.5</td>
    </tbody>
</table>


### Spindel

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Schlüsselwort</td>
        <td colspan="2">SPINDLE</td>
    </tr>
    <tr>
        <td rowspan="3">Werte</td>
        <td>Ein Rechtslauf</td>
        <td>CW</td>
    </tr>
    <tr>
        <td>Ein Linkslauf</td>
        <td>CCW</td>
    </tr>
    <tr>
        <td>Aus</td>
        <td>OFF</td>
    </tr>
        <tr>
        <td>Adresse</td>
        <td colspan="2">Spindelnummer</td>
    </tr> 
    <tr>
        <td>Beispiel</td>
        <td colspan="2">SPINDLE:1=CCW</td>
    </tr>
    </tbody>
</table>
