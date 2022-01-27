Bellabeat Data Analysis Report
================
Carlos Olivella
1/20/2022

<style>
body {
text-align: justify}
</style>

# 1. INTRODUCTION

**Bellabeat** is a high-tech manufacturer of heath-focused products for
women that provide users with health data related to their activity,
sleep, stress, menstrual cycle, and mindfulness habits. The **marketing
analytics team** at Bellabeat has been assigned the task of analyzing
smart device fitness data to identify connections, themes, and patterns
and provide Bellabeat executive team with useful insights into how
consumers are using Bellabeat products and, in turn, help guide the
company’s marketing strategy to unlock new growth opportunities. As
such, this report will be divided into sections, each one corresponding
to a phase of the data analysis life cycle.

The first section will analyze how we can **Ask** smart questions and
use structured thinking to identify what we are looking for, what data
we will need, how we will obtain this data, and how we will analyze this
data. The second section will analyze how we can **Prepare** and collect
the required data from adequate and reliable sources. The third section
will focus on how we will **Process** the collected data and clean it to
avoid errors and bias in our analysis. The fourth section will center
around how we will **Analyze** the cleaned data and perform calculations
on it to identify connections, themes, and patterns that will help us
obtain new insights and leverage these to make meaningful change
throughout the company. It will also explain how we plan to **Share**
our findings with key stakeholders through presentations, reports, or
dashboards. Finally, the fifth section will focus on our recommendations
for how Bellabeat should **Act** on our findings to unlock new growth
opportunities.

This report will produce the following deliverables:

1.  A clear summary of the business task
2.  A description of all data sources used
3.  Documentation of any cleaning or manipulation of data
4.  A summary of our analysis
5.  Supporting visualizations and key findings
6.  Our top high-level content recommendations based on our analysis

# 2. ASK Phase

In this section of our report, we will focus on summarizing the business
task that we plan to address with our analysis, the questions we plan to
resolve, and how we plan to consider key stakeholders.

A business task can be defined as *“the question or problem data
analysis resolves for a business”* (Google, n.d). In this case we have
been assigned the task of analyzing smart device usage data to identify
trend, connections, and patterns in consumer behavior regarding sleep,
activity, and body measurements. Our analysis will allow us to obtain
insights on smart device usage and help identify new growth
opportunities for Bellabeat through data-driven decision making.

To resolve these business tasks through data analysis, we must first
distill what we are trying to answer into specific questions. Some
general questions that we will use as guidelines for our analysis
throughout this report will be those proposed by Google (i.e., **What
are some trends in smart device usage?, how could these trends apply to
Bellabeat customers?**, and **how could these trends help influence
Bellabeat marketing strategy?**). However, we must also determine
specific questions that we intend to answer. On this matter, we will use
the SMART questions framework. This framework states that useful and
effective questions must be specific, measurable, action-oriented,
relevant, and time-bound. The following list includes the general
questions that we intend to answer throughout this report, an analysis
of the questions from the point of view of the SMART framework, and an
initial hypothesis on what the answers to the questions might be.

**1. How is smart device usage distributed among user types based on
their activity level?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify how users are using their
smart devices based on their activity levels.

**Measurable**: This question is measurable because it will provide us
with percentages of smart device usage across the sampled population.

**Action-Oriented**: The insights gained from resolving this question
will allow Bellabeat to identify which activity-level segments of the
population should be focused on, meaning that Bellabeat can target these
segments with tailored marketing strategies.

**Relevant**: This question is relevant because it relates to analyzing
consumer behavior and, specifically, smart device usage across activity
levels.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is that the majority of users are
physically active.

**2. How is smart device usage distributed between BMI (body mass index)
segments?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify what BMI segments are using
Bellabeat products more, and which age segments Bellabeat should focus
on attracting.

**Measurable**: This question is measurable because it will provide us
with percentages of smart device usage across the sampled population.

**Action-Oriented**: As stated above, the insights gained from resolving
this question will allow Bellabeat to identify which BMI segments of the
population should be focused on, meaning that Bellabeat can target these
segments with tailored marketing strategies.

**Relevant**: This question is relevant because it relates to analyzing
consumer behavior and, specifically, smart device usage across BMI
segments.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is that smart device usage is
concentrated in overweight individuals, meaning those individuals with a
BMI between 25.0 and 30.0, as defined by the Center for Disease Control
and Prevention (CDC, 2021).

**3. How do the total amount of steps or calories affect said user’s
average sleep state?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify how sleep is affected by
activity and caloric intake.

**Measurable**: This question is measurable because it will provide us
with a specific correlation between the two variables.

**Action-Oriented**: As stated above, the insights gained from resolving
this question will allow Bellabeat to communicate these findings to
their users in order to improve their sleep.

**Relevant**: This question is relevant because it relates to analyzing
consumer behavior and, specifically, the effect of activity and caloric
intake on sleep.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is there is a negative correlation
between the amount of steps/calories and sleep quality/state.

**4. How do daily steps and calories vary between weekdays and
weekends?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify how users behave during
different parts of the week.

**Measurable**: This question is measurable because it will provide us
with numeric differences between weekdays and weekends.

**Action-Oriented**: As stated above, the insights gained from resolving
this question will allow Bellabeat to identify how users behave in
different parts of the week, which can allow Bellabeat to inform their
users of their behavioral changes and how this might affect them.

**Relevant**: This question is relevant because it relates to analyzing
consumer behavior and, specifically, user behavior usage across time.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is that during weekdays users take more
steps but consume less calories due to the fact that human beings
usually maintain stricter and more predictable routines during weekdays,
whilst consumer behavior is more erratic and users rest more during
weekends.

**5. When are users more active throughout the day?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify how users behave during
different parts of the day.

**Measurable**: This question is measurable because it will provide us
with numeric differences between hours.

**Action-Oriented**: As stated above, the insights gained from resolving
this question will allow Bellabeat to identify how users behave in
different parts of the day, which can allow Bellabeat to inform their
users of their behavioral changes and how this might affect them.

**Relevant**: This question is relevant because it relates to analyzing
consumer behavior and, specifically, user behavior usage across time.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is that users are more active in the
morning.

**6. Do individuals that use their smart devices less often have higher
daily average steps during these uses?**

**Specific**: This question addresses the business tasks we are trying
to solve because it will help us identify if there is a concentration of
smart device usage during periods of exercise or high activity.

**Measurable**: This question is measurable because it will provide us
with numeric differences between usage types.

**Action-Oriented**: As stated above, the insights gained from resolving
this question will allow Bellabeat to identify if there is a
concentration of smart device usage during periods of exercise or high
activity. This could help the company tailor marketing strategies
emphasizing the usefulness of wearing smart devices every day.

**Relevant**: This question is relevant because it relates to analyzing
smart device usage across different types of users and activity levels.

**Time-Bound**: This question is time-bound given that it is limited to
the sampled time period.

**Hypothesis**: Our hypothesis is that users who wear their smart
devices less often usually have higher average daily steps, thus there
is a concentration of smart device usage during periods of exercise or
high activity.

We believe that these questions will allow us to obtain insights into
smart device usage and unlock new growth opportunities that will help
Bellabeat make meaningful changes in its marketing strategies to attract
new customers and improve the experience of current customers.

Another important aspect that we must consider throughout this analysis
is stakeholder integration. In this specific case, we must address three
distinct stakeholders: (i) Urška Sršen, Bellabeat’s cofounder and Chief
Creative Officer; (ii) Sando Mur, Mathematician, Bellabeat’s cofounder,
and key member of the Bellabeat executive team; and (iii) Bellabeat’s
marketing analytics team. As such, we must tailor our findings to the
specific needs of each of these stakeholders.

# 3. PREPARE Phase

This section of our report will focus on describing the data sources
that we plan to use in our analysis, how reliable they may be, as well
as the possibility of bias being a part of the data.

As is stated in the case study, Urška Sršen has directed us to the use
of the ‘Fitbit Fitness Tracker Data’ dataset. Below, we will identify
key elements of this dataset:

-   **Source**: This dataset has been retrieved from the following link
    on Kaggle: <https://www.kaggle.com/arashnic/fitbit>. However, the
    original source of the data can be found on the following link from
    Zenodo: <https://zenodo.org/record/53894#.YeW2exPMLPZ>. The original
    authors or creators are Furberg, Robert; Brinton, Julia; Keating,
    Michael; Ortiz, Alexa.

-   **Accessibility and Licensing**: This dataset can be accessed by
    anyone given that it is CC0: public domain. This means that *“a
    third party may copy, distribute, display/perform, sell, and create
    derivative works of the original creation. (…) Works committed to
    the public domain via CC0, do NOT require an attribution of any
    kind, any work in the public domain may be used without
    attribution”* (UNT, 2021).

-   **Anonymization**: The data set is anonymized, and no personally
    identifiable information is included. It is not possible to link
    this data to specific individuals, therefore no data privacy laws
    are infringed.

-   **Content**: This data set contains information from approximately
    30 eligible Fitbit users that consented to the submission of
    personal tracker data, including minute-level output for physical
    activity, heart rate, and sleep monitoring (Möbius, n.d.). It
    contains 18 tables with information on activity, calories,
    intensities, heart rate, sleep, and weight, often distributed by
    days, hours, and minutes.

-   **Limitations**: This dataset has several limitations that we must
    address:

    -   **Gender**: There is no mention of the gender of the individuals
        who consented to submit their personal information. As such, we
        cannot know, nor assume if the participants are all women or
        not. This is an important limitation for our analysis because
        Bellabeat’s products are created for use by women. This
        limitation can lead to bias within our data because we may be
        analyzing data on men, which can be significantly different to
        that of women.

    -   **Age**: There is also no mention of the age of the
        participants. This means that it is possible that we may be
        analyzing data of only a specific age segment of the population,
        which would not represent the entire population and, in turn,
        would make it impossible to give recommendations to Bellabeat
        based on age.

    -   **Location**: There is no mention of the time zone or location
        in which this data was collected. This could lead to bias on the
        basis of location-specific differences in anatomy, fitness
        levels, race, ethnicity, among others.

    -   **ROCCC**: As we can see above, this dataset has certain
        limitations. Given that the data is generated by Fitbit, we can
        argue that it is reliable and is validated from the original
        source. As for how comprehensive the data is, we have seen that
        there is no information on gender, age, or location of the
        participants. Therefore, we cannot say that it is comprehensive
        as it does not include all the information we require to answer
        our questions. The dataset is also not current because the
        collected data is from the year 2016. Finally, in terms of the
        dataset being cited, it is of the public domain, therefore no
        attribution is required as explained previously.

Unfortunately, it was not possible to find other datasets on smart
health device usage due to the fact that companies do not usually make
this information public, nor have the obligation to do so. For this
reason, we must carry out our analysis with the provided dataset, always
taking into account its limitations and biases.

# 4. PROCESS Phase

To process the data for subsequent analysis, we will use RStudio.
Microsoft Excel or Google Cloud Big Query could have been used instead,
but, for the purposes of this, project RStudio provides the necessary
tools in a single platform, especially considering the amount of data
included in some of the CSV files.

## 4.1 Installing packages and opening libraries

During this data analysis project we will used the following packages
within RStudio:

-   tidyverse
-   skimr
-   janitor
-   lubridate
-   ggpubr
-   ggrepel

``` r
library(tidyverse)
```

    ## ── Attaching packages ─────────────────────────────────────── tidyverse 1.3.1 ──

    ## ✓ ggplot2 3.3.5     ✓ purrr   0.3.4
    ## ✓ tibble  3.1.4     ✓ dplyr   1.0.7
    ## ✓ tidyr   1.1.4     ✓ stringr 1.4.0
    ## ✓ readr   2.0.1     ✓ forcats 0.5.1

    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
library(skimr)
library(janitor)
```

    ## 
    ## Attaching package: 'janitor'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     chisq.test, fisher.test

``` r
library(lubridate)
```

    ## 
    ## Attaching package: 'lubridate'

    ## The following objects are masked from 'package:base':
    ## 
    ##     date, intersect, setdiff, union

``` r
library(ggpubr)
library(ggrepel)
```

## 4.2 Importing the datasets

The dataset we have been directed to contains 18 CSV files. However, we
will not used all of them in our analysis. As such, we will only import
the following files:

-   activity_daily
-   heartrate_seconds
-   sleep_daily
-   sleep_minutes
-   steps_hourly
-   weight_logs

``` r
setwd("/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import")
activity_daily <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/activity_daily.csv")
```

    ## Rows: 940 Columns: 15

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr  (1): ActivityDate
    ## dbl (14): Id, TotalSteps, TotalDistance, TrackerDistance, LoggedActivitiesDi...

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
heartrate_seconds <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/heartrate_seconds.csv")
```

    ## Rows: 2483658 Columns: 3

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (1): Time
    ## dbl (2): Id, Value

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
sleep_daily <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/sleep_daily.csv")
```

    ## Rows: 413 Columns: 5

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (1): SleepDay
    ## dbl (4): Id, TotalSleepRecords, TotalMinutesAsleep, TotalTimeInBed

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
sleep_minutes <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/sleep_minutes.csv")
```

    ## Rows: 188521 Columns: 4

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (1): date
    ## dbl (3): Id, value, logId

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
steps_hourly <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/steps_hourly.csv")
```

    ## Rows: 22099 Columns: 3

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (1): ActivityHour
    ## dbl (2): Id, StepTotal

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

``` r
weight_logs <- read_csv(file= "/Users/carlosolivella/Library/Mobile Documents/com~apple~CloudDocs/MASY/Fall 2021/Google Certificate - Data Analyst/Capstone Project/FitBit Data/To import/weight_logs.csv")
```

    ## Rows: 67 Columns: 8

    ## ── Column specification ────────────────────────────────────────────────────────
    ## Delimiter: ","
    ## chr (1): Date
    ## dbl (6): Id, WeightKg, WeightPounds, Fat, BMI, LogId
    ## lgl (1): IsManualReport

    ## 
    ## ℹ Use `spec()` to retrieve the full column specification for this data.
    ## ℹ Specify the column types or set `show_col_types = FALSE` to quiet this message.

## 4.3 Previewing the data

Now that we have imported the files, we will preview the data and its
structure.

``` r
as_tibble(activity_daily)
```

    ## # A tibble: 940 × 15
    ##            Id ActivityDate TotalSteps TotalDistance TrackerDistance LoggedActivitie…
    ##         <dbl> <chr>             <dbl>         <dbl>           <dbl>            <dbl>
    ##  1 1503960366 4/12/2016         13162          8.5             8.5                 0
    ##  2 1503960366 4/13/2016         10735          6.97            6.97                0
    ##  3 1503960366 4/14/2016         10460          6.74            6.74                0
    ##  4 1503960366 4/15/2016          9762          6.28            6.28                0
    ##  5 1503960366 4/16/2016         12669          8.16            8.16                0
    ##  6 1503960366 4/17/2016          9705          6.48            6.48                0
    ##  7 1503960366 4/18/2016         13019          8.59            8.59                0
    ##  8 1503960366 4/19/2016         15506          9.88            9.88                0
    ##  9 1503960366 4/20/2016         10544          6.68            6.68                0
    ## 10 1503960366 4/21/2016          9819          6.34            6.34                0
    ## # … with 930 more rows, and 9 more variables: VeryActiveDistance <dbl>,
    ## #   ModeratelyActiveDistance <dbl>, LightActiveDistance <dbl>,
    ## #   SedentaryActiveDistance <dbl>, VeryActiveMinutes <dbl>,
    ## #   FairlyActiveMinutes <dbl>, LightlyActiveMinutes <dbl>,
    ## #   SedentaryMinutes <dbl>, Calories <dbl>

``` r
str(activity_daily)
```

    ## spec_tbl_df [940 × 15] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id                      : num [1:940] 1.5e+09 1.5e+09 1.5e+09 1.5e+09 1.5e+09 ...
    ##  $ ActivityDate            : chr [1:940] "4/12/2016" "4/13/2016" "4/14/2016" "4/15/2016" ...
    ##  $ TotalSteps              : num [1:940] 13162 10735 10460 9762 12669 ...
    ##  $ TotalDistance           : num [1:940] 8.5 6.97 6.74 6.28 8.16 ...
    ##  $ TrackerDistance         : num [1:940] 8.5 6.97 6.74 6.28 8.16 ...
    ##  $ LoggedActivitiesDistance: num [1:940] 0 0 0 0 0 0 0 0 0 0 ...
    ##  $ VeryActiveDistance      : num [1:940] 1.88 1.57 2.44 2.14 2.71 ...
    ##  $ ModeratelyActiveDistance: num [1:940] 0.55 0.69 0.4 1.26 0.41 ...
    ##  $ LightActiveDistance     : num [1:940] 6.06 4.71 3.91 2.83 5.04 ...
    ##  $ SedentaryActiveDistance : num [1:940] 0 0 0 0 0 0 0 0 0 0 ...
    ##  $ VeryActiveMinutes       : num [1:940] 25 21 30 29 36 38 42 50 28 19 ...
    ##  $ FairlyActiveMinutes     : num [1:940] 13 19 11 34 10 20 16 31 12 8 ...
    ##  $ LightlyActiveMinutes    : num [1:940] 328 217 181 209 221 164 233 264 205 211 ...
    ##  $ SedentaryMinutes        : num [1:940] 728 776 1218 726 773 ...
    ##  $ Calories                : num [1:940] 1985 1797 1776 1745 1863 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   ActivityDate = col_character(),
    ##   ..   TotalSteps = col_double(),
    ##   ..   TotalDistance = col_double(),
    ##   ..   TrackerDistance = col_double(),
    ##   ..   LoggedActivitiesDistance = col_double(),
    ##   ..   VeryActiveDistance = col_double(),
    ##   ..   ModeratelyActiveDistance = col_double(),
    ##   ..   LightActiveDistance = col_double(),
    ##   ..   SedentaryActiveDistance = col_double(),
    ##   ..   VeryActiveMinutes = col_double(),
    ##   ..   FairlyActiveMinutes = col_double(),
    ##   ..   LightlyActiveMinutes = col_double(),
    ##   ..   SedentaryMinutes = col_double(),
    ##   ..   Calories = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

``` r
as_tibble(heartrate_seconds)
```

    ## # A tibble: 2,483,658 × 3
    ##            Id Time                 Value
    ##         <dbl> <chr>                <dbl>
    ##  1 2022484408 4/12/2016 7:21:00 AM    97
    ##  2 2022484408 4/12/2016 7:21:05 AM   102
    ##  3 2022484408 4/12/2016 7:21:10 AM   105
    ##  4 2022484408 4/12/2016 7:21:20 AM   103
    ##  5 2022484408 4/12/2016 7:21:25 AM   101
    ##  6 2022484408 4/12/2016 7:22:05 AM    95
    ##  7 2022484408 4/12/2016 7:22:10 AM    91
    ##  8 2022484408 4/12/2016 7:22:15 AM    93
    ##  9 2022484408 4/12/2016 7:22:20 AM    94
    ## 10 2022484408 4/12/2016 7:22:25 AM    93
    ## # … with 2,483,648 more rows

``` r
str(heartrate_seconds)
```

    ## spec_tbl_df [2,483,658 × 3] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id   : num [1:2483658] 2.02e+09 2.02e+09 2.02e+09 2.02e+09 2.02e+09 ...
    ##  $ Time : chr [1:2483658] "4/12/2016 7:21:00 AM" "4/12/2016 7:21:05 AM" "4/12/2016 7:21:10 AM" "4/12/2016 7:21:20 AM" ...
    ##  $ Value: num [1:2483658] 97 102 105 103 101 95 91 93 94 93 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   Time = col_character(),
    ##   ..   Value = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

``` r
as_tibble(sleep_daily)
```

    ## # A tibble: 413 × 5
    ##            Id SleepDay              TotalSleepRecor… TotalMinutesAsl… TotalTimeInBed
    ##         <dbl> <chr>                            <dbl>            <dbl>          <dbl>
    ##  1 1503960366 4/12/2016 12:00:00 AM                1              327            346
    ##  2 1503960366 4/13/2016 12:00:00 AM                2              384            407
    ##  3 1503960366 4/15/2016 12:00:00 AM                1              412            442
    ##  4 1503960366 4/16/2016 12:00:00 AM                2              340            367
    ##  5 1503960366 4/17/2016 12:00:00 AM                1              700            712
    ##  6 1503960366 4/19/2016 12:00:00 AM                1              304            320
    ##  7 1503960366 4/20/2016 12:00:00 AM                1              360            377
    ##  8 1503960366 4/21/2016 12:00:00 AM                1              325            364
    ##  9 1503960366 4/23/2016 12:00:00 AM                1              361            384
    ## 10 1503960366 4/24/2016 12:00:00 AM                1              430            449
    ## # … with 403 more rows

``` r
str(sleep_daily)
```

    ## spec_tbl_df [413 × 5] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id                : num [1:413] 1.5e+09 1.5e+09 1.5e+09 1.5e+09 1.5e+09 ...
    ##  $ SleepDay          : chr [1:413] "4/12/2016 12:00:00 AM" "4/13/2016 12:00:00 AM" "4/15/2016 12:00:00 AM" "4/16/2016 12:00:00 AM" ...
    ##  $ TotalSleepRecords : num [1:413] 1 2 1 2 1 1 1 1 1 1 ...
    ##  $ TotalMinutesAsleep: num [1:413] 327 384 412 340 700 304 360 325 361 430 ...
    ##  $ TotalTimeInBed    : num [1:413] 346 407 442 367 712 320 377 364 384 449 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   SleepDay = col_character(),
    ##   ..   TotalSleepRecords = col_double(),
    ##   ..   TotalMinutesAsleep = col_double(),
    ##   ..   TotalTimeInBed = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

``` r
as_tibble(sleep_minutes)
```

    ## # A tibble: 188,521 × 4
    ##            Id date                 value       logId
    ##         <dbl> <chr>                <dbl>       <dbl>
    ##  1 1503960366 4/12/2016 2:47:30 AM     3 11380564589
    ##  2 1503960366 4/12/2016 2:48:30 AM     2 11380564589
    ##  3 1503960366 4/12/2016 2:49:30 AM     1 11380564589
    ##  4 1503960366 4/12/2016 2:50:30 AM     1 11380564589
    ##  5 1503960366 4/12/2016 2:51:30 AM     1 11380564589
    ##  6 1503960366 4/12/2016 2:52:30 AM     1 11380564589
    ##  7 1503960366 4/12/2016 2:53:30 AM     1 11380564589
    ##  8 1503960366 4/12/2016 2:54:30 AM     2 11380564589
    ##  9 1503960366 4/12/2016 2:55:30 AM     2 11380564589
    ## 10 1503960366 4/12/2016 2:56:30 AM     2 11380564589
    ## # … with 188,511 more rows

``` r
str(sleep_minutes)
```

    ## spec_tbl_df [188,521 × 4] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id   : num [1:188521] 1.5e+09 1.5e+09 1.5e+09 1.5e+09 1.5e+09 ...
    ##  $ date : chr [1:188521] "4/12/2016 2:47:30 AM" "4/12/2016 2:48:30 AM" "4/12/2016 2:49:30 AM" "4/12/2016 2:50:30 AM" ...
    ##  $ value: num [1:188521] 3 2 1 1 1 1 1 2 2 2 ...
    ##  $ logId: num [1:188521] 1.14e+10 1.14e+10 1.14e+10 1.14e+10 1.14e+10 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   date = col_character(),
    ##   ..   value = col_double(),
    ##   ..   logId = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

``` r
as_tibble(steps_hourly)
```

    ## # A tibble: 22,099 × 3
    ##            Id ActivityHour          StepTotal
    ##         <dbl> <chr>                     <dbl>
    ##  1 1503960366 4/12/2016 12:00:00 AM       373
    ##  2 1503960366 4/12/2016 1:00:00 AM        160
    ##  3 1503960366 4/12/2016 2:00:00 AM        151
    ##  4 1503960366 4/12/2016 3:00:00 AM          0
    ##  5 1503960366 4/12/2016 4:00:00 AM          0
    ##  6 1503960366 4/12/2016 5:00:00 AM          0
    ##  7 1503960366 4/12/2016 6:00:00 AM          0
    ##  8 1503960366 4/12/2016 7:00:00 AM          0
    ##  9 1503960366 4/12/2016 8:00:00 AM        250
    ## 10 1503960366 4/12/2016 9:00:00 AM       1864
    ## # … with 22,089 more rows

``` r
str(steps_hourly)
```

    ## spec_tbl_df [22,099 × 3] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id          : num [1:22099] 1.5e+09 1.5e+09 1.5e+09 1.5e+09 1.5e+09 ...
    ##  $ ActivityHour: chr [1:22099] "4/12/2016 12:00:00 AM" "4/12/2016 1:00:00 AM" "4/12/2016 2:00:00 AM" "4/12/2016 3:00:00 AM" ...
    ##  $ StepTotal   : num [1:22099] 373 160 151 0 0 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   ActivityHour = col_character(),
    ##   ..   StepTotal = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

``` r
as_tibble(weight_logs)
```

    ## # A tibble: 67 × 8
    ##            Id Date     WeightKg WeightPounds   Fat   BMI IsManualReport    LogId
    ##         <dbl> <chr>       <dbl>        <dbl> <dbl> <dbl> <lgl>             <dbl>
    ##  1 1503960366 5/2/201…     52.6         116.    22  22.6 TRUE            1.46e12
    ##  2 1503960366 5/3/201…     52.6         116.    NA  22.6 TRUE            1.46e12
    ##  3 1927972279 4/13/20…    134.          294.    NA  47.5 FALSE           1.46e12
    ##  4 2873212765 4/21/20…     56.7         125.    NA  21.5 TRUE            1.46e12
    ##  5 2873212765 5/12/20…     57.3         126.    NA  21.7 TRUE            1.46e12
    ##  6 4319703577 4/17/20…     72.4         160.    25  27.5 TRUE            1.46e12
    ##  7 4319703577 5/4/201…     72.3         159.    NA  27.4 TRUE            1.46e12
    ##  8 4558609924 4/18/20…     69.7         154.    NA  27.2 TRUE            1.46e12
    ##  9 4558609924 4/25/20…     70.3         155.    NA  27.5 TRUE            1.46e12
    ## 10 4558609924 5/1/201…     69.9         154.    NA  27.3 TRUE            1.46e12
    ## # … with 57 more rows

``` r
str(weight_logs)
```

    ## spec_tbl_df [67 × 8] (S3: spec_tbl_df/tbl_df/tbl/data.frame)
    ##  $ Id            : num [1:67] 1.50e+09 1.50e+09 1.93e+09 2.87e+09 2.87e+09 ...
    ##  $ Date          : chr [1:67] "5/2/2016 11:59:59 PM" "5/3/2016 11:59:59 PM" "4/13/2016 1:08:52 AM" "4/21/2016 11:59:59 PM" ...
    ##  $ WeightKg      : num [1:67] 52.6 52.6 133.5 56.7 57.3 ...
    ##  $ WeightPounds  : num [1:67] 116 116 294 125 126 ...
    ##  $ Fat           : num [1:67] 22 NA NA NA NA 25 NA NA NA NA ...
    ##  $ BMI           : num [1:67] 22.6 22.6 47.5 21.5 21.7 ...
    ##  $ IsManualReport: logi [1:67] TRUE TRUE FALSE TRUE TRUE TRUE ...
    ##  $ LogId         : num [1:67] 1.46e+12 1.46e+12 1.46e+12 1.46e+12 1.46e+12 ...
    ##  - attr(*, "spec")=
    ##   .. cols(
    ##   ..   Id = col_double(),
    ##   ..   Date = col_character(),
    ##   ..   WeightKg = col_double(),
    ##   ..   WeightPounds = col_double(),
    ##   ..   Fat = col_double(),
    ##   ..   BMI = col_double(),
    ##   ..   IsManualReport = col_logical(),
    ##   ..   LogId = col_double()
    ##   .. )
    ##  - attr(*, "problems")=<externalptr>

## 4.4 Cleaning and formatting

We will now clean the data to eliminate any errors or inconsistencies,
and format it so that it can be easily used later during analysis.

### 4.4.1 Duplicates and N/A

We will look for any duplicates.

``` r
sum(duplicated(activity_daily))
```

    ## [1] 0

``` r
sum(duplicated(heartrate_seconds))
```

    ## [1] 0

``` r
sum(duplicated(sleep_daily))
```

    ## [1] 3

``` r
sum(duplicated(sleep_minutes))
```

    ## [1] 543

``` r
sum(duplicated(steps_hourly))
```

    ## [1] 0

``` r
sum(duplicated(weight_logs))
```

    ## [1] 0

Now we will remove the duplicates and N/A.

``` r
activity_daily <- activity_daily %>% 
  distinct() %>% 
  drop_na()

heartrate_seconds <- heartrate_seconds %>% 
  distinct() %>% 
  drop_na()

sleep_daily <- sleep_daily %>% 
  distinct() %>% 
  drop_na()

sleep_minutes <- sleep_minutes %>% 
  distinct() %>% 
  drop_na()

steps_hourly <- steps_hourly %>% 
  distinct() %>% 
  drop_na()

weight_logs <- weight_logs %>% 
  distinct()
```

Note that we are not using *drop_na()* for *weight_logs* because its
*fat* column only contains two values so most of the data frame would be
dropped. In later sections, we will drop remove the *fat* column.

Now we will verify that duplicates have been removed.

``` r
sum(duplicated(activity_daily))
```

    ## [1] 0

``` r
sum(duplicated(heartrate_seconds))
```

    ## [1] 0

``` r
sum(duplicated(sleep_daily))
```

    ## [1] 0

``` r
sum(duplicated(sleep_minutes))
```

    ## [1] 0

``` r
sum(duplicated(steps_hourly))
```

    ## [1] 0

``` r
sum(duplicated(weight_logs))
```

    ## [1] 0

### 4.4.2 Formatting columns, dates, and times

Now we will clean the column names so that each column name is in lower
case and snake case.

``` r
activity_daily <- clean_names(activity_daily)
heartrate_seconds <- clean_names(heartrate_seconds)
sleep_daily <- clean_names(sleep_daily)
sleep_minutes <- clean_names(sleep_minutes)
steps_hourly <- clean_names(steps_hourly)
weight_logs <- clean_names(weight_logs)
```

We are also going to merge the *activity_daily* and *sleep_daily* data
frames given that they contain data that can be joined based on their
common time frame. However, before we merge these data frames we will
rename the corresponding date columns and format them as dates.

``` r
activity_daily <- activity_daily %>% 
  rename(date = activity_date) %>% 
  mutate(date = as_date(date, format = "%m/%d/%Y"))

sleep_daily <- sleep_daily %>% 
  rename(date = sleep_day) %>% 
  mutate(date = as_date(date, format = "%m/%d/%Y %I:%M:%S %p" , tz = Sys.timezone()))
```

    ## Warning: `tz` argument is ignored by `as_date()`

We will also make some changes to the remaining data frames such as
formatting the *date* columns as date_time given that they include
specific times.

We will rename the *value* column in the *heartrate_seconds* data frame
to *heart_rate*, and the *time* column to *date_time*.

``` r
heartrate_seconds <- heartrate_seconds %>% 
  rename(heart_rate = value, date_time = time) %>% 
  mutate(date_time = as.POSIXct(date_time, format = "%m/%d/%Y %I:%M:%S %p" , tz = Sys.timezone()))
```

We will drop the *log_id* column in the *sleep_minutes* data frame
because we have no use for it, and will rename the *value* column to
*sleep_state* given that this is what it specifically represents
according to the dataset’s metadata. This states that value of 1 =
asleep, a value of 2 = restless, and a value of 3 = awake. We will also
rename the *date* column to *date_time*.

``` r
sleep_minutes <- subset(sleep_minutes, select = -c(log_id)) %>% 
  rename(sleep_state = value, date_time = date) %>% 
  mutate(date_time = as.POSIXct(date_time, format = "%m/%d/%Y %I:%M:%S %p" , tz = Sys.timezone()))
```

We will also rename the *activity_hour* column in the *steps_hourly*
data frame to *date*, and rename the *step_total* column to
*total_steps*.

``` r
steps_hourly <- steps_hourly %>% 
  rename(date_time = activity_hour, total_steps = step_total) %>%
  mutate(date_time = as.POSIXct(date_time, format = "%m/%d/%Y %I:%M:%S %p" , tz = Sys.timezone()))
```

Finally, we will drop the *fat*, *is_manual_report* and *log_id* columns
from the *weight_logs* data frame because *fat* only contains two
values, and the other two columns are of no use to us.

``` r
weight_logs <- subset(weight_logs, select = -c(fat, is_manual_report, log_id)) %>% 
  rename(date_time = date) %>%
  mutate(date_time = as.POSIXct(date_time, format = "%m/%d/%Y %I:%M:%S %p" , tz = Sys.timezone()))
```

Now that we have finished these steps, we will now check that everything
has been done correctly.

``` r
head(activity_daily)
```

    ## # A tibble: 6 × 15
    ##           id date       total_steps total_distance tracker_distance logged_activiti…
    ##        <dbl> <date>           <dbl>          <dbl>            <dbl>            <dbl>
    ## 1 1503960366 2016-04-12       13162           8.5              8.5                 0
    ## 2 1503960366 2016-04-13       10735           6.97             6.97                0
    ## 3 1503960366 2016-04-14       10460           6.74             6.74                0
    ## 4 1503960366 2016-04-15        9762           6.28             6.28                0
    ## 5 1503960366 2016-04-16       12669           8.16             8.16                0
    ## 6 1503960366 2016-04-17        9705           6.48             6.48                0
    ## # … with 9 more variables: very_active_distance <dbl>,
    ## #   moderately_active_distance <dbl>, light_active_distance <dbl>,
    ## #   sedentary_active_distance <dbl>, very_active_minutes <dbl>,
    ## #   fairly_active_minutes <dbl>, lightly_active_minutes <dbl>,
    ## #   sedentary_minutes <dbl>, calories <dbl>

``` r
head(heartrate_seconds)
```

    ## # A tibble: 6 × 3
    ##           id date_time           heart_rate
    ##        <dbl> <dttm>                   <dbl>
    ## 1 2022484408 2016-04-12 07:21:00         97
    ## 2 2022484408 2016-04-12 07:21:05        102
    ## 3 2022484408 2016-04-12 07:21:10        105
    ## 4 2022484408 2016-04-12 07:21:20        103
    ## 5 2022484408 2016-04-12 07:21:25        101
    ## 6 2022484408 2016-04-12 07:22:05         95

``` r
head(sleep_daily)
```

    ## # A tibble: 6 × 5
    ##           id date       total_sleep_records total_minutes_asle… total_time_in_b…
    ##        <dbl> <date>                   <dbl>               <dbl>            <dbl>
    ## 1 1503960366 2016-04-12                   1                 327              346
    ## 2 1503960366 2016-04-13                   2                 384              407
    ## 3 1503960366 2016-04-15                   1                 412              442
    ## 4 1503960366 2016-04-16                   2                 340              367
    ## 5 1503960366 2016-04-17                   1                 700              712
    ## 6 1503960366 2016-04-19                   1                 304              320

``` r
head(sleep_minutes)
```

    ## # A tibble: 6 × 3
    ##           id date_time           sleep_state
    ##        <dbl> <dttm>                    <dbl>
    ## 1 1503960366 2016-04-12 02:47:30           3
    ## 2 1503960366 2016-04-12 02:48:30           2
    ## 3 1503960366 2016-04-12 02:49:30           1
    ## 4 1503960366 2016-04-12 02:50:30           1
    ## 5 1503960366 2016-04-12 02:51:30           1
    ## 6 1503960366 2016-04-12 02:52:30           1

``` r
head(steps_hourly)
```

    ## # A tibble: 6 × 3
    ##           id date_time           total_steps
    ##        <dbl> <dttm>                    <dbl>
    ## 1 1503960366 2016-04-12 00:00:00         373
    ## 2 1503960366 2016-04-12 01:00:00         160
    ## 3 1503960366 2016-04-12 02:00:00         151
    ## 4 1503960366 2016-04-12 03:00:00           0
    ## 5 1503960366 2016-04-12 04:00:00           0
    ## 6 1503960366 2016-04-12 05:00:00           0

``` r
head(weight_logs)
```

    ## # A tibble: 6 × 5
    ##           id date_time           weight_kg weight_pounds   bmi
    ##        <dbl> <dttm>                  <dbl>         <dbl> <dbl>
    ## 1 1503960366 2016-05-02 23:59:59      52.6          116.  22.6
    ## 2 1503960366 2016-05-03 23:59:59      52.6          116.  22.6
    ## 3 1927972279 2016-04-13 01:08:52     134.           294.  47.5
    ## 4 2873212765 2016-04-21 23:59:59      56.7          125.  21.5
    ## 5 2873212765 2016-05-12 23:59:59      57.3          126.  21.7
    ## 6 4319703577 2016-04-17 23:59:59      72.4          160.  27.5

### 4.4.3 Merging datasets

Now we can proceed to merge the *activity_daily* and *sleep_daily* data
frames.

``` r
daily_data_merged <- merge(activity_daily, sleep_daily, by = c("id", "date"))
glimpse(daily_data_merged)
```

    ## Rows: 410
    ## Columns: 18
    ## $ id                         <dbl> 1503960366, 1503960366, 1503960366, 1503960…
    ## $ date                       <date> 2016-04-12, 2016-04-13, 2016-04-15, 2016-0…
    ## $ total_steps                <dbl> 13162, 10735, 9762, 12669, 9705, 15506, 105…
    ## $ total_distance             <dbl> 8.50, 6.97, 6.28, 8.16, 6.48, 9.88, 6.68, 6…
    ## $ tracker_distance           <dbl> 8.50, 6.97, 6.28, 8.16, 6.48, 9.88, 6.68, 6…
    ## $ logged_activities_distance <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0…
    ## $ very_active_distance       <dbl> 1.88, 1.57, 2.14, 2.71, 3.19, 3.53, 1.96, 1…
    ## $ moderately_active_distance <dbl> 0.55, 0.69, 1.26, 0.41, 0.78, 1.32, 0.48, 0…
    ## $ light_active_distance      <dbl> 6.06, 4.71, 2.83, 5.04, 2.51, 5.03, 4.24, 4…
    ## $ sedentary_active_distance  <dbl> 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0…
    ## $ very_active_minutes        <dbl> 25, 21, 29, 36, 38, 50, 28, 19, 41, 39, 73,…
    ## $ fairly_active_minutes      <dbl> 13, 19, 34, 10, 20, 31, 12, 8, 21, 5, 14, 2…
    ## $ lightly_active_minutes     <dbl> 328, 217, 209, 221, 164, 264, 205, 211, 262…
    ## $ sedentary_minutes          <dbl> 728, 776, 726, 773, 539, 775, 818, 838, 732…
    ## $ calories                   <dbl> 1985, 1797, 1745, 1863, 1728, 2035, 1786, 1…
    ## $ total_sleep_records        <dbl> 1, 2, 1, 2, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1…
    ## $ total_minutes_asleep       <dbl> 327, 384, 412, 340, 700, 304, 360, 325, 361…
    ## $ total_time_in_bed          <dbl> 346, 407, 442, 367, 712, 320, 377, 364, 384…

# 5. ANALYZE & SHARE Phase

Having processed, cleaned, and formatted all of the data that we will
use during this project, we will now proceed to perform calculations on
this data and analyze it.

## 5.1 Types of users per activity level

No information on age or gender was provided with this dataset. As such,
we will categorize users based on their activity level. We will use the
following categories proposed by Tudor-Locke & Bassett (2004):

| Step per Day | Classification      |
|--------------|---------------------|
| \<5000       | Sedentary           |
| 5000-7499    | Physically Inactive |
| 7500-9999    | Moderately Active   |
| ≥10,000      | Physically Active   |
| ≥12,500      | Very Active         |

Now, we will calculate each user’s daily average steps.

``` r
daily_avg_steps <- daily_data_merged %>% 
  group_by(id) %>% 
  summarise(daily_avg_steps = mean(total_steps))

daily_avg_steps
```

    ## # A tibble: 24 × 2
    ##            id daily_avg_steps
    ##         <dbl>           <dbl>
    ##  1 1503960366          12406.
    ##  2 1644430081           7968.
    ##  3 1844505072           3477 
    ##  4 1927972279           1490 
    ##  5 2026352035           5619.
    ##  6 2320127002           5079 
    ##  7 2347167796           8533.
    ##  8 3977333714          11218 
    ##  9 4020332650           6597.
    ## 10 4319703577           7125.
    ## # … with 14 more rows

We will categorize each user in a specific activity level according to
their daily average steps.

``` r
user_type <- daily_avg_steps %>% 
  mutate(user_type = case_when(
    daily_avg_steps < 5000 ~ "sedentary",
    daily_avg_steps >= 5000 & daily_avg_steps < 7500 ~ "physically inactive",
    daily_avg_steps >= 7500 & daily_avg_steps < 10000 ~ "moderately active",
    daily_avg_steps >= 10000 & daily_avg_steps < 12500 ~ "physically active",
    daily_avg_steps >= 12500 ~ "very active"
  ))

head(user_type)
```

    ## # A tibble: 6 × 3
    ##           id daily_avg_steps user_type          
    ##        <dbl>           <dbl> <chr>              
    ## 1 1503960366          12406. physically active  
    ## 2 1644430081           7968. moderately active  
    ## 3 1844505072           3477  sedentary          
    ## 4 1927972279           1490  sedentary          
    ## 5 2026352035           5619. physically inactive
    ## 6 2320127002           5079  physically inactive

Now, we will calculate the percentages of user types.

``` r
user_type_percentages <- user_type %>% 
  group_by(user_type) %>% 
  summarize(total_users = n_distinct(id)) %>% 
  mutate(percentage = (total_users/sum(total_users))*100)

head(user_type_percentages)
```

    ## # A tibble: 5 × 3
    ##   user_type           total_users percentage
    ##   <chr>                     <int>      <dbl>
    ## 1 moderately active             9      37.5 
    ## 2 physically active             4      16.7 
    ## 3 physically inactive           5      20.8 
    ## 4 sedentary                     5      20.8 
    ## 5 very active                   1       4.17

We will create a pie chart to represent these percentages.

``` r
user_type_pie_chart <- ggplot(user_type_percentages, aes(x = "", y = percentage, fill = user_type)) +
  geom_col(color = "black") +
  coord_polar(theta = "y") +
  labs(title = "Distribution of User Types", x = "", y = "") +
  theme(axis.ticks = element_blank(),
        panel.grid = element_blank(),
        axis.text = element_blank(),
        plot.title = element_text(hjust = 0.5, face = "bold"),
        panel.background = element_blank(),
        legend.title = element_text(hjust = 0.5, face = "bold")) +
  geom_text(aes(label = round(percentage, 1)),
            position = position_stack(vjust = 0.5)) +
  guides(fill = guide_legend(title = "User Type"))

user_type_pie_chart
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20pie%20chart-1.png)<!-- -->

**Observations:**

-   User types are fairly distributed, except for *very active* users.
-   This can mean that individuals are using their smart devices
    throughout their entire days, and not just when they are doing
    exercise.
-   Our hypothesis that the majority of users were physically active was
    incorrect.

## 5.2 BMI

We can also plot users’ BMIs on a histogram to see their distribution.

``` r
weight_histogram <- ggplot(weight_logs, aes(x = bmi)) +
  geom_histogram(binwidth = 1, color = "white", fill = "#006699") +
  labs(title = "Distribution of users' BMI", x = "Body Mass Index", y = "Number of Users") +
  geom_vline(aes(xintercept=mean(bmi)),color = "black", size = 1) +
  theme(plot.title = element_text(hjust = 0.5, face = "bold"))

weight_histogram
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20BMI%20on%20a%20scatterplot-1.png)<!-- -->

**Observations:**

-   The average body mass index of the users whose data was collected,
    represented by the vertical line, is 25.1852238. According to the
    CDC, a BMI between 18.5 and 24.9 is considered healthy weight for
    adults. Therefore, we can state that most of the individuals who use
    these smart devices are overweight or in the upper limits of healthy
    weight when using them. This observation, along with many others
    that will be mentioned throughout this report, cannot be fully
    trusted given that we do not have any information on the age or
    gender of the users.
-   Our hypothesis that the majority of users would be overweight was
    correct.

## 5.3 Steps vs. Sleep State

We are interested in analyzing how the total amount of steps taken in a
day can affect a user’s average sleep state. Therefore, we will compare
*sleep_state* from the *sleep_minutes* data frame and *total_steps* from
the *activity_daily* data frame. However, we must first calculate the
average sleep state per day per user given that the information is
currently divided by minutes.

``` r
avg_sleep_state_per_day <- sleep_minutes %>%
  rename(date = date_time) %>% 
  mutate(date = as_date(date, tz=Sys.timezone())) %>% 
  group_by(id, date) %>% 
  summarize(avg_sleep_state = mean(sleep_state))
```

    ## `summarise()` has grouped output by 'id'. You can override using the `.groups` argument.

``` r
(avg_sleep_state_per_day)
```

    ## # A tibble: 449 × 3
    ## # Groups:   id [24]
    ##            id date       avg_sleep_state
    ##         <dbl> <date>               <dbl>
    ##  1 1503960366 2016-04-12            1.07
    ##  2 1503960366 2016-04-13            1.09
    ##  3 1503960366 2016-04-15            1.09
    ##  4 1503960366 2016-04-16            1.09
    ##  5 1503960366 2016-04-17            1.02
    ##  6 1503960366 2016-04-19            1.05
    ##  7 1503960366 2016-04-20            1.05
    ##  8 1503960366 2016-04-21            1.12
    ##  9 1503960366 2016-04-23            1.06
    ## 10 1503960366 2016-04-24            1.04
    ## # … with 439 more rows

We must combine the two variables in a single data frame.

``` r
sleep_state_vs_total_steps <- merge(avg_sleep_state_per_day, activity_daily, by = c("id", "date")) %>% select(id, date, avg_sleep_state, total_steps) %>%
  mutate(user_type = case_when(
    total_steps < 5000 ~ "sedentary",
    total_steps >= 5000 & total_steps < 7500 ~ "physically inactive",
    total_steps >= 7500 & total_steps < 10000 ~ "moderately active",
    total_steps >= 10000 & total_steps < 12500 ~ "physically active",
    total_steps >= 12500 ~ "very active"))

head(sleep_state_vs_total_steps)
```

    ##           id       date avg_sleep_state total_steps         user_type
    ## 1 1503960366 2016-04-12        1.072254       13162       very active
    ## 2 1503960366 2016-04-13        1.085995       10735 physically active
    ## 3 1503960366 2016-04-15        1.085973        9762 moderately active
    ## 4 1503960366 2016-04-16        1.090000       12669       very active
    ## 5 1503960366 2016-04-17        1.016200        9705 moderately active
    ## 6 1503960366 2016-04-19        1.050000       15506       very active

Now, we can compare *avg_sleep_state* and *total_steps* together on a
scatterplot.

``` r
ggplot(sleep_state_vs_total_steps, aes(x = total_steps, y = avg_sleep_state)) +
  geom_point(aes(color=user_type)) +
  geom_smooth() +
  labs(title = "Sleep State vs. Total Steps", x = "Total Steps", y = "Avg. Sleep State") +
  theme(plot.title = element_text(face="bold", hjust = 0.5),
        legend.title = element_text(hjust = 0.5, face = "bold")) +
  guides(fill = guide_legend(title = "User Type"))
```

    ## `geom_smooth()` using method = 'loess' and formula 'y ~ x'

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20sleep%20state%20vs.%20total%20steps-1.png)<!-- -->

**Observations:**

-   There is no correlation between the total steps taken in a day and
    the user’s sleep state.
-   Our hypothesis that there is a negative correlation between the
    amount of steps and sleep quality/state was incorrect.

## 5.4 Calories vs. Sleep State

Now we will analyze whether differences in caloric intake have an effect
on the user’s average sleep state.

``` r
sleep_state_vs_calories <- merge(avg_sleep_state_per_day, activity_daily, by = c("id", "date")) %>% select(id, date, avg_sleep_state, calories)

head(sleep_state_vs_calories)
```

    ##           id       date avg_sleep_state calories
    ## 1 1503960366 2016-04-12        1.072254     1985
    ## 2 1503960366 2016-04-13        1.085995     1797
    ## 3 1503960366 2016-04-15        1.085973     1745
    ## 4 1503960366 2016-04-16        1.090000     1863
    ## 5 1503960366 2016-04-17        1.016200     1728
    ## 6 1503960366 2016-04-19        1.050000     2035

We can now plot the relationship between the two variables.

``` r
ggplot(sleep_state_vs_calories, aes(x = calories, y = avg_sleep_state)) +
  geom_point() +
  geom_smooth() +
  labs(title = "Sleep State vs. Calories", x = "Total Calories", y = "Avg. Sleep State") +
  theme(plot.title = element_text(face = "bold", hjust = 0.5))
```

    ## `geom_smooth()` using method = 'loess' and formula 'y ~ x'

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20sleep%20state%20vs.%20calories-1.png)<!-- -->

**Observations:**

-   There is no correlation between caloric intake and average sleep
    state. If anything, users tend to be slightly more restless in some
    cases when caloric intake is around 1500 calories.
-   Our hypothesis that there is a negative correlation between the
    amount of calories and sleep quality/state was incorrect.

## 5.5 Weekdays vs. Weekends

We also wish to gain some insights into how users’ behaviors change
depending on whether its a weekday or a weekend. To carry out this
analysis, we must create a data frame that adds two columns to the
*activity_daily* data frame: (i) a column that specifies the specific
day of the week for the corresponding observation; and (ii) for the
purposes of simplifying the results for later analysis, a column that
states *weekday* if the day is Monday, Tuesday, Wednesday, Thursday, and
Friday, and *weekend* if its Saturday or Sunday.

``` r
weekdays_vs_weekends <- activity_daily %>% 
  mutate(day = weekdays(date), weekday_or_weekend = case_when(
    day == "Monday" ~ "weekday",
    day == "Tuesday" ~ "weekday",
    day == "Wednesday" ~ "weekday",
    day == "Thursday" ~ "weekday",
    day == "Friday" ~ "weekday",
    TRUE ~ "weekend")) %>% select(id, date, day, weekday_or_weekend, everything())

weekdays_vs_weekends
```

    ## # A tibble: 940 × 17
    ##            id date       day       weekday_or_weekend total_steps total_distance
    ##         <dbl> <date>     <chr>     <chr>                    <dbl>          <dbl>
    ##  1 1503960366 2016-04-12 Tuesday   weekday                  13162           8.5 
    ##  2 1503960366 2016-04-13 Wednesday weekday                  10735           6.97
    ##  3 1503960366 2016-04-14 Thursday  weekday                  10460           6.74
    ##  4 1503960366 2016-04-15 Friday    weekday                   9762           6.28
    ##  5 1503960366 2016-04-16 Saturday  weekend                  12669           8.16
    ##  6 1503960366 2016-04-17 Sunday    weekend                   9705           6.48
    ##  7 1503960366 2016-04-18 Monday    weekday                  13019           8.59
    ##  8 1503960366 2016-04-19 Tuesday   weekday                  15506           9.88
    ##  9 1503960366 2016-04-20 Wednesday weekday                  10544           6.68
    ## 10 1503960366 2016-04-21 Thursday  weekday                   9819           6.34
    ## # … with 930 more rows, and 11 more variables: tracker_distance <dbl>,
    ## #   logged_activities_distance <dbl>, very_active_distance <dbl>,
    ## #   moderately_active_distance <dbl>, light_active_distance <dbl>,
    ## #   sedentary_active_distance <dbl>, very_active_minutes <dbl>,
    ## #   fairly_active_minutes <dbl>, lightly_active_minutes <dbl>,
    ## #   sedentary_minutes <dbl>, calories <dbl>

Now we can summarize the data frame.

``` r
avg_weekdays_vs_weekends <- weekdays_vs_weekends %>% 
  group_by(weekday_or_weekend) %>% 
  summarize(avg_steps = mean(total_steps), avg_calories = mean(calories))

avg_weekdays_vs_weekends
```

    ## # A tibble: 2 × 3
    ##   weekday_or_weekend avg_steps avg_calories
    ##   <chr>                  <dbl>        <dbl>
    ## 1 weekday                7669.        2302.
    ## 2 weekend                7551.        2310.

We will now plot this data frame.

``` r
ggarrange(
  ggplot(avg_weekdays_vs_weekends, aes(x = weekday_or_weekend, y = avg_steps, fill = weekday_or_weekend)) +
  geom_col(color = "black", ) +
  labs(title = "Avg. Steps per Week Section", subtitle = "Weekdays vs. Weekends", x = "Section of Week", y = "Avg. Steps") +
  theme(plot.title = element_text(hjust = 0.5, face = "bold"),
        plot.subtitle = element_text(hjust = 0.5),
        legend.title = element_text(hjust = 0.5, face = "bold"), legend.position = "none") +
  guides(fill = guide_legend(title = "Week Section")),
  ggplot(avg_weekdays_vs_weekends, aes(x = weekday_or_weekend, y = avg_calories, fill = weekday_or_weekend)) +
    geom_col(color = "black", ) +
  labs(title = "Avg. Calories per Week Section", subtitle = "Weekdays vs. Weekends", x = "Section of Week", y = "Avg. Calories") +
  theme(plot.title = element_text(hjust=0.5, face = "bold"),
        plot.subtitle = element_text(hjust = 0.5),
        legend.title = element_text(hjust = 0.5, face = "bold")) +
  guides(fill = guide_legend(title = "Week Section"))
  )
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20data%20frame-1.png)<!-- -->

**Observations:**

-   Our hypothesis was correct. During the week, users take more steps.
    This is coherent with the fact that, in general, users work during
    weekdays and move around more (pre-pandemic era). Individuals
    usually rest more on weekends. However, caloric intake is higher on
    weekends. This is also expected due to the fact that individuals
    usually maintain healthier and more strict diets during the week,
    and relax a bit during weekends.
-   Differences in results between weekdays and weekends are minimal and
    do not provide meaningful distinctions

## 5.6 Most active hours of the day

We will analyze the activity of the users throughout different hours of
the day based on their hourly steps. First, we must summarize the
*steps_hourly* data frame.

``` r
avg_steps_hourly <- steps_hourly %>%
  separate(date_time, into = c("date", "time"), sep = " ") %>%
  mutate(date = ymd(date))

head(avg_steps_hourly)
```

    ## # A tibble: 6 × 4
    ##           id date       time     total_steps
    ##        <dbl> <date>     <chr>          <dbl>
    ## 1 1503960366 2016-04-12 00:00:00         373
    ## 2 1503960366 2016-04-12 01:00:00         160
    ## 3 1503960366 2016-04-12 02:00:00         151
    ## 4 1503960366 2016-04-12 03:00:00           0
    ## 5 1503960366 2016-04-12 04:00:00           0
    ## 6 1503960366 2016-04-12 05:00:00           0

Now we can plot the different hours of the day on a bar graph.

``` r
avg_steps_hourly %>% 
  group_by(time) %>% 
  summarize(avg_steps = mean(total_steps)) %>% 
  ggplot(aes(x = time, y = avg_steps, fill = avg_steps)) +
  geom_col() +
  labs(title = "Average Steps throughout the Day", x = "Time", y = "Avg. Steps") +
  theme(plot.title = element_text(hjust = 0.5, face = "bold"),
        legend.title = element_text(hjust = 0.5, face = "bold"),
        axis.text.x = element_text(angle = 90)) +
  guides(fill = guide_legend(title = "Avg. Steps"))
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20bar%20graph-1.png)<!-- -->

**Observations:**

-   As expected, users are less active between 11 pm and 6 am due to
    sleep.
-   Users have a significant drop in activity around 3 pm. This may be
    due to this is usually around the time when digestion of food takes
    place after lunch and individuals feel more tired and lethargic.
-   Users are most active between 6 and 7 pm.
-   Our hypothesis that users are more active in the morning was
    incorrect.

## 5.7 Usage vs. Average Daily Steps

Now, we will test the following hypothesis: that individuals who use
their smart devices less days during the month have higher average daily
steps because they generally use their smart devices on days when they
are exercising. To carry out this test, we must first segment users
based on how many days per month they use their smart device.

We will create Usage Types based on the following criteria:

-   Low Use: 1 to 14 days
-   Moderate Use: 15 to 21 days
-   High Use: 22 to 31 days

Days that have less than 200 steps will not be counted.

Given that we will later analyze if there is a correlation between usage
and average daily steps, we will also join the *daily_avg_steps* data
frame to our *usage_types* data frame based on the user’s *id*.

``` r
usage_types <- activity_daily %>% 
  filter(total_steps >200) %>% 
  group_by(id) %>% 
  summarize(days_used = sum(n())) %>% 
  mutate(use_type = case_when(
    days_used >= 1 & days_used <= 14 ~ "Low Use",
    days_used >= 15 & days_used <= 21 ~ "Moderate Use",
    days_used >= 22 & days_used <= 31 ~ "High Use")) %>% 
  mutate(use_type = factor(use_type, ordered = TRUE, level = c('Low Use', 'Moderate Use', 'High Use'))) 

head(usage_types)
```

    ## # A tibble: 6 × 3
    ##           id days_used use_type    
    ##        <dbl>     <int> <ord>       
    ## 1 1503960366        30 High Use    
    ## 2 1624580081        31 High Use    
    ## 3 1644430081        30 High Use    
    ## 4 1844505072        17 Moderate Use
    ## 5 1927972279        15 Moderate Use
    ## 6 2022484408        31 High Use

Now we will create a summary table to see the percentage of each use
type.

``` r
usage_types_summary <- usage_types %>% 
  group_by(use_type) %>% 
  summarize(users = sum(n())) %>% 
  mutate(percentage = (users/sum(users))*100)

head(usage_types_summary)
```

    ## # A tibble: 3 × 3
    ##   use_type     users percentage
    ##   <ord>        <int>      <dbl>
    ## 1 Low Use          2       6.06
    ## 2 Moderate Use     7      21.2 
    ## 3 High Use        24      72.7

We will now plot this on a pie chart.

``` r
ggplot(usage_types_summary, aes(x = "", y = percentage, fill = use_type)) +
  geom_col(color = "black") +
  coord_polar(theta = "y") +
  scale_fill_brewer(palette = 'Pastel2') +
  labs(title = "Distribution of Usage Types", x = "", y = "") +
  theme(axis.ticks = element_blank(),
        panel.grid = element_blank(),
        axis.text = element_blank(),
        plot.title = element_text(hjust = 0.5, face = "bold"),
        panel.background = element_blank(),
        legend.title = element_text(hjust = 0.5, face = "bold")) +
  geom_text(aes(label = round(percentage, 1)),
            position = position_stack(vjust = 0.5)) +
  guides(fill = guide_legend(title = "Usage Type"))
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20pice%20chart-1.png)<!-- -->

**Observations:**

-   Most of the users use their smart devices between 22 and 31 days.
    This implies that users like, or at least understand that constant
    use enhances the utility of, their smart devices.

Having categorized users by the amount of days they wear their smart
devices, we can now analyze if there is a correlation between usage and
average daily steps. To do this, we must join the *daily_avg_steps* data
frame to our *usage_types* data frame based on the user’s *id*. We did
not carry out this step when we initially created the *usage_types* data
frame because we only have data on the daily average steps of 24 users,
which would reduce our current sample of 33 users.

``` r
usage_types_vs_steps <- activity_daily %>% 
  filter(total_steps >200) %>% 
  group_by(id) %>% 
  summarize(days_used = sum(n())) %>% 
  mutate(use_type = case_when(
    days_used >= 1 & days_used <= 14 ~ "Low Use",
    days_used >= 15 & days_used <= 21 ~ "Moderate Use",
    days_used >= 22 & days_used <= 31 ~ "High Use")) %>% 
  mutate(use_type = factor(use_type, ordered = TRUE, level = c('Low Use', 'Moderate Use', 'High Use'))) %>% 
  inner_join(
    daily_avg_steps, by = 'id'
  )

head(usage_types_vs_steps)
```

    ## # A tibble: 6 × 4
    ##           id days_used use_type     daily_avg_steps
    ##        <dbl>     <int> <ord>                  <dbl>
    ## 1 1503960366        30 High Use              12406.
    ## 2 1644430081        30 High Use               7968.
    ## 3 1844505072        17 Moderate Use           3477 
    ## 4 1927972279        15 Moderate Use           1490 
    ## 5 2026352035        31 High Use               5619.
    ## 6 2320127002        31 High Use               5079

We will now summarize the average daily steps by *use_type*.

``` r
usage_types_vs_steps_summary <- usage_types_vs_steps %>% 
  group_by(use_type) %>% 
  summarize(daily_avg_steps = mean(daily_avg_steps))

usage_types_vs_steps_summary
```

    ## # A tibble: 3 × 2
    ##   use_type     daily_avg_steps
    ##   <ord>                  <dbl>
    ## 1 Low Use                6597.
    ## 2 Moderate Use           4088.
    ## 3 High Use               9004.

Now we will plot this on a bar chart.

``` r
ggplot(usage_types_vs_steps_summary, aes(x = use_type, y = daily_avg_steps, fill = use_type)) +
  geom_col() +
  labs(title = "Daily Average Steps per Use Type", subtitle = "Comparing average daily steps to days used", x = "Usage", y = "Avg. Steps") +
  theme(plot.title = element_text(hjust = 0.5, face = "bold"),
        plot.subtitle = element_text(hjust = 0.5),
        legend.title = element_text(hjust = 0.5, face = "bold")) +
  guides(fill = guide_legend(title = "Use Type")) +
  scale_fill_brewer(palette = 'Pastel1')
```

![](Bellabeat_Data_Analysis_files/figure-gfm/plotting%20bar%20chart-1.png)<!-- -->

**Observations:**

-   As we can see in the chart, our hypothesis was partially correct.
    *Low Use* users do not have the highest average daily steps out of
    the group. However, they do have higher average daily steps than the
    *Moderate Use* users. This could be due to the reasoning behind our
    hypothesis (i.e., that *Low Use* users generally only use their
    devices on days when they will exercise and, thus, take more steps),
    or it could be due to something else.

# 6. ACT Phase

After analyzing the provided data, we have the following recommendations
for Bellabeat’s executive and marketing teams:

1.  **Focus on users with lower BMIs:** What we have seen from the data
    is that users wearing smart devices are usually overweight. This
    means that users are probably purchasing and wearing these devices
    to aid them in their efforts to lose weight. However, the same does
    not occur for underweight individuals that wish to gain weight.
    Given that these individuals are not as focused on monitoring their
    activity and caloric intake because they can eat more, they probably
    don’t feel the need to purchase a smart device. We see an
    opportunity here for Bellabeat to focus its marketing efforts on
    informing these individuals of how Bellabeat products can be of use
    in their lives, whether they wish to monitor specific calories/steps
    or not (e.g., use in monitoring sleep, stress).

2.  **Focus on increasing smart device usage in period of no exercise or
    activity:** The data tells us that, to a certain degree, users that
    wear their devices less often generally use these devices when they
    are exercising or moving more. This means that there is an growth
    opportunity for Bellabeat in informing users of the benefits of
    using their products (i.e., Time, Leaf, Spring) in periods of no
    exercise or reduced movement for things like sleep quality, stress,
    and hydration.

# 7. REFERENCES

Center for Disease Control and Prevention (August 27, 2021). *About
Adult BMI*. CDC. Retrieved on January 20, 2022, from:
<https://www.cdc.gov/healthyweight/assessing/bmi/adult_bmi/index.html>

Google. (n.d.). *Ask Questions to Make Data-Driven Decisions* \[MOOC\].
Coursera. Retrieved on January 20, 2022, from:
<https://www.coursera.org/learn/ask-questions-make-decisions?specialization=google-data-analytics>

Lacasa, M. (2021). *Captsone - Case Study Bellabeat*. Kaggle. Retrieved
on January 20, 2022, from:
<https://www.kaggle.com/macarenalacasa/capstone-case-study-bellabeat/notebook>

Möbius (n.d.). *FitBit Fitness Tracker Data*. Kaggle. Retrieved on
January 20, 2022, from: <https://www.kaggle.com/arashnic/fitbit>

University of North Texas – UNT (July 20, 2021). *Understanding Creative
Commons*. UNT. Retrieved on January 20, 2022, from:
<https://clear.unt.edu/teaching-resources/copyright-guide/creative-commons>

Tudor-Locke CE, Bassett DR. *How many steps are enough?
Pedometer-determined physical activity indices*. Sports Med.
2004;34(1):1–8. doi: 10.2165/00007256-200434010-00001.
