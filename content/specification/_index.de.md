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

{{< include-html "content/specification/de/INTERPO.html" >}}

### Kreismittelpunkt
{{< include-html "content/specification/de/CENTER.html" >}}


### Bewegung
{{< include-html "content/specification/de/GOTO.html" >}}


### Arbeitsebene
{{< include-html "content/specification/de/WORKPLANE.html" >}}

### Radiuskompensation
{{< include-html "content/specification/de/COMPENSATION.html" >}}

### Offset
{{< include-html "content/specification/de/OFFSET.html" >}}

---

## Werkzeuge
 ### Werkzeugaufruf
{{< include-html "content/specification/de/TOOL_CALL.html" >}}

 ### Werkzeugvorwahl
{{< include-html "content/specification/de/TOOL_SELECT.html" >}}

---

## Maschinenfunktionen
### Maschinenbefehle

{{< include-html "content/specification/de/MACHINE_FUNCTION.html" >}}
 

### Bearbeitungszyklen

{{< include-html "content/specification/de/CYCLE.html" >}}

-----
## Bezugspunkt

### Nullpunkt
{{< include-html "content/specification/de/ORIGIN.html" >}}

### Nullpunktverschiebung
{{< include-html "content/specification/de/MATRIX.html" >}}

--------
### Vorschub
{{< include-html "content/specification/de/FEEDRATE.html" >}}

### Vorschubart
{{< include-html "content/specification/de/FEEDRATE_TYPE.html" >}}

----------

### Spindel
{{< include-html "content/specification/de/SPINDLE.html" >}}

### Drehzahl
{{< include-html "content/specification/de/RPM.html" >}}
