# Comparing `tmp/pyvrp-0.4.2.tar.gz` & `tmp/pyvrp-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvrp-0.4.2.tar", max compression
+gzip compressed data, was "pyvrp-0.4.4.tar", max compression
```

## Comparing `pyvrp-0.4.2.tar` & `pyvrp-0.4.4.tar`

### file list

```diff
@@ -1,167 +1,149 @@
--rw-r--r--   0        0        0     1175 2023-07-07 13:06:32.814027 pyvrp-0.4.2/LICENSE
--rw-r--r--   0        0        0     2963 2023-07-07 13:06:32.814027 pyvrp-0.4.2/README.md
--rw-r--r--   0        0        0     3563 2023-07-07 13:06:32.814027 pyvrp-0.4.2/build_extensions.py
--rw-r--r--   0        0        0     3747 2023-07-07 13:06:32.842027 pyvrp-0.4.2/meson.build
--rw-r--r--   0        0        0      302 2023-07-07 13:06:32.842027 pyvrp-0.4.2/meson_options.txt
--rw-r--r--   0        0        0     3505 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6822 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/GeneticAlgorithm.py
--rw-r--r--   0        0        0     8577 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Model.py
--rw-r--r--   0        0        0     8807 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/PenaltyManager.py
--rw-r--r--   0        0        0     6608 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Population.py
--rw-r--r--   0        0        0     2922 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Result.py
--rw-r--r--   0        0        0     6191 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/Statistics.py
--rw-r--r--   0        0        0     1375 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_CostEvaluator.pyi
--rw-r--r--   0        0        0      563 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_Matrix.pyi
--rw-r--r--   0        0        0     5791 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_ProblemData.pyi
--rw-r--r--   0        0        0     6397 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_Solution.pyi
--rw-r--r--   0        0        0     4089 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_SubPopulation.pyi
--rw-r--r--   0        0        0     1664 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_TimeWindowSegment.pyi
--rw-r--r--   0        0        0      267 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/_XorShift128.pyi
--rw-r--r--   0        0        0      554 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/__init__.py
--rw-r--r--   0        0        0     9091 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cli.py
--rw-r--r--   0        0        0       45 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/constants.py
--rw-r--r--   0        0        0      854 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.cpp
--rw-r--r--   0        0        0     2039 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.h
--rw-r--r--   0        0        0     1354 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/CostEvaluator_bindings.cpp
--rw-r--r--   0        0        0     2751 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Matrix.h
--rw-r--r--   0        0        0     1041 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Matrix_bindings.cpp
--rw-r--r--   0        0        0     5569 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Measure.h
--rw-r--r--   0        0        0     2698 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData.cpp
--rw-r--r--   0        0        0     4738 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData.h
--rw-r--r--   0        0        0     5227 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/ProblemData_bindings.cpp
--rw-r--r--   0        0        0      745 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/README.md
--rw-r--r--   0        0        0    11014 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution.cpp
--rw-r--r--   0        0        0     6876 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution.h
--rw-r--r--   0        0        0     5857 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/Solution_bindings.cpp
--rw-r--r--   0        0        0     4670 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation.cpp
--rw-r--r--   0        0        0     3036 2023-07-07 13:06:32.842027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation.h
--rw-r--r--   0        0        0     2744 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/SubPopulation_bindings.cpp
--rw-r--r--   0        0        0     3725 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment.h
--rw-r--r--   0        0        0     1603 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment_bindings.cpp
--rw-r--r--   0        0        0      581 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128.cpp
--rw-r--r--   0        0        0     2109 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128.h
--rw-r--r--   0        0        0      467 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/XorShift128_bindings.cpp
--rw-r--r--   0        0        0     5318 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.cpp
--rw-r--r--   0        0        0     2010 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.h
--rw-r--r--   0        0        0     8610 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange.cpp
--rw-r--r--   0        0        0      375 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange_bindings.cpp
--rw-r--r--   0        0        0     1003 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance.cpp
--rw-r--r--   0        0        0      254 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance_bindings.cpp
--rw-r--r--   0        0        0      636 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/diversity/diversity.h
--rw-r--r--   0        0        0     3048 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/CircleSector.h
--rw-r--r--   0        0        0    11425 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Exchange.h
--rw-r--r--   0        0        0     2173 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Exchange_bindings.cpp
--rw-r--r--   0        0        0    14552 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.cpp
--rw-r--r--   0        0        0     3734 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.h
--rw-r--r--   0        0        0     2647 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearchOperator.h
--rw-r--r--   0        0        0     1329 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch_bindings.cpp
--rw-r--r--   0        0        0     3733 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
--rw-r--r--   0        0        0      504 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.h
--rw-r--r--   0        0        0      482 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed_bindings.cpp
--rw-r--r--   0        0        0      970 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Node.cpp
--rw-r--r--   0        0        0     1616 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Node.h
--rw-r--r--   0        0        0     1175 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.cpp
--rw-r--r--   0        0        0      755 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.h
--rw-r--r--   0        0        0      436 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar_bindings.cpp
--rw-r--r--   0        0        0     3952 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Route.cpp
--rw-r--r--   0        0        0     5350 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/Route.h
--rw-r--r--   0        0        0    10975 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.cpp
--rw-r--r--   0        0        0     3399 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.h
--rw-r--r--   0        0        0      420 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/SwapStar_bindings.cpp
--rw-r--r--   0        0        0     4352 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.cpp
--rw-r--r--   0        0        0      922 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.h
--rw-r--r--   0        0        0      409 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt_bindings.cpp
--rw-r--r--   0        0        0       63 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/__init__.py
--rw-r--r--   0        0        0      364 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/_selective_route_exchange.pyi
--rw-r--r--   0        0        0     1949 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/selective_route_exchange.py
--rw-r--r--   0        0        0    12528 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/crossover/tests/test_selective_route_exchange.py
--rw-r--r--   0        0        0       58 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/__init__.py
--rw-r--r--   0        0        0     1444 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/_broken_pairs_distance.pyi
--rw-r--r--   0        0        0     1171 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/diversity/tests/test_broken_pairs_distance.py
--rw-r--r--   0        0        0      580 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/exceptions.py
--rw-r--r--   0        0        0      436 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/__init__.py
--rw-r--r--   0        0        0     1106 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_coordinates.py
--rw-r--r--   0        0        0     1358 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_demands.py
--rw-r--r--   0        0        0     1199 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_diversity.py
--rw-r--r--   0        0        0     1129 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_instance.py
--rw-r--r--   0        0        0     2344 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_objectives.py
--rw-r--r--   0        0        0     1608 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_result.py
--rw-r--r--   0        0        0     4690 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_route_schedule.py
--rw-r--r--   0        0        0     1136 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_runtimes.py
--rw-r--r--   0        0        0     1782 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_solution.py
--rw-r--r--   0        0        0     1226 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/plot_time_windows.py
--rw-r--r--   0        0        0        0 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/__init__.py
--rw-r--r--   0        0        0    47981 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
--rw-r--r--   0        0        0   141297 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
--rw-r--r--   0        0        0    35194 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
--rw-r--r--   0        0        0    25609 2023-07-07 13:06:32.846027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
--rw-r--r--   0        0        0    43058 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
--rw-r--r--   0        0        0     3079 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/plotting/tests/test_plotting.py
--rw-r--r--   0        0        0     6782 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/read.py
--rw-r--r--   0        0        0     6559 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/LocalSearch.py
--rw-r--r--   0        0        0      896 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_Exchange.pyi
--rw-r--r--   0        0        0      891 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_LocalSearch.pyi
--rw-r--r--   0        0        0      204 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_MoveTwoClientsReversed.pyi
--rw-r--r--   0        0        0      196 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_RelocateStar.pyi
--rw-r--r--   0        0        0      192 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_SwapStar.pyi
--rw-r--r--   0        0        0      188 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/_TwoOpt.pyi
--rw-r--r--   0        0        0      708 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/__init__.py
--rw-r--r--   0        0        0     5149 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/neighbourhood.py
--rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/__init__.py
--rw-r--r--   0        0        0    10470 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_Exchange.py
--rw-r--r--   0        0        0     8638 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_LocalSearch.py
--rw-r--r--   0        0        0     2633 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_MoveTwoClientsReversed.py
--rw-r--r--   0        0        0     3029 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_RelocateStar.py
--rw-r--r--   0        0        0     2918 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_SwapStar.py
--rw-r--r--   0        0        0     3970 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_TwoOpt.py
--rw-r--r--   0        0        0     6091 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/search/tests/test_neighbourhood.py
--rw-r--r--   0        0        0     1048 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/show_versions.py
--rw-r--r--   0        0        0      444 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/MaxIterations.py
--rw-r--r--   0        0        0      589 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/MaxRuntime.py
--rw-r--r--   0        0        0      819 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/NoImprovement.py
--rw-r--r--   0        0        0      573 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/StoppingCriterion.py
--rw-r--r--   0        0        0      575 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/TimedNoImprovement.py
--rw-r--r--   0        0        0      217 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/__init__.py
--rw-r--r--   0        0        0      839 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_MaxIterations.py
--rw-r--r--   0        0        0     1031 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_MaxRuntime.py
--rw-r--r--   0        0        0     1777 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_NoImprovement.py
--rw-r--r--   0        0        0     1292 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/stop/tests/test_TimedNoImprovement.py
--rw-r--r--   0        0        0        0 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/__init__.py
--rw-r--r--   0        0        0      189 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/DepotNotOne.txt
--rw-r--r--   0        0        0      607 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/E-n22-k4.txt
--rw-r--r--   0        0        0      671 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
--rw-r--r--   0        0        0      668 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
--rw-r--r--   0        0        0      389 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/FileWithUnknownSection.txt
--rw-r--r--   0        0        0      191 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/MoreThanOneDepot.txt
--rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotDemand.txt
--rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
--rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
--rw-r--r--   0        0        0      371 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
--rw-r--r--   0        0        0      675 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmall.txt
--rw-r--r--   0        0        0      697 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallGreedyRepair.txt
--rw-r--r--   0        0        0      754 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallPrizes.txt
--rw-r--r--   0        0        0      744 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/OkSmallReleaseTimes.txt
--rw-r--r--   0        0        0      347 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/RC208.sol
--rw-r--r--   0        0        0     7524 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/RC208.txt
--rw-r--r--   0        0        0      681 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/ReallyLargeDistance.txt
--rw-r--r--   0        0        0      369 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
--rw-r--r--   0        0        0      187 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
--rw-r--r--   0        0        0      154 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/UnknownEdgeWeightType.txt
--rw-r--r--   0        0        0     2005 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/data/p06-2-50.vrp
--rw-r--r--   0        0        0     1985 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/helpers.py
--rw-r--r--   0        0        0     4674 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_CostEvaluator.py
--rw-r--r--   0        0        0     7586 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_GeneticAlgorithm.py
--rw-r--r--   0        0        0     1348 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Matrix.py
--rw-r--r--   0        0        0     8491 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Model.py
--rw-r--r--   0        0        0     9864 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_PenaltyManager.py
--rw-r--r--   0        0        0    12503 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Population.py
--rw-r--r--   0        0        0     3570 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_ProblemData.py
--rw-r--r--   0        0        0     2645 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Result.py
--rw-r--r--   0        0        0    19074 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Solution.py
--rw-r--r--   0        0        0     1134 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_Statistics.py
--rw-r--r--   0        0        0     5882 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_SubPopulation.py
--rw-r--r--   0        0        0     2240 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_TimeWindowSegment.py
--rw-r--r--   0        0        0     1101 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_XorShift128.py
--rw-r--r--   0        0        0     7153 2023-07-07 13:06:32.850027 pyvrp-0.4.2/pyvrp/tests/test_read.py
--rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1175 2023-07-09 13:25:12.450763 pyvrp-0.4.4/LICENSE.md
+-rw-r--r--   0        0        0     2963 2023-07-09 13:25:12.450763 pyvrp-0.4.4/README.md
+-rw-r--r--   0        0        0     3563 2023-07-09 13:25:12.450763 pyvrp-0.4.4/build_extensions.py
+-rw-r--r--   0        0        0     3155 2023-07-09 13:25:12.478762 pyvrp-0.4.4/meson.build
+-rw-r--r--   0        0        0      302 2023-07-09 13:25:12.478762 pyvrp-0.4.4/meson_options.txt
+-rw-r--r--   0        0        0     3456 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     6848 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/GeneticAlgorithm.py
+-rw-r--r--   0        0        0     8536 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Model.py
+-rw-r--r--   0        0        0     8799 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/PenaltyManager.py
+-rw-r--r--   0        0        0     6551 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Population.py
+-rw-r--r--   0        0        0     2892 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Result.py
+-rw-r--r--   0        0        0     6183 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/Statistics.py
+-rw-r--r--   0        0        0      510 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/__init__.py
+-rw-r--r--   0        0        0    20429 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/_pyvrp.pyi
+-rw-r--r--   0        0        0     9113 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cli.py
+-rw-r--r--   0        0        0       45 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/constants.py
+-rw-r--r--   0        0        0      925 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.cpp
+-rw-r--r--   0        0        0     2079 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.h
+-rw-r--r--   0        0        0     2178 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.cpp
+-rw-r--r--   0        0        0     1618 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/DynamicBitset.h
+-rw-r--r--   0        0        0     2791 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Matrix.h
+-rw-r--r--   0        0        0     5732 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Measure.h
+-rw-r--r--   0        0        0     2701 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/ProblemData.cpp
+-rw-r--r--   0        0        0     4778 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/ProblemData.h
+-rw-r--r--   0        0        0      871 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/README.md
+-rw-r--r--   0        0        0    11122 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Solution.cpp
+-rw-r--r--   0        0        0     6990 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/Solution.h
+-rw-r--r--   0        0        0     4709 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/SubPopulation.cpp
+-rw-r--r--   0        0        0     3116 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/SubPopulation.h
+-rw-r--r--   0        0        0     3765 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/TimeWindowSegment.h
+-rw-r--r--   0        0        0      608 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/XorShift128.cpp
+-rw-r--r--   0        0        0     2149 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/XorShift128.h
+-rw-r--r--   0        0        0    19239 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/bindings.cpp
+-rw-r--r--   0        0        0      378 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/bindings.cpp
+-rw-r--r--   0        0        0     5508 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.cpp
+-rw-r--r--   0        0        0     2048 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.h
+-rw-r--r--   0        0        0     8327 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/crossover/selective_route_exchange.cpp
+-rw-r--r--   0        0        0      260 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/bindings.cpp
+-rw-r--r--   0        0        0     1080 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/broken_pairs_distance.cpp
+-rw-r--r--   0        0        0      698 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/diversity/diversity.h
+-rw-r--r--   0        0        0     3104 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/CircleSector.h
+-rw-r--r--   0        0        0    11481 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Exchange.h
+-rw-r--r--   0        0        0    14616 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.cpp
+-rw-r--r--   0        0        0     3790 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.h
+-rw-r--r--   0        0        0     2703 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/LocalSearchOperator.h
+-rw-r--r--   0        0        0     3728 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.cpp
+-rw-r--r--   0        0        0      560 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.h
+-rw-r--r--   0        0        0      998 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Node.cpp
+-rw-r--r--   0        0        0     1672 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Node.h
+-rw-r--r--   0        0        0     1267 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.cpp
+-rw-r--r--   0        0        0      811 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.h
+-rw-r--r--   0        0        0     4002 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Route.cpp
+-rw-r--r--   0        0        0     5421 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/Route.h
+-rw-r--r--   0        0        0    11059 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.cpp
+-rw-r--r--   0        0        0     3455 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.h
+-rw-r--r--   0        0        0     4407 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.cpp
+-rw-r--r--   0        0        0      978 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.h
+-rw-r--r--   0        0        0     4633 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/cpp/search/bindings.cpp
+-rw-r--r--   0        0        0       63 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/__init__.py
+-rw-r--r--   0        0        0      292 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/_crossover.pyi
+-rw-r--r--   0        0        0     1826 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/selective_route_exchange.py
+-rw-r--r--   0        0        0    13200 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/crossover/tests/test_selective_route_exchange.py
+-rw-r--r--   0        0        0       46 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/__init__.py
+-rw-r--r--   0        0        0     1441 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/_diversity.pyi
+-rw-r--r--   0        0        0     1171 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/diversity/tests/test_broken_pairs_distance.py
+-rw-r--r--   0        0        0      580 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/exceptions.py
+-rw-r--r--   0        0        0      436 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/__init__.py
+-rw-r--r--   0        0        0     1106 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_coordinates.py
+-rw-r--r--   0        0        0     1358 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_demands.py
+-rw-r--r--   0        0        0     1199 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_diversity.py
+-rw-r--r--   0        0        0     1129 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_instance.py
+-rw-r--r--   0        0        0     2344 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_objectives.py
+-rw-r--r--   0        0        0     1608 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_result.py
+-rw-r--r--   0        0        0     4690 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_route_schedule.py
+-rw-r--r--   0        0        0     1136 2023-07-09 13:25:12.478762 pyvrp-0.4.4/pyvrp/plotting/plot_runtimes.py
+-rw-r--r--   0        0        0     1782 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/plot_solution.py
+-rw-r--r--   0        0        0     1226 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/plot_time_windows.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/__init__.py
+-rw-r--r--   0        0        0    47981 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png
+-rw-r--r--   0        0        0   141297 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png
+-rw-r--r--   0        0        0    35194 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png
+-rw-r--r--   0        0        0    25609 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png
+-rw-r--r--   0        0        0    43058 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png
+-rw-r--r--   0        0        0     3079 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/plotting/tests/test_plotting.py
+-rw-r--r--   0        0        0     6776 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/read.py
+-rw-r--r--   0        0        0     6515 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/LocalSearch.py
+-rw-r--r--   0        0        0      643 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/__init__.py
+-rw-r--r--   0        0        0     2113 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/_search.pyi
+-rw-r--r--   0        0        0     5105 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/neighbourhood.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/__init__.py
+-rw-r--r--   0        0        0    10448 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_Exchange.py
+-rw-r--r--   0        0        0     8605 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_LocalSearch.py
+-rw-r--r--   0        0        0     2633 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_MoveTwoClientsReversed.py
+-rw-r--r--   0        0        0     3029 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_RelocateStar.py
+-rw-r--r--   0        0        0     2918 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_SwapStar.py
+-rw-r--r--   0        0        0     3970 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_TwoOpt.py
+-rw-r--r--   0        0        0     6091 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/search/tests/test_neighbourhood.py
+-rw-r--r--   0        0        0     1048 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/show_versions.py
+-rw-r--r--   0        0        0      444 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/MaxIterations.py
+-rw-r--r--   0        0        0      589 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/MaxRuntime.py
+-rw-r--r--   0        0        0      819 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/NoImprovement.py
+-rw-r--r--   0        0        0      573 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/StoppingCriterion.py
+-rw-r--r--   0        0        0      575 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/TimedNoImprovement.py
+-rw-r--r--   0        0        0      217 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/__init__.py
+-rw-r--r--   0        0        0      839 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_MaxIterations.py
+-rw-r--r--   0        0        0     1031 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_MaxRuntime.py
+-rw-r--r--   0        0        0     1777 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_NoImprovement.py
+-rw-r--r--   0        0        0     1292 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/stop/tests/test_TimedNoImprovement.py
+-rw-r--r--   0        0        0        0 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/__init__.py
+-rw-r--r--   0        0        0      189 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/DepotNotOne.txt
+-rw-r--r--   0        0        0      607 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/E-n22-k4.txt
+-rw-r--r--   0        0        0      671 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNoExplicit.txt
+-rw-r--r--   0        0        0      668 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt
+-rw-r--r--   0        0        0      389 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/FileWithUnknownSection.txt
+-rw-r--r--   0        0        0      191 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/MoreThanOneDepot.txt
+-rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotDemand.txt
+-rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotOpenTimeWindow.txt
+-rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotReleaseTime.txt
+-rw-r--r--   0        0        0      371 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/NonZeroDepotServiceDuration.txt
+-rw-r--r--   0        0        0      675 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmall.txt
+-rw-r--r--   0        0        0      697 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallGreedyRepair.txt
+-rw-r--r--   0        0        0      754 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallPrizes.txt
+-rw-r--r--   0        0        0      744 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/OkSmallReleaseTimes.txt
+-rw-r--r--   0        0        0      347 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/RC208.sol
+-rw-r--r--   0        0        0     7524 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/RC208.txt
+-rw-r--r--   0        0        0      681 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/ReallyLargeDistance.txt
+-rw-r--r--   0        0        0      369 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/TimeWindowOpenLargerThanClose.txt
+-rw-r--r--   0        0        0      187 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/UnknownEdgeWeightFmt.txt
+-rw-r--r--   0        0        0      154 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/UnknownEdgeWeightType.txt
+-rw-r--r--   0        0        0     2005 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/data/p06-2-50.vrp
+-rw-r--r--   0        0        0     1985 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/helpers.py
+-rw-r--r--   0        0        0     4674 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/test_CostEvaluator.py
+-rw-r--r--   0        0        0     2869 2023-07-09 13:25:12.482762 pyvrp-0.4.4/pyvrp/tests/test_DynamicBitset.py
+-rw-r--r--   0        0        0     7717 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_GeneticAlgorithm.py
+-rw-r--r--   0        0        0     1347 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Matrix.py
+-rw-r--r--   0        0        0     8491 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Model.py
+-rw-r--r--   0        0        0     9864 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_PenaltyManager.py
+-rw-r--r--   0        0        0    12503 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Population.py
+-rw-r--r--   0        0        0     3570 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_ProblemData.py
+-rw-r--r--   0        0        0     2645 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Result.py
+-rw-r--r--   0        0        0    19074 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Solution.py
+-rw-r--r--   0        0        0     1134 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_Statistics.py
+-rw-r--r--   0        0        0     5874 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_SubPopulation.py
+-rw-r--r--   0        0        0     2203 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_TimeWindowSegment.py
+-rw-r--r--   0        0        0     1088 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_XorShift128.py
+-rw-r--r--   0        0        0     7153 2023-07-09 13:25:12.486762 pyvrp-0.4.4/pyvrp/tests/test_read.py
+-rw-r--r--   0        0        0      616 2023-07-09 13:25:12.486762 pyvrp-0.4.4/subprojects/pybind11.wrap
+-rw-r--r--   0        0        0     4088 1970-01-01 00:00:00.000000 pyvrp-0.4.4/PKG-INFO
```

### Comparing `pyvrp-0.4.2/LICENSE` & `pyvrp-0.4.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/README.md` & `pyvrp-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/build_extensions.py` & `pyvrp-0.4.4/build_extensions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/meson.build` & `pyvrp-0.4.4/meson.build`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 project(
-    'pyvrp', 
-    'cpp', 
+    'pyvrp',
+    'cpp',
+    version: run_command('poetry', 'version', '--short', check : true).stdout(),
     default_options : [
         'cpp_std=c++20',
         'b_lto=true',  # sets -flto
         'werror=true',  # sets -Werror
         'warning_level=3',  # level 3 sets -Wextra and -Wpedantic
     ]
 )
 
-# The following lines define compiler and linker options for the debug build.
-# In particular, we also set up debug builds to provide coverage results.
-compiler = meson.get_compiler('cpp')
-
 if get_option('buildtype') == 'debug'
+    compiler = meson.get_compiler('cpp')
+
     if compiler.has_argument('-fprofile-abs-path')
         # clang does not have this particular flag, so we only add it when
         # compiling with gcc. It's helpful in determining code coverage.
         add_project_arguments('-fprofile-abs-path', language: 'cpp')
     endif
 
     add_project_arguments('--coverage', language: 'cpp')
@@ -41,14 +40,15 @@
 SRC_DIR = 'pyvrp' / 'cpp'
 INCLUDES = [include_directories(SRC_DIR)]
 
 libcommon = static_library(
     'common',
     [
         SRC_DIR / 'CostEvaluator.cpp',
+        SRC_DIR / 'DynamicBitset.cpp',
         SRC_DIR / 'ProblemData.cpp',
         SRC_DIR / 'XorShift128.cpp',
         SRC_DIR / 'Solution.cpp',
         SRC_DIR / 'SubPopulation.cpp',
         SRC_DIR / 'crossover' / 'selective_route_exchange.cpp',
         SRC_DIR / 'crossover' / 'crossover.cpp',
         SRC_DIR / 'diversity' / 'broken_pairs_distance.cpp',
@@ -61,47 +61,34 @@
         SRC_DIR / 'search' / 'SwapStar.cpp',
     ],
     include_directories: INCLUDES,
 )
 
 # Next we get the extension dependencies.
 py = import('python').find_installation()
-pybind11 = dependency('pybind11')
-dependencies = [py.dependency(), pybind11]
+dependencies = [py.dependency(), dependency('pybind11')]
 
-# Extension as [extension name, subdirectory]. Here 'extension name' names the
-# eventual module name and the bindings source file, and 'subdirectory' gives 
-# the source and installation directories (relative to SRC_DIR and INST_DIR).
+# Extension as [extension name, subdirectory]. The 'extension name' names the
+# eventual module name, and 'subdirectory' gives the source and installation 
+# directories (relative to SRC_DIR and INST_DIR).
 extensions = [
-    ['Matrix', ''],
-    ['CostEvaluator', ''],
-    ['ProblemData', ''],
-    ['SubPopulation', ''],
-    ['TimeWindowSegment', ''],
-    ['XorShift128', ''],
-    ['Solution', ''],
-    ['selective_route_exchange', 'crossover'],
-    ['broken_pairs_distance', 'diversity'],
-    ['LocalSearch', 'search'],
-    ['Exchange', 'search'],
-    ['MoveTwoClientsReversed', 'search'],
-    ['TwoOpt', 'search'],
-    ['RelocateStar', 'search'],
-    ['SwapStar', 'search'],
+    ['_pyvrp', ''],
+    ['_crossover', 'crossover'],
+    ['_diversity', 'diversity'],
+    ['_search', 'search'],
 ]
 
-foreach extension : extensions  # extension[0] = name, extension[1] = subdir
-    message('Going to build ' + extension[0])
-
-    source_dir = '/'.join([SRC_DIR, extension[1]])
-    install_dir = '/'.join([INST_DIR, extension[1]])
+foreach extension : extensions
+    name = extension[0]
+    subdir = extension[1]
 
+    message('Going to build ' + subdir / name)
     py.extension_module(
-        '_' + extension[0],  # native extensions are prepended by an underscore
-        source_dir / extension[0] + '_bindings.cpp',
+        name,
+        SRC_DIR / subdir / 'bindings.cpp',
         dependencies: dependencies,
         link_with: libcommon,
         install: true,
-        subdir: install_dir,
+        subdir: INST_DIR / subdir,
         include_directories: INCLUDES,
     )
 endforeach
```

### Comparing `pyvrp-0.4.2/pyproject.toml` & `pyvrp-0.4.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "pyvrp"
-version = "0.4.2"
+version = "0.4.4"
 description = "A state-of-the-art vehicle routing problem solver."
 authors = [
     "Niels Wouda <nielswouda@gmail.com>",
     "Leon Lan <leon.lanyidong@gmail.com>",
     "Wouter Kool <wouter.kool@ortec.com>",
 ]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/PyVRP/PyVRP"
 include = [
     { path = "LICENSE.md" },
     { path = "meson.build", format = "sdist" },
     { path = "meson_options.txt", format = "sdist" },
     { path = "build_extensions.py", format = "sdist" },
+    { path = "subprojects/*.wrap", format = "sdist" },
     { path = "pyvrp/**/*.so", format = "wheel" },
     { path = "pyvrp/**/*.pyd", format = "wheel" },
 ]
 packages = [
     { include = "pyvrp" },
 ]
 classifiers = [
@@ -117,18 +118,17 @@
     "venv/*",
     "docs/*",
 ]
 
 
 [tool.coverage.report]
 exclude_lines = [
-    # This excludes all abstract methods from code coverage checks as they are
-    # never instantiated directly anyway.
     "pragma: no cover",
     "@abstract",
+    "if TYPE_CHECKING:",
 ]
 
 
 [tool.cibuildwheel]
 # We do not support old Python versions (<3.8) and somewhat uncommon platforms.
 # For musllinux-based builds we assume users can compile the thing themselves.
 skip = "cp36-* cp37-* pp* *_ppc64le *_i686 *_s390x *-win32 *-musllinux*"
@@ -138,10 +138,10 @@
 
 [tool.poetry.build]
 generate-setup-file = false
 script = "build_extensions.py"
 
 
 [build-system]
-# meson and ninja are needed to build the C++ extensions.
-requires = ["poetry-core", "meson", "ninja"]
+# We need meson and ninja to build the C++ extensions.
+requires = ["poetry", "meson", "ninja"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyvrp-0.4.2/pyvrp/GeneticAlgorithm.py` & `pyvrp-0.4.4/pyvrp/GeneticAlgorithm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
+from __future__ import annotations
+
 import time
 from dataclasses import dataclass
-from typing import Callable, Collection, Tuple
-
-from pyvrp.search.LocalSearch import LocalSearch
-from pyvrp.stop import StoppingCriterion
+from typing import TYPE_CHECKING, Callable, Collection, Tuple
 
-from .PenaltyManager import PenaltyManager
-from .Population import Population
 from .Result import Result
 from .Statistics import Statistics
-from ._CostEvaluator import CostEvaluator
-from ._ProblemData import ProblemData
-from ._Solution import Solution
-from ._XorShift128 import XorShift128
-
-_Parents = Tuple[Solution, Solution]
-CrossoverOperator = Callable[
-    [_Parents, ProblemData, CostEvaluator, XorShift128], Solution
-]
+
+if TYPE_CHECKING:
+    from pyvrp.search.LocalSearch import LocalSearch
+    from pyvrp.stop import StoppingCriterion
+
+    from .PenaltyManager import PenaltyManager
+    from .Population import Population
+    from ._pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
+
+    _Parents = Tuple[Solution, Solution]
+    CrossoverOperator = Callable[
+        [_Parents, ProblemData, CostEvaluator, XorShift128], Solution
+    ]
 
 
 @dataclass
 class GeneticAlgorithmParams:
     repair_probability: float = 0.80
     collect_statistics: bool = False
     intensify_probability: float = 0.15
```

### Comparing `pyvrp-0.4.2/pyvrp/Model.py` & `pyvrp-0.4.4/pyvrp/Model.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,21 @@
 
 import numpy as np
 
 from pyvrp.GeneticAlgorithm import GeneticAlgorithm, GeneticAlgorithmParams
 from pyvrp.PenaltyManager import PenaltyManager
 from pyvrp.Population import Population, PopulationParams
 from pyvrp.Result import Result
-from pyvrp._ProblemData import Client, ProblemData, VehicleType
-from pyvrp._Solution import Solution
-from pyvrp._XorShift128 import XorShift128
+from pyvrp._pyvrp import (
+    Client,
+    ProblemData,
+    Solution,
+    VehicleType,
+    XorShift128,
+)
 from pyvrp.constants import MAX_USER_VALUE, MAX_VALUE
 from pyvrp.crossover import selective_route_exchange as srex
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.exceptions import ScalingWarning
 from pyvrp.stop import StoppingCriterion
 
 Depot = Client
@@ -30,15 +34,15 @@
 
 
 class Model:
     """
     A simple interface for modelling vehicle routing problems with PyVRP.
     """
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._clients: List[Client] = []
         self._depots: List[Depot] = []
         self._edges: List[Edge] = []
         self._vehicle_types: List[VehicleType] = []
 
     @property
     def locations(self) -> List[Client]:
@@ -50,15 +54,15 @@
         return self._depots + self._clients
 
     @property
     def vehicle_types(self) -> List[VehicleType]:
         """
         Returns the vehicle types in the current model. The routes of the
         solution returned by :meth:`~solve` have a property
-        :meth:`~pyvrp._Solution.Route.vehicle_type()` that can be used to index
+        :meth:`~pyvrp._pyvrp.Route.vehicle_type()` that can be used to index
         these vehicle types.
         """
         return self._vehicle_types
 
     @classmethod
     def from_data(cls, data: ProblemData) -> "Model":
         """
@@ -107,15 +111,15 @@
         tw_late: int = 0,
         release_time: int = 0,
         prize: int = 0,
         required: bool = True,
     ) -> Client:
         """
         Adds a client with the given attributes to the model. Returns the
-        created :class:`~pyvrp._ProblemData.Client` instance.
+        created :class:`~pyvrp._pyvrp.Client` instance.
         """
         client = Client(
             x,
             y,
             demand,
             service_duration,
             tw_early,
@@ -133,15 +137,15 @@
         x: int,
         y: int,
         tw_early: int = 0,
         tw_late: int = 0,
     ) -> Depot:
         """
         Adds a depot with the given attributes to the model. Returns the
-        created :class:`~pyvrp._ProblemData.Client` instance.
+        created :class:`~pyvrp._pyvrp.Client` instance.
 
         .. warning::
 
            PyVRP does not yet support multi-depot VRPs. For now, only one depot
            can be added to the model.
         """
         if len(self._depots) >= 1:
@@ -198,15 +202,15 @@
 
         vehicle_type = VehicleType(capacity, num_available)
         self._vehicle_types.append(vehicle_type)
         return vehicle_type
 
     def data(self) -> ProblemData:
         """
-        Creates and returns a :class:`~pyvrp._ProblemData.ProblemData` instance
+        Creates and returns a :class:`~pyvrp._pyvrp.ProblemData` instance
         from this model's attributes.
         """
         locs = self.locations
         loc2idx = {id(loc): idx for idx, loc in enumerate(locs)}
 
         max_data_value = max(max(e.distance, e.duration) for e in self._edges)
         if max_data_value > MAX_USER_VALUE:
@@ -223,20 +227,15 @@
 
         for edge in self._edges:
             frm = loc2idx[id(edge.frm)]
             to = loc2idx[id(edge.to)]
             distances[frm, to] = edge.distance
             durations[frm, to] = edge.duration
 
-        return ProblemData(
-            locs,
-            self.vehicle_types,
-            distances,
-            durations,
-        )
+        return ProblemData(locs, self.vehicle_types, distances, durations)
 
     def solve(self, stop: StoppingCriterion, seed: int = 0) -> Result:
         """
         Solve this model.
 
         Parameters
         ----------
@@ -259,24 +258,25 @@
             compute_neighbours,
         )
 
         data = self.data()
         rng = XorShift128(seed=seed)
         ls = LocalSearch(data, rng, compute_neighbours(data))
 
-        for op in NODE_OPERATORS:
-            ls.add_node_operator(op(data))
+        for node_op in NODE_OPERATORS:
+            ls.add_node_operator(node_op(data))
 
-        for op in ROUTE_OPERATORS:
-            ls.add_route_operator(op(data))
+        for route_op in ROUTE_OPERATORS:
+            ls.add_route_operator(route_op(data))
 
         pm = PenaltyManager()
         pop_params = PopulationParams()
         pop = Population(bpd, pop_params)
         init = [
             Solution.make_random(data, rng)
             for _ in range(pop_params.min_pop_size)
         ]
 
         gen_params = GeneticAlgorithmParams(collect_statistics=True)
-        algo = GeneticAlgorithm(data, pm, rng, pop, ls, srex, init, gen_params)
+        gen_args = (data, pm, rng, pop, ls, srex, init, gen_params)
+        algo = GeneticAlgorithm(*gen_args)  # type: ignore
         return algo.run(stop)
```

### Comparing `pyvrp-0.4.2/pyvrp/PenaltyManager.py` & `pyvrp-0.4.4/pyvrp/PenaltyManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from statistics import fmean
 from typing import List
 
-from pyvrp._CostEvaluator import CostEvaluator
+from pyvrp._pyvrp import CostEvaluator
 
 
 @dataclass
 class PenaltyParams:
     """
     The penalty manager parameters.
```

### Comparing `pyvrp-0.4.2/pyvrp/Population.py` & `pyvrp-0.4.4/pyvrp/Population.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from __future__ import annotations
 
 from typing import Callable, Generator, Tuple
 from warnings import warn
 
-from ._CostEvaluator import CostEvaluator
-from ._Solution import Solution
-from ._SubPopulation import PopulationParams, SubPopulation
-from ._XorShift128 import XorShift128
+from ._pyvrp import (
+    CostEvaluator,
+    PopulationParams,
+    Solution,
+    SubPopulation,
+    XorShift128,
+)
 from .exceptions import EmptySolutionWarning
 
 
 class Population:
     """
     Creates a Population instance.
```

### Comparing `pyvrp-0.4.2/pyvrp/Result.py` & `pyvrp-0.4.4/pyvrp/Result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import math
 from dataclasses import dataclass
 
 from .Statistics import Statistics
-from ._CostEvaluator import CostEvaluator
-from ._Solution import Solution
+from ._pyvrp import CostEvaluator, Solution
 
 
 @dataclass
 class Result:
     """
     Stores the outcomes of a single run. An instance of this class is returned
     once the GeneticAlgorithm completes.
```

### Comparing `pyvrp-0.4.2/pyvrp/Statistics.py` & `pyvrp-0.4.4/pyvrp/Statistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from math import nan
 from pathlib import Path
 from statistics import fmean
 from time import perf_counter
 from typing import List, Union
 
 from .Population import Population, SubPopulation
-from ._CostEvaluator import CostEvaluator
+from ._pyvrp import CostEvaluator
 
 _FEAS_CSV_PREFIX = "feas_"
 _INFEAS_CSV_PREFIX = "infeas_"
 
 
 @dataclass
 class _Datum:
```

### Comparing `pyvrp-0.4.2/pyvrp/cli.py` & `pyvrp-0.4.4/pyvrp/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,23 +135,23 @@
     neighbours = compute_neighbours(data, nb_params)
     ls = LocalSearch(data, rng, neighbours)
 
     node_ops = NODE_OPERATORS
     if "node_ops" in config:
         node_ops = [getattr(pyvrp.search, op) for op in config["node_ops"]]
 
-    for op in node_ops:
-        ls.add_node_operator(op(data))
+    for node_op in node_ops:
+        ls.add_node_operator(node_op(data))
 
     route_ops = ROUTE_OPERATORS
     if "route_ops" in config:
         route_ops = [getattr(pyvrp.search, op) for op in config["route_ops"]]
 
-    for op in route_ops:
-        ls.add_route_operator(op(data))
+    for route_op in route_ops:
+        ls.add_route_operator(route_op(data))
 
     init = [
         Solution.make_random(data, rng) for _ in range(pop_params.min_pop_size)
     ]
     algo = GeneticAlgorithm(
         data, pen_manager, rng, pop, ls, srex, init, gen_params
     )
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.cpp` & `pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 #include "CostEvaluator.h"
 
 #include <limits>
 
+using pyvrp::Cost;
+using pyvrp::CostEvaluator;
+using pyvrp::Solution;
+
 CostEvaluator::CostEvaluator(Cost capacityPenalty, Cost timeWarpPenalty)
     : capacityPenalty(capacityPenalty), timeWarpPenalty(timeWarpPenalty)
 {
 }
 
 Cost CostEvaluator::penalisedCost(Solution const &solution) const
 {
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/CostEvaluator.h` & `pyvrp-0.4.4/pyvrp/cpp/CostEvaluator.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #ifndef PYVRP_COSTEVALUATOR_H
 #define PYVRP_COSTEVALUATOR_H
 
 #include "Measure.h"
 #include "Solution.h"
 
+namespace pyvrp
+{
 /**
  * Cost evaluator class that computes penalty values for timewarp and load.
  */
 class CostEvaluator
 {
     Cost capacityPenalty;
     Cost timeWarpPenalty;
@@ -62,9 +64,10 @@
 {
 #ifdef PYVRP_NO_TIME_WINDOWS
     return 0;
 #else
     return static_cast<Cost>(timeWarp) * timeWarpPenalty;
 #endif
 }
+}  // namespace pyvrp
 
 #endif  // PYVRP_COSTEVALUATOR_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/Matrix.h` & `pyvrp-0.4.4/pyvrp/cpp/Matrix.h`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #define PYVRP_MATRIX_H
 
 #include <algorithm>
 #include <sstream>
 #include <stdexcept>
 #include <vector>
 
+namespace pyvrp
+{
 template <typename T> class Matrix
 {
     size_t cols_;          // The number of columns of the matrix
     size_t rows_;          // The number of rows of the matrix
     std::vector<T> data_;  // Data vector
 
 public:
@@ -105,9 +107,10 @@
 
 template <typename T> T Matrix<T>::max() const
 {
     return *std::max_element(data_.begin(), data_.end());
 }
 
 template <typename T> size_t Matrix<T>::size() const { return data_.size(); }
+}  // namespace pyvrp
 
 #endif  // PYVRP_MATRIX_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/Measure.h` & `pyvrp-0.4.4/pyvrp/cpp/Measure.h`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #include <cmath>
 #include <compare>
 #include <functional>
 #include <iostream>
 #include <limits>
 #include <type_traits>
 
+namespace pyvrp
+{
 #ifdef PYVRP_DOUBLE_PRECISION
 using Value = double;
 #else
 using Value = int;
 #endif
 
 enum class MeasureType
@@ -171,43 +173,50 @@
 }
 
 template <MeasureType Type>
 Measure<Type> operator/(Measure<Type> const lhs, Measure<Type> const rhs)
 {
     return lhs.get() / rhs.get();
 }
+}  // namespace pyvrp
 
 // For printing.
-template <MeasureType Type>
-std::ostream &operator<<(std::ostream &out, Measure<Type> const measure)
+template <pyvrp::MeasureType Type>
+std::ostream &operator<<(std::ostream &out, pyvrp::Measure<Type> const measure)
 {
     return out << measure.get();
 }
 
 // Specialisations for hashing and numerical limits.
 namespace std
 {
-template <MeasureType Type> struct hash<Measure<Type>>
+template <pyvrp::MeasureType Type> struct hash<pyvrp::Measure<Type>>
 {
-    size_t operator()(Measure<Type> const measure) const
+    size_t operator()(pyvrp::Measure<Type> const measure) const
     {
 #ifdef PYVRP_DOUBLE_PRECISION
         // When using double precision, this hashes 'equal' items differently
         // when they are very close to halfway between an integer value. Not
         // ideal, but this should work well enough for our application.
-        return std::hash<Value>()(std::round(measure.get()));
+        return std::hash<pyvrp::Value>()(std::round(measure.get()));
 #else
-        return std::hash<Value>()(measure.get());
+        return std::hash<pyvrp::Value>()(measure.get());
 #endif
     }
 };
 
-template <MeasureType Type> class numeric_limits<Measure<Type>>
+template <pyvrp::MeasureType Type> class numeric_limits<pyvrp::Measure<Type>>
 {
 public:  // TODO should return type be Measure<Type>?
-    static Value min() { return std::numeric_limits<Value>::min(); }
-    static Value max() { return std::numeric_limits<Value>::max(); }
-};
+    static pyvrp::Value max()
+    {
+        return std::numeric_limits<pyvrp::Value>::max();
+    }
 
+    static pyvrp::Value min()
+    {
+        return std::numeric_limits<pyvrp::Value>::min();
+    }
+};
 }  // namespace std
 
 #endif  // PYVRP_MEASURE_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/ProblemData.cpp` & `pyvrp-0.4.4/pyvrp/cpp/ProblemData.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #include "ProblemData.h"
 
-#include <cmath>
-#include <fstream>
 #include <numeric>
-#include <sstream>
-#include <string>
-#include <vector>
+
+using pyvrp::Distance;
+using pyvrp::Duration;
+using pyvrp::Matrix;
+using pyvrp::ProblemData;
 
 ProblemData::Client::Client(Coordinate x,
                             Coordinate y,
                             Load demand,
                             Duration serviceDuration,
                             Duration twEarly,
                             Duration twLate,
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/ProblemData.h` & `pyvrp-0.4.4/pyvrp/cpp/ProblemData.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #include "Matrix.h"
 #include "Measure.h"
 #include "XorShift128.h"
 
 #include <iosfwd>
 #include <vector>
 
+namespace pyvrp
+{
 class ProblemData
 {
 public:
     struct Client
     {
         Coordinate const x;
         Coordinate const y;
@@ -150,9 +152,10 @@
     return dist_(first, second);
 }
 
 Duration ProblemData::duration(size_t first, size_t second) const
 {
     return dur_(first, second);
 }
+}  // namespace pyvrp
 
 #endif  // PYVRP_PROBLEMDATA_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/README.md` & `pyvrp-0.4.4/pyvrp/cpp/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-# CPP
+# Native extensions
 
 This folder contains all C++ extension classes and functions. These extensions
 are ordered in the way they will appear in the `pyvrp` package: everything in
 this top-level folder will be made available in the top-level `pyvrp` package,
 whereas for example everything in `cpp/search` will be present in 
 `pyvrp.search` after installation (and so on for the other folders).
 
-When building on our implementation, please refrain from defining symbols 
-starting with the `PYVRP_` prefix. PyVRP reserves any such global declarations
-for internal use.
+> When building on our implementation, please refrain from defining symbols 
+> starting with the `PYVRP_` prefix. PyVRP reserves any such global declarations
+> for internal use.
 
-We use `pybind11` to generate the Python bindings for the C++ codebase. These
-bindings are generated in the `X_bindings.cpp` source files of each object `X`
-that we want to expose to Python. 
+## Bindings
+
+We use `pybind11` to generate Python bindings for the C++ codebase. These
+bindings are generated from the `bindings.cpp` source files of each folder. 
+Each `bindings.cpp` file is compiled into a single extension module named after
+the installation folder, prefixed with an underscore.
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/Solution.cpp` & `pyvrp-0.4.4/pyvrp/cpp/Solution.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 #include "Solution.h"
 #include "ProblemData.h"
 
 #include <fstream>
 #include <numeric>
 #include <unordered_map>
 
+using pyvrp::Cost;
+using pyvrp::Distance;
+using pyvrp::Duration;
+using pyvrp::Load;
+using pyvrp::Solution;
+
 using Client = int;
 using Visits = std::vector<Client>;
 using Routes = std::vector<Solution::Route>;
 
 void Solution::evaluate(ProblemData const &data)
 {
     Cost allPrizes = 0;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/Solution.h` & `pyvrp-0.4.4/pyvrp/cpp/Solution.h`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #include "ProblemData.h"
 #include "XorShift128.h"
 
 #include <functional>
 #include <iosfwd>
 #include <vector>
 
+namespace pyvrp
+{
 class Solution
 {
     using Client = int;
     using VehicleType = size_t;
 
 public:
     /**
@@ -187,29 +189,31 @@
      * Constructs a solution from the given list of Routes.
      *
      * @param data   Data instance describing the problem that's being solved.
      * @param routes Solution's route list.
      */
     Solution(ProblemData const &data, std::vector<Route> const &routes);
 };
+}  // namespace pyvrp
 
-std::ostream &operator<<(std::ostream &out, Solution const &sol);
-std::ostream &operator<<(std::ostream &out, Solution::Route const &route);
+std::ostream &operator<<(std::ostream &out, pyvrp::Solution const &sol);
+std::ostream &operator<<(std::ostream &out,
+                         pyvrp::Solution::Route const &route);
 
 namespace std
 {
-template <> struct hash<Solution>
+template <> struct hash<pyvrp::Solution>
 {
-    size_t operator()(Solution const &sol) const
+    size_t operator()(pyvrp::Solution const &sol) const
     {
         size_t res = 17;
         res = res * 31 + std::hash<size_t>()(sol.numRoutes());
-        res = res * 31 + std::hash<Distance>()(sol.distance());
-        res = res * 31 + std::hash<Load>()(sol.excessLoad());
-        res = res * 31 + std::hash<Duration>()(sol.timeWarp());
+        res = res * 31 + std::hash<pyvrp::Distance>()(sol.distance());
+        res = res * 31 + std::hash<pyvrp::Load>()(sol.excessLoad());
+        res = res * 31 + std::hash<pyvrp::Duration>()(sol.timeWarp());
 
         return res;
     }
 };
 }  // namespace std
 
 #endif  // PYVRP_SOLUTION_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/SubPopulation.cpp` & `pyvrp-0.4.4/pyvrp/cpp/SubPopulation.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #include "SubPopulation.h"
 
 #include <numeric>
 
+using pyvrp::SubPopulation;
 using const_iter = std::vector<SubPopulation::Item>::const_iterator;
 using iter = std::vector<SubPopulation::Item>::iterator;
 
-SubPopulation::SubPopulation(DiversityMeasure divOp,
+SubPopulation::SubPopulation(diversity::DiversityMeasure divOp,
                              PopulationParams const &params)
     : divOp(divOp), params(params)
 {
 }
 
 SubPopulation::~SubPopulation()
 {
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/SubPopulation.h` & `pyvrp-0.4.4/pyvrp/cpp/SubPopulation.h`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 #include "diversity/diversity.h"
 
 #include <functional>
 #include <iosfwd>
 #include <stdexcept>
 #include <vector>
 
+namespace pyvrp
+{
 struct PopulationParams
 {
     size_t minPopSize;
     size_t generationSize;
     size_t nbElite;
     size_t nbClose;
     double lbDiversity;
@@ -46,15 +48,15 @@
     }
 
     size_t maxPopSize() const { return minPopSize + generationSize; }
 };
 
 class SubPopulation
 {
-    DiversityMeasure divOp;
+    diversity::DiversityMeasure divOp;
     PopulationParams const &params;  // owned by Population, on the Python side
 
 public:
     struct Item
     {
         using Proximity = std::vector<std::pair<double, Solution const *>>;
 
@@ -77,15 +79,16 @@
 private:
     std::vector<Item> items;
 
     // Removes the element at the given iterator location from the items.
     void remove(std::vector<Item>::iterator const &iterator);
 
 public:
-    SubPopulation(DiversityMeasure divOp, PopulationParams const &params);
+    SubPopulation(diversity::DiversityMeasure divOp,
+                  PopulationParams const &params);
 
     ~SubPopulation();
 
     void add(Solution const *solution, CostEvaluator const &costEvaluator);
 
     std::vector<Item>::const_iterator cbegin() const;
 
@@ -97,9 +100,10 @@
 
     void purge(CostEvaluator const &costEvaluator);
 
     // Recomputes the fitness of all solutions maintained by this subpopulation.
     // This is called whenever a solution is added or removed.
     void updateFitness(CostEvaluator const &costEvaluator);
 };
+}  // namespace pyvrp
 
 #endif  // PYVRP_SUBPOPULATION_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/TimeWindowSegment.h` & `pyvrp-0.4.4/pyvrp/cpp/TimeWindowSegment.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #ifndef PYVRP_TIMEWINDOWSEGMENT_H
 #define PYVRP_TIMEWINDOWSEGMENT_H
 
 #include "Matrix.h"
 #include "Measure.h"
 
+namespace pyvrp
+{
 class TimeWindowSegment
 {
     using TWS = TimeWindowSegment;
 
     int idxFirst = 0;          // Index of the first client in the segment
     int idxLast = 0;           // Index of the last client in the segment
     Duration duration = 0;     // Total duration, incl. waiting and servicing
@@ -102,9 +104,10 @@
       duration(duration),
       timeWarp(timeWarp),
       twEarly(twEarly),
       twLate(twLate),
       releaseTime(releaseTime)
 {
 }
+}  // namespace pyvrp
 
 #endif  // PYVRP_TIMEWINDOWSEGMENT_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/XorShift128.cpp` & `pyvrp-0.4.4/pyvrp/cpp/XorShift128.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #include "XorShift128.h"
 
+using pyvrp::XorShift128;
+
 XorShift128::XorShift128(uint32_t seed)
 {
     state_[0] = seed;
     state_[1] = 123456789;
     state_[2] = 362436069;
     state_[3] = 521288629;
 }
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/XorShift128.h` & `pyvrp-0.4.4/pyvrp/cpp/XorShift128.h`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #define PYVRP_XORSHIFT128_H
 
 #include <cstddef>
 #include <cstdint>
 #include <limits>
 #include <type_traits>
 
+namespace pyvrp
+{
 /**
  * This class implements a XOR-shift pseudo-random number generator. It
  * generates the next number of a sequence by repeatedly taking the 'exclusive
  * or' (the ^ operator) of a number with a bit-shifted version of itself. See
  * also here for more details: https://en.wikipedia.org/wiki/Xorshift.
  */
 class XorShift128
@@ -33,30 +35,30 @@
 
     /**
      * @return The maximum value this pRNG can generate.
      */
     static constexpr size_t max();
 
     /**
-     * Generates one pseudo-random integer in the range <code>[min(), max()]
+     * Generates one pseudo-random integer in the range <code>[min(), max())
      * </code>.
      *
      * @return A pseudo-random integer.
      */
     result_type operator()();
 
     /**
      * Generators one pseudo-random double uniformly in the range [0, 1].
      *
      * @return A pseudo-random number in the range [0, 1].
      */
     template <typename T> T rand();
 
     /**
-     * Generates one pseudo-random integer in the range <code>[0, high]</code>.
+     * Generates one pseudo-random integer in the range <code>[0, high)</code>.
      *
      * @param high Upper bound on the integer to generate.
      * @return A pseudo-random integer.
      */
     template <typename T> result_type randint(T high);
 };
 
@@ -77,9 +79,10 @@
 }
 
 template <typename T> XorShift128::result_type XorShift128::randint(T high)
 {
     static_assert(std::is_integral<T>::value);
     return operator()() % high;
 }
+}  // namespace pyvrp
 
 #endif  // PYVRP_XORSHIFT128_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.cpp` & `pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 #include "crossover.h"
 #include "Measure.h"
 
 #include <cmath>
 #include <limits>
 
+using pyvrp::Cost;
+using pyvrp::Duration;
+
 using Client = int;
 using Route = std::vector<Client>;
 using Routes = std::vector<Route>;
 
 namespace
 {
 // Approximates the cost change of inserting client between prev and next.
 Cost deltaCost(Client client,
                Client prev,
                Client next,
-               ProblemData const &data,
-               [[maybe_unused]] CostEvaluator const &costEvaluator)
+               pyvrp::ProblemData const &data,
+               [[maybe_unused]] pyvrp::CostEvaluator const &costEvaluator)
 {
     auto const currDist = data.dist(prev, next);
     auto const propDist = data.dist(prev, client) + data.dist(client, next);
 
 #ifdef PYVRP_NO_TIME_WINDOWS
     return static_cast<Cost>(propDist - currDist);
 #else
@@ -54,18 +57,18 @@
     return static_cast<Cost>(propDist - currDist)
            + costEvaluator.twPenalty(clientTimeWarp + nextTimeWarp)  // proposed
            - costEvaluator.twPenalty(currTimeWarp);                  // current
 #endif
 }
 }  // namespace
 
-void crossover::greedyRepair(Routes &routes,
-                             std::vector<Client> const &unplanned,
-                             ProblemData const &data,
-                             CostEvaluator const &costEvaluator)
+void pyvrp::crossover::greedyRepair(Routes &routes,
+                                    pyvrp::DynamicBitset const &unplanned,
+                                    pyvrp::ProblemData const &data,
+                                    pyvrp::CostEvaluator const &costEvaluator)
 {
     auto const numRoutes = routes.size();
 
     // Determine centroids of each route.
     std::vector<std::pair<double, double>> centroids(numRoutes, {0, 0});
     for (size_t rIdx = 0; rIdx != numRoutes; ++rIdx)
         for (Client client : routes[rIdx])
@@ -74,16 +77,19 @@
             auto const x = static_cast<double>(data.client(client).x);
             auto const y = static_cast<double>(data.client(client).y);
 
             centroids[rIdx].first += x / size;
             centroids[rIdx].second += y / size;
         }
 
-    for (Client client : unplanned)
+    for (size_t client = 1; client != data.numClients() + 1; ++client)
     {
+        if (!unplanned[client])
+            continue;
+
         auto const x = static_cast<double>(data.client(client).x);
         auto const y = static_cast<double>(data.client(client).y);
 
         // Determine non-empty route with centroid nearest to this client.
         auto bestDistance = std::numeric_limits<double>::max();
         auto bestRouteIdx = 0;
         for (size_t rIdx = 0; rIdx != numRoutes; ++rIdx)
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/crossover/crossover.h` & `pyvrp-0.4.4/pyvrp/cpp/crossover/crossover.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #ifndef PYVRP_CROSSOVER_H
 #define PYVRP_CROSSOVER_H
 
 #include "CostEvaluator.h"
+#include "DynamicBitset.h"
 #include "ProblemData.h"
 #include "Solution.h"
 #include "XorShift128.h"
 
 #include <functional>
 #include <vector>
 
-namespace crossover
+namespace pyvrp::crossover
 {
 /**
  * Greedily inserts each unplanned client into the route that's nearest to the
  * client.
  */
 void greedyRepair(std::vector<std::vector<int>> &routes,
-                  std::vector<int> const &unplanned,
+                  DynamicBitset const &unplanned,
                   ProblemData const &data,
                   CostEvaluator const &costEvaluator);
-}  // namespace crossover
 
 /**
  * Performs two SREX crossovers of the given parents. SREX is a method that
  * selects a set of routes for each parent and replaces the selected routes of
  * the first parent with those of the second parent. The routes are selected by
  * minimizing the overlap between the two sets of routes. This is achieved
  * through a heuristic that iteratively shifts adjacent routes until no further
@@ -46,9 +46,10 @@
  */
 Solution selectiveRouteExchange(
     std::pair<Solution const *, Solution const *> const &parents,
     ProblemData const &data,
     CostEvaluator const &costEvaluator,
     std::pair<size_t, size_t> const startIndices,
     size_t const numMovedRoutes);
+}  // namespace pyvrp::crossover
 
 #endif  // PYVRP_CROSSOVER_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/crossover/selective_route_exchange.cpp` & `pyvrp-0.4.4/pyvrp/cpp/crossover/selective_route_exchange.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,45 @@
 #include "crossover.h"
 
-#include <cassert>
+#include "DynamicBitset.h"
+
 #include <cmath>
-#include <unordered_set>
 
 using Client = int;
 using Clients = std::vector<Client>;
-using ClientSet = std::unordered_set<Client>;
-using Route = Solution::Route;
+using Route = pyvrp::Solution::Route;
 using Routes = std::vector<Route>;
 
 namespace
 {
 // Angle of the given route w.r.t. the centroid of all client locations.
-double routeAngle(ProblemData const &data, Route const &route)
+double routeAngle(pyvrp::ProblemData const &data, Route const &route)
 {
     // This computes a pseudo-angle that sorts roughly equivalently to the atan2
     // angle, but is much faster to compute. See the following post for details:
     // https://stackoverflow.com/a/16561333/4316405.
     auto const [dataX, dataY] = data.centroid();
     auto const [routeX, routeY] = route.centroid();
     auto const dx = routeX - dataX;
     auto const dy = routeY - dataY;
     return std::copysign(1. - dx / (std::fabs(dx) + std::fabs(dy)), dy);
 }
 
-Routes sortByAscAngle(ProblemData const &data, Routes routes)
+Routes sortByAscAngle(pyvrp::ProblemData const &data, Routes routes)
 {
     auto cmp = [&data](Route a, Route b) {
         return routeAngle(data, a) < routeAngle(data, b);
     };
 
     std::sort(routes.begin(), routes.end(), cmp);
     return routes;
 }
 }  // namespace
 
-Solution selectiveRouteExchange(
+pyvrp::Solution pyvrp::crossover::selectiveRouteExchange(
     std::pair<Solution const *, Solution const *> const &parents,
     ProblemData const &data,
     CostEvaluator const &costEvaluator,
     std::pair<size_t, size_t> const startIndices,
     size_t const numMovedRoutes)
 {
     // We create two candidate offsprings, both based on parent A:
@@ -77,158 +76,152 @@
         throw std::invalid_argument(msg);
     }
 
     // Sort parents' routes by (ascending) polar angle.
     auto const routesA = sortByAscAngle(data, parents.first->getRoutes());
     auto const routesB = sortByAscAngle(data, parents.second->getRoutes());
 
-    ClientSet selectedA;
-    ClientSet selectedB;
+    DynamicBitset selectedA(data.numClients() + 1);
+    DynamicBitset selectedB(data.numClients() + 1);
 
     // Routes are sorted on polar angle, so selecting adjacent routes in both
     // parents should result in a large overlap when the start indices are
     // close to each other.
     for (size_t r = 0; r < numMovedRoutes; r++)
     {
-        auto const &routeA = routesA[(startA + r) % nRoutesA];
-        selectedA.insert(routeA.begin(), routeA.end());
+        for (Client c : routesA[(startA + r) % nRoutesA])
+            selectedA[c] = true;
 
-        auto const &routeB = routesB[(startB + r) % nRoutesB];
-        selectedB.insert(routeB.begin(), routeB.end());
+        for (Client c : routesB[(startB + r) % nRoutesB])
+            selectedB[c] = true;
     }
 
     // For the selection, we want to minimize |A\B| as these need replanning
     while (true)
     {
         // Difference for moving 'left' in parent A
         int differenceALeft = 0;
 
         for (Client c : routesA[(startA - 1 + nRoutesA) % nRoutesA])
-            differenceALeft += !selectedB.contains(c);
+            differenceALeft += !selectedB[c];
 
         for (Client c : routesA[(startA + numMovedRoutes - 1) % nRoutesA])
-            differenceALeft -= !selectedB.contains(c);
+            differenceALeft -= !selectedB[c];
 
         // Difference for moving 'right' in parent A
         int differenceARight = 0;
 
         for (Client c : routesA[(startA + numMovedRoutes) % nRoutesA])
-            differenceARight += !selectedB.contains(c);
+            differenceARight += !selectedB[c];
 
         for (Client c : routesA[startA])
-            differenceARight -= !selectedB.contains(c);
+            differenceARight -= !selectedB[c];
 
         // Difference for moving 'left' in parent B
         int differenceBLeft = 0;
 
         for (Client c : routesB[(startB - 1 + numMovedRoutes) % nRoutesB])
-            differenceBLeft += selectedA.contains(c);
+            differenceBLeft += selectedA[c];
 
         for (Client c : routesB[(startB - 1 + nRoutesB) % nRoutesB])
-            differenceBLeft -= selectedA.contains(c);
+            differenceBLeft -= selectedA[c];
 
         // Difference for moving 'right' in parent B
         int differenceBRight = 0;
 
         for (Client c : routesB[startB])
-            differenceBRight += selectedA.contains(c);
+            differenceBRight += selectedA[c];
 
         for (Client c : routesB[(startB + numMovedRoutes) % nRoutesB])
-            differenceBRight -= selectedA.contains(c);
+            differenceBRight -= selectedA[c];
 
         int const bestDifference = std::min({differenceALeft,
                                              differenceARight,
                                              differenceBLeft,
                                              differenceBRight});
 
         if (bestDifference >= 0)  // there are no further improving moves
             break;
 
         if (bestDifference == differenceALeft)
         {
             for (Client c : routesA[(startA + numMovedRoutes - 1) % nRoutesA])
-                selectedA.erase(c);
+                selectedA[c] = false;
 
             startA = (startA - 1 + nRoutesA) % nRoutesA;
-            selectedA.insert(routesA[startA].begin(), routesA[startA].end());
+            for (Client c : routesA[startA])
+                selectedA[c] = true;
         }
         else if (bestDifference == differenceARight)
         {
             for (Client c : routesA[startA])
-                selectedA.erase(c);
+                selectedA[c] = false;
 
             startA = (startA + 1) % nRoutesA;
-
             for (Client c : routesA[(startA + numMovedRoutes - 1) % nRoutesA])
-                selectedA.insert(c);
+                selectedA[c] = true;
         }
         else if (bestDifference == differenceBLeft)
         {
             for (Client c : routesB[(startB + numMovedRoutes - 1) % nRoutesB])
-                selectedB.erase(c);
+                selectedB[c] = false;
 
             startB = (startB - 1 + nRoutesB) % nRoutesB;
-            selectedB.insert(routesB[startB].begin(), routesB[startB].end());
+            for (Client c : routesB[startB])
+                selectedB[c] = true;
         }
         else if (bestDifference == differenceBRight)
         {
             for (Client c : routesB[startB])
-                selectedB.erase(c);
+                selectedB[c] = false;
 
             startB = (startB + 1) % nRoutesB;
             for (Client c : routesB[(startB + numMovedRoutes - 1) % nRoutesB])
-                selectedB.insert(c);
+                selectedB[c] = true;
         }
     }
 
     // Identify differences between route sets
-    ClientSet clientsInSelectedBNotA;
-    for (Client c : selectedB)
-        if (!selectedA.contains(c))
-            clientsInSelectedBNotA.insert(c);
+    auto const selectedBNotA = selectedB & ~selectedA;
 
     std::vector<std::vector<Client>> visits1(nRoutesA);
     std::vector<std::vector<Client>> visits2(nRoutesA);
 
     // Replace selected routes from parent A with routes from parent B
     for (size_t r = 0; r < numMovedRoutes; r++)
     {
         size_t indexA = (startA + r) % nRoutesA;
         size_t indexB = (startB + r) % nRoutesB;
 
         for (Client c : routesB[indexB])
         {
             visits1[indexA].push_back(c);  // c in B
 
-            if (!clientsInSelectedBNotA.contains(c))
+            if (!selectedBNotA[c])
                 visits2[indexA].push_back(c);  // c in A^B
         }
     }
 
     // Move routes from parent A that are kept
     for (size_t r = numMovedRoutes; r < nRoutesA; r++)
     {
         size_t indexA = (startA + r) % nRoutesA;
 
         for (Client c : routesA[indexA])
         {
-            if (!clientsInSelectedBNotA.contains(c))
+            if (!selectedBNotA[c])
                 visits1[indexA].push_back(c);  // c in Ac\B
 
             visits2[indexA].push_back(c);  // c in Ac
         }
     }
 
     // Insert unplanned clients (those that were in the removed routes of A, but
     // not the inserted routes of B).
-    Clients unplanned;
-    for (Client c : selectedA)
-        if (!selectedB.contains(c))
-            unplanned.push_back(c);
-
+    auto const unplanned = selectedA & ~selectedB;
     crossover::greedyRepair(visits1, unplanned, data, costEvaluator);
     crossover::greedyRepair(visits2, unplanned, data, costEvaluator);
 
     // Assign correct types to routes (from parents) and filter empty
     std::vector<Solution::Route> routes1;
     routes1.reserve(nRoutesA);
     std::vector<Solution::Route> routes2;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/diversity/broken_pairs_distance.cpp` & `pyvrp-0.4.4/pyvrp/cpp/diversity/broken_pairs_distance.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 #include "diversity.h"
 
-double brokenPairsDistance(Solution const &first, Solution const &second)
+double pyvrp::diversity::brokenPairsDistance(pyvrp::Solution const &first,
+                                             pyvrp::Solution const &second)
 {
     auto const &fNeighbours = first.getNeighbours();
     auto const &sNeighbours = second.getNeighbours();
 
     // The neighbours vector contains the depot, so its size is always at least
     // one. Thus numClients >= 0.
     size_t const numClients = fNeighbours.size() - 1;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/CircleSector.h` & `pyvrp-0.4.4/pyvrp/cpp/search/CircleSector.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 #ifndef PYVRP_CIRCLESECTOR_H
 #define PYVRP_CIRCLESECTOR_H
 
+namespace pyvrp::search
+{
 // Data structure to represent circle sectors
 // Angles are measured in [0,65535] instead of [0,359], in such a way that
 // modulo operations are much faster (since 2^16 = 65536) Credit to Fabian
 // Giesen at "https://web.archive.org/web/20200912191950" and
 // "https://fgiesen.wordpress.com/2015/09/24/intervals-in-modular-arithmetic/"
 // for useful implementation tips regarding interval overlaps in modular
 // arithmetics
@@ -74,9 +76,10 @@
             if (positive_mod(point - end) <= positive_mod(start - point))
                 end = point;
             else
                 start = point;
         }
     }
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_CIRCLESECTOR_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/Exchange.h` & `pyvrp-0.4.4/pyvrp/cpp/search/Exchange.h`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 #define PYVRP_EXCHANGE_H
 
 #include "LocalSearchOperator.h"
 #include "TimeWindowSegment.h"
 
 #include <cassert>
 
+namespace pyvrp::search
+{
 using TWS = TimeWindowSegment;
 
 /**
  * Template class that exchanges N consecutive nodes from U's route (starting at
  * U) with M consecutive nodes from V's route (starting at V). As special cases,
  * (1, 0) is pure relocate, and (1, 1) pure swap.
  */
@@ -313,9 +315,10 @@
     for (size_t count = 0; count != M; ++count)
     {
         U->swapWith(V);
         U = n(U);
         V = n(V);
     }
 }
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_EXCHANGE_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 #include <algorithm>
 #include <cassert>
 #include <numeric>
 #include <set>
 #include <stdexcept>
 #include <vector>
 
-using TWS = TimeWindowSegment;
+using pyvrp::Solution;
+using pyvrp::search::LocalSearch;
+using TWS = pyvrp::TimeWindowSegment;
 
 Solution LocalSearch::search(Solution &solution,
                              CostEvaluator const &costEvaluator)
 {
     loadSolution(solution);
 
     if (nodeOps.empty())
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearch.h` & `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearch.h`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 #include "Solution.h"
 #include "XorShift128.h"
 
 #include <functional>
 #include <stdexcept>
 #include <vector>
 
+namespace pyvrp::search
+{
 class LocalSearch
 {
     using NodeOp = LocalSearchOperator<Node>;
     using RouteOp = LocalSearchOperator<Route>;
     using Neighbours = std::vector<std::vector<int>>;
 
     ProblemData const &data;
@@ -105,9 +107,10 @@
      * Shuffles the order in which the node and route pairs are evaluated, and
      * the order in which node and route operators are applied.
      */
     void shuffle(XorShift128 &rng);
 
     LocalSearch(ProblemData const &data, Neighbours neighbours);
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_LOCALSEARCH_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/LocalSearchOperator.h` & `pyvrp-0.4.4/pyvrp/cpp/search/LocalSearchOperator.h`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #include "CostEvaluator.h"
 #include "Measure.h"
 #include "Node.h"
 #include "ProblemData.h"
 #include "Route.h"
 #include "Solution.h"
 
+namespace pyvrp::search
+{
 template <typename Arg> class LocalSearchOperatorBase
 {
     // Can only be specialised into either a Node or Route operator; there
     // are no other types that are expected to work.
     static_assert(std::is_same<Arg, Node>::value
                   || std::is_same<Arg, Route>::value);
 
@@ -70,9 +72,10 @@
     /**
      * Called when a route has been changed. Can be used to update caches, but
      * the implementation should be fast: this is called every time something
      * changes!
      */
     virtual void update([[maybe_unused]] Route *U){};
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_LOCALSEARCHOPERATOR_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/MoveTwoClientsReversed.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/MoveTwoClientsReversed.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #include "MoveTwoClientsReversed.h"
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
 #include <cassert>
 
-using TWS = TimeWindowSegment;
+using pyvrp::search::MoveTwoClientsReversed;
+using TWS = pyvrp::TimeWindowSegment;
 
-Cost MoveTwoClientsReversed::evaluate(Node *U,
-                                      Node *V,
-                                      CostEvaluator const &costEvaluator)
+pyvrp::Cost MoveTwoClientsReversed::evaluate(
+    Node *U, Node *V, pyvrp::CostEvaluator const &costEvaluator)
 {
     if (U == n(V) || n(U) == V || n(U)->isDepot())
         return 0;
 
     auto const posU = U->position;
     auto const posV = V->position;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/Node.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/Node.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 #include "Node.h"
 
+using pyvrp::search::Node;
+
 void Node::insertAfter(Node *other)
 {
     if (route)  // If we're in a route, we first stitch up the current route.
     {           // If we're not in a route, this step should be skipped.
         prev->next = next;
         next->prev = prev;
     }
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/Node.h` & `pyvrp-0.4.4/pyvrp/cpp/search/Node.h`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #ifndef PYVRP_NODE_H
 #define PYVRP_NODE_H
 
 #include "Measure.h"
 #include "TimeWindowSegment.h"
 
+namespace pyvrp::search
+{
 class Route;
 
 struct Node
 {
     int client;       // Client represented with this node
     size_t position;  // Position in the route
     Node *next;       // Next node in the route order
@@ -48,9 +50,10 @@
  */
 inline Node *p(Node *node) { return node->prev; }
 
 /**
  * Convenience method accessing the node directly after the argument.
  */
 inline Node *n(Node *node) { return node->next; }
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_NODE_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 #include "RelocateStar.h"
 
-Cost RelocateStar::evaluate(Route *U,
-                            Route *V,
-                            CostEvaluator const &costEvaluator)
+using pyvrp::search::RelocateStar;
+using pyvrp::search::Route;
+
+pyvrp::Cost RelocateStar::evaluate(Route *U,
+                                   Route *V,
+                                   pyvrp::CostEvaluator const &costEvaluator)
 {
     move = {};
 
     for (auto *nodeU = n(U->depot); !nodeU->isDepot(); nodeU = n(nodeU))
     {
         // Test inserting U after V's depot
         Cost deltaCost = relocate.evaluate(nodeU, V->depot, costEvaluator);
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/RelocateStar.h` & `pyvrp-0.4.4/pyvrp/cpp/search/RelocateStar.h`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #ifndef PYVRP_RELOCATESTAR_H
 #define PYVRP_RELOCATESTAR_H
 
 #include "Exchange.h"
 #include "LocalSearchOperator.h"
 
+namespace pyvrp::search
+{
 /**
  * Performs the best (1, 0)-exchange move between routes U and V. Tests both
  * ways: from U to V, and from V to U.
  */
 class RelocateStar : public LocalSearchOperator<Route>
 {
     struct Move
@@ -27,9 +29,10 @@
     void apply(Route *U, Route *V) const override;
 
     RelocateStar(ProblemData const &data)
         : LocalSearchOperator<Route>(data), relocate(data)
     {
     }
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_RELOCATESTAR_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/Route.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/Route.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 // TODO use std::numbers::pi instead of M_PI when C++20 is supported by CIBW
 
 #include "Route.h"
 
 #include <cmath>
 #include <ostream>
 
-using TWS = TimeWindowSegment;
+using pyvrp::search::Route;
+using TWS = pyvrp::TimeWindowSegment;
 
 Route::Route(ProblemData const &data, size_t const idx, size_t const vehType)
     : data(data), vehicleType_(vehType), idx(idx)
 {
 }
 
 void Route::setupNodes()
@@ -125,15 +126,15 @@
     load_ = nodes.back()->cumulatedLoad;
     isLoadFeasible_ = load_ <= capacity();
 
     timeWarp_ = nodes.back()->twBefore.totalTimeWarp();
     isTimeWarpFeasible_ = timeWarp_ == 0;
 }
 
-std::ostream &operator<<(std::ostream &out, Route const &route)
+std::ostream &operator<<(std::ostream &out, pyvrp::search::Route const &route)
 {
     out << "Route #" << route.idx + 1 << ":";  // route number
     for (auto *node = n(route.depot); !node->isDepot(); node = n(node))
         out << ' ' << node->client;  // client index
     out << '\n';
 
     return out;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/Route.h` & `pyvrp-0.4.4/pyvrp/cpp/search/Route.h`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 #include "TimeWindowSegment.h"
 
 #include <array>
 #include <bit>
 #include <cassert>
 #include <iosfwd>
 
+namespace pyvrp::search
+{
 class Route
 {
     ProblemData const &data;
     size_t const vehicleType_;
 
     std::vector<Node *> nodes;  // List of nodes (in order) in this solution.
     CircleSector sector;        // Circle sector of the route's clients
@@ -192,12 +194,13 @@
     auto const startLoad = startNode->cumulatedLoad;
     auto const endLoad = nodes[end - 1]->cumulatedLoad;
 
     assert(startLoad <= endLoad);
 
     return endLoad - startLoad + atStart;
 }
+}  // namespace pyvrp::search
 
 // Outputs a route into a given ostream in CVRPLib format
-std::ostream &operator<<(std::ostream &out, Route const &route);
+std::ostream &operator<<(std::ostream &out, pyvrp::search::Route const &route);
 
 #endif  // PYVRP_ROUTE_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 #include "SwapStar.h"
 
-using TWS = TimeWindowSegment;
+using pyvrp::Cost;
+using pyvrp::search::Node;
+using pyvrp::search::SwapStar;
+using TWS = pyvrp::TimeWindowSegment;
 
 void SwapStar::updateRemovalCosts(Route *R1, CostEvaluator const &costEvaluator)
 {
     for (Node *U = n(R1->depot); !U->isDepot(); U = n(U))
     {
         auto twData
             = TWS::merge(data.durationMatrix(), p(U)->twBefore, n(U)->twAfter);
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/SwapStar.h` & `pyvrp-0.4.4/pyvrp/cpp/search/SwapStar.h`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 #include "Matrix.h"
 #include "Measure.h"
 
 #include <array>
 #include <limits>
 #include <vector>
 
+namespace pyvrp::search
+{
 /**
  * Explores the SWAP* neighbourhood of [1]. The SWAP* neighbourhood explores
  * free form re-insertions of nodes U and V in the given routes (so the nodes
  * are exchanged between routes, but they are not necessarily inserted in
  * the same place as the other exchanged node). Our implementation of the
  * neighbourhood follows Algorithm 2 of [1] fairly faithfully.
  * <br />
@@ -103,9 +105,10 @@
         : LocalSearchOperator<Route>(data),
           cache(data.numVehicles(), data.numClients() + 1),
           removalCosts(data.numVehicles(), data.numClients() + 1),
           updated(data.numVehicles(), true)
     {
     }
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_SWAPSTAR_H
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.cpp` & `pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #include "TwoOpt.h"
 
 #include "Route.h"
 #include "TimeWindowSegment.h"
 
-using TWS = TimeWindowSegment;
+using pyvrp::Cost;
+using pyvrp::search::TwoOpt;
+using TWS = pyvrp::TimeWindowSegment;
 
 Cost TwoOpt::evalWithinRoute(Node *U,
                              Node *V,
                              CostEvaluator const &costEvaluator) const
 {
     if (U->position + 1 >= V->position)
         return 0;
```

### Comparing `pyvrp-0.4.2/pyvrp/cpp/search/TwoOpt.h` & `pyvrp-0.4.4/pyvrp/cpp/search/TwoOpt.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #ifndef PYVRP_TWOOPT_H
 #define PYVRP_TWOOPT_H
 
 #include "LocalSearchOperator.h"
 
+namespace pyvrp::search
+{
 /**
  * 2-OPT moves.
  *
  * Between routes: replaces U -> X and V -> Y by U -> Y and V -> X, if that is
  * an improving move. Within route: replaces U -> X and V -> Y by U -> V and
  * X -> Y, if that is an improving move.
  */
@@ -27,9 +29,10 @@
 
 public:
     Cost
     evaluate(Node *U, Node *V, CostEvaluator const &costEvaluator) override;
 
     void apply(Node *U, Node *V) const override;
 };
+}  // namespace pyvrp::search
 
 #endif  // PYVRP_TWOOPT_H
```

### Comparing `pyvrp-0.4.2/pyvrp/crossover/selective_route_exchange.py` & `pyvrp-0.4.4/pyvrp/crossover/selective_route_exchange.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from typing import Tuple
 
-from pyvrp._CostEvaluator import CostEvaluator
-from pyvrp._ProblemData import ProblemData
-from pyvrp._Solution import Solution
-from pyvrp._XorShift128 import XorShift128
+from pyvrp._pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
 
-from ._selective_route_exchange import selective_route_exchange as _srex
+from ._crossover import selective_route_exchange as _srex
 
 
 def selective_route_exchange(
     parents: Tuple[Solution, Solution],
     data: ProblemData,
     cost_evaluator: CostEvaluator,
     rng: XorShift128,
@@ -42,19 +39,21 @@
     .. [1] Nagata, Y., & Kobayashi, S. (2010). A Memetic Algorithm for the
            Pickup and Delivery Problem with Time Windows Using Selective Route
            Exchange Crossover. *Parallel Problem Solving from Nature*, PPSN XI,
            536 - 545.
     """
     first, second = parents
 
+    if first.num_clients() == 0:
+        return second
+
+    if second.num_clients() == 0:
+        return first
+
     idx1 = rng.randint(first.num_routes())
     idx2 = idx1 if idx1 < second.num_routes() else 0
     max_routes_to_move = min(first.num_routes(), second.num_routes())
-
-    if max_routes_to_move == 0:  # rng.randint() cannot be called in this case
-        num_routes_to_move = 1
-    else:
-        num_routes_to_move = rng.randint(max_routes_to_move) + 1
+    num_routes_to_move = rng.randint(max_routes_to_move) + 1
 
     return _srex(
         parents, data, cost_evaluator, (idx1, idx2), num_routes_to_move
     )
```

### Comparing `pyvrp-0.4.2/pyvrp/crossover/tests/test_selective_route_exchange.py` & `pyvrp-0.4.4/pyvrp/crossover/tests/test_selective_route_exchange.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import itertools
 
 from numpy.testing import assert_equal, assert_raises
 from pytest import mark
 
 from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
 from pyvrp.crossover import selective_route_exchange as srex
-from pyvrp.crossover._selective_route_exchange import (
-    selective_route_exchange as cpp_srex,
-)
+from pyvrp.crossover._crossover import selective_route_exchange as cpp_srex
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_same_parents_same_offspring():
     """
     Tests that SREX produces identical offspring when both parents are the
     same.
@@ -22,14 +20,33 @@
 
     solution = Solution(data, [[1, 2], [3, 4]])
     offspring = srex((solution, solution), data, cost_evaluator, rng)
 
     assert_equal(offspring, solution)
 
 
+def test_srex_empty_solution():
+    data = read("data/p06-2-50.vrp", round_func="dimacs")
+    cost_evaluator = CostEvaluator(20, 6)
+    rng = XorShift128(seed=42)
+
+    empty = Solution(data, [])
+    nonempty = Solution(data, [[1, 2, 3, 4]])
+
+    # If both parents are empty the returned offspring must also be empty.
+    offspring = srex((empty, empty), data, cost_evaluator, rng)
+    assert_equal(offspring, empty)
+
+    # If one of the two parents is empty but the other is not, the returned
+    # solution is the nonempty parent.
+    for parents in [(empty, nonempty), (nonempty, empty)]:
+        offspring = srex(parents, data, cost_evaluator, rng)
+        assert_equal(offspring, nonempty)
+
+
 @mark.parametrize(
     "idx1, idx2, num_moved_routes",
     [
         (10, 0, 1),  # idx1 >= # routes first
         (0, 10, 1),  # idx2 >= # routes second
         (0, 0, 0),  # num_moved_routes < 1
         (0, 0, 2),  # num_moved_routes > min(# routes first, # routes second)
```

### Comparing `pyvrp-0.4.2/pyvrp/diversity/_broken_pairs_distance.pyi` & `pyvrp-0.4.4/pyvrp/diversity/_diversity.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyvrp._Solution import Solution
+from pyvrp._pyvrp import Solution
 
 def broken_pairs_distance(first: Solution, second: Solution) -> float:
     """
     Computes the symmetric broken pairs distance (BPD) between the given two
     solutions. This function determines whether each client in the problem
     shares neighbours between the first and second solution. If not, the
     client is part of a 'broken pair': a link that is part of one solution,
```

### Comparing `pyvrp-0.4.2/pyvrp/diversity/tests/test_broken_pairs_distance.py` & `pyvrp-0.4.4/pyvrp/diversity/tests/test_broken_pairs_distance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/exceptions.py` & `pyvrp-0.4.4/pyvrp/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_coordinates.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_coordinates.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_demands.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_demands.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_diversity.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_diversity.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_instance.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_instance.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_objectives.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_objectives.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_result.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_route_schedule.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_route_schedule.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_runtimes.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_runtimes.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_solution.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_solution.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/plot_time_windows.py` & `pyvrp-0.4.4/pyvrp/plotting/plot_time_windows.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png` & `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_instance.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png` & `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_result.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png` & `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_route_schedule.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png` & `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png` & `pyvrp-0.4.4/pyvrp/plotting/tests/baseline_images/test_plotting/plot_solution_with_customers.png`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/plotting/tests/test_plotting.py` & `pyvrp-0.4.4/pyvrp/plotting/tests/test_plotting.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/read.py` & `pyvrp-0.4.4/pyvrp/read.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import numpy as np
 import vrplib
 
 from pyvrp.constants import MAX_USER_VALUE
 from pyvrp.exceptions import ScalingWarning
 
-from ._ProblemData import Client, ProblemData, VehicleType
+from ._pyvrp import Client, ProblemData, VehicleType
 
 _Routes = List[List[int]]
 _RoundingFunc = Callable[[np.ndarray], np.ndarray]
 
 _INT_MAX = np.iinfo(np.int32).max
```

### Comparing `pyvrp-0.4.2/pyvrp/search/LocalSearch.py` & `pyvrp-0.4.4/pyvrp/search/LocalSearch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,13 @@
 from typing import List
 
-from pyvrp._CostEvaluator import CostEvaluator
-from pyvrp._ProblemData import ProblemData
-from pyvrp._Solution import Solution
-from pyvrp._XorShift128 import XorShift128
+from pyvrp import CostEvaluator, ProblemData, Solution, XorShift128
 
-from ._LocalSearch import LocalSearch as _LocalSearch
-
-Neighbours = List[List[int]]
+from ._search import LocalSearch as _LocalSearch
+from ._search import NodeOperator, RouteOperator
 
 
 class LocalSearch:
     """
     Local search method. This search method explores a granular neighbourhood
     in a very efficient manner using user-provided node and route operators.
     This quickly results in much improved solutions.
@@ -23,57 +19,57 @@
     rng
         Random number generator.
     neighbours
         List of lists that defines the local search neighbourhood.
     """
 
     def __init__(
-        self, data: ProblemData, rng: XorShift128, neighbours: Neighbours
+        self, data: ProblemData, rng: XorShift128, neighbours: List[List[int]]
     ):
         self._ls = _LocalSearch(data, neighbours)
         self._rng = rng
 
-    def add_node_operator(self, op):
+    def add_node_operator(self, op: NodeOperator):
         """
         Adds a node operator to this local search object. The node operator
         will be used by :meth:`~search` to improve a solution.
 
         Parameters
         ----------
         op
             The node operator to add to this local search object.
         """
         self._ls.add_node_operator(op)
 
-    def add_route_operator(self, op):
+    def add_route_operator(self, op: RouteOperator):
         """
         Adds a route operator to this local search object. The route operator
         will be used by :meth:`~intensify` to improve a solution using more
         expensive route operators.
 
         Parameters
         ----------
         op
             The route operator to add to this local search object.
         """
         self._ls.add_route_operator(op)
 
-    def set_neighbours(self, neighbours: Neighbours):
+    def set_neighbours(self, neighbours: List[List[int]]):
         """
         Convenience method to replace the current granular neighbourhood used
         by the local search object.
 
         Parameters
         ----------
         neighbours
             A new granular neighbourhood.
         """
         self._ls.set_neighbours(neighbours)
 
-    def get_neighbours(self) -> Neighbours:
+    def get_neighbours(self) -> List[List[int]]:
         """
         Returns the granular neighbourhood currently used by the local search.
 
         Returns
         -------
         list
             The current granular neighbourhood.
```

### Comparing `pyvrp-0.4.2/pyvrp/search/__init__.py` & `pyvrp-0.4.4/pyvrp/search/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from .LocalSearch import LocalSearch
-from ._Exchange import (
+from ._search import (
     Exchange10,
     Exchange11,
     Exchange20,
     Exchange21,
     Exchange22,
     Exchange30,
     Exchange31,
     Exchange32,
     Exchange33,
+    MoveTwoClientsReversed,
+    NodeOperator,
+    RelocateStar,
+    RouteOperator,
+    SwapStar,
+    TwoOpt,
 )
-from ._MoveTwoClientsReversed import MoveTwoClientsReversed
-from ._RelocateStar import RelocateStar
-from ._SwapStar import SwapStar
-from ._TwoOpt import TwoOpt
-from .neighbourhood import NeighbourhoodParams, Neighbours, compute_neighbours
+from .neighbourhood import NeighbourhoodParams, compute_neighbours
 
 NODE_OPERATORS = [
     Exchange10,
     Exchange20,
     Exchange30,
     Exchange11,
     Exchange21,
```

### Comparing `pyvrp-0.4.2/pyvrp/search/neighbourhood.py` & `pyvrp-0.4.4/pyvrp/search/neighbourhood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import List
 
 import numpy as np
 
-from pyvrp._ProblemData import ProblemData
-
-Neighbours = List[List[int]]
+from pyvrp import ProblemData
 
 
 @dataclass
 class NeighbourhoodParams:
     """
     Configuration for calculating a granular neighbourhood.
 
@@ -52,28 +50,28 @@
     def __post_init__(self):
         if self.nb_granular <= 0:
             raise ValueError("nb_granular <= 0 not understood.")
 
 
 def compute_neighbours(
     data: ProblemData, params: NeighbourhoodParams = NeighbourhoodParams()
-) -> Neighbours:
+) -> List[List[int]]:
     """
     Computes neighbours defining the neighbourhood for a problem instance.
 
     Parameters
     ----------
     data
         ProblemData for which to compute the neighbourhood.
     params
         NeighbourhoodParams that define how the neighbourhood is computed.
 
     Returns
     -------
-    Neighbours
+    list
         A list of list of integers representing the neighbours for each client.
         The first element represents the depot and is an empty list.
     """
     proximity = _compute_proximity(
         data,
         params.weight_wait_time,
         params.weight_time_warp,
```

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_Exchange.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_Exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,27 @@
     CostEvaluator,
     ProblemData,
     Route,
     Solution,
     VehicleType,
     XorShift128,
 )
-from pyvrp.search import LocalSearch, NeighbourhoodParams, compute_neighbours
-from pyvrp.search._Exchange import (
+from pyvrp.search import (
     Exchange10,
     Exchange11,
     Exchange20,
     Exchange21,
     Exchange22,
     Exchange30,
     Exchange31,
     Exchange32,
     Exchange33,
+    LocalSearch,
+    NeighbourhoodParams,
+    compute_neighbours,
 )
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 @mark.parametrize(
     "operator",
     [
```

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_LocalSearch.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_LocalSearch.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 
 from pyvrp import CostEvaluator, Route, Solution, VehicleType, XorShift128
 from pyvrp.search import (
     Exchange10,
     Exchange11,
     LocalSearch,
     NeighbourhoodParams,
-    Neighbours,
     compute_neighbours,
 )
-from pyvrp.search._LocalSearch import LocalSearch as cpp_LocalSearch
+from pyvrp.search._search import LocalSearch as cpp_LocalSearch
 from pyvrp.tests.helpers import make_heterogeneous, read
 
 
 def test_local_search_raises_when_there_are_no_operators():
     data = read("data/OkSmall.txt")
     cost_evaluator = CostEvaluator(20, 6)
     rng = XorShift128(seed=42)
@@ -140,15 +139,15 @@
     sol = Solution(data, [[1, 2, 3, 4]])
 
     # We make neighbours only contain 1 -> 2, so the only feasible move
     # is changing [1, 2, 3, 4] into [2, 1, 3, 4] or moving one of the nodes
     # into its own route. Since those solutions have larger distance but
     # smaller time warp, they are considered improving moves with a
     # sufficiently large time warp penalty.
-    neighbours: Neighbours = [[], [2], [], [], []]  # 1 -> 2 only
+    neighbours = [[], [2], [], [], []]  # 1 -> 2 only
     ls = LocalSearch(data, rng, neighbours)
     ls.add_node_operator(Exchange10(data))
 
     # With 0 timewarp penalty, the solution should not change since
     # the solution [2, 1, 3, 4] has larger distance
     improved_sol = ls.search(sol, CostEvaluator(0, 0))
     assert_equal(sol, improved_sol)
```

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_MoveTwoClientsReversed.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_MoveTwoClientsReversed.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_RelocateStar.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_RelocateStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_SwapStar.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_SwapStar.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_TwoOpt.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_TwoOpt.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/search/tests/test_neighbourhood.py` & `pyvrp-0.4.4/pyvrp/search/tests/test_neighbourhood.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/show_versions.py` & `pyvrp-0.4.4/pyvrp/show_versions.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/MaxRuntime.py` & `pyvrp-0.4.4/pyvrp/stop/MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/NoImprovement.py` & `pyvrp-0.4.4/pyvrp/stop/NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/StoppingCriterion.py` & `pyvrp-0.4.4/pyvrp/stop/StoppingCriterion.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/TimedNoImprovement.py` & `pyvrp-0.4.4/pyvrp/stop/TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/tests/test_MaxIterations.py` & `pyvrp-0.4.4/pyvrp/stop/tests/test_MaxIterations.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/tests/test_MaxRuntime.py` & `pyvrp-0.4.4/pyvrp/stop/tests/test_MaxRuntime.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/tests/test_NoImprovement.py` & `pyvrp-0.4.4/pyvrp/stop/tests/test_NoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/stop/tests/test_TimedNoImprovement.py` & `pyvrp-0.4.4/pyvrp/stop/tests/test_TimedNoImprovement.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/E-n22-k4.txt` & `pyvrp-0.4.4/pyvrp/tests/data/E-n22-k4.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNoExplicit.txt` & `pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNoExplicit.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt` & `pyvrp-0.4.4/pyvrp/tests/data/EdgeWeightsNotFullMatrix.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/OkSmall.txt` & `pyvrp-0.4.4/pyvrp/tests/data/OkSmall.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/OkSmallGreedyRepair.txt` & `pyvrp-0.4.4/pyvrp/tests/data/OkSmallGreedyRepair.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/OkSmallPrizes.txt` & `pyvrp-0.4.4/pyvrp/tests/data/OkSmallPrizes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/OkSmallReleaseTimes.txt` & `pyvrp-0.4.4/pyvrp/tests/data/OkSmallReleaseTimes.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/RC208.txt` & `pyvrp-0.4.4/pyvrp/tests/data/RC208.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/ReallyLargeDistance.txt` & `pyvrp-0.4.4/pyvrp/tests/data/ReallyLargeDistance.txt`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/data/p06-2-50.vrp` & `pyvrp-0.4.4/pyvrp/tests/data/p06-2-50.vrp`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/helpers.py` & `pyvrp-0.4.4/pyvrp/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_CostEvaluator.py` & `pyvrp-0.4.4/pyvrp/tests/test_CostEvaluator.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_GeneticAlgorithm.py` & `pyvrp-0.4.4/pyvrp/tests/test_GeneticAlgorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     "intensify_probability,"
     "intensify_on_best,"
     "nb_iter_no_improvement",
     [
         (-0.25, True, 0.5, True, 0),  # repair_probability < 0
         (1.25, True, 0.5, True, 0),  # repair_probability > 1
         (0.0, True, 0.5, True, -1),  # nb_iter_no_improvement < 0
+        (0.0, True, -0.25, True, 1),  # intensify_probability < 0
+        (0.0, True, 1.25, True, 1),  # intensify_probability > 1
     ],
 )
 def test_params_constructor_throws_when_arguments_invalid(
     repair_probability: float,
     collect_statistics: bool,
     intensify_probability: int,
     intensify_on_best: bool,
```

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Matrix.py` & `pyvrp-0.4.4/pyvrp/tests/test_Matrix.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from numpy.testing import assert_equal, assert_raises
 
-from pyvrp._Matrix import Matrix
+from pyvrp._pyvrp import Matrix
 
 
 def test_dimension_constructor():
     square = Matrix(10)
     assert_equal(square.num_rows, 10)
     assert_equal(square.num_cols, 10)
     assert_equal(square.size(), 10 * 10)
```

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Model.py` & `pyvrp-0.4.4/pyvrp/tests/test_Model.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_PenaltyManager.py` & `pyvrp-0.4.4/pyvrp/tests/test_PenaltyManager.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Population.py` & `pyvrp-0.4.4/pyvrp/tests/test_Population.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_ProblemData.py` & `pyvrp-0.4.4/pyvrp/tests/test_ProblemData.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Result.py` & `pyvrp-0.4.4/pyvrp/tests/test_Result.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Solution.py` & `pyvrp-0.4.4/pyvrp/tests/test_Solution.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_Statistics.py` & `pyvrp-0.4.4/pyvrp/tests/test_Statistics.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_SubPopulation.py` & `pyvrp-0.4.4/pyvrp/tests/test_SubPopulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from numpy.testing import assert_, assert_allclose, assert_equal
 from pytest import mark
 
-from pyvrp import CostEvaluator, Solution, XorShift128
-from pyvrp._SubPopulation import PopulationParams, SubPopulation
+from pyvrp import CostEvaluator, PopulationParams, Solution, XorShift128
+from pyvrp._pyvrp import SubPopulation
 from pyvrp.diversity import broken_pairs_distance as bpd
 from pyvrp.tests.helpers import read
 
 
 @mark.parametrize("nb_close", [5, 10, 25])
 def test_avg_distance_closest_is_same_up_to_nb_close(nb_close: int):
     data = read("data/RC208.txt", "solomon", "dimacs")
```

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_TimeWindowSegment.py` & `pyvrp-0.4.4/pyvrp/tests/test_TimeWindowSegment.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from numpy.testing import assert_equal
 from pytest import mark
 
-from pyvrp._Matrix import Matrix
-from pyvrp._TimeWindowSegment import TimeWindowSegment
+from pyvrp._pyvrp import Matrix, TimeWindowSegment
 
 
 @mark.parametrize("existing_time_warp", [2, 5, 10])
 def test_total_time_warp(existing_time_warp):
     tws1 = TimeWindowSegment(0, 0, 0, existing_time_warp, 0, 0, 0)
     assert_equal(tws1.total_time_warp(), existing_time_warp)
```

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_XorShift128.py` & `pyvrp-0.4.4/pyvrp/tests/test_XorShift128.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 from numpy.testing import assert_, assert_allclose, assert_equal
 from pytest import mark
 
-from pyvrp._XorShift128 import XorShift128
+from pyvrp import XorShift128
 
 
 def test_bounds():
     assert_equal(XorShift128.min(), 0)
     assert_equal(XorShift128.max(), np.iinfo(np.uint32).max)
```

### Comparing `pyvrp-0.4.2/pyvrp/tests/test_read.py` & `pyvrp-0.4.4/pyvrp/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `pyvrp-0.4.2/PKG-INFO` & `pyvrp-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvrp
-Version: 0.4.2
+Version: 0.4.4
 Summary: A state-of-the-art vehicle routing problem solver.
 Home-page: https://github.com/PyVRP/PyVRP
 License: MIT
 Author: Niels Wouda
 Author-email: nielswouda@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

