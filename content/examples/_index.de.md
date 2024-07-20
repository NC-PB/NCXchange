+++
title = "Beispiele"
weight = 3
+++


## Fanuc
### Kreise und Kreisbogen

<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Kreis mit Mittelpunkt im Uhrzeigersinn</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="column2">Ausgang</td>
            <td>G2 X20 Y20 I10 J10</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[INTERPO=ARC,CW,CENTER][GOTO:X=20][GOTO:Y=20][CENTER:X=10][CENTER:Y=10]</td>
        </tr>
    </tbody>
</table>



<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Kreis mit Mittelpunkt im Gegenuhrzeigersinn</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="column2">Ausgang</td>
            <td>G3 X20 Y20 I10 J10</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[INTERPO=ARC,CCW,CENTER][GOTO:X=20][GOTO:Y=20][CENTER:X=10][CENTER:Y=10]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Kreis mit Radius im Uhrzeigersinn</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td class="column2">Ausgang</td>
            <td>G2 X20 Y20 R10</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[INTERPO=ARC,CW,CENTER][GOTO:X=20][GOTO:Y=20][RADIUS=10]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Kreis mit Radius im Gegenuhrzeigersinn</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G3 X20 Y20 R10</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[INTERPO=ARC,CCW,CENTER][GOTO:X=20][GOTO:Y=20][RADIUS=10]</td>
        </tr>
    </tbody>
</table>



### Bearbeitungszyklen

<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Bohren</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G81 Z-21.732 F565</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=DRILL][GOTO:Z=-21.732][FEEDRATE=565]</td>
        </tr>
    </tbody>
</table>



<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Bohren mit Verweilzeit</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G82 Z-21.732 P0.5 F565</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=DRILL,DELAY][GOTO:Z=-21.732][CYCLE_DELAY=0.5][FEEDRATE=565]</td>
        </tr>
    </tbody>
</table>



<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Tieflochbohren</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G83 Z-21.732 R5. Q1.2</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=DRILL,DEEP_HOLE][GOTO:Z=-21.732][CYCLE_SURFACE_ALTITUDE=5][CYCLE_DEPTH_INCREMENT=1.2]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Gewindebohren</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G84 Z-20. F750</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=TAP][GOTO:Z=-21.732][FEEDRATE=750]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Reiben</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G85 Z-20. F420</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=REAM][GOTO:Z=-20][FEEDRATE=420]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Zyklus halt</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G80</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[CYCLE=STOP]</td>
        </tr>
    </tbody>
</table>

### Längen und Radiuskompensation


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Längenkompensation</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G43 Z5. H1</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[GOTO:Z=5][OFFSET:LEN=1]</td>
        </tr>
    </tbody>
</table>


<table id="myTable">
    <thead>
        <tr>
            <th class="column2">Typ</th>
            <th>Radiuskompensation Links</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Ausgang</td>
            <td>G41 Y2. D1</td>
        </tr>
        <tr>
            <td>Ziel</td>
            <td>[COMPENSATION=LEFT][GOTO:Z=5][OFFSET:DIAM=1]</td>
        </tr>
    </tbody>
</table>

## Heidenhain
