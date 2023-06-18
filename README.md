# ARIMA Time Series Forecasting - Python to R

Created by Rafal K and Marcin Z.

This project is a reproduction and hopefully an extension of ARIMA Time Series Forecasting - S&P 500 Stock by Yassine Sfaihi.The aim of the research is to verify whether the S&P 500 market price can be accurately forecasted using conventional time series analysis tools.In the extension of the project, the ARIMA model will be compared with a much more advanced machine learning technique - the LSTM neural network.

# How to reproduce

The `/output` directory contains prerendered output files for your convenience. However, if you want, you can render them yourself.

How to reproduce:

1.  Install dependencies:

    1.1 Install tinytex (for pdf renders)

    ```         
      quarto install tinytex
    ```

    1.2 Install required R libraries:

    ```{r}
    install.packages("xts")
    install.packages("foreach")
    install.packages("doParallel")
    install.packages("cowplot")
    install.packages("readr")
    install.packages("ggplot2")
    install.packages("quantmod")
    install.packages("tseries")
    install.packages("forecast")
    install.packages("gridExtra")
    install.packages("keras")
    install.packages("Metrics")
    install.packages("stats")
    ```

    1.3 Install tensorflow via pip (requires python and pip installed). Run the following command in your terminal:

    ```         
    pip install tensorflow
    ```

2.  Clone the repository:

```         
  git clone https://github.com/Sosik1/RR2023_project.git
```

3.  Set working directory and run quarto_render in R console:

```         
  setwd("[...your path]/RR2023_project") # Enter your working directory here
  quarto_render("/ARIMA_Time_Series_Forcasting_Python_to_R.qmd") # render the files
```

# Acknowledgements

This project is part of a university course called Reproducible Research led by Wojciech Hardy at the University of Warsaw. AI models GPT-3.5 and GPT-4 have been used to generate parts of the code and help with debugging. Exact prompts can be found in `misc/prompts.txt`.

# References

[Sfaihi Y. (2023), ARIMA Time Series Forecasting - S&P 500 Stock](https://www.kaggle.com/code/yassinesfaihi/arima-time-series-forecasting-s-p-500-stock)
