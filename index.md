# Presentation with plotly
Bram van Dam  
July 25, 2017  

<style type="text/css">
body, td {
   font-size: 14px;
}
code.r{
  font-size: 10px;
}
pre {
  font-size: 14px
}
</style>



## Overview

This is an R Markdown presentation for the course "Developing data products", which is part of the Data science specialization on Coursera (https://www.coursera.org/specializations/jhu-data-science/).

The next three slides contain:  
- Some background of the plot  
- The plotly plot  
- The code for the plot  

From my own testing, the plot does show up correctly in Microsoft Edge or Internet Explorer; the plot is not evaluated well with Firefox. So please use another browser if the plot doesn't show up.

## Background of plot

A dataset which can be found in any R installation is used. See http://stat.ethz.ch/R-manual/R-patched/library/datasets/html/state.html for more background on the data set.

On the following slide, the life expectancy (in years) is plotted against income per capita and the percentage of high-school graduates. Markers are colored by the murder rate per 100,000 population.  

By no way is any connection suggested, it just shows what kind of plots can be made with the plotly package in R.

## Plotly plot

<!--html_preserve--><div id="a5c44073b95" style="width:720px;height:432px;" class="plotly html-widget"></div>
<script type="application/json" data-for="a5c44073b95">{"x":{"visdat":{"a5c26d92301":["function () ","plotlyVisDat"]},"cur_data":"a5c26d92301","attrs":{"a5c26d92301":{"x":{},"y":{},"z":{},"showlegend":false,"mode":"markers","marker":{"color":{},"colorscale":["#FFE1A1","#683531"],"showscale":true,"colorbar":{"x":0.8,"y":0.5,"yanchor":"middle","title":"Murder rate per<br /> 100,000 population"}},"alpha":1,"sizes":[10,100],"type":"scatter3d"}},"layout":{"margin":{"b":40,"l":60,"t":25,"r":10},"title":"Life expectancy to income and high-school graduation","scene":{"xaxis":{"title":"Income (per capita)"},"yaxis":{"title":"High-school Graduates (%)"},"zaxis":{"title":"Life expectancy (years)"}},"xaxis":{"domain":[0,1]},"yaxis":{"domain":[0,1]},"hovermode":"closest","showlegend":false},"source":"A","config":{"modeBarButtonsToAdd":[{"name":"Collaborate","icon":{"width":1000,"ascent":500,"descent":-50,"path":"M487 375c7-10 9-23 5-36l-79-259c-3-12-11-23-22-31-11-8-22-12-35-12l-263 0c-15 0-29 5-43 15-13 10-23 23-28 37-5 13-5 25-1 37 0 0 0 3 1 7 1 5 1 8 1 11 0 2 0 4-1 6 0 3-1 5-1 6 1 2 2 4 3 6 1 2 2 4 4 6 2 3 4 5 5 7 5 7 9 16 13 26 4 10 7 19 9 26 0 2 0 5 0 9-1 4-1 6 0 8 0 2 2 5 4 8 3 3 5 5 5 7 4 6 8 15 12 26 4 11 7 19 7 26 1 1 0 4 0 9-1 4-1 7 0 8 1 2 3 5 6 8 4 4 6 6 6 7 4 5 8 13 13 24 4 11 7 20 7 28 1 1 0 4 0 7-1 3-1 6-1 7 0 2 1 4 3 6 1 1 3 4 5 6 2 3 3 5 5 6 1 2 3 5 4 9 2 3 3 7 5 10 1 3 2 6 4 10 2 4 4 7 6 9 2 3 4 5 7 7 3 2 7 3 11 3 3 0 8 0 13-1l0-1c7 2 12 2 14 2l218 0c14 0 25-5 32-16 8-10 10-23 6-37l-79-259c-7-22-13-37-20-43-7-7-19-10-37-10l-248 0c-5 0-9-2-11-5-2-3-2-7 0-12 4-13 18-20 41-20l264 0c5 0 10 2 16 5 5 3 8 6 10 11l85 282c2 5 2 10 2 17 7-3 13-7 17-13z m-304 0c-1-3-1-5 0-7 1-1 3-2 6-2l174 0c2 0 4 1 7 2 2 2 4 4 5 7l6 18c0 3 0 5-1 7-1 1-3 2-6 2l-173 0c-3 0-5-1-8-2-2-2-4-4-4-7z m-24-73c-1-3-1-5 0-7 2-2 3-2 6-2l174 0c2 0 5 0 7 2 3 2 4 4 5 7l6 18c1 2 0 5-1 6-1 2-3 3-5 3l-174 0c-3 0-5-1-7-3-3-1-4-4-5-6z"},"click":"function(gd) { \n        // is this being viewed in RStudio?\n        if (location.search == '?viewer_pane=1') {\n          alert('To learn about plotly for collaboration, visit:\\n https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html');\n        } else {\n          window.open('https://cpsievert.github.io/plotly_book/plot-ly-for-collaboration.html', '_blank');\n        }\n      }"}],"cloud":false},"data":[{"x":[3624,6315,4530,3378,5114,4884,5348,4809,4815,4091,4963,4119,5107,4458,4628,4669,3712,3545,3694,5299,4755,4751,4675,3098,4254,4347,4508,5149,4281,5237,3601,4903,3875,5087,4561,3983,4660,4449,4558,3635,4167,3821,4188,4022,3907,4701,4864,3617,4468,4566],"y":[41.3,66.7,58.1,39.9,62.6,63.9,56,54.6,52.6,40.6,61.9,59.5,52.6,52.9,59,59.9,38.5,42.2,54.7,52.3,58.5,52.8,57.6,41,48.8,59.2,59.3,65.2,57.6,52.5,55.2,52.7,38.5,50.3,53.2,51.6,60,50.2,46.4,37.8,53.3,41.8,47.4,67.3,57.1,47.8,63.5,41.6,54.5,62.9],"z":[69.05,69.31,70.55,70.66,71.71,72.06,72.48,70.06,70.66,68.54,73.6,71.87,70.14,70.88,72.56,72.58,70.1,68.76,70.39,70.22,71.83,70.63,72.96,68.09,70.69,70.56,72.6,69.03,71.23,70.93,70.32,70.55,69.21,72.78,70.82,71.42,72.13,70.43,71.9,67.96,72.08,70.11,70.9,72.9,71.64,70.08,71.72,69.48,72.48,70.29],"showlegend":false,"mode":"markers","marker":{"fillcolor":"rgba(31,119,180,1)","color":[15.1,11.3,7.8,10.1,10.3,6.8,3.1,6.2,10.7,13.9,6.2,5.3,10.3,7.1,2.3,4.5,10.6,13.2,2.7,8.5,3.3,11.1,2.3,12.5,9.3,5,2.9,11.5,3.3,5.2,9.7,10.9,11.1,1.4,7.4,6.4,4.2,6.1,2.4,11.6,1.7,11,12.2,4.5,5.5,9.5,4.3,6.7,3,6.9],"colorscale":["#FFE1A1","#683531"],"showscale":true,"colorbar":{"x":0.8,"y":0.5,"yanchor":"middle","title":"Murder rate per<br /> 100,000 population"},"line":{"color":"transparent"}},"type":"scatter3d","frame":null}],"highlight":{"on":"plotly_click","persistent":false,"dynamic":false,"selectize":false,"opacityDim":0.2,"selected":{"opacity":1}},"base_url":"https://plot.ly"},"evals":["config.modeBarButtonsToAdd.0.click"],"jsHooks":{"render":[{"code":"function(el, x) { var ctConfig = crosstalk.var('plotlyCrosstalkOpts').set({\"on\":\"plotly_click\",\"persistent\":false,\"dynamic\":false,\"selectize\":false,\"opacityDim\":0.2,\"selected\":{\"opacity\":1}}); }","data":null}]}}</script><!--/html_preserve-->


## R Code for the plot


```r
library(plotly); library(datasets)
sdf <- as.data.frame(state.x77)

mstyle = list(color = ~`Murder`,
              colorscale = c('#FFE1A1', '#683531'),
              showscale = TRUE,
              colorbar = list(x = 0.8, y = 0.5, yanchor = "middle",
                              title = "Murder rate per\n 100,000 population"))
plot_ly(sdf, x = ~`Income`, y = ~`HS Grad`, z = ~`Life Exp`,
        type = "scatter3d",
        showlegend = FALSE,
        mode = "markers",
        marker = mstyle) %>%
    layout(title = "Life expectancy to income and high-school graduation",
           scene = list(xaxis = list(title = 'Income (per capita)'),
                        yaxis = list(title = 'High-school Graduates (%)'),
                        zaxis = list(title = 'Life expectancy (years)'))
           )
```
