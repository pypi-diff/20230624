# Comparing `tmp/apricopt-0.0.2a3.dev8.tar.gz` & `tmp/apricopt-0.0.2a3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apricopt-0.0.2a3.dev8.tar", last modified: Tue Mar 15 15:02:48 2022, max compression
+gzip compressed data, was "apricopt-0.0.2a3.dev9.tar", last modified: Mon Apr 11 21:17:36 2022, max compression
```

## Comparing `apricopt-0.0.2a3.dev8.tar` & `apricopt-0.0.2a3.dev9.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    35148 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/COPYING
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2131 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/PKG-INFO
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1614 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/README.md
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.284244 apricopt-0.0.2a3.dev8/apricopt/
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.284244 apricopt-0.0.2a3.dev8/apricopt/IO/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/IO/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4076 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/IO/data_input.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/model/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1298 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/FastObservable.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10286 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/Model.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1610 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/ModelInstance.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     7670 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/Observable.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     7524 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/ObservableFunction.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      359 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/ObservableFunctionNotFoundError.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1376 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/Parameter.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/model/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/sampling/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3900 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/sampling/Sampler.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/sampling/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/simulation/
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10736 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/COPASIEngine.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    12241 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/COPASIModelInstance.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1530 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/MockUpModelInstance.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1951 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/MockUpSimulationEngine.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3434 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/SimulationEngine.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     6012 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/RoadRunnerEngine.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3014 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/RoadRunnerModelInstance.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/solving/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10702 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/BlackBox.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2388 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/BlackBoxSolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     8989 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/FunctionBlackBox.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/MockUp/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2557 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/MockUp/MockUpSolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/MockUp/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/NOMAD/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     9203 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/NOMAD/NOMADSolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/NOMAD/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     6582 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/SimulableModelBlackBox.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.288244 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/pyswarms/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4648 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/pyswarms/PySwarmsSolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/pyswarms/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/scipy/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4530 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/scipy/SciPySolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/scipy/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2482 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASIOptimisationMethod.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    12208 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASISolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      876 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASISolverParameter.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2028 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIDifferentialEvolution.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1989 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryProgramming.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2059 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryStrategySR.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2002 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithm.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2097 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithmSR.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1830 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIHookeJeeves.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1996 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASILevenbergMarquardt.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1837 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASINelderMead.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2032 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIParticleSwarm.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1617 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIPraxis.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1757 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIRandomSearch.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1830 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIScatterSearch.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1985 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASISimulatedAnnealing.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1778 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASISteepestDescent.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1512 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASITruncatedNewton.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1721 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/WhiteBoxSolver.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/mockup/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/mockup/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/model/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/model/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1138 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/model/formulas.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/model/observables/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/model/observables/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1217 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/model/observables/main.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3374 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/GriewankBB.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/NOMAD/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      993 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/NOMAD/GriewankTest.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/NOMAD/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1493 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/ackley.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2815 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/MockUpBlackBox.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1554 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/mockup_test.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1382 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/ackley_test.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1231 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/sphere_test.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/scipy/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/scipy/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1969 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/scipy/sphere_test.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1156 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/sphere.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/stybtang.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     5933 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MaxRosenbrock.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     5846 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MinRosenbrock.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/__init__.py
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/__init__.py
-drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-03-15 15:02:48.284244 apricopt-0.0.2a3.dev8/apricopt.egg-info/
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2131 2022-03-15 15:02:48.000000 apricopt-0.0.2a3.dev8/apricopt.egg-info/PKG-INFO
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4315 2022-03-15 15:02:48.000000 apricopt-0.0.2a3.dev8/apricopt.egg-info/SOURCES.txt
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        1 2022-03-15 15:02:48.000000 apricopt-0.0.2a3.dev8/apricopt.egg-info/dependency_links.txt
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      362 2022-03-15 15:02:48.000000 apricopt-0.0.2a3.dev8/apricopt.egg-info/requires.txt
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        9 2022-03-15 15:02:48.000000 apricopt-0.0.2a3.dev8/apricopt.egg-info/top_level.txt
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)       38 2022-03-15 15:02:48.292245 apricopt-0.0.2a3.dev8/setup.cfg
--rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1335 2022-03-15 15:00:42.000000 apricopt-0.0.2a3.dev8/setup.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    35148 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/COPYING
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2160 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/PKG-INFO
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1643 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/README.md
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.465011 apricopt-0.0.2a3.dev9/apricopt/
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.465011 apricopt-0.0.2a3.dev9/apricopt/IO/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/IO/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4076 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/IO/data_input.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/model/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1298 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/FastObservable.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10286 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/Model.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1610 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/ModelInstance.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     7670 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/Observable.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     7524 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/ObservableFunction.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      359 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/ObservableFunctionNotFoundError.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1453 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/Parameter.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/model/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/sampling/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3996 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/sampling/Sampler.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/sampling/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/simulation/
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10766 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/COPASIEngine.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    12241 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/COPASIModelInstance.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1530 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/MockUpModelInstance.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1951 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/MockUpSimulationEngine.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3457 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/SimulationEngine.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     6335 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/RoadRunnerEngine.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3014 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/RoadRunnerModelInstance.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    10702 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/BlackBox.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2388 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/BlackBoxSolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     8989 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/FunctionBlackBox.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/MockUp/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2557 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/MockUp/MockUpSolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/MockUp/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/NOMAD/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     9203 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/NOMAD/NOMADSolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/NOMAD/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     6582 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/SimulableModelBlackBox.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/pyswarms/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4648 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/pyswarms/PySwarmsSolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/pyswarms/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/scipy/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4530 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/scipy/SciPySolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/scipy/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.469010 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2482 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASIOptimisationMethod.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)    12208 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASISolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      876 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASISolverParameter.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2028 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIDifferentialEvolution.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1989 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryProgramming.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2059 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryStrategySR.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2002 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithm.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2097 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithmSR.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1830 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIHookeJeeves.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1996 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASILevenbergMarquardt.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1837 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASINelderMead.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2032 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIParticleSwarm.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1617 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIPraxis.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1757 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIRandomSearch.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1830 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIScatterSearch.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1985 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASISimulatedAnnealing.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1778 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASISteepestDescent.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1512 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASITruncatedNewton.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1721 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/WhiteBoxSolver.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/mockup/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/mockup/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/model/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/model/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1138 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/model/formulas.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/model/observables/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/model/observables/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1217 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/model/observables/main.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     3374 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/GriewankBB.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/NOMAD/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      993 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/NOMAD/GriewankTest.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/NOMAD/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1493 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/ackley.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2815 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/MockUpBlackBox.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1554 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/mockup_test.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1382 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/ackley_test.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1231 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/sphere_test.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/scipy/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/scipy/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1969 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/scipy/sphere_test.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1156 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/sphere.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/stybtang.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     5933 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MaxRosenbrock.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     5846 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MinRosenbrock.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/__init__.py
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/__init__.py
+drwxrwxr-x   0 leonardo  (1000) leonardo  (1000)        0 2022-04-11 21:17:36.465011 apricopt-0.0.2a3.dev9/apricopt.egg-info/
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     2160 2022-04-11 21:17:36.000000 apricopt-0.0.2a3.dev9/apricopt.egg-info/PKG-INFO
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     4315 2022-04-11 21:17:36.000000 apricopt-0.0.2a3.dev9/apricopt.egg-info/SOURCES.txt
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        1 2022-04-11 21:17:36.000000 apricopt-0.0.2a3.dev9/apricopt.egg-info/dependency_links.txt
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)      317 2022-04-11 21:17:36.000000 apricopt-0.0.2a3.dev9/apricopt.egg-info/requires.txt
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)        9 2022-04-11 21:17:36.000000 apricopt-0.0.2a3.dev9/apricopt.egg-info/top_level.txt
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)       38 2022-04-11 21:17:36.473011 apricopt-0.0.2a3.dev9/setup.cfg
+-rw-rw-r--   0 leonardo  (1000) leonardo  (1000)     1267 2022-04-11 21:16:00.000000 apricopt-0.0.2a3.dev9/setup.py
```

### Comparing `apricopt-0.0.2a3.dev8/COPYING` & `apricopt-0.0.2a3.dev9/COPYING`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/PKG-INFO` & `apricopt-0.0.2a3.dev9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apricopt
-Version: 0.0.2a3.dev8
+Version: 0.0.2a3.dev9
 Summary: A library for simulation-based parameter optimization
 Home-page: http://mclab.di.uniroma1.it
 Author: Marco Esposito
 Author-email: esposito@di.uniroma1.it
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,21 +37,21 @@
 
 * COPASI. It supports several optimisation algorithms for biological processes. More info [here](http://copasi.org/Support/User_Manual/Methods/Optimization_Methods/)
 
 ### Info ###
 
 WIP
 
-* Version 0.0.2a3dev8
+* Version 0.0.2a3dev9
 
 
 ### Who do I talk to? ###
 
 * Marco Esposito (author) - esposito@di.uniroma1.it
 * Leonardo Picchiami (author) - picchiami@di.uniroma1.it
 
 
-Copyright (C) 2020-2022  Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022  Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 
 Distributed under GNU General Public License v3.
```

### Comparing `apricopt-0.0.2a3.dev8/README.md` & `apricopt-0.0.2a3.dev9/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,19 +21,19 @@
 
 * COPASI. It supports several optimisation algorithms for biological processes. More info [here](http://copasi.org/Support/User_Manual/Methods/Optimization_Methods/)
 
 ### Info ###
 
 WIP
 
-* Version 0.0.2a3dev8
+* Version 0.0.2a3dev9
 
 
 ### Who do I talk to? ###
 
 * Marco Esposito (author) - esposito@di.uniroma1.it
 * Leonardo Picchiami (author) - picchiami@di.uniroma1.it
 
 
-Copyright (C) 2020-2022  Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022  Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 
 Distributed under GNU General Public License v3.
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/IO/data_input.py` & `apricopt-0.0.2a3.dev9/apricopt/IO/data_input.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/FastObservable.py` & `apricopt-0.0.2a3.dev9/apricopt/model/FastObservable.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/Model.py` & `apricopt-0.0.2a3.dev9/apricopt/model/Model.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/ModelInstance.py` & `apricopt-0.0.2a3.dev9/apricopt/model/ModelInstance.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/Observable.py` & `apricopt-0.0.2a3.dev9/apricopt/model/Observable.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/ObservableFunction.py` & `apricopt-0.0.2a3.dev9/apricopt/model/ObservableFunction.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/model/Parameter.py` & `apricopt-0.0.2a3.dev9/apricopt/model/Parameter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,27 +10,28 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Apricopt.  If not, see <http://www.gnu.org/licenses/>.
 
-Copyright (C) 2020-2021 Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022 Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 """
 
 
 class Parameter:
 
     def __init__(self, param_id: str, name: str, lower_bound: float = float("-inf"),
                  upper_bound: float = float("inf"), nominal_value: float = float("-inf"),
                  distribution: str = 'uniform', mu: float = 0, sigma: float = 0,
-                 granularity: float = 0, optimize: bool = True):
+                 granularity: float = 0, optimize: bool = True, fixed: bool = False):
         self.id = param_id
         self.name = name
         self.lower_bound = lower_bound
         self.upper_bound = upper_bound
         self.nominal_value = nominal_value
         self.distribution = distribution
         self.mu = mu
         self.sigma = sigma
         self.granularity = granularity
         self.optimize = optimize
+        self.fixed = fixed
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/sampling/Sampler.py` & `apricopt-0.0.2a3.dev9/apricopt/sampling/Sampler.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 from scipy import stats
 
 
 def sample_parameters(parameters: Collection[Parameter]) -> Dict[str, float]:
     result: Dict[str, float] = dict()
     samples = np.random.rand(len(parameters))
     for i, param in enumerate(parameters):
+        if param.fixed:
+            result[param.id] = param.nominal_value
+            continue
         if param.distribution == 'uniform':
             result[param.id] = \
                 round(param.lower_bound + (
                         param.upper_bound - param.lower_bound) * samples[i])
         elif param.distribution == 'loguniform':
             result[param.id] = 10 ** \
                                          (math.log(param.lower_bound, 10) + (
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/COPASIEngine.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/COPASIEngine.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Apricopt.  If not, see <http://www.gnu.org/licenses/>.
 
-Copyright (C) 2020-2021 Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022 Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 """
 
 from typing import Dict, List, Type
 import COPASI
 import sys
 
 from apricopt.model.Model import Model
@@ -85,15 +85,15 @@
         model_instance.set_species_initial_values(changed_metabolites)
         model_instance.set_parameters(changed_params)
         model_instance.set_compartments_initial_sizes(changed_compartments)
 
         return self._get_simulation_output(model, time_series)
 
     def simulate_trajectory_and_get_state(self, model: Model, horizon: float, exclude=None) -> \
-            Dict[str,Dict[str, float]]:
+            Dict[str, Dict[str, float]]:
         if not isinstance(model.instance, COPASIModelInstance):
             raise TypeError(
                 "The object in the field 'instance' of a 'Model' object passed to "
                 "'COPASIEngine::simulate_trajectory_and_get_state' method must have type 'COPASIModelInstance'.")
 
         if exclude is None:
             exclude = []
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/COPASI/COPASIModelInstance.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/COPASI/COPASIModelInstance.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/MockUpModelInstance.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/MockUpModelInstance.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/MockUp/MockUpSimulationEngine.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/MockUp/MockUpSimulationEngine.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/SimulationEngine.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/SimulationEngine.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with Apricopt.  If not, see <http://www.gnu.org/licenses/>.
 
-Copyright (C) 2020-2021 Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022 Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 """
 
 from abc import ABC, abstractmethod
 from typing import Dict, List, Type, Set
 
 from apricopt.model.Model import Model
 from apricopt.model.ModelInstance import ModelInstance
@@ -74,15 +74,15 @@
         pass
 
     @abstractmethod
     def simulate_trajectory_and_set(self, model: Model, horizon: float, exclude=None) -> Dict[str, List[float]]:
         pass
 
     @abstractmethod
-    def simulate_trajectory_and_get_state(self, model: Model, horizon: float, exclude=None) -> Dict[str, List[float]]:
+    def simulate_trajectory_and_get_state(self, model: Model, horizon: float, exclude=None) -> Dict[str, float]:
         pass
 
     @abstractmethod
     def restore_state(self, model: Model, changed_values: dict) -> None:
         pass
 
     @abstractmethod
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/RoadRunnerEngine.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/RoadRunnerEngine.py`

 * *Files 9% similar despite different names*

```diff
@@ -63,50 +63,55 @@
             if out_id not in exclude_from_set:
                 changed_values[out_id] = traj
                 model_obj.model[f'init({out_id})'] = traj[-1]
 
         model_obj.resetAll()
         return changed_values
 
-    def simulate_trajectory_and_get_state(self, model: Model, horizon: float, exclude=None) -> Dict[str, List[float]]:
-        raise NotImplementedError()
+    def simulate_trajectory_and_get_state(self, model: Model, horizon: float, exclude=None) -> Dict[str, float]:
+        model_obj: RoadRunner = model.instance.model_obj
+        observed_outputs = model_obj.model.getFloatingSpeciesIds() + \
+                           model_obj.model.getGlobalParameterIds() + \
+                           model_obj.model.getCompartmentIds()
+
+        sim_output = self._run_simulation_task(model, horizon, observed_outputs)
+        exclude_from_set = self._exclude_from_simulate_and_set(model, exclude)
+        changed_values: Dict[str, float] = dict()
+        for out_id, traj in sim_output.items():
+            if out_id == 'time':
+                continue
 
-    def restore_state(self, model: Model, changed_values: dict) -> None:
-        raise NotImplementedError()
+            if out_id not in exclude_from_set:
+                changed_values[out_id] = traj[-1]
+
+        model_obj.resetAll()
+        return changed_values
+
+    def restore_state(self, model: Model, changed_values: Dict[str, float]) -> None:
+        model_obj: RoadRunner = model.instance.model_obj
+        for var_id, state_value in changed_values.items():
+            model_obj[f'init({var_id})'] = state_value
 
     def model_instance_class(self) -> Type[ModelInstance]:
         return RoadRunnerModelInstance
 
-    def _exclude_from_simulate_and_set(self, model: Model, exclude: List[str] = None):
-        # document = libsbml.readSBML(model_filename)
-        # sbml_model = document.getModel()
+    def _exclude_from_simulate_and_set(self, model: Model, exclude: List[str] = None) -> List[str]:
         model_obj = model.instance.model_obj
 
         init_exclude: List[str] = []
         if exclude:
             init_exclude = list(exclude)
 
         for init_ass in model_obj.getInitialAssignmentIds():
             if init_ass not in init_exclude:
                 init_exclude.append(init_ass)
 
         for ass in model_obj.getAssignmentRuleIds():
             if ass not in init_exclude:
                 init_exclude.append(ass)
-        '''
-        for init_ass_obj in sbml_model.getListOfInitialAssignments():
-            elem = libsbml.InitialAssignment.getId(init_ass_obj)
-            if elem not in init_exclude:
-                init_exclude.append(elem)
-
-        for ass_obj in sbml_model.getListOfRules():
-            elem = libsbml.AssignmentRule.getId(ass_obj)
-            if elem not in init_exclude:
-                init_exclude.append(elem)
-        '''
         return init_exclude
 
     def _get_simulation_output(self, model: Model, time_series: np.ndarray, observed) -> Dict[str, List[float]]:
         if not isinstance(model.instance, RoadRunnerModelInstance):
             raise TypeError("The object in the field 'instance' of a 'Model' object passed to "
                             "'RoadRunnerEngine::simulate_trajectory' method must have type 'RoadRunnerModelInstance'.")
         sim_output: Dict[str, List[float]] = dict()
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt/simulation/roadrunner/RoadRunnerModelInstance.py` & `apricopt-0.0.2a3.dev9/apricopt/simulation/roadrunner/RoadRunnerModelInstance.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/BlackBox.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/BlackBox.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/BlackBoxSolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/BlackBoxSolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/FunctionBlackBox.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/FunctionBlackBox.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/MockUp/MockUpSolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/MockUp/MockUpSolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/NOMAD/NOMADSolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/NOMAD/NOMADSolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/SimulableModelBlackBox.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/SimulableModelBlackBox.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/pyswarms/PySwarmsSolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/pyswarms/PySwarmsSolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/blackbox/scipy/SciPySolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/blackbox/scipy/SciPySolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASIOptimisationMethod.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASIOptimisationMethod.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASISolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASISolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/COPASISolverParameter.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/COPASISolverParameter.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIDifferentialEvolution.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIDifferentialEvolution.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryProgramming.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryProgramming.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryStrategySR.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIEvolutionaryStrategySR.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithm.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithm.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithmSR.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIGeneticAlgorithmSR.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIHookeJeeves.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIHookeJeeves.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASILevenbergMarquardt.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASILevenbergMarquardt.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASINelderMead.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASINelderMead.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIParticleSwarm.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIParticleSwarm.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIPraxis.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIPraxis.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIRandomSearch.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIRandomSearch.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASIScatterSearch.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASIScatterSearch.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASISimulatedAnnealing.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASISimulatedAnnealing.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASISteepestDescent.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASISteepestDescent.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/COPASI/method/COPASITruncatedNewton.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/COPASI/method/COPASITruncatedNewton.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/solving/whitebox/WhiteBoxSolver.py` & `apricopt-0.0.2a3.dev9/apricopt/solving/whitebox/WhiteBoxSolver.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/model/formulas.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/model/formulas.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/model/observables/main.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/model/observables/main.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/GriewankBB.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/GriewankBB.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/NOMAD/GriewankTest.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/NOMAD/GriewankTest.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/ackley.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/ackley.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/MockUpBlackBox.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/MockUpBlackBox.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/mockup/mockup_test.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/mockup/mockup_test.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/ackley_test.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/ackley_test.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/pyswarms/sphere_test.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/pyswarms/sphere_test.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/scipy/sphere_test.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/scipy/sphere_test.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/blackbox/sphere.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/blackbox/sphere.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MaxRosenbrock.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MaxRosenbrock.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MinRosenbrock.py` & `apricopt-0.0.2a3.dev9/apricopt/tests/solving/whitebox/COPASI/rosenbrock/MinRosenbrock.py`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/apricopt.egg-info/PKG-INFO` & `apricopt-0.0.2a3.dev9/apricopt.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apricopt
-Version: 0.0.2a3.dev8
+Version: 0.0.2a3.dev9
 Summary: A library for simulation-based parameter optimization
 Home-page: http://mclab.di.uniroma1.it
 Author: Marco Esposito
 Author-email: esposito@di.uniroma1.it
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -37,21 +37,21 @@
 
 * COPASI. It supports several optimisation algorithms for biological processes. More info [here](http://copasi.org/Support/User_Manual/Methods/Optimization_Methods/)
 
 ### Info ###
 
 WIP
 
-* Version 0.0.2a3dev8
+* Version 0.0.2a3dev9
 
 
 ### Who do I talk to? ###
 
 * Marco Esposito (author) - esposito@di.uniroma1.it
 * Leonardo Picchiami (author) - picchiami@di.uniroma1.it
 
 
-Copyright (C) 2020-2022  Marco Esposito, Leonardo Picchiami.
+Copyright (C) 2020-2022  Sapienza University of Rome, Marco Esposito, Leonardo Picchiami.
 
 Distributed under GNU General Public License v3.
```

### Comparing `apricopt-0.0.2a3.dev8/apricopt.egg-info/SOURCES.txt` & `apricopt-0.0.2a3.dev9/apricopt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apricopt-0.0.2a3.dev8/setup.py` & `apricopt-0.0.2a3.dev9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,43 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="apricopt",
-    version="0.0.2a3dev8",
+    version="0.0.2a3dev9",
     author="Marco Esposito",
     author_email="esposito@di.uniroma1.it",
     description="A library for simulation-based parameter optimization",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://mclab.di.uniroma1.it",
     packages=setuptools.find_packages(),
     install_requires=[
         'attrs==21.2.0',
         'chaospy==4.2.1',
         'cycler==0.10.0',
         'future==0.18.2',
         'importlib-metadata==3.1.0',
         'kiwisolver==1.3.2',
-        'libroadrunner==2.2.0',
         'matplotlib==3.4.3',
         'mpmath==1.2.1',
         'numpy==1.22.3',
         'Pillow==8.3.2',
         'pyparsing==2.4.7',
-        'python-copasi==4.33.246',
         'python-dateutil==2.8.2',
         'python-libsbml==5.19.0',
         'PyYAML==5.4.1',
         'scipy==1.7.1',
         'seaborn==0.11.0',
         'six==1.16.0',
         'sympy==1.8',
         'tqdm==4.62.2',
         'zipp==3.4.0',
-
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
```

