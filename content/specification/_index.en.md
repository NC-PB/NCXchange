+++
title = "Spezification"
weight = 2
+++

### Programm

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Keyword</td>
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
    <td rowspan="4">Values</td>
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
    <td rowspan="3">Example</td>
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
    <td class="column1">Keyword</td>
    <td><b>INTERPO</B></td>
  </tr>
  <tr>
    <td rowspan="6">Values</td>
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
    <td>Example</td>
    <td>INTERPO=ARC,CCW</td>
  </tr>
</tbody>
</table>

### Arc center

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Keyword</td>
    <td>CENTER</td>
  </tr>
  <tr>
    <td>Adresse</td>
    <td>Axis</td>
  </tr>
  <tr>
    <td>Wert</td>
    <td>Position</td>
  </tr>
    <tr>
    <td>Example</td>
    <td>CENTER:X=20</td>
  </tr>
</tbody>
</table>

### Movement

<table id="myTable">
<tbody>
  <tr>
    <td class="column1">Keyword</td>
    <td>GOTO</td>
</tr>
<tr>
    <td>Adresse</td>
    <td>Axis</td>
  </tr>
  <tr>
    <td>Value</td>
    <td>Position</td>
  </tr>
<tr>
    <td>Example</td>
    <td>GOTO:X=-22-543</td>
  </tr>
</tbody>
</table>

### Workplane

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>WORKPLANE</td>
    </tr>
      <tr>
        <td rowspan="3">Values</td>
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


### Radius compensation

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>COMPENSATION</td>
    </tr>
    <tr>
        <td rowspan="3">Values</td>
        <td>LEFT</td>
    </tr>
    <tr>
        <td>RIGHT</td>
    </tr>
    <tr>
        <td>OFF</td>
    </tr>
  <tr>
    <td>Example</td>
    <td>COMPENSATOIN=OFF</td>
  </tr>
    </tbody>
</table>


### Offset

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>OFFSET</td>
    </tr>
  <tr>
    <td>Wert</td>
    <td>Offset number</td>
  </tr>
    <tr>
        <td rowspan="2">Address</td>
        <td>LEN</td>
    </tr>
     <tr>
        <td>DIAM</td>
    </tr>
    <tr>
        <td>Example</td>
        <td>OFFSET:LEN=10</td>
    </tr>
    </tbody>
</table>


 ### Tool call

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>TOOL_CALL</td>
    </tr>
    <tr>
        <td>Parameter</td>
        <td>Tool number</td>
    </tr>
    <tr>
        <td>Example</td>
        <td>TOOL_CALL=12</td>
    </tr>
    </tbody>
</table>


### Spindle speed

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>RPM</td>
    </tr>
  <tr>
    <td>Example</td>
    <td>RPM=1200</td>
  </tr>
    </tbody>
</table>


### Machine functions

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>FUNCTION_MACHINE</td>
    </tr>
    <tr>
        <td>Value</td>
        <td>M-Code number</td>
    </tr>
    <tr>
        <td>Example</td>
        <td>FUNCTION_MACHINE=56</td>
    </tr>
    </tbody>
</table>



### Comment

<table id="myTable">
    <tbody>
        <tr>
            <td class="column1">Keyword</td>
            <td>COMM</td>
        </tr>
        <tr>
            <td>Example</td>
            <td>COMM=PLANFRAESEN</td>
        </tr>
    </tbody>
</table>


### Cycle

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td colspan="2">CYCLE</td>
    </tr>
    <tr>
        <td rowspan="6">Values</td>
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
        <td class="column1">Example</td>
        <td colspan="2">CYCLE=DRILL,DEEP_HOLE</td>
    </tbody>
</table>


### Origin

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>ORIGIN</td>
    </tr>
    <tr>
        <td>Wert</td>
        <td>Nullpunknummer</td>
    </tr>
    <tr>
        <td>Example</td>
        <td>ORIGIN=1</td>
    </tr>
    </tbody>
</table>


### Feedrate

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td>FEEDRATE</td>
    </tr>
    <tr>
        <td>Value</td>
        <td>Feedrate</td>
    </tr>
    <tr>
        <td>Example</td>
        <td>FEEDRATE=200</td>
    </tr>
    </tbody>
</table>

### Feedrate type

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
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
        <td>Example</td>
        <td>FEEDRATE_TYPE=MIN</td>
    </tr>
    </tbody>
</table>

 ### Datum shift


<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td colspan="2">MATRIX</td>
    </tr>
    <tr>
        <td rowspan="3">Adresse</td>
        <td>Shift in X</td>
        <td>SHIFT_X</td>
    </tr>
    <tr>
        <td>Shift in Y</td>
        <td>SHIFT_Y</td>
    </tr>
    <tr>
        <td>Shift in Z</td>
        <td>SHIFT_Z</td>
    </tr>
    <tr>
        <td class="column1">Example</td>
        <td colspan="2">MATRIX:SHIFT_X=33.5</td>
    </tbody>
</table>


### Spindle

<table id="myTable">
    <tbody>
    <tr>
        <td class="column1">Keyword</td>
        <td colspan="2">SPINDLE</td>
    </tr>
    <tr>
        <td rowspan="3">Values</td>
        <td>On clockwise</td>
        <td>CW</td>
    </tr>
    <tr>
        <td>On counterclockwise </td>
        <td>CCW</td>
    </tr>
    <tr>
        <td>Off</td>
        <td>OFF</td>
    </tr>
        <tr>
        <td>Address</td>
        <td colspan="2">Spindle number</td>
    </tr> 
    <tr>
        <td>Example</td>
        <td colspan="2">SPINDLE:1=CCW</td>
    </tr>
    </tbody>
</table>
