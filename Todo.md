- separate data (maybe interface so every XY.. is a Data), same with Options and Datasets -> should enable more generic possibilities so the charts, datas, datasets - etc aren't linked as hard together as they're now
- (just maybe) create empty interfaces for chart types which also implement IChartType and then have lineAxis and LineTicks etc implement ILine. this would allow to have maybe a generic TChart (where : IChartType) for the config which could be ILine and all the Ticks, Options etc would automatically have to be for a line chart (also implement ILine)
- check the summaries of the axis when Data etc are separated
- namespaces
  - line stuff
  - axes
  - time stuff
- add remaining axes
- remake point styles
- add static DefaultFormat dict (https://www.chartjs.org/docs/latest/axes/cartesian/time.html#display-formats)
- add static de-ch dict (or find a way to generate/get it without manually specifying everything)
- find out how to set localization at startup of each site (moment.js)
- test everything (create and or use samples)
- Maybe restrict to https://www.chartjs.org/docs/latest/charts/line.html#data-structure 
  - This would mean only allowing the wrappers. In the Datasets instead of every class
- Find out if its a bad practise to use js to include the CSS (maybe so question)