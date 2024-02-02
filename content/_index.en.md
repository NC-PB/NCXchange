+++
title = "NCXchange"
+++

{{< mermaid align="center" zoom="false" >}}
graph TB;
    id1([NC-Code Heidenhain]) --> id2[Converter]
    id4([NC-Code Fanuc]) --> id2
    id5([NC-Code Siemens]) --> id2
    id6([NC-Code ...]) --> id2
    id2 --> id3[/NCX Format/]
{{< /mermaid >}}

NCXchange represents a manufacturer-independent format for displaying NC code that is designed as a universal output format. This enables conversion into the formats of various control systems, the development of analysis functions and integration and use in further software applications.

 The development project is still in the implementation phase and is undergoing continuous further development. Anyone interested in contributing to the specifications or discussions is welcome to do so via the project page on GitHub.

 {{< mermaid align="center" zoom="false" >}}
graph TB;
    id3([NCX Format]) --> id2[Converter]
    id2 --> id4([NC-Code Fanuc])
    id2 -->  id5([NC-Code Siemens]) 
    id2 --> id1([NC-Code Heidenhain])
    id2 --> id6([NC-Code ...])
{{< /mermaid >}}
