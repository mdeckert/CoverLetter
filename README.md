# CoverLetter

To whom it may concern,

Over the last 25 years I have worked primarily as a software developer doing backend web development.
Additionally, I have worked as a test automation engineer, systems administrator and technical writer.
While creating REST APIs for large variety of software systems, I discovered a passion for maintaining the accuracy and usability of the documentation accompanying these APIs.
I am presently searching for a new role that will allow me to leverage both my experience as a backend dev and my passion for creating highly usable documentation.

## Writing Samples

Here's a quick inline sample of some engineering writing:

```
Accumulating Peak Connections Data Across Nodes into 5 Minute Buckets

Since stats data will come in at 30 second intervals and the intervals
are not guaranteed to have aligned timestamps across nodes, we must make an 
approximation of overall peak connections based on available data. If we 
assume that the number of concurrent connections is reasonably well distributed 
across nodes by the load balancer, we can capture a reasonable peak total 
connections estimate by having the worker process run at a frequency that will
cover a small but nonzero number of readings from each node in redis (e.g. 2 
minute interval gets approximately 4 entries for each node). At each interval, 
we find the maximum peak connections for each node over that small period and 
combine those maximums for an approximate peak total connections over the period 
spanned by all the timestamps currently in redis. This peak connections number
is then compared to any previously recorded peak connections already in the 
relevant 5 min time bucket and updated with the maximum value.

Such an approximation could be slightly higher than the actual peak connections 
but should never underestimate the peak connections. Furthermore, this estimate
provides a good analogue for the actual expected enforcement behavior since the 
type of connection load that would contribute to overestimation (uneven, bursty 
connection load) is the same type of connection load that could lead to 
admission control limits being enforced when the total connection count is 
actually under the limit (i.e. if individual node got more than its share of 
connections).
```

And here are a few more historical samples:

- Product Documentation:
  - [3rd Rail](https://htmlpreview.github.io/?https://github.com/mdeckert/CoverLetter/blob/main/Samples/3rdRailDocs/index.html)
- Internal Engineering:
  - [Customer Visible Optimization Status](Samples/CustomerVisibleOptimizationStatus.png)
  - [Kernel Crashdumps](Samples/KernelCrashdumps.png) 
- Academic:
  - [Thesis Excerpt](Samples/MarkDeckertThesisExcerpt.pdf)
  - [Peer to PCAST](https://www.researchgate.net/profile/Warren-Sack/publication/262324560_Peer_to_PCAST_What_does_open_video_have_to_do_with_open_government/links/550722230cf26ff55f7bc9f4/Peer-to-PCAST-What-does-open-video-have-to-do-with-open-government.pdf)
  - [Metavid.org](https://d1wqtxts1xzle7.cloudfront.net/49404861/Metavid.org_A_Social_Website_and_Open_Ar20161006-14837-93hxwh-libre.pdf?1475771353=&response-content-disposition=inline%3B+filename%3DMetavid_org_A_Social_Website_and_Open_Ar.pdf&Expires=1703886484&Signature=Vx-ksAO9Yqf5tQptsvCopdAcnEExjNr~bYHi5dwc-Be23LCFJ3E~nf~ib41mUG1O4gIMBLsoDD~iNxKJblC95JT5-hWlVpqZnIa3zjCzXzyIjqkGmMzxrt-v~LEw0I8~xFB1-fiYRQJ2M~Sm-2~7o2xBplFG~VHmkqBO0Zy~egVdrYmdV-pITfjNSua8GvUzRaaw42ZygDKf~Tg6fkotc6ERqBs0R9BMP1AkRg6RPQqOirYZVu21sYLNS-TXpSgUJZGoZosNK3ZVgqAdQ6aheGJEoLwzonFPvgW-VcsoAa9VlBHwUSW7VSnOZm-dSgarxBfQlJ~yjlgrQTDBUnIhqQ__&Key-Pair-Id=APKAJLOHF5GGSLRBV4ZA)

And, finally, a resume:

- [Resume](MarkDeckertTechWriter.pdf)
