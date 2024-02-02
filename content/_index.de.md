+++
title = "NCXchange"
+++

{{< mermaid align="center" zoom="false" >}}
graph TB;
    id1([NC-Code Heidenhain]) --> id2[Konverter]
    id4([NC-Code Fanuc]) --> id2
    id5([NC-Code Siemens]) --> id2
    id6([NC-Code ...]) --> id2
    id2 --> id3[/NCX Format/]
{{< /mermaid >}}

NCXchange repräsentiert ein herstellerunabhängiges Format zur Darstellung von NC-Code, das als universelles Ausgabeformat konzipiert ist. Dies ermöglicht die Konvertierung in die Formate verschiedener Steuerungssysteme, den Aufbau von Analysefunktionen sowie die Integration und Nutzung in weiterführende Softwareapplikationen.

 Das Entwicklungsprojekt befindet sich noch in der Durchführungsphase und erfährt eine kontinuierliche Weiterentwicklung. Interessenten, die sich hinsichtlich der Spezifikationen beteiligen oder Diskussionen beisteuern möchten, sind herzlich eingeladen, dies über die Projektseite auf GitHub zu tun.

{{< mermaid align="center" zoom="false" >}}
graph TB;
    id3([NCX Format]) --> id2[Konverter]
    id2 --> id4([NC-Code Fanuc])
    id2 -->  id5([NC-Code Siemens]) 
    id2 --> id1([NC-Code Heidenhain])
    id2 --> id6([NC-Code ...])
{{< /mermaid >}}
