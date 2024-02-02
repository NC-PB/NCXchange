+++
title = "Definition"
weight = 1
+++

```bnf
<program>	::=	<block>+ <new-line> 
<new-line>  ::= "\n"
<block>		::=	<cell>+ 
<cell>		::=	"[" <content> "]"
<content>	::=	<function> "=" <target>
<function>	::=	<text> | <text>:<address>
<address>	::=	<text>
<target>	::=	<value> | <text>
<value>		::=	<text> | <decimal> | <integer>
<decimal>	::=	<integer> "." <integer>
<integer>	::=	<digit>+
<digit>		::=	"0" | "1" | "2" | "3" | "4" | "5" | "6" | "7" | "8" | "9"
<text>		::=	<characters>+
<character>	::=	'A' ... 'Z' | '_'
```

- `<program>`: Ein Programm besteht aus einer oder mehreren Blöcken.
- `<block>`: Ein Block ist eine Sammlung einer oder mehrerer Zellen.
- `<cell>`: Eine Zelle ist die grundlegende Einheit eines Programms. Jede Zelle besteht aus einem Inhalt, der in eckigen Klammern [...] eingeschlossen ist.
- `<content>`: Der Inhalt einer Zelle setzt sich aus einer Funktion und einem Ziel zusammen, ge-trennt durch ein Gleichheitszeichen =.
- `<function>`: Die Funktion gibt an, welche Aktion in der Zelle ausgeführt wird. Eine Funktion kann entweder aus einem Text oder aus einem Text gefolgt von einem Doppelpunkt : und einer Adresse bestehen.
- `<address>`: Die Adresse ist optional und wird nur verwendet, wenn die Funktion sie benötigt. Sie besteht aus Text.
- `<target>`: Das Ziel gibt an, auf welches Element oder auf welche Daten die Funktion angewendet wird. Das Ziel kann entweder ein Wert (value) oder Text sein.
- `<value>`: Ein Wert kann Text, eine Dezimalzahl oder eine Ganzzahl sein.
- `<decimal>`: Eine Dezimalzahl besteht aus einem Ganzzahlteil und einem Dezimalteil, die durch einen Punkt . getrennt wird.
- `<integer>`: Eine Ganzzahl ist eine positive oder negative ganze Zahl ohne Dezimalstellen.
- `<text>`: Text ist eine Abfolge von Zeichen, die aus Buchstaben (Gross- oder Kleinbuchstaben) bestehen kann.
- `<characters>`: Die Zeichenkette <characters> steht für eine Abfolge von einem oder mehr Zei-chen.
- `<character>`: Ein einzelnes Zeichen kann ein Grossbuchstabe oder ein ‘_’ sein. 


