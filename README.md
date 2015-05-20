# simple-latex : Less latex more text
The little package that makes my relation with LaTeX nice.
(Just add simpltex.sty in your sources, and \usepackage{simpltex})
###Summary
* [Figures in one line](#fig)
* [List apparent](#li)
* [Quick table](#tab)
* [Sections an subsections](#s)
* [Frame in 4 characters](#f)

### Make figures in one line <a id="fig"></a>
```tex

\fig[otpional-graphics-properties]<optional-label>{picture}{title}

\fig<optional-label>{picture}{title}

\fig{picture}{title}
```
=============
### Make list faster and apparent <a id="li"></a>
```tex
\li{
    item 1;
    item 2;
    item 3
}
```
=============
### Split your text in table quick <a id="tab"></a>
Use:
```tex
\tab<optional-bottom-marge-after><optional-left-marge-before>[optional-tabular-arguments]{}
```
Examples:
```tex
tab{
    item 1 & item 2
    \row
    item 3 & item 4
}


% Two columns and 5mm space after

tab<5mm><0mm>{
    text for the left side
    &
    text for the right side
}


% Table with three rows and three columns of 4cm

tab[p{4cm} p{4cm} p{4cm}]{
    item 1 & item 2 & item 3
    \row
    item 4 & item 5 & item 6
    \row
    item 7 & item 8 & item 9
}
```
=============
### Section and subsection are now s and subs <a id="s"></a>
Rename section and redefine your one section style for all (l.41)
```tex
\s{title}
\subs{subtitle}
```
=============
### Frame is now f <a id="f"></a>
```tex
\f[title]{
    Text in my frame
}
```
