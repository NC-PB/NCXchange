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

-------

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
    <td>GOTO:X=-22.543</td>
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

## Werkzeuge

{{% include file="specification/de/TOOL_CALL.md" %}}
{{% include file="specification/de/TOOL_SELECT.md" %}}


## Maschinenfunktionen

{{% include file="specification/de/MACHINE_FUNCTION.md" %}}
 


{{% include file="specification/de/CYCLE.md" %}}

-----
## Bezugspunkt

{{% include file="specification/de/ORIGIN.md" %}}

{{% include file="specification/de/MATRIX.md" %}}

--------

{{% include file="specification/de/FEEDRATE.md" %}}

{{% include file="specification/de/FEEDRATE_TYPE.md" %}}

----------

{{% include file="specification/de/SPINDLE.md" %}}

{{% include file="specification/de/RPM.md" %}}
