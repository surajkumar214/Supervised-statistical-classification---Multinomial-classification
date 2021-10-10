Supervised statistical classification-Multinomial
================
Suraj Kumar
15/09/2021

<table style="width: auto;" class="table table-condensed">
<caption>
Data summary
</caption>
<thead>
<tr>
<th style="text-align:left;">
</th>
<th style="text-align:left;">
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
Name
</td>
<td style="text-align:left;">
ablone
</td>
</tr>
<tr>
<td style="text-align:left;">
Number of rows
</td>
<td style="text-align:left;">
4177
</td>
</tr>
<tr>
<td style="text-align:left;">
Number of columns
</td>
<td style="text-align:left;">
9
</td>
</tr>
<tr>
<td style="text-align:left;">
\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
Column type frequency:
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
factor
</td>
<td style="text-align:left;">
2
</td>
</tr>
<tr>
<td style="text-align:left;">
numeric
</td>
<td style="text-align:left;">
7
</td>
</tr>
<tr>
<td style="text-align:left;">
\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_
</td>
<td style="text-align:left;">
</td>
</tr>
<tr>
<td style="text-align:left;">
Group variables
</td>
<td style="text-align:left;">
None
</td>
</tr>
</tbody>
</table>

**Variable type: factor**

<table>
<thead>
<tr>
<th style="text-align:left;">
skim\_variable
</th>
<th style="text-align:right;">
n\_missing
</th>
<th style="text-align:right;">
complete\_rate
</th>
<th style="text-align:left;">
ordered
</th>
<th style="text-align:right;">
n\_unique
</th>
<th style="text-align:left;">
top\_counts
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
sex
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:left;">
FALSE
</td>
<td style="text-align:right;">
3
</td>
<td style="text-align:left;">
M: 1528, I: 1342, F: 1307
</td>
</tr>
<tr>
<td style="text-align:left;">
rings
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:left;">
FALSE
</td>
<td style="text-align:right;">
28
</td>
<td style="text-align:left;">
9: 689, 10: 634, 8: 568, 11: 487
</td>
</tr>
</tbody>
</table>

**Variable type: numeric**

<table>
<thead>
<tr>
<th style="text-align:left;">
skim\_variable
</th>
<th style="text-align:right;">
n\_missing
</th>
<th style="text-align:right;">
complete\_rate
</th>
<th style="text-align:right;">
mean
</th>
<th style="text-align:right;">
sd
</th>
<th style="text-align:right;">
p0
</th>
<th style="text-align:right;">
p25
</th>
<th style="text-align:right;">
p50
</th>
<th style="text-align:right;">
p75
</th>
<th style="text-align:right;">
p100
</th>
<th style="text-align:left;">
hist
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
length
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.52
</td>
<td style="text-align:right;">
0.12
</td>
<td style="text-align:right;">
0.07
</td>
<td style="text-align:right;">
0.45
</td>
<td style="text-align:right;">
0.54
</td>
<td style="text-align:right;">
0.62
</td>
<td style="text-align:right;">
0.81
</td>
<td style="text-align:left;">
▁▂▅▇▂
</td>
</tr>
<tr>
<td style="text-align:left;">
diameter
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.41
</td>
<td style="text-align:right;">
0.10
</td>
<td style="text-align:right;">
0.06
</td>
<td style="text-align:right;">
0.35
</td>
<td style="text-align:right;">
0.42
</td>
<td style="text-align:right;">
0.48
</td>
<td style="text-align:right;">
0.65
</td>
<td style="text-align:left;">
▁▂▆▇▁
</td>
</tr>
<tr>
<td style="text-align:left;">
height
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.14
</td>
<td style="text-align:right;">
0.04
</td>
<td style="text-align:right;">
0.00
</td>
<td style="text-align:right;">
0.12
</td>
<td style="text-align:right;">
0.14
</td>
<td style="text-align:right;">
0.16
</td>
<td style="text-align:right;">
1.13
</td>
<td style="text-align:left;">
▇▁▁▁▁
</td>
</tr>
<tr>
<td style="text-align:left;">
whole.weight
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.83
</td>
<td style="text-align:right;">
0.49
</td>
<td style="text-align:right;">
0.00
</td>
<td style="text-align:right;">
0.44
</td>
<td style="text-align:right;">
0.80
</td>
<td style="text-align:right;">
1.15
</td>
<td style="text-align:right;">
2.83
</td>
<td style="text-align:left;">
▇▇▅▁▁
</td>
</tr>
<tr>
<td style="text-align:left;">
shucked.weight
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.36
</td>
<td style="text-align:right;">
0.22
</td>
<td style="text-align:right;">
0.00
</td>
<td style="text-align:right;">
0.19
</td>
<td style="text-align:right;">
0.34
</td>
<td style="text-align:right;">
0.50
</td>
<td style="text-align:right;">
1.49
</td>
<td style="text-align:left;">
▇▇▂▁▁
</td>
</tr>
<tr>
<td style="text-align:left;">
viscera.weight
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.18
</td>
<td style="text-align:right;">
0.11
</td>
<td style="text-align:right;">
0.00
</td>
<td style="text-align:right;">
0.09
</td>
<td style="text-align:right;">
0.17
</td>
<td style="text-align:right;">
0.25
</td>
<td style="text-align:right;">
0.76
</td>
<td style="text-align:left;">
▇▇▂▁▁
</td>
</tr>
<tr>
<td style="text-align:left;">
shell.weight
</td>
<td style="text-align:right;">
0
</td>
<td style="text-align:right;">
1
</td>
<td style="text-align:right;">
0.24
</td>
<td style="text-align:right;">
0.14
</td>
<td style="text-align:right;">
0.00
</td>
<td style="text-align:right;">
0.13
</td>
<td style="text-align:right;">
0.23
</td>
<td style="text-align:right;">
0.33
</td>
<td style="text-align:right;">
1.00
</td>
<td style="text-align:left;">
▇▇▂▁▁
</td>
</tr>
</tbody>
</table>

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-1.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-2.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-3.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-4.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-5.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-6.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-7.png)<!-- -->

    ## $x
    ## [1] "ablone rings"
    ## 
    ## $y
    ## [1] "length"
    ## 
    ## $title
    ## [1] "Boxplot of ablone length vs rings"
    ## 
    ## attr(,"class")
    ## [1] "labels"

<table class="table" style="margin-left: auto; margin-right: auto;">
<caption>
</caption>
<thead>
<tr>
<th style="text-align:left;">
sex
</th>
<th style="text-align:right;">
n
</th>
</tr>
</thead>
<tbody>
<tr>
<td style="text-align:left;">
F
</td>
<td style="text-align:right;">
1307
</td>
</tr>
<tr>
<td style="text-align:left;">
I
</td>
<td style="text-align:right;">
1342
</td>
</tr>
<tr>
<td style="text-align:left;">
M
</td>
<td style="text-align:right;">
1528
</td>
</tr>
</tbody>
</table>

![](classification_files/figure-gfm/Exploratory%20analysis%20ablone-8.png)<!-- -->
