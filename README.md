# Prediction-Based Prefetch Scheduling in Mobile Networks

This repository provides additional resources related to the evaluation results of "Prediction-Based Prefetch Scheduling in Mobile Networks", a paper by Michael Borkowski, Stefan Schulte and Schahram Dustdar (Distributed Systems Group, TU Wien; see below).

The paper is currently under review.

## Authors
Michael Borkowski, Stefan Schulte, Schahram Dustdar  
Distributed Systems Group  
TU Wien  
Vienna, Austria  
{m.borkowski, s.schulte, dustdar}@infosys.tuwien.ac.at

## Abstract
The usage of Web or Cloud-based applications on mobile devices suffers from varying link quality, which causes user-perceivable delays and therefore reduces the Quality of Experience (QoE). In turn, mobile devices are increasingly feature-rich, allowing to make usage of context data in order to predict network quality based on the user’s location.

In this paper, we propose a prefetching scheduling algorithm based on network quality predictions, and evaluate it using data collected from real-world field tests. We show that our approach fulfills the expected gain of QoE. Using network quality prediction to optimize data prefetching can improve the user-perceived response time by up to 95 %.

## Evaluation
The evaluation in our paper consists of two parts. First, data collected from a real-world route is used to show the impact of our prefetching algorithm. Second, we perform regression tests to measure the influence of other variables. This repository shows additional results of the first part.

For the real-world evaluation, we drove along routes with a car, continuously recording the network speed. We then used this information in order to run our algorithm with different parameters. Ultimately, we performed two runs for each route, which we call A and B.

Run A performs naive prefetching, i.e., maintains a constant buffer of data. Run B performs prediction-based prefetching, in other words, employs the algorithm presented in our paper.

## Routes
We recorded three routes in different parts of the Vienna urban area. The routes have varying characteristics regarding network quality. In the following, we present the three routes.

* [Route 1](route-1)
* [Route 2](route-2)
* [Route 3](route-3)
