# Meta Characters

[R Vocab Topics](index) &#187; [Character Strings](characters) &#187; [Regular Expressions](regex) &#187; [Regex Syntax](regex_syntax) &#187; Meta characters

Metacharacters consist of non-alphanumeric symbols such as: 

<center> . &nbsp;&nbsp; \\\ &nbsp;&nbsp; | &nbsp;&nbsp; ( &nbsp;&nbsp; ) &nbsp;&nbsp; [ &nbsp;&nbsp; { &nbsp;&nbsp; $ &nbsp;&nbsp; * &nbsp;&nbsp; + &nbsp;&nbsp;? </center>

To match metacharacters in R you need to escape them with a double backslash "\\\\".  The following displays the general escape syntax for the most common metacharacters:


<center>
<img src="images/metacharacter_escape.png" alt="Escaping Metacharacters">
</center>     

<br>

The following provides examples to show how to use the escape syntax to find and replace metacharacters:

```r

sub(pattern = "\\$", "\\!", "I love R$")
## [1] "I love R!"

sub(pattern = "\\^", "carrot", "My daughter has a ^ with almost every meal!")
## [1] "My daughter has a carrot with almost every meal!"

gsub(pattern = "\\\\", " ", "I\\need\\space")
## [1] "I need space"
```
