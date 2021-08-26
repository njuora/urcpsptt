# Lower bounds and heuristics for the unit-capacity resource constrained project scheduling problem with transfer times

---

This repository is maintained by Ying Liu (liuyingsme@smail.nju.edu.cn), and Qian Hu (huqian@nju.edu.cn) to supplement the article '"Lower bounds and heuristics for the unit-capacity resource constrained project scheduling problem with transfer times" published at *Computers & Industrial Engineering*.

- `instances`:  the data set
- `results_urcpsptt_20210331.xlsx`: the results of the lower bounds, models, and two heuristics. The tables in our article are also included.
- `detailed results.zip`:  the solutions of all the instances of lower bounds, models, and two heuristics. The solution of every instance is reported as a `json` file.

> Liu, Y., Zhou, J., Lim, A., & Hu, Q. (2021). Lower bounds and heuristics for the unit-capacity resource constrained project scheduling problem with transfer times. *Computers & Industrial Engineering*, *161*, 107605. https://doi.org/10.1016/j.cie.2021.107605

## Abstract

Resources are often transferred between two activities, especially if the two activities are processed at different locations. In this work, we study the unit-capacity resource constrained project scheduling problem with transfer times, where the resources with one unit capacity are considered. The objective is to find a feasible schedule satisfying the precedence relations, the resource requirements and the resource transfer constraints such that the project makespan is minimized. The problem can be transformed into a multiple traveling salesperson problem with synchronization and precedence constraints, based on which a good lower bound is derived. By exploring neighborhoods in the solution spaces based on both scheduling and routing representations, we propose two heuristics for the problem. Computational experiments based on randomly generated test instances are conducted to evaluate the performance of the approaches. The computational results show the good quality of the lower bounds and demonstrate the effectiveness of our approaches.

## Algorithm

At present, the source codes are only accessible to our team members. We will make it available to public at a later stage.

## Instances

Each instance is characterized by the following parameters:
(1) n: the number of non-dummy activities, {30, 60, 90, 120}
(2) m: the number of unit-capacity resources, {4, 6, 8, 10}
(3) network complexity: {1.50, 1.80, 2.10}
(4) resource factor: {0.25, 0.50, 0.75}
(5) transfer factor:{0.25, 0.50, 0.75}

Totally, 432 instances are generated. Each instance file is named as `jn_m_index.rcp`.

## Results

Our algorithms were implemented in Java and executed on a workstation with an Intel(R) Xeon(R) Platinum 8163 CPU clocked at 2.50 gigahertz and 64 gigabytes memory. The MIP model F1 and the restricted models of the subproblems in the two-phase optimization-based heuristic were solved by IBM ILOG CPLEX 12.8.  

- Tables and a summary of results are reported in `results_urcpsptt_20210331.xlsx`.
- If the readers are interested in the detailed solution of every instance,  please refer to`detailed_results.zip` .

