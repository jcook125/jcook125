## Jack Cook
### MA Student, American University

I'm currently studying R programming language in American University's Global Governance, Politics, and Security graduate program. This page will serve as a portfolio of my data analytic work.

### Skills


- Software
  - `R/RStudio`
  - Advanced Excel
  
  
- Statistical Skills
  - Regression Analysis
  - Inference
  
  
- Other Data Knowledge
  - Mapping 
  - `ggplot` visualizations


### Programming Examples 

Here's some code I wrote in `R`:

```
# Summary Table Function

sumtable = function(.data, x){
  x = enquo(x)
  t(summarize(.data,
            min = min(!!x, na.rm=T),
            mean = mean(!!x, na.rm=T),
            med = median(!!x, na.rm=T),
            max = max(!!x, na.rm=T),
            'NA' = sum(is.na(!!x)))) %>%
    knitr::kable(digits = 1L) %>%
    kableExtra::kable_styling("striped", font_size = 10)
}
```
