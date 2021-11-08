# Steve's Stock Analysis

## Overview of Project (Background)

Steve needed my help conducting analysis on a few stocks, so I developed a tool for him to quickly calculate the daily volume of those stocks for 2017 and 2018, along with their overall returns. This was yesterday. Now he wants to expand the dataset to include data for the entire stock market...and for years prior to 2017. I should've seen that coming. I needed to refactor the initial code for the calculator to run faster and more efficiently.

### Purpose

Steve will continue to use this tool to quickly calculate volume and return figures for any subset of stocks in the market for however many years of data he's able to provide.

## Results

The refactored code runs approximately five times as fast now.

### Ticker Index

I created and included a ticker index to access the appropriate indices associated with volume and price data for each identified ticker. This helped reduce the run time of the macro.

The addition of the following code resulted in faster runtimes as indicated by the images further below.

<img width="259" alt="Pre_Ticker_Index" src="https://user-images.githubusercontent.com/92264929/140678777-8023dc64-38b1-43bd-818e-5fc3cd413c09.png">

RUN TIMES BEFORE ADDITION OF TICKER INDEX

2017 <img width="219" alt="Pre_Ticker_2017" src="https://user-images.githubusercontent.com/92264929/140679540-2a37c17d-093d-4aae-8b77-a97d484bbe83.png">

2018 <img width="236" alt="Pre_Ticker_2018" src="https://user-images.githubusercontent.com/92264929/140679557-241f4a70-1226-4cc1-9095-ef60dd4590cf.png">


RUN TIMES AFTER ADDITION OF TICKER INDEX

2017
<img width="234" alt="VBA_Challenge_2017" src="https://user-images.githubusercontent.com/92264929/140678876-2001b8e6-a7f1-44d4-9af3-38202a032f3d.png">

2018
<img width="234" alt="VBA_Challenge_2018" src="https://user-images.githubusercontent.com/92264929/140678894-51165d73-4a90-40ca-8ca4-6c0dda125e80.png">

### 2017 vs 2018

Overall, the twelve stocks had significantly greater return percentages in 2017 than they did in 2018. 40% of the listed stocks reported higher daily volumes in 2017, while around 60% of the stocks performed better in 2018.

2017

<img width="211" alt="All_Stocks_2017" src="https://user-images.githubusercontent.com/92264929/140680414-567af693-0549-4b04-aead-d0cb089b257b.png">

2018

<img width="210" alt="All_Stocks_2018" src="https://user-images.githubusercontent.com/92264929/140680436-60f459f4-83da-4108-b3a6-60ab80151ade.png">

### Formatting

The refactored code includes an automatic highlighting function on return amounts for Steve to quickly identify those stocks who gained (highlighted in green) vs those who had negative return values (highlighted in red). The return values are now also in percentage form, and the volume figures include commas for easier reading. The headers have been boldened and the header row defined with an outline.

PRE REFACTOR

<img width="259" alt="Pre_Formatted" src="https://user-images.githubusercontent.com/92264929/140682204-b633feaa-2fb0-4d0c-a1fe-4d0f97fe4f93.png">

POST REFACTOR

<img width="258" alt="Post_Formatted" src="https://user-images.githubusercontent.com/92264929/140682531-c7207529-c1f5-462b-b7e1-e013d6ccc481.png">

My additional formatting code:

<img width="384" alt="Formatting_Code" src="https://user-images.githubusercontent.com/92264929/140682709-52a5a24b-a7d9-4db8-8fed-85a2538e148a.png">

## Summary

### Pros and Cons

There are advantages and disadvantages to refactoring code. On one hand, "if it ain't broke, don't fix it." If existing code works, refactoring introduces the possibility of ruining the code. However, a developer that continually saves and commits versions of the code will be able to use former versions in the event s/he becomes stumped by a new error.

The advantages outweigh the disadvantages, though. Successfully refactored code runs more efficiently, improves upon the readability of the application (and hopefully, the code) and runs quicker. 

In my case, compared to the original VBA script, there were only advantages to refactoring my code. I wasn't prohibited from any actions or capabilities after refactoring, and the process improved the run time of the calculator as well as the overall ease of use.



