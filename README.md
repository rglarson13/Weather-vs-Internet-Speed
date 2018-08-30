# Weather-vs-Internet-Speed
Comparing weather data with internet speed test data to determine if weather influences my internet speed

I wanted to put together a Jupyter Notebook of my analysis of whether outdoor weather conditions affected my internet speed.

I scrape weather data from Weather Underground, use internet speed data that I collected myself (using speedtest-cli on my Raspberry Pi), and then compare them to see if there's any feature of the weather that predicts my internet speed.

Spoiler: there's not.
I used linear regression because the data actually _is_ fairly linear -- it just has a slope of near-zero.

I also tried but didn't include a K-Nearest Neighbors, Random Forest, and Gradient Boosting regressions, but those were pretty useless, too.

Ultimately, my data falls into the trap where the best accuracy I can get is to just predict that my speeds are always going to be good, because for a variety of reasons (not the least of which is that there's an upper bound on my speed imposed by Comcast) weather isn't a strong predictor of my internet speed.
