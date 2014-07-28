# Telesto Report
This repository contains the current state of the report for the Telesto Message Passing System developed by Simon Marti and Dominic Langenegger during the Advanced Systems Lab course at ETH Zurich in fall 2013. You can check out the code to the report in [this repo](https://github.com/dola/Telesto).

## License
This report is licensed under the [Creative Commons Attribution-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-sa/4.0/).

## Comments on System

### Database
 - Used multi-value indices +
 - Sound and simple design +
 - Duplicate message for each queue on multi-put
 - Used integrity constraints +
 - No proper transaction handling -

### System
 - Very good documented in report +
 - Uses binary protocol for communication between client and middleware +
 - Used Java NIO +
 - Sound error handling +
 - Configuration via files +
 - Thread pool +
 - DB connection pool +
 - Works stable +

### Client
 - Sound client design +
 - Experiments
 - 5% Quantile +
 - 2h trace +
 - Created a response time distribution +
 - Profiled Middleware +
 - Good mini-benchmark to figure out best configuration +
 - Middleware scale-out experiment to show that the DB is limiting factor and not middleware +
    - But on the same machine -
 
## Comments on Grading
This first milestone for the course project had a maximum possible score of 260 points. We got 193 with the following remarks:

### System
 - Sound DB-Schema
 - Sound design
 - Transaction handling wrong
 - Testing was done
 - Sound design
 - Didn’t implement different client types
 - Good documented code
 - No dynamic configuration

98/115 Points
 
### Experiments
 - Throughput measured in bytes is a bad idea - numbers get difficult to analyze
 - No proper bottleneck analysis
 - Several middleware servers on same machine
 - No correlation with design

79/115 Points
 
### Report
 - In general a good report
 - Testing not covered in Report
 - Incomplete Analysis in Report

20/30 Points
 
**Total:** 197/260 Points
