# Keywords

Keywords are builtin language features that come with IndicaScript.

All keywords are reserved, and thus cannot be used as variable or input names.

## input

You can use the `input` keyword to signal a variable that the user has control over. For example:

```
input length = 14
input buyValue = 0.5
```

This creates two inputs, `length` and `buyValue`, giving them default values of 14 and 0.5, respectively (default values are required).

In ThinkOrSwim, inputs can be changed by the user without having to interact with the code, useful for dealing with variables that need to change often.

You can also chain inputs together, like so:

```
input length = 14, buyValue = 0.5
```

In your code, you can use inputs wherever you please.

## plot

`plot` is used to plot values returned by functions.

Take this code:

```
smaValue = SMA(close, 14)
wmaValue = WMA(close, 14)

plot smaValue with color green
plot wmaValue with color blue
```

`plot` expects a variable that can be plotted, along with a color code that can be `red`, `green`, `blue`, `yellow`, `purple`, `orange`, `black`, or `white`.
