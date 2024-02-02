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

- `<program>`: A program consists of one or more blocks.
- `<block>`: A block is a collection of one or more cells.
- `<cell>`: A cell is the basic unit of a program. Each cell consists of content enclosed in square brackets [...].
- `<content>`: The content of a cell is made up of a function and a target, separated by an equals sign =.
- `<function>`: The function specifies which action is performed in the cell. A function can either be text or text followed by a colon : and an address.
- `<address>`: The address is optional and is only used if the function requires it. It consists of text.
- `<target>`: The target specifies which element or data the function is applied to. The target can either be a value (value) or text.
- `<value>`: A value can be text, a decimal, or an integer.
- `<decimal>`: A decimal consists of an integer part and a decimal part, separated by a point .
- `<integer>`: An integer is a positive or negative whole number without decimal places.
- `<text>`: Text is a sequence of characters that can consist of letters (uppercase or lowercase).
- `<characters>`: The character string <characters> represents a sequence of one or more characters.
- `<character>`: A single character can be an uppercase letter or an ‘_’.