# Comparing `tmp/qibocal-0.0.7.tar.gz` & `tmp/qibocal-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibocal-0.0.7.tar", max compression
+gzip compressed data, was "qibocal-0.0.8.tar", max compression
```

## Comparing `qibocal-0.0.7.tar` & `qibocal-0.0.8.tar`

### file list

```diff
@@ -1,133 +1,128 @@
--rw-r--r--   0        0        0    11357 2024-02-16 06:00:28.361148 qibocal-0.0.7/LICENSE
--rw-r--r--   0        0        0     3045 2024-02-16 06:00:28.361148 qibocal-0.0.7/README.md
--rw-r--r--   0        0        0     3316 2024-02-16 06:00:28.377148 qibocal-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      173 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/__init__.py
--rw-r--r--   0        0        0       30 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/__init__.py
--rw-r--r--   0        0        0      968 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/draw.py
--rw-r--r--   0        0        0     5363 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/execute.py
--rw-r--r--   0        0        0     1979 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/graph.py
--rw-r--r--   0        0        0     1422 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/history.py
--rw-r--r--   0        0        0      153 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/mode.py
--rw-r--r--   0        0        0    10002 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/operation.py
--rw-r--r--   0        0        0     2568 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/runcard.py
--rw-r--r--   0        0        0      758 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/serialize.py
--rw-r--r--   0        0        0     1180 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/status.py
--rw-r--r--   0        0        0     8630 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/task.py
--rw-r--r--   0        0        0      664 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/validate.py
--rw-r--r--   0        0        0     2274 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/validation.py
--rw-r--r--   0        0        0      108 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/validators/__init__.py
--rw-r--r--   0        0        0     1294 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/auto/validators/chi2.py
--rw-r--r--   0        0        0     3399 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/bootstrap.py
--rw-r--r--   0        0        0       51 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/__init__.py
--rw-r--r--   0        0        0     4106 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/_base.py
--rw-r--r--   0        0        0     1756 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/acquisition.py
--rw-r--r--   0        0        0     2240 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/autocalibration.py
--rw-r--r--   0        0        0     1638 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/fit.py
--rw-r--r--   0        0        0     3697 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/report.py
--rw-r--r--   0        0        0     2538 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/upload.py
--rw-r--r--   0        0        0     2735 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/cli/utils.py
--rw-r--r--   0        0        0     1755 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/config.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/__init__.py
--rw-r--r--   0        0        0     1224 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/ada_boost.py
--rw-r--r--   0        0        0      804 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/data.py
--rw-r--r--   0        0        0     1139 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/decision_tree.py
--rw-r--r--   0        0        0      895 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/gaussian_process.py
--rw-r--r--   0        0        0      801 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/linear_svm.py
--rw-r--r--   0        0        0      737 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/naive_bayes.py
--rw-r--r--   0        0        0     1255 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/nn.py
--rw-r--r--   0        0        0     1675 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/qblox_fit.py
--rw-r--r--   0        0        0     4530 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/qubit_fit.py
--rw-r--r--   0        0        0     1241 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/random_forest.py
--rw-r--r--   0        0        0     1133 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/rbf_svm.py
--rw-r--r--   0        0        0     8127 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/run.py
--rw-r--r--   0        0        0     1121 2024-02-16 06:00:28.377148 qibocal-0.0.7/src/qibocal/fitting/classifier/scikit_utils.py
--rw-r--r--   0        0        0     5662 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/__init__.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/__init__.py
--rw-r--r--   0        0        0     7588 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/allxy.py
--rw-r--r--   0        0        0     4829 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py
--rw-r--r--   0        0        0     8099 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/drag_pulse_tuning.py
--rw-r--r--   0        0        0    14353 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/classification.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/__init__.py
--rw-r--r--   0        0        0     6510 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/spin_echo.py
--rw-r--r--   0        0        0     5016 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/spin_echo_sequence.py
--rw-r--r--   0        0        0     7027 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1.py
--rw-r--r--   0        0        0     3264 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1_sequences.py
--rw-r--r--   0        0        0     5219 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1_signal.py
--rw-r--r--   0        0        0     5976 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2.py
--rw-r--r--   0        0        0     2517 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2_sequences.py
--rw-r--r--   0        0        0     4384 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2_signal.py
--rw-r--r--   0        0        0     2601 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/utils.py
--rw-r--r--   0        0        0     6338 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/zeno.py
--rw-r--r--   0        0        0     5732 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/zeno_signal.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/__init__.py
--rw-r--r--   0        0        0     4452 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py
--rw-r--r--   0        0        0     6479 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py
--rw-r--r--   0        0        0     2350 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/utils.py
--rw-r--r--   0        0        0    11021 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/dispersive_shift.py
--rw-r--r--   0        0        0     9477 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/fast_reset/_init__.py
--rw-r--r--   0        0        0     6879 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/fast_reset/fast_reset.py
--rw-r--r--   0        0        0     9482 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flipping.py
--rw-r--r--   0        0        0     8657 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flipping_signal.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/__init__.py
--rw-r--r--   0        0        0    11511 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py
--rw-r--r--   0        0        0     5438 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py
--rw-r--r--   0        0        0     8777 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py
--rw-r--r--   0        0        0     5232 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py
--rw-r--r--   0        0        0     5234 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py
--rw-r--r--   0        0        0     9425 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/resonator_flux_dependence.py
--rw-r--r--   0        0        0     7918 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/utils.py
--rw-r--r--   0        0        0     4730 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/qubit_spectroscopy.py
--rw-r--r--   0        0        0     5928 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py
--rw-r--r--   0        0        0     5669 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/qutrit_classification.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/__init__.py
--rw-r--r--   0        0        0     6460 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/amplitude.py
--rw-r--r--   0        0        0     5839 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/amplitude_signal.py
--rw-r--r--   0        0        0     3737 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/ef.py
--rw-r--r--   0        0        0     6491 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length.py
--rw-r--r--   0        0        0     2805 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length_sequences.py
--rw-r--r--   0        0        0     5976 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length_signal.py
--rw-r--r--   0        0        0     5819 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/utils.py
--rw-r--r--   0        0        0    14240 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/ramsey.py
--rw-r--r--   0        0        0     3145 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/ramsey_sequences.py
--rw-r--r--   0        0        0     9985 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/ramsey_signal.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/__init__.py
--rw-r--r--   0        0        0     3734 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/circuit_tools.py
--rw-r--r--   0        0        0      538 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/data.py
--rw-r--r--   0        0        0     7677 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py
--rw-r--r--   0        0        0     1798 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py
--rw-r--r--   0        0        0    16108 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py
--rw-r--r--   0        0        0     7638 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/utils.py
--rw-r--r--   0        0        0     8489 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_characterization.py
--rw-r--r--   0        0        0     6577 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_mitigation_matrix.py
--rw-r--r--   0        0        0     7030 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py
--rw-r--r--   0        0        0     7516 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/__init__.py
--rw-r--r--   0        0        0     6115 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency.py
--rw-r--r--   0        0        0     8172 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py
--rw-r--r--   0        0        0     7697 2024-02-16 06:00:28.381148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py
--rw-r--r--   0        0        0     5801 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py
--rw-r--r--   0        0        0     7886 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power_SNR.py
--rw-r--r--   0        0        0     8151 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_punchout.py
--rw-r--r--   0        0        0     8117 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py
--rw-r--r--   0        0        0     6923 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_spectroscopy.py
--rw-r--r--   0        0        0     7010 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_spectroscopy_attenuation.py
--rw-r--r--   0        0        0     6915 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py
--rw-r--r--   0        0        0     4684 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py
--rw-r--r--   0        0        0      111 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/__init__.py
--rw-r--r--   0        0        0    10185 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chevron.py
--rw-r--r--   0        0        0       49 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/__init__.py
--rw-r--r--   0        0        0     2970 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py
--rw-r--r--   0        0        0     9646 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py
--rw-r--r--   0        0        0     3269 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py
--rw-r--r--   0        0        0      722 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py
--rw-r--r--   0        0        0    13283 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py
--rw-r--r--   0        0        0     2259 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py
--rw-r--r--   0        0        0    20145 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/protocols/characterization/utils.py
--rw-r--r--   0        0        0     7198 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/update.py
--rw-r--r--   0        0        0     1150 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/utils.py
--rw-r--r--   0        0        0        0 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/web/__init__.py
--rw-r--r--   0        0        0      811 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/web/report.py
--rw-r--r--   0        0        0     4168 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/web/static/styles.css
--rw-r--r--   0        0        0     8557 2024-02-16 06:00:28.385148 qibocal-0.0.7/src/qibocal/web/templates/template.html
--rw-r--r--   0        0        0     5069 1970-01-01 00:00:00.000000 qibocal-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-06 07:35:22.825498 qibocal-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3045 2024-04-06 07:35:22.825498 qibocal-0.0.8/README.md
+-rw-r--r--   0        0        0     2797 2024-04-06 07:35:22.837499 qibocal-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      173 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/__init__.py
+-rw-r--r--   0        0        0     2293 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/execute.py
+-rw-r--r--   0        0        0     1422 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/history.py
+-rw-r--r--   0        0        0      153 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/mode.py
+-rw-r--r--   0        0        0    10411 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/operation.py
+-rw-r--r--   0        0        0     2602 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/runcard.py
+-rw-r--r--   0        0        0      758 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/serialize.py
+-rw-r--r--   0        0        0     1180 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/status.py
+-rw-r--r--   0        0        0     6064 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/auto/task.py
+-rw-r--r--   0        0        0       51 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/__init__.py
+-rw-r--r--   0        0        0     4479 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/_base.py
+-rw-r--r--   0        0        0     1602 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/acquisition.py
+-rw-r--r--   0        0        0     2137 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/autocalibration.py
+-rw-r--r--   0        0        0     2518 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/fit.py
+-rw-r--r--   0        0        0     3627 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/report.py
+-rw-r--r--   0        0        0     2538 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/upload.py
+-rw-r--r--   0        0        0     2290 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/cli/utils.py
+-rw-r--r--   0        0        0     1755 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/config.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/__init__.py
+-rw-r--r--   0        0        0     1224 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/ada_boost.py
+-rw-r--r--   0        0        0      804 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/data.py
+-rw-r--r--   0        0        0     1139 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/decision_tree.py
+-rw-r--r--   0        0        0      895 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/gaussian_process.py
+-rw-r--r--   0        0        0      801 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/linear_svm.py
+-rw-r--r--   0        0        0      737 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/naive_bayes.py
+-rw-r--r--   0        0        0     1675 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/qblox_fit.py
+-rw-r--r--   0        0        0     4530 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/qubit_fit.py
+-rw-r--r--   0        0        0     1241 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/random_forest.py
+-rw-r--r--   0        0        0     1133 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/rbf_svm.py
+-rw-r--r--   0        0        0     8095 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/run.py
+-rw-r--r--   0        0        0     1121 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/fitting/classifier/scikit_utils.py
+-rw-r--r--   0        0        0     5501 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/__init__.py
+-rw-r--r--   0        0        0     7601 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy.py
+-rw-r--r--   0        0        0     4842 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py
+-rw-r--r--   0        0        0    14336 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/classification.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/__init__.py
+-rw-r--r--   0        0        0     6247 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo.py
+-rw-r--r--   0        0        0     6804 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo_signal.py
+-rw-r--r--   0        0        0     6230 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1.py
+-rw-r--r--   0        0        0     3329 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_sequences.py
+-rw-r--r--   0        0        0     6343 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_signal.py
+-rw-r--r--   0        0        0     5411 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2.py
+-rw-r--r--   0        0        0     2551 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_sequences.py
+-rw-r--r--   0        0        0     5492 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_signal.py
+-rw-r--r--   0        0        0     3939 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/utils.py
+-rw-r--r--   0        0        0     5757 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno.py
+-rw-r--r--   0        0        0     5676 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno_signal.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/__init__.py
+-rw-r--r--   0        0        0     4905 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_chevron.py
+-rw-r--r--   0        0        0     4892 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py
+-rw-r--r--   0        0        0     5858 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py
+-rw-r--r--   0        0        0     2047 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/utils.py
+-rw-r--r--   0        0        0    11118 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift.py
+-rw-r--r--   0        0        0     9492 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py
+-rw-r--r--   0        0        0     8688 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/drag.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/_init__.py
+-rw-r--r--   0        0        0     6896 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/fast_reset.py
+-rw-r--r--   0        0        0     9675 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flipping.py
+-rw-r--r--   0        0        0     9992 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flipping_signal.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.841499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/__init__.py
+-rw-r--r--   0        0        0    11514 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py
+-rw-r--r--   0        0        0     5808 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py
+-rw-r--r--   0        0        0     8921 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py
+-rw-r--r--   0        0        0     5439 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py
+-rw-r--r--   0        0        0     5546 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py
+-rw-r--r--   0        0        0    14467 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_flux_dependence.py
+-rw-r--r--   0        0        0     8839 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/utils.py
+-rw-r--r--   0        0        0     5647 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy.py
+-rw-r--r--   0        0        0     6371 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py
+-rw-r--r--   0        0        0     5732 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/qutrit_classification.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/__init__.py
+-rw-r--r--   0        0        0     5971 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude.py
+-rw-r--r--   0        0        0     6553 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude_signal.py
+-rw-r--r--   0        0        0     3760 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/ef.py
+-rw-r--r--   0        0        0     6744 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length.py
+-rw-r--r--   0        0        0     2843 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_sequences.py
+-rw-r--r--   0        0        0     6712 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_signal.py
+-rw-r--r--   0        0        0     5819 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/__init__.py
+-rw-r--r--   0        0        0    10249 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey.py
+-rw-r--r--   0        0        0     9650 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey_signal.py
+-rw-r--r--   0        0        0     3351 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/__init__.py
+-rw-r--r--   0        0        0     2496 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/circuit_tools.py
+-rw-r--r--   0        0        0     7044 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py
+-rw-r--r--   0        0        0     1808 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py
+-rw-r--r--   0        0        0    14201 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py
+-rw-r--r--   0        0        0     5997 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/utils.py
+-rw-r--r--   0        0        0     8532 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_characterization.py
+-rw-r--r--   0        0        0     6498 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_mitigation_matrix.py
+-rw-r--r--   0        0        0     7038 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py
+-rw-r--r--   0        0        0     7546 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/__init__.py
+-rw-r--r--   0        0        0     6140 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency.py
+-rw-r--r--   0        0        0     8192 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py
+-rw-r--r--   0        0        0     7707 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py
+-rw-r--r--   0        0        0     5805 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py
+-rw-r--r--   0        0        0     7938 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power_SNR.py
+-rw-r--r--   0        0        0     8182 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout.py
+-rw-r--r--   0        0        0     8168 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py
+-rw-r--r--   0        0        0     9282 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_spectroscopy.py
+-rw-r--r--   0        0        0     6928 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py
+-rw-r--r--   0        0        0     4706 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py
+-rw-r--r--   0        0        0      178 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/__init__.py
+-rw-r--r--   0        0        0       72 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/__init__.py
+-rw-r--r--   0        0        0    10062 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron.py
+-rw-r--r--   0        0        0     4199 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron_signal.py
+-rw-r--r--   0        0        0     2290 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/utils.py
+-rw-r--r--   0        0        0       49 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/__init__.py
+-rw-r--r--   0        0        0     2970 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py
+-rw-r--r--   0        0        0    11961 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py
+-rw-r--r--   0        0        0     3269 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py
+-rw-r--r--   0        0        0      722 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py
+-rw-r--r--   0        0        0    15482 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py
+-rw-r--r--   0        0        0     4868 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz_signal.py
+-rw-r--r--   0        0        0     2342 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py
+-rw-r--r--   0        0        0    22117 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/protocols/characterization/utils.py
+-rw-r--r--   0        0        0     7198 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/update.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/__init__.py
+-rw-r--r--   0        0        0      811 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/report.py
+-rw-r--r--   0        0        0     4168 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/static/styles.css
+-rw-r--r--   0        0        0     8558 2024-04-06 07:35:22.845499 qibocal-0.0.8/src/qibocal/web/templates/template.html
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 qibocal-0.0.8/PKG-INFO
```

### Comparing `qibocal-0.0.7/LICENSE` & `qibocal-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/README.md` & `qibocal-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/pyproject.toml` & `qibocal-0.0.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibocal"
-version = "0.0.7"
+version = "0.0.8"
 description = "Qibo's quantum calibration, characterization and validation module."
 authors = ["andrea-pasquale <andreapasquale97@gmail.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibocal/"
 documentation = "https://qibo.science/qibocal/stable/"
@@ -13,41 +13,34 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-qibolab = "^0.1.5"
-qibo = "^0.2.1"
-numpy = "^1.24.0"
+qibolab = "^0.1.6"
+qibo ="^0.2.6"
+numpy = "^1.26.4"
 scipy = "^1.10.1"
 pandas = "^1.4.3"
-networkx = "^3.0"
 pydantic = "^1.10.5"
 click = "^8.1.3"
 jinja2 = "^3.1.2"
 plotly = "^5.15.0"
 dash = "^2.6.0"
 skops = "^0.6.0"
 scikit-learn = "^1.2.1"
 # Explicit dependency required to cope for dash: https://github.com/plotly/dash/issues/2557
 setuptools = "^67.8.0"
-keras-tuner = { version = "^1.3.0,<1.3.1", optional = true, markers = "sys_platform == 'linux' or sys_platform == 'darwin'" }
 matplotlib = { version = "^3.7.0", optional = true }
 seaborn = { version = "^0.12.2", optional = true }
 pydot = { version = "^1.4.2", optional = true }
-tensorflow = { version = "^2.12.0", optional = true, markers = "sys_platform == 'linux' or sys_platform == 'darwin'" }
-# TODO: the marker is a temporary solution due to the lack of the tensorflow-io 0.32.0's wheels for Windows, this package is one of
-# the tensorflow requirements
 skl2onnx = { version = "^1.14.0", optional = true }
-onnxruntime = { version = "^1.14.1", optional = true }
-onnx = { version = "^1.13.1", optional = true }
 pyyaml = "^6.0"
-
+onnxruntime = { version = "^1.14.1", optional = true }
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
 pylint = "^2.17"
 pytest = "^7.1.2"
@@ -72,21 +65,18 @@
 pdbpp = "^0.10.3"
 ipython = "^8.0"
 devtools = "^0.10.0"
 
 [tool.poetry.extras]
 
 classify = [
-  "tensorflow",
-  "keras-tuner",
   "matplotlib",
   "seaborn",
   "skl2onnx",
-  "onnxruntime",
-  "onnx",
+  "onnxruntime"
 ]
 viz = ["pydot"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `qibocal-0.0.7/src/qibocal/auto/execute.py` & `qibocal-0.0.8/src/qibocal/auto/task.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,167 +1,197 @@
-"""Tasks execution."""
+"""Action execution tracker."""
 
-from dataclasses import dataclass, field
+import copy
+from dataclasses import dataclass
 from pathlib import Path
-from typing import Optional, Set
+from statistics import mode
+from typing import Optional
 
 from qibolab.platform import Platform
+from qibolab.serialize import dump_platform
 
-from qibocal.config import log
-
-from .graph import Graph
-from .history import History
-from .runcard import Id, Runcard
-from .task import Qubits, Task
+from ..config import log, raise_error
+from ..protocols.characterization import Operation
+from .mode import ExecutionMode
+from .operation import Data, DummyPars, Results, Routine, dummy_operation
+from .runcard import Action, Id, Targets
+
+MAX_PRIORITY = int(1e9)
+"""A number bigger than whatever will be manually typed. But not so insanely big not to fit in a native integer."""
+DEFAULT_NSHOTS = 100
+"""Default number on shots when the platform is not provided."""
+TaskId = tuple[Id, int]
+"""Unique identifier for executed tasks."""
+PLATFORM_DIR = "platform"
+"""Folder where platform will be dumped."""
 
 
 @dataclass
-class Executor:
-    """Execute a tasks' graph and tracks its history."""
+class Task:
+    action: Action
+    """Action object parsed from Runcard."""
+    iteration: int = 0
+    """Task iteration."""
+
+    @property
+    def targets(self) -> Targets:
+        """Protocol targets."""
+        return self.action.targets
+
+    @property
+    def id(self) -> Id:
+        """Task Id."""
+        return self.action.id
+
+    @property
+    def uid(self) -> TaskId:
+        """Task unique Id."""
+        return (self.action.id, self.iteration)
+
+    @property
+    def operation(self):
+        """Routine object from Operation Enum."""
+        if self.action.operation is None:
+            raise RuntimeError("No operation specified")
 
-    graph: Graph
-    """The graph to be executed."""
-    history: History
-    """The execution history, with results and exit states."""
-    output: Path
-    """Output path."""
-    qubits: Qubits
-    """Qubits to be calibrated."""
-    platform: Platform
-    """Qubits' platform."""
-    max_iterations: int
-    """Maximum number of iterations."""
-    update: bool = True
-    """Runcard update mechanism."""
-    head: Optional[Id] = None
-    """The current position."""
-    pending: Set[Id] = field(default_factory=set)
-    """The branched off tasks, not yet executed."""
-
-    # TODO: find a more elegant way to pass everything
-    @classmethod
-    def load(
-        cls,
-        card: Runcard,
-        output: Path,
+        return Operation[self.action.operation].value
+
+    @property
+    def parameters(self):
+        """Inputs parameters for self.operation."""
+        return self.operation.parameters_type.load(self.action.parameters)
+
+    @property
+    def update(self):
+        """Local update parameter."""
+        return self.action.update
+
+    def run(
+        self,
+        max_iterations: int,
         platform: Platform = None,
-        qubits: Qubits = None,
-        update: bool = True,
+        targets: Targets = list,
+        mode: ExecutionMode = None,
+        folder: Path = None,
     ):
-        """Load execution graph and associated executor from a runcard."""
-
-        return cls(
-            graph=Graph.from_actions(card.actions),
-            history=History({}),
-            max_iterations=card.max_iterations,
-            output=output,
-            platform=platform,
-            qubits=qubits,
-            update=update,
-        )
-
-    def available(self, task: Task):
-        """Check if a task has all dependencies satisfied."""
-        for pred in self.graph.predecessors(task.id):
-            ptask = self.graph.task(pred)
-
-            if ptask.uid not in self.history:
-                return False
-
-        return True
-
-    def successors(self, task: Task):
-        """Retrieve successors of a specified task."""
-        succs: list[Task] = []
-
-        if task.main is not None:
-            # main task has always more priority on its own, with respect to
-            # same with the same level
-            succs.append(self.graph.task(task.main))
-        # add all possible successors to the list of successors
-        succs.extend([self.graph.task(id) for id in task.next])
-
-        return succs
-
-    def next(self) -> Optional[Id]:
-        """Resolve the next task to be executed.
-
-        Returns `None` if the execution is completed.
-
-        .. todo::
-
-            consider transforming this into an iterator, and this could be its
-            `__next__` method, raising a `StopIteration` instead of returning
-            `None`.
-            it would be definitely more Pythonic...
-
-        """
-        candidates = self.successors(self.current)
-        if len(candidates) == 0:
-            candidates.extend([])
-
-        candidates = list(filter(lambda t: self.available(t), candidates))
-
-        # sort accord to priority
-        candidates.sort(key=lambda t: t.priority)
-        if len(candidates) != 0:
-            self.pending.update([t.id for t in candidates[1:]])
-            return candidates[0].id
-
-        availables = list(
-            filter(lambda t: self.available(self.graph.task(t)), self.pending)
-        )
-        if len(availables) == 0:
-            if len(self.pending) == 0:
-                return None
-            raise RuntimeError("")
-
-        selected = min(availables, key=lambda t: self.graph.task(t).priority)
-        self.pending.remove(selected)
-        return selected
-
-    @property
-    def current(self):
-        """Retrieve current task, associated to the `head` pointer."""
-        assert self.head is not None
-        return self.graph.task(self.head)
-
-    def run(self, mode):
-        """Actual execution.
-
-        The platform's update method is called if:
-        - self.update is True and task.update is None
-        - task.update is True
-        """
-        self.head = self.graph.start
-        while self.head is not None:
-            task = self.current
-            task.iteration = self.history.iterations(task.id)
-            log.info(
-                f"Executing mode {mode.name} on {task.id} iteration {task.iteration}."
-            )
-            completed = task.run(
-                max_iterations=self.max_iterations,
-                platform=self.platform,
-                qubits=self.qubits,
-                folder=self.output,
-                mode=mode,
+        if self.iteration > max_iterations:
+            raise_error(
+                ValueError,
+                f"Maximum number of iterations {max_iterations} reached!",
             )
-            self.history.push(completed)
-            if mode.name == "autocalibration":
-                # TODO: find a way to use new parameters
-                new_head, new_params = completed.validate()
-
-                if new_params is not None:
-                    # if new_params are present we update the parameters of the
-                    # node pointed by the validator and we move the head
-                    self.graph.task(new_head).action.parameters.update(new_params)
-                    self.head = new_head
-                else:
-                    # normal flow
-                    self.head = self.next()
+
+        if self.targets is None:
+            self.action.targets = targets
+
+        completed = Completed(self, folder)
+
+        try:
+            if platform is not None:
+                if self.parameters.nshots is None:
+                    self.action.parameters["nshots"] = platform.settings.nshots
+                if self.parameters.relaxation_time is None:
+                    self.action.parameters["relaxation_time"] = (
+                        platform.settings.relaxation_time
+                    )
+            else:
+                if self.parameters.nshots is None:
+                    self.action.parameters["nshots"] = DEFAULT_NSHOTS
+
+            operation: Routine = self.operation
+            parameters = self.parameters
+
+        except (RuntimeError, AttributeError):
+            operation = dummy_operation
+            parameters = DummyPars()
+
+        if mode.name in ["autocalibration", "acquire"]:
+            if operation.platform_dependent and operation.targets_dependent:
+                completed.data, completed.data_time = operation.acquisition(
+                    parameters,
+                    platform=platform,
+                    targets=self.targets,
+                )
+
             else:
-                self.head = self.next()
-            if mode.name in ["autocalibration", "fit"] and self.platform is not None:
-                completed.update_platform(platform=self.platform, update=self.update)
+                completed.data, completed.data_time = operation.acquisition(
+                    parameters, platform=platform
+                )
+        if mode.name in ["autocalibration", "fit"]:
+            completed.results, completed.results_time = operation.fit(completed.data)
+        return completed
+
+
+@dataclass
+class Completed:
+    """A completed task."""
+
+    task: Task
+    """A snapshot of the task when it was completed.
 
-            yield completed.task.uid
+    .. todo::
+
+        once tasks will be immutable, a separate `iteration` attribute should
+        be added
+
+    """
+    folder: Path
+    """Folder with data and results."""
+    _data: Optional[Data] = None
+    """Protocol data."""
+    _results: Optional[Results] = None
+    """Fitting output."""
+    data_time: float = 0
+    """Protocol data."""
+    results_time: float = 0
+    """Fitting output."""
+
+    def __post_init__(self):
+        self.task = copy.deepcopy(self.task)
+
+    @property
+    def datapath(self):
+        """Path contaning data and results file for task."""
+        path = self.folder / "data" / f"{self.task.id}_{self.task.iteration}"
+        if not path.is_dir():
+            path.mkdir(parents=True)
+        return path
+
+    @property
+    def results(self):
+        """Access task's results."""
+        if self._results is None:
+            Results = self.task.operation.results_type
+            self._results = Results.load(self.datapath)
+        return self._results
+
+    @results.setter
+    def results(self, results: Results):
+        """Set and store results."""
+        self._results = results
+        self._results.save(self.datapath)
+
+    @property
+    def data(self):
+        """Access task's data."""
+        if self._data is None:
+            Data = self.task.operation.data_type
+            self._data = Data.load(self.datapath)
+        return self._data
+
+    @data.setter
+    def data(self, data: Data):
+        """Set and store data."""
+        self._data = data
+        self._data.save(self.datapath)
+
+    def update_platform(self, platform: Platform, update: bool):
+        """Perform update on platform' parameters by looping over qubits or pairs."""
+        if self.task.update and update:
+            for qubit in self.task.targets:
+                try:
+                    self.task.operation.update(self.results, platform, qubit)
+                except KeyError:
+                    log.warning(
+                        f"Skipping update of qubit {qubit} due to error in fit."
+                    )
+            (self.datapath / PLATFORM_DIR).mkdir(parents=True, exist_ok=True)
+            dump_platform(platform, self.datapath / PLATFORM_DIR)
```

### Comparing `qibocal-0.0.7/src/qibocal/auto/history.py` & `qibocal-0.0.8/src/qibocal/auto/history.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/auto/operation.py` & `qibocal-0.0.8/src/qibocal/auto/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import inspect
 import json
 import time
 from copy import deepcopy
-from dataclasses import asdict, dataclass
+from dataclasses import asdict, dataclass, fields
 from functools import wraps
 from pathlib import Path
 from typing import Callable, Generic, NewType, Optional, TypeVar, Union
 
 import numpy as np
 import numpy.typing as npt
 from qibolab.platform import Platform
@@ -218,14 +218,26 @@
         return super().load(path, filename=DATAFILE)
 
 
 @dataclass
 class Results(AbstractData):
     """Generic runcard update."""
 
+    def __contains__(self, key: Union[QubitId, QubitPairId, tuple[QubitId, ...]]):
+        """Checking if qubit is in Results.
+
+        If key is not present means that fitting failed or
+        was not performed.
+        """
+        return all(
+            key in getattr(self, field.name)
+            for field in fields(self)
+            if isinstance(getattr(self, field.name), dict)
+        )
+
     @classmethod
     def load(cls, path: Path):
         """Load results."""
         return super().load(path, filename=RESULTSFILE)
 
     def save(self, path: Path):
         """Store results to file."""
@@ -272,27 +284,27 @@
     @property
     def data_type(self):
         """ "Data object type return by data acquisition."""
         return inspect.signature(self.acquisition).return_annotation
 
     @property
     def results_type(self):
-        """ "Results object type return by data acquisition."""
+        """Results object type returned by data acquisition."""
         return inspect.signature(self.fit).return_annotation
 
     # TODO: I don't like these properties but it seems to work
     @property
     def platform_dependent(self):
         """Check if acquisition involves platform."""
         return "platform" in inspect.signature(self.acquisition).parameters
 
     @property
-    def qubits_dependent(self):
+    def targets_dependent(self):
         """Check if acquisition involves qubits."""
-        return "qubits" in inspect.signature(self.acquisition).parameters
+        return "targets" in inspect.signature(self.acquisition).parameters
 
 
 @dataclass
 class DummyPars(Parameters):
     """Dummy parameters."""
```

### Comparing `qibocal-0.0.7/src/qibocal/auto/runcard.py` & `qibocal-0.0.8/src/qibocal/auto/runcard.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,80 @@
 """Specify runcard layout, handles (de)serialization."""
 
 import os
-from functools import cached_property
 from typing import Any, NewType, Optional, Union
 
-from pydantic import Field
 from pydantic.dataclasses import dataclass
 from qibo.backends import Backend, GlobalBackend
+from qibo.transpiler.pipeline import Passes
 from qibolab.platform import Platform
-from qibolab.qubits import QubitId
+from qibolab.qubits import QubitId, QubitPairId
 
 from .operation import OperationId
-from .validation import Validator
 
 Id = NewType("Id", str)
 """Action identifiers type."""
 
+Targets = Union[list[QubitId], list[QubitPairId], list[tuple[QubitId, ...]]]
+"""Elements to be calibrated by a single protocol."""
+
 MAX_ITERATIONS = 5
 """Default max iterations."""
 
 
 @dataclass(config=dict(smart_union=True))
 class Action:
     """Action specification in the runcard."""
 
     id: Id
     """Action unique identifier."""
     operation: Optional[OperationId] = None
     """Operation to be performed by the executor."""
-    main: Optional[Id] = None
-    """Main subsequent for action in normal flow."""
-    next: Optional[Union[list[Id], Id]] = None
-    """Alternative subsequent actions, branching from the current one."""
-    priority: Optional[int] = None
-    """Priority level, determining the execution order."""
-    qubits: Union[list[QubitId], list[tuple[QubitId, QubitId]], list[list[QubitId]]] = (
-        Field(default_factory=list)
-    )
+    targets: Optional[Targets] = None
     """Local qubits (optional)."""
     update: bool = True
     """Runcard update mechanism."""
-    validator: Optional[Validator] = None
-    """Define validation scheme and parameters."""
     parameters: Optional[dict[str, Any]] = None
     """Input parameters, either values or provider reference."""
 
     def __hash__(self) -> int:
         """Each action is uniquely identified by its id."""
         return hash(self.id)
 
 
 @dataclass(config=dict(smart_union=True))
 class Runcard:
     """Structure of an execution runcard."""
 
     actions: list[Action]
     """List of action to be executed."""
-    qubits: Optional[Union[list[QubitId], list[tuple[QubitId, QubitId]]]] = None
-    """Qubits to be calibrated."""
+    targets: Optional[Targets] = None
+    """Qubits to be calibrated.
+       If `None` the protocols will be executed on all qubits
+       available in the platform."""
     backend: str = "qibolab"
     """Qibo backend."""
     platform: str = os.environ.get("QIBO_PLATFORM", "dummy")
     """Qibolab platform."""
     max_iterations: int = MAX_ITERATIONS
     """Maximum number of iterations."""
 
-    @cached_property
+    def __post_init__(self):
+        if self.targets is None and self.platform_obj is not None:
+            self.targets = list(self.platform_obj.qubits)
+
+    @property
     def backend_obj(self) -> Backend:
         """Allocate backend."""
-        GlobalBackend.set_backend(self.backend, self.platform)
-        return GlobalBackend()
+        GlobalBackend.set_backend(self.backend, platform=self.platform)
+        backend = GlobalBackend()
+        if backend.platform is not None:
+            backend.transpiler = Passes(connectivity=backend.platform.topology)
+            backend.transpiler.passes = backend.transpiler.passes[-1:]
+        return backend
 
     @property
     def platform_obj(self) -> Platform:
         """Allocate platform."""
         return self.backend_obj.platform
 
     @classmethod
```

### Comparing `qibocal-0.0.7/src/qibocal/auto/serialize.py` & `qibocal-0.0.8/src/qibocal/auto/serialize.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/auto/status.py` & `qibocal-0.0.8/src/qibocal/auto/status.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/auto/task.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,270 +1,271 @@
-"""Action execution tracker."""
-
-import copy
 from dataclasses import dataclass, field
-from pathlib import Path
-from statistics import mode
-from typing import Optional, Union
+from typing import Optional
 
+import numpy as np
+import numpy.typing as npt
+import plotly.graph_objects as go
+from plotly.subplots import make_subplots
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
-from qibolab.qubits import QubitId, QubitPairId
-from qibolab.serialize import dump_platform
+from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
+from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from ..config import log, raise_error
-from ..protocols.characterization import Operation
-from ..utils import (
-    allocate_qubits_pairs,
-    allocate_single_qubits,
-    allocate_single_qubits_lists,
-)
-from .mode import ExecutionMode
-from .operation import (
-    Data,
-    DummyPars,
-    Qubits,
-    QubitsPairs,
-    Results,
-    Routine,
-    dummy_operation,
-)
-from .runcard import Action, Id
-from .status import Failure, Normal
+from qibocal import update
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
-MAX_PRIORITY = int(1e9)
-"""A number bigger than whatever will be manually typed. But not so insanely big not to fit in a native integer."""
-TaskId = tuple[Id, int]
-"""Unique identifier for executed tasks."""
-PLATFORM_DIR = "platform"
-"""Folder where platform will be dumped."""
+from .utils import HZ_TO_GHZ, fit_punchout, norm, table_dict, table_html
 
 
 @dataclass
-class Task:
-    action: Action
-    """Action object parsed from Runcard."""
-    iteration: int = 0
-    """Task iteration."""
-    qubits: list[QubitId, QubitPairId] = field(default_factory=list)
-    """List of QubitIds or QubitPairIds for task."""
-
-    def __post_init__(self):
-        if len(self.qubits) == 0:
-            self.qubits = self.action.qubits
-
-    # TODO: to be removed in https://github.com/qiboteam/qibocal/pull/682
-    def _allocate_local_qubits(self, qubits, platform):
-        """Create qubits dictionary from QubitIds."""
-        if len(self.qubits) > 0:
-            if platform is not None:
-                if any(isinstance(i, tuple) for i in self.qubits):
-                    task_qubits = allocate_qubits_pairs(platform, self.qubits)
-                elif any(
-                    isinstance(i, tuple) or isinstance(i, list) for i in self.qubits
-                ):
-                    task_qubits = allocate_single_qubits_lists(platform, self.qubits)
-                else:
-                    task_qubits = allocate_single_qubits(platform, self.qubits)
-            else:
-                # None platform use just ids
-                task_qubits = self.qubits
-        else:
-            task_qubits = qubits
-
-        self.qubits = list(task_qubits)
-
-        return task_qubits
-
-    @property
-    def id(self) -> Id:
-        """Task Id."""
-        return self.action.id
-
-    @property
-    def uid(self) -> TaskId:
-        """Task unique Id."""
-        return (self.action.id, self.iteration)
-
-    @property
-    def operation(self):
-        """Routine object from Operation Enum."""
-        if self.action.operation is None:
-            raise RuntimeError("No operation specified")
-
-        return Operation[self.action.operation].value
-
-    @property
-    def main(self):
-        """Main node to be executed next."""
-        return self.action.main
-
-    @property
-    def next(self) -> list[Id]:
-        """Node unlocked after the execution of this task."""
-        if self.action.next is None:
-            return []
-        if isinstance(self.action.next, str):
-            return [self.action.next]
-
-        return self.action.next
-
-    @property
-    def priority(self):
-        """Priority level."""
-        if self.action.priority is None:
-            return MAX_PRIORITY
-        return self.action.priority
-
-    @property
-    def parameters(self):
-        """Inputs parameters for self.operation."""
-        return self.operation.parameters_type.load(self.action.parameters)
-
-    @property
-    def update(self):
-        """Local update parameter."""
-        return self.action.update
-
-    def run(
-        self,
-        max_iterations: int,
-        platform: Platform = None,
-        qubits: Union[Qubits, QubitsPairs] = dict,
-        mode: ExecutionMode = None,
-        folder: Path = None,
-    ):
-        if self.iteration > max_iterations:
-            raise_error(
-                ValueError,
-                f"Maximum number of iterations {max_iterations} reached!",
-            )
+class ResonatorPunchoutParameters(Parameters):
+    """ResonatorPunchout runcard inputs."""
 
-        completed = Completed(self, folder)
+    freq_width: int
+    """Width for frequency sweep relative  to the readout frequency [Hz]."""
+    freq_step: int
+    """Frequency step for sweep [Hz]."""
+    min_amp_factor: float
+    """Minimum amplitude multiplicative factor."""
+    max_amp_factor: float
+    """Maximum amplitude multiplicative factor."""
+    step_amp_factor: float
+    """Step amplitude multiplicative factor."""
+    amplitude: float = None
+    """Initial readout amplitude."""
 
-        try:
-            if self.parameters.nshots is None:
-                self.action.parameters["nshots"] = platform.settings.nshots
-            if self.parameters.relaxation_time is None:
-                self.action.parameters["relaxation_time"] = (
-                    platform.settings.relaxation_time
-                )
-            operation: Routine = self.operation
-            parameters = self.parameters
-
-        except (RuntimeError, AttributeError):
-            operation = dummy_operation
-            parameters = DummyPars()
-        if mode.name in ["autocalibration", "acquire"]:
-            if operation.platform_dependent and operation.qubits_dependent:
-                completed.data, completed.data_time = operation.acquisition(
-                    parameters,
-                    platform=platform,
-                    qubits=self._allocate_local_qubits(qubits, platform),
-                )
-                # need to reassign qubit since when task
-                # is passed it is deepcopied
-                completed.task.qubits = self.qubits
-            else:
-                completed.data, completed.data_time = operation.acquisition(
-                    parameters, platform=platform
-                )
-        if mode.name in ["autocalibration", "fit"]:
-            completed.results, completed.results_time = operation.fit(completed.data)
-        return completed
+
+@dataclass
+class ResonatorPunchoutResults(Results):
+    """ResonatorPunchout outputs."""
+
+    readout_frequency: dict[QubitId, float]
+    """Readout frequency [GHz] for each qubit."""
+    bare_frequency: Optional[dict[QubitId, float]]
+    """Bare resonator frequency [GHz] for each qubit."""
+    readout_amplitude: dict[QubitId, float]
+    """Readout amplitude for each qubit."""
+
+
+ResPunchoutType = np.dtype(
+    [
+        ("freq", np.float64),
+        ("amp", np.float64),
+        ("signal", np.float64),
+        ("phase", np.float64),
+    ]
+)
+"""Custom dtype for resonator punchout."""
 
 
 @dataclass
-class Completed:
-    """A completed task."""
+class ResonatorPunchoutData(Data):
+    """ResonatorPunchout data acquisition."""
+
+    resonator_type: str
+    """Resonator type."""
+    amplitudes: dict[QubitId, float]
+    """Amplitudes provided by the user."""
+    data: dict[QubitId, npt.NDArray[ResPunchoutType]] = field(default_factory=dict)
+    """Raw data acquired."""
+
+    def register_qubit(self, qubit, freq, amp, signal, phase):
+        """Store output for single qubit."""
+        size = len(freq) * len(amp)
+        frequency, amplitude = np.meshgrid(freq, amp)
+        ar = np.empty(size, dtype=ResPunchoutType)
+        ar["freq"] = frequency.ravel()
+        ar["amp"] = amplitude.ravel()
+        ar["signal"] = signal.ravel()
+        ar["phase"] = phase.ravel()
+        self.data[qubit] = np.rec.array(ar)
+
+
+def _acquisition(
+    params: ResonatorPunchoutParameters,
+    platform: Platform,
+    targets: list[QubitId],
+) -> ResonatorPunchoutData:
+    """Data acquisition for Punchout over amplitude."""
+    # create a sequence of pulses for the experiment:
+    # MZ
+
+    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
+    sequence = PulseSequence()
+
+    ro_pulses = {}
+    amplitudes = {}
+    for qubit in targets:
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
+        if params.amplitude is not None:
+            ro_pulses[qubit].amplitude = params.amplitude
+
+        amplitudes[qubit] = ro_pulses[qubit].amplitude
+        sequence.add(ro_pulses[qubit])
+
+    # define the parameters to sweep and their range:
+    # resonator frequency
+    delta_frequency_range = np.arange(
+        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+    )
+    freq_sweeper = Sweeper(
+        Parameter.frequency,
+        delta_frequency_range,
+        [ro_pulses[qubit] for qubit in targets],
+        type=SweeperType.OFFSET,
+    )
+
+    # amplitude
+    amplitude_range = np.arange(
+        params.min_amp_factor, params.max_amp_factor, params.step_amp_factor
+    )
+    amp_sweeper = Sweeper(
+        Parameter.amplitude,
+        amplitude_range,
+        [ro_pulses[qubit] for qubit in targets],
+        type=SweeperType.FACTOR,
+    )
+
+    data = ResonatorPunchoutData(
+        amplitudes=amplitudes,
+        resonator_type=platform.resonator_type,
+    )
+
+    results = platform.sweep(
+        sequence,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=AveragingMode.CYCLIC,
+        ),
+        amp_sweeper,
+        freq_sweeper,
+    )
+
+    # retrieve the results for every qubit
+    for qubit, ro_pulse in ro_pulses.items():
+        # average signal, phase, i and q over the number of shots defined in the runcard
+        result = results[ro_pulse.serial]
+        data.register_qubit(
+            qubit,
+            signal=result.magnitude,
+            phase=result.phase,
+            freq=delta_frequency_range + ro_pulse.frequency,
+            amp=amplitude_range * amplitudes[qubit],
+        )
+
+    return data
+
+
+def _fit(data: ResonatorPunchoutData, fit_type="amp") -> ResonatorPunchoutResults:
+    """Fit frequency and attenuation at high and low power for a given resonator."""
+
+    return ResonatorPunchoutResults(*fit_punchout(data, fit_type))
+
+
+def _plot(
+    data: ResonatorPunchoutData, target: QubitId, fit: ResonatorPunchoutResults = None
+):
+    """Plotting function for ResonatorPunchout."""
+    figures = []
+    fitting_report = ""
+    fig = make_subplots(
+        rows=1,
+        cols=2,
+        horizontal_spacing=0.1,
+        vertical_spacing=0.2,
+        subplot_titles=(
+            "Normalised Signal [a.u.]",
+            "phase [rad]",
+        ),
+    )
+    qubit_data = data[target]
+    frequencies = qubit_data.freq * HZ_TO_GHZ
+    amplitudes = qubit_data.amp
+    n_amps = len(np.unique(qubit_data.amp))
+    n_freq = len(np.unique(qubit_data.freq))
+    for i in range(n_amps):
+        qubit_data.signal[i * n_freq : (i + 1) * n_freq] = norm(
+            qubit_data.signal[i * n_freq : (i + 1) * n_freq]
+        )
+
+    fig.add_trace(
+        go.Heatmap(
+            x=frequencies,
+            y=amplitudes,
+            z=qubit_data.signal,
+            colorbar_x=0.46,
+        ),
+        row=1,
+        col=1,
+    )
+
+    fig.add_trace(
+        go.Heatmap(
+            x=frequencies,
+            y=amplitudes,
+            z=qubit_data.phase,
+            colorbar_x=1.01,
+        ),
+        row=1,
+        col=2,
+    )
+
+    if fit is not None:
+        fig.add_trace(
+            go.Scatter(
+                x=[
+                    fit.readout_frequency[target] * HZ_TO_GHZ,
+                ],
+                y=[
+                    fit.readout_amplitude[target],
+                ],
+                mode="markers",
+                marker=dict(
+                    size=8,
+                    color="gray",
+                    symbol="circle",
+                ),
+                name="Estimated readout point",
+                showlegend=True,
+            )
+        )
+        fitting_report = table_html(
+            table_dict(
+                target,
+                [
+                    "Low Power Resonator Frequency [Hz]",
+                    "Low Power readout amplitude [a.u.]",
+                    "High Power Resonator Frequency [Hz]",
+                ],
+                [
+                    np.round(fit.readout_frequency[target]),
+                    np.round(fit.readout_amplitude[target], 3),
+                    np.round(fit.bare_frequency[target]),
+                ],
+            )
+        )
+
+    fig.update_layout(
+        showlegend=True,
+        legend=dict(orientation="h"),
+    )
+
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
+    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
+    fig.update_yaxes(title_text="Amplitude [a.u.]", row=1, col=1)
+
+    figures.append(fig)
+
+    return figures, fitting_report
 
-    task: Task
-    """A snapshot of the task when it was completed.
 
-    .. todo::
+def _update(results: ResonatorPunchoutResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.readout_frequency[target], platform, target)
+    update.bare_resonator_frequency(results.bare_frequency[target], platform, target)
+    update.readout_amplitude(results.readout_amplitude[target], platform, target)
 
-        once tasks will be immutable, a separate `iteration` attribute should
-        be added
-
-    """
-    folder: Path
-    """Folder with data and results."""
-    _data: Optional[Data] = None
-    """Protocol data."""
-    _results: Optional[Results] = None
-    """Fitting output."""
-    data_time: float = 0
-    """Protocol data."""
-    results_time: float = 0
-    """Fitting output."""
-
-    def __post_init__(self):
-        self.task = copy.deepcopy(self.task)
-
-    @property
-    def datapath(self):
-        """Path contaning data and results file for task."""
-        path = self.folder / "data" / f"{self.task.id}_{self.task.iteration}"
-        if not path.is_dir():
-            path.mkdir(parents=True)
-        return path
-
-    @property
-    def results(self):
-        """Access task's results."""
-        if self._results is None:
-            Results = self.task.operation.results_type
-            self._results = Results.load(self.datapath)
-        return self._results
-
-    @results.setter
-    def results(self, results: Results):
-        """Set and store results."""
-        self._results = results
-        self._results.save(self.datapath)
-
-    @property
-    def data(self):
-        """Access task's data."""
-        if self._data is None:
-            Data = self.task.operation.data_type
-            self._data = Data.load(self.datapath)
-        return self._data
-
-    @data.setter
-    def data(self, data: Data):
-        """Set and store data."""
-        self._data = data
-        self._data.save(self.datapath)
-
-    def update_platform(self, platform: Platform, update: bool):
-        """Perform update on platform' parameters by looping over qubits or pairs."""
-        if self.task.update and update:
-            for qubit in self.task.qubits:
-                try:
-                    self.task.operation.update(self.results, platform, qubit)
-                except KeyError:
-                    log.warning(
-                        f"Skipping update of qubit {qubit} due to error in fit."
-                    )
-            (self.datapath / PLATFORM_DIR).mkdir(parents=True, exist_ok=True)
-            dump_platform(platform, self.datapath / PLATFORM_DIR)
-
-    def validate(self) -> tuple[Optional[TaskId], Optional[dict]]:
-        """Check status of completed and handle Failure using handler."""
-        if self.task.action.validator is not None:
-            status = []
-            for target in self.task.qubits:
-                # TODO: how to handle multiple targets?
-                # dummy solution for now: take the mode.
-                qubit_status, params = self.task.action.validator.validate(
-                    self.results, target
-                )
-                status.append(qubit_status)
-            output = mode(status)
-            if isinstance(output, Failure):
-                return None, None
-            elif isinstance(output, Normal):
-                return self.task.id, None
-            else:
-                return output, params
 
-        return self.task.id, None
+resonator_punchout = Routine(_acquisition, _fit, _plot, _update)
+"""ResonatorPunchout Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/cli/_base.py` & `qibocal-0.0.8/src/qibocal/cli/_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -128,31 +128,47 @@
 
     """
     reporting(folder)
 
 
 @command.command(context_settings=CONTEXT_SETTINGS)
 @click.argument(
-    "folder", metavar="folder", type=click.Path(exists=True, path_type=pathlib.Path)
+    "input_folder",
+    metavar="input_folder",
+    type=click.Path(exists=True, path_type=pathlib.Path),
+)
+@click.option(
+    "output_folder",
+    "-o",
+    type=click.Path(path_type=pathlib.Path),
+    help="Output folder where fit is generated.",
+)
+@click.option(
+    "force",
+    "-f",
+    is_flag=True,
+    help="Use --force option to overwrite the output folder.",
 )
 @click.option(
     "--update/--no-update",
     default=True,
     help="Use --no-update option to avoid updating iteratively the platform."
     "With this option the new runcard will not be produced.",
 )
-def fit(folder: pathlib.Path, update):
+def fit(
+    input_folder: pathlib.Path, update: bool, output_folder: pathlib.Path, force: bool
+):
     """Post-processing analysis
 
     Arguments:
 
     - FOLDER: input folder.
 
     """
-    fitting(folder, update)
+    fitting(input_folder, update, output_folder, force)
 
 
 @command.command(context_settings=CONTEXT_SETTINGS)
 @click.argument(
     "path", metavar="FOLDER", type=click.Path(exists=True, path_type=pathlib.Path)
 )
 @click.option(
```

### Comparing `qibocal-0.0.7/src/qibocal/cli/acquisition.py` & `qibocal-0.0.8/src/qibocal/cli/autocalibration.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,65 +4,70 @@
 
 import yaml
 from qibolab.serialize import dump_platform
 
 from ..auto.execute import Executor
 from ..auto.history import add_timings_to_meta
 from ..auto.mode import ExecutionMode
+from ..cli.report import ReportBuilder
 from .utils import (
     META,
     PLATFORM,
     RUNCARD,
-    create_qubits_dict,
+    UPDATED_PLATFORM,
     generate_meta,
     generate_output_folder,
 )
 
 
-def acquire(runcard, folder, force):
-    """Data acquisition
+def autocalibrate(runcard, folder, force, update):
+    """Autocalibration
 
     Arguments:
 
      - RUNCARD: runcard with declarative inputs.
     """
 
     # rename for brevity
     backend = runcard.backend_obj
     platform = runcard.platform_obj
     # generate output folder
     path = generate_output_folder(folder, force)
 
-    # set backend, platform and qubits
-    qubits = create_qubits_dict(qubits=runcard.qubits, platform=platform)
-
     # generate meta
     meta = generate_meta(backend, platform, path)
     # dump platform
     if backend.name == "qibolab":
         (path / PLATFORM).mkdir(parents=True, exist_ok=True)
         dump_platform(platform, path / PLATFORM)
 
     # dump action runcard
     (path / RUNCARD).write_text(yaml.safe_dump(asdict(runcard)))
     # dump meta
     (path / META).write_text(json.dumps(meta, indent=4))
 
-    executor = Executor.load(runcard, path, platform, qubits)
+    # allocate executor
+    executor = Executor.load(runcard, path, platform, runcard.targets, update)
 
     # connect and initialize platform
     if platform is not None:
         platform.connect()
 
     # run protocols
-    list(executor.run(mode=ExecutionMode.acquire))
-
-    e = datetime.datetime.now(datetime.timezone.utc)
-    meta["end-time"] = e.strftime("%H:%M:%S")
+    for _ in executor.run(mode=ExecutionMode.autocalibration):
+        report = ReportBuilder(path, runcard.targets, executor, meta, executor.history)
+        report.run(path)
+        # meta needs to be updated after each report to show correct end-time
+        e = datetime.datetime.now(datetime.timezone.utc)
+        meta["end-time"] = e.strftime("%H:%M:%S")
+        # dump updated meta
+        meta = add_timings_to_meta(meta, executor.history)
+        (path / META).write_text(json.dumps(meta, indent=4))
 
     # stop and disconnect platform
     if platform is not None:
         platform.disconnect()
 
-    # dump updated meta
-    meta = add_timings_to_meta(meta, executor.history)
-    (path / META).write_text(json.dumps(meta, indent=4))
+    # dump updated runcard
+    if platform is not None:
+        (path / UPDATED_PLATFORM).mkdir(parents=True, exist_ok=True)
+        dump_platform(platform, path / UPDATED_PLATFORM)
```

### Comparing `qibocal-0.0.7/src/qibocal/cli/report.py` & `qibocal-0.0.8/src/qibocal/cli/report.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,55 +7,69 @@
 from qibo.backends import GlobalBackend
 from qibolab.qubits import QubitId
 
 from qibocal.auto.execute import Executor
 from qibocal.auto.mode import ExecutionMode
 from qibocal.auto.runcard import Runcard
 from qibocal.auto.task import TaskId
-
-from .utils import create_qubits_dict
+from qibocal.config import log
 
 META = "meta.json"
 RUNCARD = "runcard.yml"
 UPDATED_PLATFORM = "new_platform.yml"
 PLATFORM = "platform.yml"
 
 
+def generate_figures_and_report(node, target):
+    """Returns figures and table for report."""
+
+    if node.results is None:
+        # plot acquisition data
+        return node.task.operation.report(data=node.data, fit=None, target=target)
+    if target not in node.results:
+        # plot acquisition data and message for unsuccessful fit
+        figures = node.task.operation.report(data=node.data, fit=None, target=target)[0]
+        return figures, "An error occurred when performing the fit."
+    # plot acquisition and fit
+    return node.task.operation.report(data=node.data, fit=node.results, target=target)
+
+
 def report(path):
     """Report generation
 
     Arguments:
 
     - FOLDER: input folder.
 
     """
+    if path.exists():
+        log.warning(f"Regenerating {path}/index.html")
     # load meta
     meta = json.loads((path / META).read_text())
     # load runcard
     runcard = Runcard.load(yaml.safe_load((path / RUNCARD).read_text()))
 
     # set backend, platform and qubits
     GlobalBackend.set_backend(backend=meta["backend"], platform=meta["platform"])
     backend = GlobalBackend()
     platform = backend.platform
-    qubits = create_qubits_dict(qubits=runcard.qubits, platform=platform)
 
     # load executor
-    executor = Executor.load(runcard, path, qubits=qubits)
+    executor = Executor.load(runcard, path, targets=runcard.targets)
     # produce html
-    builder = ReportBuilder(path, qubits, executor, meta)
+    builder = ReportBuilder(path, runcard.targets, executor, meta)
     builder.run(path)
 
 
 class ReportBuilder:
     """Builder to produce html report."""
 
-    def __init__(self, path: Path, qubits, executor: Executor, metadata, history=None):
+    def __init__(self, path: Path, targets, executor: Executor, metadata, history=None):
         self.path = self.title = path
-        self.qubits = qubits
+        self.targets = targets
         self.executor = executor
         self.metadata = metadata
         self._history = history
 
     @cached_property
     def history(self):
         if self._history is None:
@@ -65,41 +79,23 @@
             return self._history
 
     def routine_name(self, routine, iteration):
         """Prettify routine's name for report headers."""
         name = routine.replace("_", " ").title()
         return f"{name} - {iteration}"
 
-    def routine_qubits(self, task_id: TaskId):
-        """Get local qubits parameter from Task if available otherwise use global one."""
-        local_qubits = self.history[task_id].task.qubits
-        return local_qubits if len(local_qubits) > 0 else self.qubits
+    def routine_targets(self, task_id: TaskId):
+        """Get local targets parameter from Task if available otherwise use global one."""
+        local_targets = self.history[task_id].task.targets
+        return local_targets if len(local_targets) > 0 else self.targets
 
     def single_qubit_plot(self, task_id: TaskId, qubit: QubitId):
         """Generate single qubit plot."""
         node = self.history[task_id]
-        figures, fitting_report = node.task.operation.report(
-            data=node.data, fit=node.results, qubit=qubit
-        )
-        with tempfile.NamedTemporaryFile(delete=False) as temp:
-            html_list = []
-            for figure in figures:
-                figure.write_html(temp.name, include_plotlyjs=False, full_html=False)
-                temp.seek(0)
-                fightml = temp.read().decode("utf-8")
-                html_list.append(fightml)
-
-        all_html = "".join(html_list)
-        return all_html, fitting_report
-
-    def plot(self, task_id: TaskId):
-        """Generate plot when only acquisition data are provided."""
-        node = self.history[task_id]
-        data = node.task.data
-        figures, fitting_report = node.task.operation.report(data)
+        figures, fitting_report = generate_figures_and_report(node, qubit)
         with tempfile.NamedTemporaryFile(delete=False) as temp:
             html_list = []
             for figure in figures:
                 figure.write_html(temp.name, include_plotlyjs=False, full_html=False)
                 temp.seek(0)
                 fightml = temp.read().decode("utf-8")
                 html_list.append(fightml)
```

### Comparing `qibocal-0.0.7/src/qibocal/cli/upload.py` & `qibocal-0.0.8/src/qibocal/cli/upload.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/config.py` & `qibocal-0.0.8/src/qibocal/config.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/ada_boost.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/ada_boost.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/data.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/data.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/decision_tree.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/decision_tree.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/gaussian_process.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/linear_svm.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/linear_svm.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/naive_bayes.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/nn.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/random_forest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import numpy as np
+from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import GridSearchCV, RepeatedStratifiedKFold
-from sklearn.neural_network import MLPClassifier
 
 from . import scikit_utils
 
 
 def constructor(hyperpars):
     r"""Return the model class.
 
     Args:
-        hyperparams: Model hyperparameters.
+        _hyperparams: Model hyperparameters.
     """
-    return MLPClassifier().set_params(**hyperpars)
+    return RandomForestClassifier().set_params(**hyperpars)
 
 
 def hyperopt(x_train, y_train, _path):
     r"""Perform an hyperparameter optimization and return the hyperparameters.
 
     Args:
         x_train: Training inputs.
         y_train: Training outputs.
         _path (path): Model save path.
 
     Returns:
         Dictionary with model's hyperparameters.
     """
-    clf = MLPClassifier()
+    clf = RandomForestClassifier()
     cv = RepeatedStratifiedKFold(n_splits=10, n_repeats=3, random_state=1)
     space = {}
-    space["hidden_layer_sizes"] = [(16, 16), (16, 32), (16, 64)]
-    space["learning_rate_init"] = np.linspace(1e-4, 1e-2, num=3)
-    space["activation"] = ["logistic", "tanh", "relu"]
-    space["solver"] = ["lbfgs", "sgd", "adam"]
+    space["n_estimators"] = np.arange(10, 200, 10, dtype=int)
+    space["criterion"] = ["gini", "entropy", "log_loss"]
+    space["max_features"] = ["sqrt", "log2", None]
     search = GridSearchCV(clf, space, scoring="accuracy", n_jobs=-1, cv=cv)
-    _ = search.fit(x_train, y_train)
-
+    _ = search.fit(x_train, y_train.tolist())
     return search.best_params_
 
 
-normalize = lambda x: x
+normalize = scikit_utils.scikit_normalize
 dump = scikit_utils.scikit_dump
 predict_from_file = scikit_utils.scikit_predict
```

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/qblox_fit.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/qblox_fit.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/qubit_fit.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/qubit_fit.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/random_forest.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/rbf_svm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 import numpy as np
-from sklearn.ensemble import RandomForestClassifier
 from sklearn.model_selection import GridSearchCV, RepeatedStratifiedKFold
+from sklearn.svm import SVC
 
 from . import scikit_utils
 
+GAMMA = "auto"
+
 
 def constructor(hyperpars):
     r"""Return the model class.
 
     Args:
         _hyperparams: Model hyperparameters.
     """
-    return RandomForestClassifier().set_params(**hyperpars)
+    return SVC(gamma=GAMMA).set_params(**hyperpars)
 
 
 def hyperopt(x_train, y_train, _path):
     r"""Perform an hyperparameter optimization and return the hyperparameters.
 
     Args:
         x_train: Training inputs.
         y_train: Training outputs.
         _path (path): Model save path.
 
     Returns:
         Dictionary with model's hyperparameters.
     """
-    clf = RandomForestClassifier()
+    clf = SVC(gamma=GAMMA)
+
     cv = RepeatedStratifiedKFold(n_splits=10, n_repeats=3, random_state=1)
     space = {}
-    space["n_estimators"] = np.arange(10, 200, 10, dtype=int)
-    space["criterion"] = ["gini", "entropy", "log_loss"]
-    space["max_features"] = ["sqrt", "log2", None]
+    space["C"] = np.linspace(0.01, 2, num=50)
+    space["degree"] = [2, 3, 4]
     search = GridSearchCV(clf, space, scoring="accuracy", n_jobs=-1, cv=cv)
-    _ = search.fit(x_train, y_train.tolist())
+    _ = search.fit(x_train, y_train.astype(np.int))
+
     return search.best_params_
 
 
 normalize = scikit_utils.scikit_normalize
 dump = scikit_utils.scikit_dump
 predict_from_file = scikit_utils.scikit_predict
```

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/run.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/run.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,28 +14,26 @@
 from . import data
 
 CLS_MODULES = [
     "linear_svm",
     "ada_boost",
     "gaussian_process",
     "naive_bayes",
-    "nn",
     "qubit_fit",
     "random_forest",
     "rbf_svm",
     "qblox_fit",
     "decision_tree",
 ]
 
 PRETTY_NAME = [
     "Linear SVM",
     "Ada Boost",
     "Gaussian Process",
     "Naive Bayes",
-    "Neural Network",
     "Qubit Fit",
     "Random Forest",
     "RBF SVM",
     "Qblox Fit",
     "Decision Tree",
 ]
```

### Comparing `qibocal-0.0.7/src/qibocal/fitting/classifier/scikit_utils.py` & `qibocal-0.0.8/src/qibocal/fitting/classifier/scikit_utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/__init__.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from enum import Enum
 
 from .allxy.allxy import allxy
-from .allxy.allxy_drag_pulse_tuning import allxy_drag_pulse_tuning
-from .allxy.drag_pulse_tuning import drag_pulse_tuning
 from .classification import single_shot_classification
 from .coherence.spin_echo import spin_echo
-from .coherence.spin_echo_sequence import spin_echo_sequence
+from .coherence.spin_echo_signal import spin_echo_signal
 from .coherence.t1 import t1
 from .coherence.t1_sequences import t1_sequences
 from .coherence.t1_signal import t1_signal
 from .coherence.t2 import t2
 from .coherence.t2_sequences import t2_sequences
 from .coherence.t2_signal import t2_signal
 from .coherence.zeno import zeno
 from .coherence.zeno_signal import zeno_signal
+from .couplers.coupler_chevron import coupler_chevron
 from .couplers.coupler_qubit_spectroscopy import coupler_qubit_spectroscopy
 from .couplers.coupler_resonator_spectroscopy import coupler_resonator_spectroscopy
 from .dispersive_shift import dispersive_shift
 from .dispersive_shift_qutrit import dispersive_shift_qutrit
+from .drag import drag_tuning
 from .fast_reset.fast_reset import fast_reset
 from .flipping import flipping
 from .flipping_signal import flipping_signal
 from .flux_dependence.avoided_crossing import avoided_crossing
 from .flux_dependence.qubit_crosstalk import qubit_crosstalk
 from .flux_dependence.qubit_flux_dependence import qubit_flux
 from .flux_dependence.qubit_flux_tracking import qubit_flux_tracking
@@ -32,41 +32,45 @@
 from .qutrit_classification import qutrit_classification
 from .rabi.amplitude import rabi_amplitude
 from .rabi.amplitude_signal import rabi_amplitude_signal
 from .rabi.ef import rabi_amplitude_ef
 from .rabi.length import rabi_length
 from .rabi.length_sequences import rabi_length_sequences
 from .rabi.length_signal import rabi_length_signal
-from .ramsey import ramsey
-from .ramsey_sequences import ramsey_sequences
-from .ramsey_signal import ramsey_signal
+from .ramsey.ramsey import ramsey
+from .ramsey.ramsey_signal import ramsey_signal
 from .randomized_benchmarking.standard_rb import standard_rb
 from .readout_characterization import readout_characterization
 from .readout_mitigation_matrix import readout_mitigation_matrix
 from .readout_optimization.resonator_amplitude import resonator_amplitude
 from .readout_optimization.resonator_frequency import resonator_frequency
 from .readout_optimization.twpa_calibration.frequency import twpa_frequency
 from .readout_optimization.twpa_calibration.frequency_power import twpa_frequency_power
 from .readout_optimization.twpa_calibration.frequency_SNR import twpa_frequency_snr
 from .readout_optimization.twpa_calibration.power import twpa_power
 from .readout_optimization.twpa_calibration.power_SNR import twpa_power_snr
 from .resonator_punchout import resonator_punchout
 from .resonator_punchout_attenuation import resonator_punchout_attenuation
 from .resonator_spectroscopy import resonator_spectroscopy
-from .resonator_spectroscopy_attenuation import resonator_spectroscopy_attenuation
 from .signal_experiments.calibrate_state_discrimination import (
     calibrate_state_discrimination,
 )
 from .signal_experiments.time_of_flight_readout import time_of_flight_readout
-from .two_qubit_interaction import chevron, chsh_circuits, chsh_pulses, cz_virtualz
+from .two_qubit_interaction import (
+    chevron,
+    chevron_signal,
+    chsh_circuits,
+    chsh_pulses,
+    cz_virtualz,
+    cz_virtualz_signal,
+)
 
 
 class Operation(Enum):
     resonator_spectroscopy = resonator_spectroscopy
-    resonator_spectroscopy_attenuation = resonator_spectroscopy_attenuation
     resonator_punchout = resonator_punchout
     resonator_punchout_attenuation = resonator_punchout_attenuation
     resonator_flux = resonator_flux
     resonator_crosstalk = resonator_crosstalk
     qubit_spectroscopy = qubit_spectroscopy
     qubit_flux = qubit_flux
     qubit_flux_tracking = qubit_flux_tracking
@@ -74,31 +78,30 @@
     rabi_amplitude = rabi_amplitude
     rabi_length = rabi_length
     rabi_length_sequences = rabi_length_sequences
     rabi_amplitude_signal = rabi_amplitude_signal
     rabi_length_signal = rabi_length_signal
     ramsey = ramsey
     ramsey_signal = ramsey_signal
-    ramsey_sequences = ramsey_sequences
     t1 = t1
     t1_signal = t1_signal
     t1_sequences = t1_sequences
     t2 = t2
     t2_signal = t2_signal
     t2_sequences = t2_sequences
     time_of_flight_readout = time_of_flight_readout
     single_shot_classification = single_shot_classification
     spin_echo = spin_echo
-    spin_echo_sequence = spin_echo_sequence
+    spin_echo_signal = spin_echo_signal
     allxy = allxy
-    allxy_drag_pulse_tuning = allxy_drag_pulse_tuning
-    drag_pulse_tuning = drag_pulse_tuning
+    drag_tuning = drag_tuning
     flipping = flipping
     dispersive_shift = dispersive_shift
     chevron = chevron
+    chevron_signal = chevron_signal
     cz_virtualz = cz_virtualz
     standard_rb = standard_rb
     readout_characterization = readout_characterization
     resonator_frequency = resonator_frequency
     fast_reset = fast_reset
     zeno = zeno
     zeno_signal = zeno_signal
@@ -114,9 +117,11 @@
     qubit_spectroscopy_ef = qubit_spectroscopy_ef
     qutrit_classification = qutrit_classification
     resonator_amplitude = resonator_amplitude
     avoided_crossing = avoided_crossing
     dispersive_shift_qutrit = dispersive_shift_qutrit
     coupler_resonator_spectroscopy = coupler_resonator_spectroscopy
     coupler_qubit_spectroscopy = coupler_qubit_spectroscopy
+    cz_virtualz_signal = cz_virtualz_signal
+    coupler_chevron = coupler_chevron
     flipping_signal = flipping_signal
     calibrate_state_discrimination = calibrate_state_discrimination
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/allxy.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 
 @dataclass
 class AllXYParameters(Parameters):
     """AllXY runcard inputs."""
 
     beta_param: float = None
@@ -64,15 +64,15 @@
     ["Y9", "Y9"],
 ]
 
 
 def _acquisition(
     params: AllXYParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> AllXYData:
     r"""
     Data acquisition for allXY experiment.
     The AllXY experiment is a simple test of the calibration of single qubit gatesThe qubit (initialized in the |0> state)
     is subjected to two back-to-back single-qubit gates and measured. In each round, we run 21 different gate pairs:
     ideally, the first 5 return the qubit to |0>, the next 12 drive it to superposition state, and the last 4 put the
     qubit in |1> state.
@@ -83,15 +83,15 @@
 
     # repeat the experiment as many times as defined by software_averages
     # for iteration in range(params.software_averages):
     sequences, all_ro_pulses = [], []
     for gates in gatelist:
         sequences.append(PulseSequence())
         all_ro_pulses.append({})
-        for qubit in qubits:
+        for qubit in targets:
             sequences[-1], all_ro_pulses[-1][qubit] = add_gate_pair_pulses_to_sequence(
                 platform, gates, qubit, sequences[-1], params.beta_param
             )
 
     # execute the pulse sequence
     options = ExecutionParameters(
         nshots=params.nshots, averaging_mode=AveragingMode.CYCLIC
@@ -101,15 +101,15 @@
     else:
         results = [
             platform.execute_pulse_sequence(sequence, options) for sequence in sequences
         ]
 
     for ig, (gates, ro_pulses) in enumerate(zip(gatelist, all_ro_pulses)):
         gate = "-".join(gates)
-        for qubit in qubits:
+        for qubit in targets:
             serial = ro_pulses[qubit].serial
             if params.unrolling:
                 z_proj = 2 * results[serial][ig].probability(0) - 1
             else:
                 z_proj = 2 * results[ig][serial].probability(0) - 1
             data.register_qubit(
                 AllXYType, (qubit), dict(prob=np.array([z_proj]), gate=np.array([gate]))
@@ -212,22 +212,22 @@
 
 def _fit(_data: AllXYData) -> AllXYResults:
     """Post-Processing for allXY"""
     return AllXYResults()
 
 
 # allXY
-def _plot(data: AllXYData, qubit, fit: AllXYResults = None):
+def _plot(data: AllXYData, target: QubitId, fit: AllXYResults = None):
     """Plotting function for allXY."""
 
     figures = []
     fitting_report = ""
     fig = go.Figure()
 
-    qubit_data = data[qubit]
+    qubit_data = data[target]
 
     fig.add_trace(
         go.Scatter(
             x=qubit_data.gate,
             y=qubit_data.prob,
             mode="markers",
             text=gatelist,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/allxy/allxy_drag_pulse_tuning.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from . import allxy
 
 
 @dataclass
 class AllXYDragParameters(Parameters):
     """AllXYDrag runcard inputs."""
@@ -47,15 +47,15 @@
         """Access qubits from data structure."""
         return np.unique([b[1] for b in self.data])
 
 
 def _acquisition(
     params: AllXYDragParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> AllXYDragData:
     r"""
     Data acquisition for allXY experiment varying beta.
     The AllXY experiment is a simple test of the calibration of single qubit gatesThe qubit (initialized in the |0> state)
     is subjected to two back-to-back single-qubit gates and measured. In each round, we run 21 different gate pairs:
     ideally, the first 5 return the qubit to |0>, the next 12 drive it to superposition state, and the last 4 put the
     qubit in |1> state.
@@ -69,15 +69,15 @@
     betas = np.arange(params.beta_start, params.beta_end, params.beta_step).round(4)
     # sweep the parameters
     for beta_param in betas:
         for gates in allxy.gatelist:
             # create a sequence of pulses
             ro_pulses = {}
             sequence = PulseSequence()
-            for qubit in qubits:
+            for qubit in targets:
                 sequence, ro_pulses[qubit] = allxy.add_gate_pair_pulses_to_sequence(
                     platform, gates, qubit, sequence, beta_param
                 )
 
             # execute the pulse sequence
             results = platform.execute_pulse_sequence(
                 sequence,
@@ -85,15 +85,15 @@
                     nshots=params.nshots,
                     relaxation_time=params.relaxation_time,
                     averaging_mode=AveragingMode.CYCLIC,
                 ),
             )
 
             # retrieve the results for every qubit
-            for qubit in qubits:
+            for qubit in targets:
                 z_proj = 2 * results[ro_pulses[qubit].serial].probability(0) - 1
                 # store the results
                 gate = "-".join(gates)
                 data.register_qubit(
                     allxy.AllXYType,
                     (qubit, beta_param),
                     dict(prob=np.array([z_proj]), gate=np.array([gate])),
@@ -102,25 +102,25 @@
 
 
 def _fit(_data: AllXYDragData) -> AllXYDragResults:
     """Post-processing for allXYDrag."""
     return AllXYDragResults()
 
 
-def _plot(data: AllXYDragData, qubit, fit: AllXYDragResults = None):
+def _plot(data: AllXYDragData, target: QubitId, fit: AllXYDragResults = None):
     """Plotting function for allXYDrag."""
 
     figures = []
     fitting_report = ""
 
     fig = go.Figure()
     beta_params = data.beta_params
 
     for j, beta_param in enumerate(beta_params):
-        beta_param_data = data[qubit, beta_param]
+        beta_param_data = data[target, beta_param]
         fig.add_trace(
             go.Scatter(
                 x=beta_param_data.gate,
                 y=beta_param_data.prob,
                 mode="markers+lines",
                 opacity=0.5,
                 name=f"Beta {beta_param}",
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/allxy/drag_pulse_tuning.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo_signal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,261 +1,227 @@
-from dataclasses import dataclass, field
+from copy import deepcopy
+from dataclasses import dataclass
 
 import numpy as np
-import numpy.typing as npt
 import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Qubits, Results, Routine
-from qibocal.config import log
+from qibocal.auto.operation import Parameters, Results, Routine
 
 from ..utils import table_dict, table_html
-from . import allxy_drag_pulse_tuning
+from .t1_signal import T1SignalData
+from .utils import CoherenceType, exp_decay, exponential_fit
 
 
 @dataclass
-class DragPulseTuningParameters(allxy_drag_pulse_tuning.AllXYDragParameters):
-    """DragPulseTuning runcard inputs."""
+class SpinEchoSignalParameters(Parameters):
+    """SpinEcho Signal runcard inputs."""
 
-    beta_start: float
-    """DRAG pulse beta start sweep parameter."""
-    beta_end: float
-    """DRAG pulse beta end sweep parameter."""
-    beta_step: float
-    """DRAG pulse beta sweep step parameter."""
+    delay_between_pulses_start: int
+    """Initial delay between pulses [ns]."""
+    delay_between_pulses_end: int
+    """Final delay between pulses [ns]."""
+    delay_between_pulses_step: int
+    """Step delay between pulses [ns]."""
+    unrolling: bool = False
+    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
+    Defaults to ``False``."""
+    single_shot: bool = False
+    """If ``True`` save single shot signal data."""
 
 
 @dataclass
-class DragPulseTuningResults(Results):
-    """DragPulseTuning outputs."""
+class SpinEchoSignalResults(Results):
+    """SpinEchoSignal outputs."""
 
-    betas: dict[QubitId, float]
-    """Optimal beta paramter for each qubit."""
+    t2_spin_echo: dict[QubitId, tuple[float]]
+    """T2 echo for each qubit."""
     fitted_parameters: dict[QubitId, dict[str, float]]
     """Raw fitting output."""
+    pcov: dict[QubitId, list[float]]
+    """Approximate covariance of fitted parameters."""
 
 
-DragPulseTuningType = np.dtype([("signal", np.float64), ("beta", np.float64)])
-
-
-@dataclass
-class DragPulseTuningData(Data):
-    """DragPulseTuning acquisition outputs."""
-
-    data: dict[QubitId, npt.NDArray[DragPulseTuningType]] = field(default_factory=dict)
-    """Raw data acquired."""
+class SpinEchoSignalData(T1SignalData):
+    """SpinEcho acquisition outputs."""
 
 
 def _acquisition(
-    params: DragPulseTuningParameters,
+    params: SpinEchoSignalParameters,
     platform: Platform,
-    qubits: Qubits,
-) -> DragPulseTuningData:
-    r"""
-    Data acquisition for drag pulse tuning experiment.
-    In this experiment, we apply two sequences in a given qubit: Rx(pi/2) - Ry(pi) and Ry(pi) - Rx(pi/2) for a range
-    of different beta parameter values. After fitting, we obtain the best coefficient value for a pi pulse with drag shape.
-    """
-    # define the parameter to sweep and its range:
-    # qubit drive DRAG pulse beta parameter
-    beta_param_range = np.arange(
-        params.beta_start, params.beta_end, params.beta_step
-    ).round(4)
-
-    data = DragPulseTuningData()
-
-    for beta_param in beta_param_range:
-        # create two sequences of pulses
-        # seq1: RX(pi/2) - RY(pi) - MZ
-        # seq1: RY(pi/2) - RX(pi) - MZ
-
-        ro_pulses = {}
-        seq1 = PulseSequence()
-        seq2 = PulseSequence()
-        for qubit in qubits:
-            # drag pulse RX(pi/2)
-            RX90_drag_pulse = platform.create_RX90_drag_pulse(
-                qubit, start=0, beta=beta_param
-            )
-            # drag pulse RY(pi)
-            RY_drag_pulse = platform.create_RX_drag_pulse(
-                qubit,
-                start=RX90_drag_pulse.finish,
-                relative_phase=+np.pi / 2,
-                beta=beta_param,
-            )
-            # drag pulse RY(pi/2)
-            RY90_drag_pulse = platform.create_RX90_drag_pulse(
-                qubit, start=0, relative_phase=np.pi / 2, beta=beta_param
-            )
-            # drag pulse RX(pi)
-            RX_drag_pulse = platform.create_RX_drag_pulse(
-                qubit, start=RY90_drag_pulse.finish, beta=beta_param
-            )
-
-            # RO pulse
-            ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-                qubit,
-                start=2
-                * RX90_drag_pulse.duration,  # assumes all single-qubit gates have same duration
-            )
-            # RX(pi/2) - RY(pi) - RO
-            seq1.add(RX90_drag_pulse)
-            seq1.add(RY_drag_pulse)
-            seq1.add(ro_pulses[qubit])
-
-            # RX(pi/2) - RY(pi) - RO
-            seq2.add(RY90_drag_pulse)
-            seq2.add(RX_drag_pulse)
-            seq2.add(ro_pulses[qubit])
-
-        # execute the pulse sequences
-        result1 = platform.execute_pulse_sequence(
-            seq1,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.INTEGRATION,
-                averaging_mode=AveragingMode.CYCLIC,
-            ),
+    targets: list[QubitId],
+) -> SpinEchoSignalData:
+    """Data acquisition for SpinEcho"""
+    # create a sequence of pulses for the experiment:
+    # Spin Echo 3 Pulses: RX(pi/2) - wait t(rotates z) - RX(pi) - wait t(rotates z) - RX(pi/2) - readout
+    ro_pulses = {}
+    RX90_pulses1 = {}
+    RX_pulses = {}
+    RX90_pulses2 = {}
+    sequence = PulseSequence()
+    for qubit in targets:
+        RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
+        RX_pulses[qubit] = platform.create_RX_pulse(
+            qubit, start=RX90_pulses1[qubit].finish
         )
-        result2 = platform.execute_pulse_sequence(
-            seq2,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.INTEGRATION,
-                averaging_mode=AveragingMode.CYCLIC,
-            ),
+        RX90_pulses2[qubit] = platform.create_RX90_pulse(
+            qubit, start=RX_pulses[qubit].finish
+        )
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=RX90_pulses2[qubit].finish
         )
+        sequence.add(RX90_pulses1[qubit])
+        sequence.add(RX_pulses[qubit])
+        sequence.add(RX90_pulses2[qubit])
+        sequence.add(ro_pulses[qubit])
+
+    # define the parameter to sweep and its range:
+    # delay between pulses
+    ro_wait_range = np.arange(
+        params.delay_between_pulses_start,
+        params.delay_between_pulses_end,
+        params.delay_between_pulses_step,
+    )
+
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.INTEGRATION,
+        averaging_mode=(
+            AveragingMode.SINGLESHOT if params.single_shot else AveragingMode.CYCLIC
+        ),
+    )
+
+    sequences, all_ro_pulses = [], []
 
-        # retrieve the results for every qubit
-        for qubit in qubits:
-            r1 = result1[ro_pulses[qubit].serial]
-            r2 = result2[ro_pulses[qubit].serial]
-            # store the results
+    # sweep the parameter
+    for wait in ro_wait_range:
+        # save data as often as defined by points
+
+        for qubit in targets:
+            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait // 2
+            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait // 2
+            ro_pulses[qubit].start = RX90_pulses2[qubit].finish
+
+        sequences.append(deepcopy(sequence))
+        all_ro_pulses.append(deepcopy(sequence).ro_pulses)
+
+    if params.unrolling:
+        results = platform.execute_pulse_sequences(sequences, options)
+
+    elif not params.unrolling:
+        results = [
+            platform.execute_pulse_sequence(sequence, options) for sequence in sequences
+        ]
+
+    data = SpinEchoSignalData()
+    for ig, (wait, ro_pulses) in enumerate(zip(ro_wait_range, all_ro_pulses)):
+        for qubit in targets:
+            serial = ro_pulses.get_qubit_pulses(qubit)[0].serial
+            if params.unrolling:
+                result = results[serial][0]
+            else:
+                result = results[ig][serial]
+            if params.single_shot:
+                _wait = np.array(len(result.magnitude) * [wait])
+            else:
+                _wait = np.array([wait])
             data.register_qubit(
-                DragPulseTuningType,
+                CoherenceType,
                 (qubit),
                 dict(
-                    signal=np.array([r1.magnitude - r2.magnitude]),
-                    beta=np.array([beta_param]),
+                    wait=_wait,
+                    signal=np.array([result.magnitude]),
+                    phase=np.array([result.phase]),
                 ),
             )
 
+    if params.single_shot:
+        data.data = {
+            qubit: values.reshape((len(ro_wait_range), params.nshots)).T
+            for qubit, values in data.data.items()
+        }
+
     return data
 
 
-def drag_fit(x, p0, p1, p2, p3):
-    # Offset                  : p[0]
-    # Amplitude               : p[1]
-    # Period                  : p[2]
-    # Phase                   : p[3]
-    return p0 + p1 * np.cos(2 * np.pi * x / p2 + p3)
-
-
-def _fit(data: DragPulseTuningData) -> DragPulseTuningResults:
-    r"""
-    Fitting routine for drag tunning. The used model is
-
-        .. math::
-
-            y = p_1 cos \Big(\frac{2 \pi x}{p_2} + p_3 \Big) + p_0.
-
-    """
-    qubits = data.qubits
-    betas_optimal = {}
-    fitted_parameters = {}
-
-    for qubit in qubits:
-        qubit_data = data[qubit]
-        voltages = qubit_data.signal
-        beta_params = qubit_data.beta
-
-        try:
-            popt, pcov = curve_fit(drag_fit, beta_params, voltages)
-            smooth_dataset = drag_fit(beta_params, popt[0], popt[1], popt[2], popt[3])
-            min_abs_index = np.abs(smooth_dataset).argmin()
-            beta_optimal = beta_params[min_abs_index]
-        except:
-            log.warning("drag_tuning_fit: the fitting was not succesful")
-            popt = np.array([0, 0, 1, 0])
-            beta_optimal = 0
-
-        fitted_parameters[qubit] = popt.tolist()
-        betas_optimal[qubit] = beta_optimal
-    return DragPulseTuningResults(betas_optimal, fitted_parameters)
+def _fit(data: SpinEchoSignalData) -> SpinEchoSignalResults:
+    """Post-processing for SpinEcho."""
+    data = data.average
+
+    t2echos, fitted_parameters, pcov = exponential_fit(data)
 
+    return SpinEchoSignalResults(t2echos, fitted_parameters, pcov)
 
-def _plot(data: DragPulseTuningData, qubit, fit: DragPulseTuningResults):
-    """Plotting function for DragPulseTuning."""
+
+def _plot(data: SpinEchoSignalData, target: QubitId, fit: SpinEchoSignalResults = None):
+    """Plotting for SpinEcho"""
+    data = data.average
 
     figures = []
-    fitting_report = ""
+    fig = go.Figure()
+
+    # iterate over multiple data folders
+    fitting_report = None
+
+    qubit_data = data[target]
+    waits = qubit_data.wait
 
-    fig = make_subplots(
-        rows=1,
-        cols=1,
-        horizontal_spacing=0.01,
-        vertical_spacing=0.01,
-    )
-    qubit_data = data[qubit]
     fig.add_trace(
         go.Scatter(
-            x=qubit_data.beta,
+            x=waits,
             y=qubit_data.signal,
-            mode="markers",
-            name="Probability",
+            opacity=1,
+            name="Signal",
             showlegend=True,
-            legendgroup="group1",
+            legendgroup="Signal",
         ),
     )
 
-    # add fitting traces
     if fit is not None:
-        beta_range = np.linspace(
-            min(qubit_data.beta),
-            max(qubit_data.beta),
-            20,
+        # add fitting trace
+        waitrange = np.linspace(
+            min(waits),
+            max(waits),
+            2 * len(qubit_data),
         )
+        params = fit.fitted_parameters[target]
 
         fig.add_trace(
             go.Scatter(
-                x=beta_range,
-                y=drag_fit(
-                    beta_range,
-                    float(fit.fitted_parameters[qubit][0]),
-                    float(fit.fitted_parameters[qubit][1]),
-                    float(fit.fitted_parameters[qubit][2]),
-                    float(fit.fitted_parameters[qubit][3]),
-                ),
+                x=waitrange,
+                y=exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             ),
         )
+
         fitting_report = table_html(
-            table_dict(qubit, "Optimal Beta Param", np.round(fit.betas[qubit], 4))
+            table_dict(
+                target,
+                ["T2 Spin Echo [ns]"],
+                [np.round(fit.t2_spin_echo[target])],
+                display_error=True,
+            )
         )
 
     fig.update_layout(
         showlegend=True,
-        xaxis_title="Beta parameter",
-        yaxis_title="Signal [a.u.] [Rx(pi/2) - Ry(pi)] - [Ry(pi/2) - Rx(pi)]",
+        xaxis_title="Time [ns]",
+        yaxis_title="Signal [a.u.]",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: DragPulseTuningResults, platform: Platform, qubit: QubitId):
-    update.drag_pulse_beta(results.betas[qubit], platform, qubit)
+def _update(results: SpinEchoSignalResults, platform: Platform, target: QubitId):
+    update.t2_spin_echo(results.t2_spin_echo[target], platform, target)
 
 
-drag_pulse_tuning = Routine(_acquisition, _fit, _plot, _update)
-"""DragPulseTuning Routine object."""
+spin_echo_signal = Routine(_acquisition, _fit, _plot, _update)
+"""SpinEcho Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/classification.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/classification.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,22 +10,15 @@
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from sklearn.metrics import roc_auc_score, roc_curve
 
 from qibocal import update
-from qibocal.auto.operation import (
-    RESULTSFILE,
-    Data,
-    Parameters,
-    Qubits,
-    Results,
-    Routine,
-)
+from qibocal.auto.operation import RESULTSFILE, Data, Parameters, Results, Routine
 from qibocal.auto.serialize import serialize
 from qibocal.fitting.classifier import run
 from qibocal.protocols.characterization.utils import (
     LEGEND_FONT_SIZE,
     MESH_SIZE,
     TITLE_SIZE,
     evaluate_grid,
@@ -127,45 +120,43 @@
                 classifier.savedir.mkdir(parents=True, exist_ok=True)
                 dump_dir = classifier.base_dir / classifier.name / classifier.name
                 classifier.dump()(self.models[qubit][i], dump_dir)
                 classifier.dump_hyper(self.classifiers_hpars[qubit][classifier.name])
         asdict_class = asdict(self)
         asdict_class.pop("models")
         asdict_class.pop("classifiers_hpars")
-        (path / RESULTSFILE).write_text(json.dumps(serialize(asdict_class)))
+        (path / f"{RESULTSFILE}.json").write_text(json.dumps(serialize(asdict_class)))
 
 
 def _acquisition(
     params: SingleShotClassificationParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> SingleShotClassificationData:
     """
     Args:
         nshots (int): number of times the pulse sequence will be repeated.
         classifiers (list): list of classifiers, the available ones are:
             - linear_svm
             - ada_boost
             - gaussian_process
             - naive_bayes
-            - nn
             - qubit_fit
             - random_forest
             - rbf_svm
             - qblox_fit.
         The default value is `["qubit_fit"]`.
         savedir (str): Dumping folder of the classification results.
         If not given the dumping folder will be the report one.
         relaxation_time (float): Relaxation time.
 
         Example:
         .. code-block:: yaml
 
             - id: single_shot_classification_1
-                priority: 0
                 operation: single_shot_classification
                 parameters:
                 nshots: 5000
                 savedir: "single_shot"
                 classifiers_list: ["qubit_fit","naive_bayes", "linear_svm"]
 
     """
@@ -176,30 +167,30 @@
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequences, all_ro_pulses = [], []
     for state in [0, 1]:
         sequence = PulseSequence()
         RX_pulses = {}
         ro_pulses = {}
-        for qubit in qubits:
+        for qubit in targets:
             RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
             ro_pulses[qubit] = platform.create_qubit_readout_pulse(
                 qubit, start=RX_pulses[qubit].finish
             )
             if state == 1:
                 sequence.add(RX_pulses[qubit])
             sequence.add(ro_pulses[qubit])
 
         sequences.append(sequence)
         all_ro_pulses.append(ro_pulses)
 
     data = SingleShotClassificationData(
         nshots=params.nshots,
         qubit_frequencies={
-            qubit: platform.qubits[qubit].drive_frequency for qubit in qubits
+            qubit: platform.qubits[qubit].drive_frequency for qubit in targets
         },
         classifiers_list=params.classifiers_list,
         savedir=params.savedir,
     )
 
     options = ExecutionParameters(
         nshots=params.nshots,
@@ -211,15 +202,15 @@
         results = platform.execute_pulse_sequences(sequences, options)
     else:
         results = [
             platform.execute_pulse_sequence(sequence, options) for sequence in sequences
         ]
 
     for ig, (state, ro_pulses) in enumerate(zip([0, 1], all_ro_pulses)):
-        for qubit in qubits:
+        for qubit in targets:
             serial = ro_pulses[qubit].serial
             if params.unrolling:
                 result = results[serial][ig]
             else:
                 result = results[ig][serial]
             data.register_qubit(
                 ClassificationType,
@@ -307,31 +298,33 @@
         savedir=data.savedir,
         y_preds=y_test_predict,
         grid_preds=grid_preds_dict,
     )
 
 
 def _plot(
-    data: SingleShotClassificationData, qubit, fit: SingleShotClassificationResults
+    data: SingleShotClassificationData,
+    target: QubitId,
+    fit: SingleShotClassificationResults,
 ):
     fitting_report = ""
     models_name = data.classifiers_list
-    figures = plot_results(data, qubit, 2, fit)
+    figures = plot_results(data, target, 2, fit)
     if fit is not None:
-        y_test = fit.y_tests[qubit]
-        y_pred = fit.y_preds[qubit]
+        y_test = fit.y_tests[target]
+        y_pred = fit.y_preds[target]
 
         if len(models_name) != 1:
             # Evaluate the ROC curve
             fig_roc = go.Figure()
             fig_roc.add_shape(
                 type="line", line=dict(dash="dash"), x0=0.0, x1=1.0, y0=0.0, y1=1.0
             )
             for i, model in enumerate(models_name):
-                y_pred = fit.y_preds[qubit][i]
+                y_pred = fit.y_preds[target][i]
                 fpr, tpr, _ = roc_curve(y_test, y_pred)
                 auc_score = roc_auc_score(y_test, y_pred)
                 name = f"{model} (AUC={auc_score:.2f})"
                 fig_roc.add_trace(
                     go.Scatter(
                         x=fpr,
                         y=tpr,
@@ -355,47 +348,47 @@
                 range=[0, 1],
             )
             figures.append(fig_roc)
 
         if "qubit_fit" in models_name:
             fitting_report = table_html(
                 table_dict(
-                    qubit,
+                    target,
                     [
                         "Average State 0",
                         "Average State 1",
                         "Rotational Angle",
                         "Threshold",
                         "Readout Fidelity",
                         "Assignment Fidelity",
                         "Effective Qubit Temperature [K]",
                     ],
                     [
-                        np.round(fit.mean_gnd_states[qubit], 3),
-                        np.round(fit.mean_exc_states[qubit], 3),
-                        np.round(fit.rotation_angle[qubit], 3),
-                        np.round(fit.threshold[qubit], 6),
-                        np.round(fit.fidelity[qubit], 3),
-                        np.round(fit.assignment_fidelity[qubit], 3),
+                        np.round(fit.mean_gnd_states[target], 3),
+                        np.round(fit.mean_exc_states[target], 3),
+                        np.round(fit.rotation_angle[target], 3),
+                        np.round(fit.threshold[target], 6),
+                        np.round(fit.fidelity[target], 3),
+                        np.round(fit.assignment_fidelity[target], 3),
                         format_error_single_cell(
-                            round_report([fit.effective_temperature[qubit]])
+                            round_report([fit.effective_temperature[target]])
                         ),
                     ],
                 )
             )
 
     return figures, fitting_report
 
 
 def _update(
-    results: SingleShotClassificationResults, platform: Platform, qubit: QubitId
+    results: SingleShotClassificationResults, platform: Platform, target: QubitId
 ):
-    update.iq_angle(results.rotation_angle[qubit], platform, qubit)
-    update.threshold(results.threshold[qubit], platform, qubit)
-    update.mean_gnd_states(results.mean_gnd_states[qubit], platform, qubit)
-    update.mean_exc_states(results.mean_exc_states[qubit], platform, qubit)
-    update.readout_fidelity(results.fidelity[qubit], platform, qubit)
-    update.assignment_fidelity(results.assignment_fidelity[qubit], platform, qubit)
+    update.iq_angle(results.rotation_angle[target], platform, target)
+    update.threshold(results.threshold[target], platform, target)
+    update.mean_gnd_states(results.mean_gnd_states[target], platform, target)
+    update.mean_exc_states(results.mean_exc_states[target], platform, target)
+    update.readout_fidelity(results.fidelity[target], platform, target)
+    update.assignment_fidelity(results.assignment_fidelity[target], platform, target)
 
 
 single_shot_classification = Routine(_acquisition, _fit, _plot, _update)
 """Qubit classification routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/spin_echo.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/spin_echo.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,59 @@
+from copy import deepcopy
 from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal import update
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 
-from ..utils import chi2_reduced, table_dict, table_html
+from ..utils import table_dict, table_html
 from . import t1
+from .spin_echo_signal import SpinEchoSignalParameters, SpinEchoSignalResults, _update
 from .utils import exp_decay, exponential_fit_probability
 
 
 @dataclass
-class SpinEchoParameters(Parameters):
+class SpinEchoParameters(SpinEchoSignalParameters):
     """SpinEcho runcard inputs."""
 
-    delay_between_pulses_start: int
-    """Initial delay between pulses [ns]."""
-    delay_between_pulses_end: int
-    """Final delay between pulses [ns]."""
-    delay_between_pulses_step: int
-    """Step delay between pulses [ns]."""
-
 
 @dataclass
-class SpinEchoResults(Results):
+class SpinEchoResults(SpinEchoSignalResults):
     """SpinEcho outputs."""
 
-    t2_spin_echo: dict[QubitId, float]
-    """T2 echo for each qubit."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
     chi2: Optional[dict[QubitId, tuple[float, Optional[float]]]] = field(
         default_factory=dict
     )
     """Chi squared estimate mean value and error."""
 
 
 class SpinEchoData(t1.T1Data):
     """SpinEcho acquisition outputs."""
 
 
 def _acquisition(
     params: SpinEchoParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> SpinEchoData:
     """Data acquisition for SpinEcho"""
     # create a sequence of pulses for the experiment:
     # Spin Echo 3 Pulses: RX(pi/2) - wait t(rotates z) - RX(pi) - wait t(rotates z) - RX(pi/2) - readout
     ro_pulses = {}
     RX90_pulses1 = {}
     RX_pulses = {}
     RX90_pulses2 = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
         RX_pulses[qubit] = platform.create_RX_pulse(
             qubit, start=RX90_pulses1[qubit].finish
         )
         RX90_pulses2[qubit] = platform.create_RX90_pulse(
             qubit, start=RX_pulses[qubit].finish
         )
@@ -79,77 +69,79 @@
     # delay between pulses
     ro_wait_range = np.arange(
         params.delay_between_pulses_start,
         params.delay_between_pulses_end,
         params.delay_between_pulses_step,
     )
 
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.DISCRIMINATION,
+        averaging_mode=AveragingMode.SINGLESHOT,
+    )
+
     data = SpinEchoData()
-    probs = {qubit: [] for qubit in qubits}
+    sequences, all_ro_pulses = [], []
     # sweep the parameter
     for wait in ro_wait_range:
         # save data as often as defined by points
 
-        for qubit in qubits:
-            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait
-            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait
+        for qubit in targets:
+            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait // 2
+            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait // 2
             ro_pulses[qubit].start = RX90_pulses2[qubit].finish
 
-        # execute the pulse sequence
-        results = platform.execute_pulse_sequence(
-            sequence,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.DISCRIMINATION,
-                averaging_mode=AveragingMode.SINGLESHOT,
-            ),
-        )
+        sequences.append(deepcopy(sequence))
+        all_ro_pulses.append(deepcopy(sequence).ro_pulses)
 
-        for qubit in qubits:
-            prob = results[ro_pulses[qubit].serial].probability(state=0)
-            probs[qubit].append(prob)
-
-    for qubit in qubits:
-        errors = [np.sqrt(prob * (1 - prob) / params.nshots) for prob in probs[qubit]]
-        data.register_qubit(
-            t1.CoherenceProbType,
-            (qubit),
-            dict(wait=ro_wait_range, prob=probs[qubit], error=errors),
-        )
+    if params.unrolling:
+        results = platform.execute_pulse_sequences(sequences, options)
+
+    elif not params.unrolling:
+        results = [
+            platform.execute_pulse_sequence(sequence, options) for sequence in sequences
+        ]
+
+    for ig, (wait, ro_pulses) in enumerate(zip(ro_wait_range, all_ro_pulses)):
+        for qubit in targets:
+            serial = ro_pulses.get_qubit_pulses(qubit)[0].serial
+            if params.unrolling:
+                result = results[serial][0]
+            else:
+                result = results[ig][serial]
+            prob = result.probability(state=0)
+            error = np.sqrt(prob * (1 - prob) / params.nshots)
+            data.register_qubit(
+                t1.CoherenceProbType,
+                (qubit),
+                dict(
+                    wait=np.array([wait]),
+                    prob=np.array([prob]),
+                    error=np.array([error]),
+                ),
+            )
 
     return data
 
 
 def _fit(data: SpinEchoData) -> SpinEchoResults:
     """Post-processing for SpinEcho."""
-    t2Echos, fitted_parameters = exponential_fit_probability(data)
-    chi2 = {
-        qubit: (
-            chi2_reduced(
-                data[qubit].prob,
-                exp_decay(data[qubit].wait, *fitted_parameters[qubit]),
-                data[qubit].error,
-            ),
-            np.sqrt(2 / len(data[qubit].prob)),
-        )
-        for qubit in data.qubits
-    }
-
+    t2Echos, fitted_parameters, chi2 = exponential_fit_probability(data)
     return SpinEchoResults(t2Echos, fitted_parameters, chi2)
 
 
-def _plot(data: SpinEchoData, qubit, fit: SpinEchoResults = None):
+def _plot(data: SpinEchoData, target: QubitId, fit: SpinEchoResults = None):
     """Plotting for SpinEcho"""
 
     figures = []
     # iterate over multiple data folders
     fitting_report = ""
 
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     waits = qubit_data.wait
     probs = qubit_data.prob
     error_bars = qubit_data.error
 
     fig = go.Figure(
         [
             go.Scatter(
@@ -176,29 +168,29 @@
     if fit is not None:
         # add fitting trace
         waitrange = np.linspace(
             min(waits),
             max(waits),
             2 * len(qubit_data),
         )
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
 
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             ),
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["T2 Spin Echo [ns]", "chi2 reduced"],
-                [fit.t2_spin_echo[qubit], fit.chi2[qubit]],
+                [fit.t2_spin_echo[target], fit.chi2[target]],
                 display_error=True,
             )
         )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Time [ns]",
@@ -206,13 +198,9 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: SpinEchoResults, platform: Platform, qubit: QubitId):
-    update.t2_spin_echo(results.t2_spin_echo[qubit], platform, qubit)
-
-
 spin_echo = Routine(_acquisition, _fit, _plot, _update)
 """SpinEcho Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/spin_echo_sequence.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_signal.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,173 +2,196 @@
 
 import numpy as np
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
+from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Parameters, Results, Routine
 
 from ..utils import table_dict, table_html
-from . import spin_echo
-from .t1_signal import CoherenceType, T1SignalData
-from .utils import exp_decay, exponential_fit
+from . import t1_signal, t2, utils
 
 
 @dataclass
-class SpinEchoSignalParameters(spin_echo.SpinEchoParameters):
-    """SpinEcho Signal runcard inputs."""
+class T2SignalParameters(Parameters):
+    """T2Signal runcard inputs."""
 
+    delay_between_pulses_start: int
+    """Initial delay between RX(pi/2) pulses in ns."""
+    delay_between_pulses_end: int
+    """Final delay between RX(pi/2) pulses in ns."""
+    delay_between_pulses_step: int
+    """Step delay between RX(pi/2) pulses in ns."""
+    single_shot: bool = False
+    """If ``True`` save single shot signal data."""
 
-@dataclass
-class SpinEchoSignalResults(spin_echo.SpinEchoResults):
-    """SpinEchoSignal outputs."""
 
+@dataclass
+class T2SignalResults(Results):
+    """T2Signal outputs."""
 
-class SpinEchoSignalData(T1SignalData):
-    """SpinEcho acquisition outputs."""
+    t2: dict[QubitId, tuple[float]]
+    """T2 for each qubit [ns]."""
+    fitted_parameters: dict[QubitId, dict[str, float]]
+    """Raw fitting output."""
+    pcov: dict[QubitId, list[float]]
+    """Approximate covariance of fitted parameters."""
+
+
+class T2SignalData(t1_signal.T1SignalData):
+    """T2Signal acquisition outputs."""
+
+    t2: dict[QubitId, float]
+    """T2 for each qubit [ns]."""
+    fitted_parameters: dict[QubitId, dict[str, float]]
+    """Raw fitting output."""
 
 
 def _acquisition(
-    params: SpinEchoSignalParameters,
+    params: T2SignalParameters,
     platform: Platform,
-    qubits: Qubits,
-) -> SpinEchoSignalData:
-    """Data acquisition for SpinEcho"""
-    # create a sequence of pulses for the experiment:
-    # Spin Echo 3 Pulses: RX(pi/2) - wait t(rotates z) - RX(pi) - wait t(rotates z) - RX(pi/2) - readout
+    targets: list[QubitId],
+) -> T2SignalData:
+    """Data acquisition for Ramsey Experiment (detuned)."""
+    # create a sequence of pulses for the experiment
+    # RX90 - t - RX90 - MZ
     ro_pulses = {}
     RX90_pulses1 = {}
-    RX_pulses = {}
     RX90_pulses2 = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
-        RX_pulses[qubit] = platform.create_RX_pulse(
-            qubit, start=RX90_pulses1[qubit].finish
-        )
         RX90_pulses2[qubit] = platform.create_RX90_pulse(
-            qubit, start=RX_pulses[qubit].finish
+            qubit,
+            start=RX90_pulses1[qubit].finish,
         )
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=RX90_pulses2[qubit].finish
         )
         sequence.add(RX90_pulses1[qubit])
-        sequence.add(RX_pulses[qubit])
         sequence.add(RX90_pulses2[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
-    # delay between pulses
-    ro_wait_range = np.arange(
+    waits = np.arange(
+        # wait time between RX90 pulses
         params.delay_between_pulses_start,
         params.delay_between_pulses_end,
         params.delay_between_pulses_step,
     )
 
-    data = SpinEchoSignalData()
+    sweeper = Sweeper(
+        Parameter.start,
+        waits,
+        [RX90_pulses2[qubit] for qubit in targets],
+        type=SweeperType.ABSOLUTE,
+    )
 
-    # sweep the parameter
-    for wait in ro_wait_range:
-        # save data as often as defined by points
-
-        for qubit in qubits:
-            RX_pulses[qubit].start = RX90_pulses1[qubit].finish + wait
-            RX90_pulses2[qubit].start = RX_pulses[qubit].finish + wait
-            ro_pulses[qubit].start = RX90_pulses2[qubit].finish
-
-        # execute the pulse sequence
-        results = platform.execute_pulse_sequence(
-            sequence,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.INTEGRATION,
-                averaging_mode=AveragingMode.CYCLIC,
+    # execute the sweep
+    results = platform.sweep(
+        sequence,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=(
+                AveragingMode.SINGLESHOT if params.single_shot else AveragingMode.CYCLIC
             ),
-        )
+        ),
+        sweeper,
+    )
 
-        for qubit in qubits:
-            result = results[ro_pulses[qubit].serial]
-            data.register_qubit(
-                CoherenceType,
-                (qubit),
-                dict(
-                    wait=np.array([wait]),
-                    signal=np.array([result.magnitude]),
-                    phase=np.array([result.phase]),
-                ),
-            )
+    data = T2SignalData()
+    for qubit in targets:
+        result = results[ro_pulses[qubit].serial]
+        if params.single_shot:
+            _waits = np.array(len(result.magnitude) * [waits])
+        else:
+            _waits = waits
+        data.register_qubit(
+            utils.CoherenceType,
+            (qubit),
+            dict(wait=_waits, signal=result.magnitude, phase=result.phase),
+        )
     return data
 
 
-def _fit(data: SpinEchoSignalData) -> SpinEchoSignalResults:
-    """Post-processing for SpinEcho."""
-    t2Echos, fitted_parameters = exponential_fit(data)
+def _fit(data: T2SignalData) -> T2SignalResults:
+    r"""
+    Fitting routine for Ramsey experiment. The used model is
+    .. math::
+        y = p_0 - p_1 e^{-x p_2}.
+    """
+    data = data.average
+
+    t2s, fitted_parameters, pcovs = utils.exponential_fit(data)
+    return T2SignalResults(t2s, fitted_parameters, pcovs)
 
-    return SpinEchoSignalResults(t2Echos, fitted_parameters)
 
-
-def _plot(data: SpinEchoSignalData, qubit, fit: SpinEchoSignalResults = None):
-    """Plotting for SpinEcho"""
+def _plot(data: T2SignalData, target: QubitId, fit: T2SignalResults = None):
+    """Plotting function for Ramsey Experiment."""
+    data = data.average
 
     figures = []
     fig = go.Figure()
-
-    # iterate over multiple data folders
     fitting_report = None
 
-    qubit_data = data[qubit]
-    waits = qubit_data.wait
+    qubit_data = data[target]
 
     fig.add_trace(
         go.Scatter(
-            x=waits,
+            x=qubit_data.wait,
             y=qubit_data.signal,
             opacity=1,
             name="Signal",
             showlegend=True,
             legendgroup="Signal",
-        ),
+        )
     )
 
     if fit is not None:
         # add fitting trace
         waitrange = np.linspace(
-            min(waits),
-            max(waits),
+            min(qubit_data.wait),
+            max(qubit_data.wait),
             2 * len(qubit_data),
         )
-        params = fit.fitted_parameters[qubit]
 
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
-                y=exp_decay(waitrange, *params),
+                y=utils.exp_decay(
+                    waitrange,
+                    *params,
+                ),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
-            ),
+            )
         )
-
         fitting_report = table_html(
-            table_dict(qubit, "T2 Spin Echo [ns]", np.round(fit.t2_spin_echo[qubit]))
+            table_dict(
+                target, ["T2 [ns]"], [np.round(fit.t2[target])], display_error=True
+            )
         )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Time [ns]",
         yaxis_title="Signal [a.u.]",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: SpinEchoSignalResults, platform: Platform, qubit: QubitId):
-    update.t2_spin_echo(results.t2_spin_echo[qubit], platform, qubit)
+def _update(results: T2SignalResults, platform: Platform, target: QubitId):
+    update.t2(results.t2[target], platform, target)
 
 
-spin_echo_sequence = Routine(_acquisition, _fit, _plot, _update)
-"""SpinEcho Routine object."""
+t2_signal = Routine(_acquisition, _fit, _plot, _update)
+"""T2Signal Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,32 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Routine
 
-from ..utils import chi2_reduced, table_dict, table_html
-from . import utils
+from ..utils import table_dict, table_html
+from . import t1_signal, utils
 
 COLORBAND = "rgba(0,100,80,0.2)"
 COLORBAND_LINE = "rgba(255,255,255,0)"
 
 
 @dataclass
-class T1Parameters(Parameters):
+class T1Parameters(t1_signal.T1SignalParameters):
     """T1 runcard inputs."""
 
-    delay_before_readout_start: int
-    """Initial delay before readout [ns]."""
-    delay_before_readout_end: int
-    """Final delay before readout [ns]."""
-    delay_before_readout_step: int
-    """Step delay before readout [ns]."""
-
 
 @dataclass
-class T1Results(Results):
+class T1Results(t1_signal.T1SignalResults):
     """T1 outputs."""
 
-    t1: dict[QubitId, tuple[float]]
-    """T1 for each qubit."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
     chi2: Optional[dict[QubitId, tuple[float, Optional[float]]]] = field(
         default_factory=dict
     )
     """Chi squared estimate mean value and error."""
 
 
 CoherenceProbType = np.dtype(
@@ -56,39 +44,41 @@
 class T1Data(Data):
     """T1 acquisition outputs."""
 
     data: dict[QubitId, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
 
-def _acquisition(params: T1Parameters, platform: Platform, qubits: Qubits) -> T1Data:
+def _acquisition(
+    params: T1Parameters, platform: Platform, targets: list[QubitId]
+) -> T1Data:
     r"""Data acquisition for T1 experiment.
     In a T1 experiment, we measure an excited qubit after a delay. Due to decoherence processes
     (e.g. amplitude damping channel), it is possible that, at the time of measurement, after the delay,
     the qubit will not be excited anymore. The larger the delay time is, the more likely is the qubit to
     fall to the ground state. The goal of the experiment is to characterize the decay rate of the qubit
     towards the ground state.
 
     Args:
         params:
         platform (Platform): Qibolab platform object
-        qubits (list): list of target qubits to perform the action
+        targets (list): list of target qubits to perform the action
         delay_before_readout_start (int): Initial time delay before ReadOut
         delay_before_readout_end (list): Maximum time delay before ReadOut
         delay_before_readout_step (int): Scan range step for the delay before ReadOut
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
     """
 
     # create a sequence of pulses for the experiment
     # RX - wait t - MZ
     qd_pulses = {}
     ro_pulses = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].duration
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
@@ -99,15 +89,15 @@
         params.delay_before_readout_end,
         params.delay_before_readout_step,
     )
 
     sweeper = Sweeper(
         Parameter.start,
         ro_wait_range,
-        [ro_pulses[qubit] for qubit in qubits],
+        [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
     data = T1Data()
 
     # sweep the parameter
     # execute the pulse sequence
@@ -118,15 +108,15 @@
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.DISCRIMINATION,
             averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
 
-    for qubit in qubits:
+    for qubit in targets:
         probs = results[ro_pulses[qubit].serial].probability(state=1)
         errors = np.sqrt(probs * (1 - probs) / params.nshots)
         data.register_qubit(
             CoherenceProbType,
             (qubit),
             dict(wait=ro_wait_range, prob=probs, error=errors),
         )
@@ -138,36 +128,24 @@
     """
     Fitting routine for T1 experiment. The used model is
 
         .. math::
 
             y = p_0-p_1 e^{-x p_2}.
     """
-    t1s, fitted_parameters = utils.exponential_fit_probability(data)
-    chi2 = {
-        qubit: (
-            chi2_reduced(
-                data[qubit].prob,
-                utils.exp_decay(data[qubit].wait, *fitted_parameters[qubit]),
-                data[qubit].error,
-            ),
-            np.sqrt(2 / len(data[qubit].prob)),
-        )
-        for qubit in data.qubits
-    }
-
+    t1s, fitted_parameters, chi2 = utils.exponential_fit_probability(data)
     return T1Results(t1s, fitted_parameters, chi2)
 
 
-def _plot(data: T1Data, qubit, fit: T1Results = None):
+def _plot(data: T1Data, target: QubitId, fit: T1Results = None):
     """Plotting function for T1 experiment."""
 
     figures = []
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     waits = qubit_data.wait
     probs = qubit_data.prob
     error_bars = qubit_data.error
 
     fig = go.Figure(
         [
             go.Scatter(
@@ -194,31 +172,31 @@
     if fit is not None:
         waitrange = np.linspace(
             min(waits),
             max(waits),
             2 * len(qubit_data),
         )
 
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=utils.exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "T1 [ns]",
                     "chi2 reduced",
                 ],
-                [fit.t1[qubit], fit.chi2[qubit]],
+                [fit.t1[target], fit.chi2[target]],
                 display_error=True,
             )
         )
     # last part
     fig.update_layout(
         showlegend=True,
         xaxis_title="Time [ns]",
@@ -226,13 +204,9 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: T1Results, platform: Platform, qubit: QubitId):
-    update.t1(results.t1[qubit], platform, qubit)
-
-
-t1 = Routine(_acquisition, _fit, _plot, _update)
+t1 = Routine(_acquisition, _fit, _plot, t1_signal._update)
 """T1 Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1_sequences.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_sequences.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
-from . import t1, t1_signal
+from . import t1_signal
+from .utils import CoherenceType
 
 
 def _acquisition(
-    params: t1_signal.T1SignalParameters, platform: Platform, qubits: Qubits
+    params: t1_signal.T1SignalParameters, platform: Platform, targets: list[QubitId]
 ) -> t1_signal.T1SignalData:
     r"""Data acquisition for T1 experiment.
     In a T1 experiment, we measure an excited qubit after a delay. Due to decoherence processes
     (e.g. amplitude damping channel), it is possible that, at the time of measurement, after the delay,
     the qubit will not be excited anymore. The larger the delay time is, the more likely is the qubit to
     fall to the ground state. The goal of the experiment is to characterize the decay rate of the qubit
     towards the ground state.
 
     Args:
         params:
         platform (Platform): Qibolab platform object
-        qubits (list): list of target qubits to perform the action
+        targets (list): list of target qubits to perform the action
         delay_before_readout_start (int): Initial time delay before ReadOut
         delay_before_readout_end (list): Maximum time delay before ReadOut
         delay_before_readout_step (int): Scan range step for the delay before ReadOut
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
     """
 
     # create a sequence of pulses for the experiment
     # RX - wait t - MZ
     qd_pulses = {}
     ro_pulses = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].duration
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
@@ -51,36 +53,36 @@
     )
 
     data = t1_signal.T1SignalData()
 
     # repeat the experiment as many times as defined by software_averages
     # sweep the parameter
     for wait in ro_wait_range:
-        for qubit in qubits:
+        for qubit in targets:
             ro_pulses[qubit].start = qd_pulses[qubit].duration + wait
 
         # execute the pulse sequence
         results = platform.execute_pulse_sequence(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
                 relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
         )
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             data.register_qubit(
-                t1_signal.CoherenceType,
+                CoherenceType,
                 (qubit),
                 dict(
                     wait=np.array([wait]),
                     signal=np.array([result.magnitude]),
                     phase=np.array([result.phase]),
                 ),
             )
     return data
 
 
-t1_sequences = Routine(_acquisition, t1_signal._fit, t1_signal._plot, t1._update)
+t1_sequences = Routine(_acquisition, t1_signal._fit, t1_signal._plot, t1_signal._update)
 """T1 Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t1_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t1_signal.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,71 +5,88 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Data, Qubits, Routine
+from qibocal import update
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from ..utils import table_dict, table_html
-from . import t1, utils
+from . import utils
 
 
 @dataclass
-class T1SignalParameters(t1.T1Parameters):
-    """T1 Signal runcard inputs."""
+class T1SignalParameters(Parameters):
+    """T1 runcard inputs."""
+
+    delay_before_readout_start: int
+    """Initial delay before readout [ns]."""
+    delay_before_readout_end: int
+    """Final delay before readout [ns]."""
+    delay_before_readout_step: int
+    """Step delay before readout [ns]."""
+    single_shot: bool = False
+    """If ``True`` save single shot signal data."""
 
 
 @dataclass
-class T1SignalResults(t1.T1Results):
+class T1SignalResults(Results):
     """T1 Signal outputs."""
 
-
-CoherenceType = np.dtype(
-    [("wait", np.float64), ("signal", np.float64), ("phase", np.float64)]
-)
-"""Custom dtype for coherence routines."""
+    t1: dict[QubitId, tuple[float]]
+    """T1 for each qubit."""
+    fitted_parameters: dict[QubitId, dict[str, float]]
+    """Raw fitting output."""
+    pcov: dict[QubitId, list[float]]
+    """Approximate covariance of fitted parameters."""
 
 
 @dataclass
 class T1SignalData(Data):
     """T1 acquisition outputs."""
 
     data: dict[QubitId, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
+    @property
+    def average(self):
+        if len(next(iter(self.data.values())).shape) > 1:
+            return utils.average_single_shots(self.__class__, self.data)
+        return self
+
 
 def _acquisition(
-    params: T1SignalParameters, platform: Platform, qubits: Qubits
+    params: T1SignalParameters, platform: Platform, targets: list[QubitId]
 ) -> T1SignalData:
     r"""Data acquisition for T1 experiment.
     In a T1 experiment, we measure an excited qubit after a delay. Due to decoherence processes
     (e.g. amplitude damping channel), it is possible that, at the time of measurement, after the delay,
     the qubit will not be excited anymore. The larger the delay time is, the more likely is the qubit to
     fall to the ground state. The goal of the experiment is to characterize the decay rate of the qubit
     towards the ground state.
 
     Args:
         params:
         platform (Platform): Qibolab platform object
-        qubits (list): list of target qubits to perform the action
+        targets (list): list of target qubits to perform the action
         delay_before_readout_start (int): Initial time delay before ReadOut
         delay_before_readout_end (list): Maximum time delay before ReadOut
         delay_before_readout_step (int): Scan range step for the delay before ReadOut
         software_averages (int): Number of executions of the routine for averaging results
         points (int): Save data results in a file every number of points
     """
 
     # create a sequence of pulses for the experiment
     # RX - wait t - MZ
     qd_pulses = {}
     ro_pulses = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].duration
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
@@ -80,65 +97,72 @@
         params.delay_before_readout_end,
         params.delay_before_readout_step,
     )
 
     sweeper = Sweeper(
         Parameter.start,
         ro_wait_range,
-        [ro_pulses[qubit] for qubit in qubits],
+        [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
-    data = T1SignalData()
-
     # sweep the parameter
     # execute the pulse sequence
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
+            averaging_mode=(
+                AveragingMode.SINGLESHOT if params.single_shot else AveragingMode.CYCLIC
+            ),
         ),
         sweeper,
     )
 
-    for qubit in qubits:
+    data = T1SignalData()
+    for qubit in targets:
         result = results[ro_pulses[qubit].serial]
+        if params.single_shot:
+            _waits = np.array(len(result.magnitude) * [ro_wait_range])
+        else:
+            _waits = ro_wait_range
         data.register_qubit(
-            CoherenceType,
+            utils.CoherenceType,
             (qubit),
-            dict(wait=ro_wait_range, signal=result.magnitude, phase=result.phase),
+            dict(wait=_waits, signal=result.magnitude, phase=result.phase),
         )
 
     return data
 
 
 def _fit(data: T1SignalData) -> T1SignalResults:
     """
     Fitting routine for T1 experiment. The used model is
 
         .. math::
 
             y = p_0-p_1 e^{-x p_2}.
     """
-    t1s, fitted_parameters = utils.exponential_fit(data)
+    data = data.average
+    t1s, fitted_parameters, pcovs = utils.exponential_fit(data)
 
-    return T1SignalResults(t1s, fitted_parameters)
+    return T1SignalResults(t1s, fitted_parameters, pcovs)
 
 
-def _plot(data: T1SignalData, qubit, fit: T1SignalResults = None):
+def _plot(data: T1SignalData, target: QubitId, fit: T1SignalResults = None):
     """Plotting function for T1 experiment."""
+    data = data.average
 
     figures = []
     fig = go.Figure()
 
     fitting_report = None
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     waits = qubit_data.wait
 
     fig.add_trace(
         go.Scatter(
             x=waits,
             y=qubit_data.signal,
             opacity=1,
@@ -151,34 +175,40 @@
     if fit is not None:
         waitrange = np.linspace(
             min(waits),
             max(waits),
             2 * len(qubit_data),
         )
 
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=utils.exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
-            table_dict(qubit, "T1 [ns]", np.round(fit.t1[qubit]))
+            table_dict(
+                target, ["T1 [ns]"], [np.round(fit.t1[target])], display_error=True
+            )
         )
 
     # last part
     fig.update_layout(
         showlegend=True,
         xaxis_title="Time [ns]",
         yaxis_title="Signal [a.u.]",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-t1_signal = Routine(_acquisition, _fit, _plot, t1._update)
+def _update(results: T1SignalResults, platform: Platform, target: QubitId):
+    update.t1(results.t1[target], platform, target)
+
+
+t1_signal = Routine(_acquisition, _fit, _plot, _update)
 """T1 Signal Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,64 +5,59 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal import update
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 
-from ..utils import chi2_reduced, table_dict, table_html
-from . import t1, utils
+from ..utils import table_dict, table_html
+from . import t1, t2_signal, utils
 
 
 @dataclass
-class T2Parameters(Parameters):
+class T2Parameters(t2_signal.T2SignalParameters):
     """T2 runcard inputs."""
 
     delay_between_pulses_start: int
     """Initial delay between RX(pi/2) pulses in ns."""
     delay_between_pulses_end: int
     """Final delay between RX(pi/2) pulses in ns."""
     delay_between_pulses_step: int
     """Step delay between RX(pi/2) pulses in ns."""
 
 
 @dataclass
-class T2Results(Results):
+class T2Results(t2_signal.T2SignalResults):
     """T2 outputs."""
 
-    t2: dict[QubitId, float]
-    """T2 for each qubit [ns]."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
     chi2: Optional[dict[QubitId, tuple[float, Optional[float]]]] = field(
         default_factory=dict
     )
     """Chi squared estimate mean value and error."""
 
 
 class T2Data(t1.T1Data):
     """T2 acquisition outputs."""
 
 
 def _acquisition(
     params: T2Parameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> T2Data:
     """Data acquisition for Ramsey Experiment (detuned)."""
     # create a sequence of pulses for the experiment
     # RX90 - t - RX90 - MZ
     ro_pulses = {}
     RX90_pulses1 = {}
     RX90_pulses2 = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
         RX90_pulses2[qubit] = platform.create_RX90_pulse(
             qubit,
             start=RX90_pulses1[qubit].finish,
         )
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=RX90_pulses2[qubit].finish
@@ -80,15 +75,15 @@
     )
 
     data = T2Data()
 
     sweeper = Sweeper(
         Parameter.start,
         waits,
-        [RX90_pulses2[qubit] for qubit in qubits],
+        [RX90_pulses2[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
     # execute the sweep
     results = platform.sweep(
         sequence,
         ExecutionParameters(
@@ -96,50 +91,39 @@
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.DISCRIMINATION,
             averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
 
-    for qubit in qubits:
+    for qubit in targets:
         probs = results[ro_pulses[qubit].serial].probability(state=1)
         errors = np.sqrt(probs * (1 - probs) / params.nshots)
         data.register_qubit(
             t1.CoherenceProbType, (qubit), dict(wait=waits, prob=probs, error=errors)
         )
     return data
 
 
 def _fit(data: T2Data) -> T2Results:
     r"""
     Fitting routine for Ramsey experiment. The used model is
     .. math::
         y = p_0 - p_1 e^{-x p_2}.
     """
-    t2s, fitted_parameters = utils.exponential_fit_probability(data)
-    chi2 = {
-        qubit: (
-            chi2_reduced(
-                data[qubit].prob,
-                utils.exp_decay(data[qubit].wait, *fitted_parameters[qubit]),
-                data[qubit].error,
-            ),
-            np.sqrt(2 / len(data[qubit].prob)),
-        )
-        for qubit in data.qubits
-    }
+    t2s, fitted_parameters, chi2 = utils.exponential_fit_probability(data)
     return T2Results(t2s, fitted_parameters, chi2)
 
 
-def _plot(data: T2Data, qubit, fit: T2Results = None):
+def _plot(data: T2Data, target: QubitId, fit: T2Results = None):
     """Plotting function for Ramsey Experiment."""
 
     figures = []
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     waits = qubit_data.wait
     probs = qubit_data.prob
     error_bars = qubit_data.error
 
     fig = go.Figure(
         [
             go.Scatter(
@@ -167,47 +151,43 @@
         # add fitting trace
         waitrange = np.linspace(
             min(qubit_data.wait),
             max(qubit_data.wait),
             2 * len(qubit_data),
         )
 
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=utils.exp_decay(
                     waitrange,
                     *params,
                 ),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "T2 [ns]",
                     "chi2 reduced",
                 ],
-                [fit.t2[qubit], fit.chi2[qubit]],
+                [fit.t2[target], fit.chi2[target]],
                 display_error=True,
             )
         )
     fig.update_layout(
         showlegend=True,
         xaxis_title="Time [ns]",
         yaxis_title="Probability of State 1",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: T2Results, platform: Platform, qubit: QubitId):
-    update.t2(results.t2[qubit], platform, qubit)
-
-
-t2 = Routine(_acquisition, _fit, _plot, _update)
+t2 = Routine(_acquisition, _fit, _plot, t2_signal._update)
 """T2 Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2_sequences.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/t2_sequences.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
-from .t1_signal import CoherenceType
 from .t2_signal import T2SignalData, T2SignalParameters, _fit, _plot, _update
+from .utils import CoherenceType
 
 
 def _acquisition(
     params: T2SignalParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> T2SignalData:
     """Data acquisition for Ramsey Experiment (detuned)."""
     # create a sequence of pulses for the experiment
     # RX90 - t - RX90 - MZ
     ro_pulses = {}
     RX90_pulses1 = {}
     RX90_pulses2 = {}
     sequence = PulseSequence()
-    for qubit in qubits:
+    for qubit in targets:
         RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
         RX90_pulses2[qubit] = platform.create_RX90_pulse(
             qubit,
             start=RX90_pulses1[qubit].finish,
         )
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=RX90_pulses2[qubit].finish
@@ -42,29 +43,29 @@
         params.delay_between_pulses_step,
     )
 
     data = T2SignalData()
 
     # sweep the parameter
     for wait in waits:
-        for qubit in qubits:
+        for qubit in targets:
             RX90_pulses2[qubit].start = RX90_pulses1[qubit].finish + wait
             ro_pulses[qubit].start = RX90_pulses2[qubit].finish
 
         # execute the pulse sequence
         results = platform.execute_pulse_sequence(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
                 relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
         )
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             data.register_qubit(
                 CoherenceType,
                 (qubit),
                 dict(
                     wait=np.array([wait]),
                     signal=np.array([result.magnitude]),
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/t2_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,166 +1,141 @@
-from dataclasses import dataclass
-
 import numpy as np
-import plotly.graph_objects as go
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
-from qibolab.platform import Platform
-from qibolab.pulses import PulseSequence
-from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
-
-from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
-
-from ..utils import table_dict, table_html
-from . import t1_signal, t2, utils
-
-
-@dataclass
-class T2SignalParameters(t2.T2Parameters):
-    """T2Signal runcard inputs."""
-
-
-@dataclass
-class T2SignalResults(t2.T2Results):
-    """T2Signal outputs."""
-
-
-class T2SignalData(t1_signal.T1SignalData):
-    """T2Signal acquisition outputs."""
-
-
-def _acquisition(
-    params: T2SignalParameters,
-    platform: Platform,
-    qubits: Qubits,
-) -> T2SignalData:
-    """Data acquisition for Ramsey Experiment (detuned)."""
-    # create a sequence of pulses for the experiment
-    # RX90 - t - RX90 - MZ
-    ro_pulses = {}
-    RX90_pulses1 = {}
-    RX90_pulses2 = {}
-    sequence = PulseSequence()
-    for qubit in qubits:
-        RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
-        RX90_pulses2[qubit] = platform.create_RX90_pulse(
-            qubit,
-            start=RX90_pulses1[qubit].finish,
-        )
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=RX90_pulses2[qubit].finish
-        )
-        sequence.add(RX90_pulses1[qubit])
-        sequence.add(RX90_pulses2[qubit])
-        sequence.add(ro_pulses[qubit])
-
-    # define the parameter to sweep and its range:
-    waits = np.arange(
-        # wait time between RX90 pulses
-        params.delay_between_pulses_start,
-        params.delay_between_pulses_end,
-        params.delay_between_pulses_step,
-    )
-
-    data = T2SignalData()
-
-    sweeper = Sweeper(
-        Parameter.start,
-        waits,
-        [RX90_pulses2[qubit] for qubit in qubits],
-        type=SweeperType.ABSOLUTE,
-    )
-
-    # execute the sweep
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        sweeper,
-    )
+from scipy.optimize import curve_fit
 
-    for qubit in qubits:
-        result = results[ro_pulses[qubit].serial]
-        data.register_qubit(
-            t1_signal.CoherenceType,
-            (qubit),
-            dict(wait=waits, signal=result.magnitude, phase=result.phase),
-        )
-    return data
+from qibocal.config import log
 
+from ..utils import chi2_reduced
 
-def _fit(data: T2SignalData) -> T2SignalResults:
-    r"""
-    Fitting routine for Ramsey experiment. The used model is
-    .. math::
-        y = p_0 - p_1 e^{-x p_2}.
-    """
-    t2s, fitted_parameters = utils.exponential_fit(data)
-    return T2SignalResults(t2s, fitted_parameters)
+CoherenceType = np.dtype(
+    [("wait", np.float64), ("signal", np.float64), ("phase", np.float64)]
+)
+"""Custom dtype for coherence routines."""
 
 
-def _plot(data: T2SignalData, qubit, fit: T2SignalResults = None):
-    """Plotting function for Ramsey Experiment."""
+def average_single_shots(data_type, single_shots):
+    """Convert single shot acquisition results of signal routines to averaged.
 
-    figures = []
-    fig = go.Figure()
-    fitting_report = None
-
-    qubit_data = data[qubit]
-
-    fig.add_trace(
-        go.Scatter(
-            x=qubit_data.wait,
-            y=qubit_data.signal,
-            opacity=1,
-            name="Signal",
-            showlegend=True,
-            legendgroup="Signal",
+    Args:
+        data_type: Type of produced data object (eg. ``T1SignalData``, ``T2SignalData`` etc.).
+        single_shots (dict): Dictionary containing acquired single shot data.
+    """
+    data = data_type()
+    for qubit, values in single_shots.items():
+        data.register_qubit(
+            CoherenceType,
+            (qubit),
+            {name: values[name].mean(axis=0) for name in values.dtype.names},
         )
-    )
+    return data
 
-    if fit is not None:
-        # add fitting trace
-        waitrange = np.linspace(
-            min(qubit_data.wait),
-            max(qubit_data.wait),
-            2 * len(qubit_data),
-        )
 
-        params = fit.fitted_parameters[qubit]
-        fig.add_trace(
-            go.Scatter(
-                x=waitrange,
-                y=utils.exp_decay(
-                    waitrange,
-                    *params,
-                ),
-                name="Fit",
-                line=go.scatter.Line(dash="dot"),
-            )
-        )
-        fitting_report = table_html(
-            table_dict(qubit, "T2 [ns]", np.round(fit.t2[qubit]))
-        )
+def exp_decay(x, *p):
+    return p[0] - p[1] * np.exp(-1 * x / p[2])
 
-    fig.update_layout(
-        showlegend=True,
-        xaxis_title="Time [ns]",
-        yaxis_title="Signal [a.u.]",
-    )
 
-    figures.append(fig)
+def exponential_fit(data, zeno=None):
+    qubits = data.qubits
 
-    return figures, fitting_report
+    decay = {}
+    fitted_parameters = {}
+    pcovs = {}
 
+    for qubit in qubits:
+        voltages = data[qubit].signal
+        if zeno:
+            times = np.arange(1, len(data[qubit].signal) + 1)
+        else:
+            times = data[qubit].wait
+
+        try:
+            y_max = np.max(voltages)
+            y_min = np.min(voltages)
+            y = (voltages - y_min) / (y_max - y_min)
+            x_max = np.max(times)
+            x_min = np.min(times)
+            x = (times - x_min) / (x_max - x_min)
+
+            p0 = [
+                0.5,
+                0.5,
+                5,
+            ]
+            popt, pcov = curve_fit(
+                exp_decay,
+                x,
+                y,
+                p0=p0,
+                maxfev=2000000,
+                bounds=(
+                    [-2, -2, 0],
+                    [2, 2, np.inf],
+                ),
+            )
+            popt = [
+                (y_max - y_min) * popt[0] + y_min,
+                (y_max - y_min) * popt[1] * np.exp(x_min * popt[2] / (x_max - x_min)),
+                popt[2] * (x_max - x_min),
+            ]
+            fitted_parameters[qubit] = popt
+            pcovs[qubit] = pcov.tolist()
+            decay[qubit] = (popt[2], np.sqrt(pcov[2, 2]) * (x_max - x_min))
+
+        except Exception as e:
+            log.warning(f"Exponential decay fit failed for qubit {qubit} due to {e}")
+
+    return decay, fitted_parameters, pcovs
+
+
+def exponential_fit_probability(data):
+    qubits = data.qubits
+
+    decay = {}
+    fitted_parameters = {}
+    chi2 = {}
 
-def _update(results: T2SignalResults, platform: Platform, qubit: QubitId):
-    update.t2(results.t2[qubit], platform, qubit)
+    for qubit in qubits:
+        times = data[qubit].wait
+        x_max = np.max(times)
+        x_min = np.min(times)
+        x = (times - x_min) / (x_max - x_min)
+        probability = data[qubit].prob
+        p0 = [
+            0.5,
+            0.5,
+            5,
+        ]
+
+        try:
+            popt, perr = curve_fit(
+                exp_decay,
+                x,
+                probability,
+                p0=p0,
+                maxfev=2000000,
+                bounds=(
+                    [-2, -2, 0],
+                    [2, 2, np.inf],
+                ),
+                sigma=data[qubit].error,
+            )
+            popt = [
+                popt[0],
+                popt[1] * np.exp(x_min * popt[2] / (x_max - x_min)),
+                popt[2] * (x_max - x_min),
+            ]
+            perr = np.sqrt(np.diag(perr))
+            fitted_parameters[qubit] = popt
+            dec = popt[2]
+            decay[qubit] = (dec, perr[2])
+            chi2[qubit] = (
+                chi2_reduced(
+                    data[qubit].prob,
+                    exp_decay(data[qubit].wait, *fitted_parameters[qubit]),
+                    data[qubit].error,
+                ),
+                np.sqrt(2 / len(data[qubit].prob)),
+            )
 
+        except Exception as e:
+            log.warning(f"Exponential decay fit failed for qubit {qubit} due to {e}")
 
-t2_signal = Routine(_acquisition, _fit, _plot, _update)
-"""T2Signal Routine object."""
+    return decay, fitted_parameters, chi2
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/zeno.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,51 +4,44 @@
 import numpy as np
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal import update
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 
-from ..utils import chi2_reduced, table_dict, table_html
+from ..utils import table_dict, table_html
 from . import t1, utils
+from .zeno_signal import ZenoSignalParameters, ZenoSignalResults, _update
 
 
 @dataclass
-class ZenoParameters(Parameters):
+class ZenoParameters(ZenoSignalParameters):
     """Zeno runcard inputs."""
 
-    readouts: int
-    "Number of readout pulses"
-
 
 @dataclass
 class ZenoData(t1.T1Data):
     readout_duration: dict[QubitId, float] = field(default_factory=dict)
     """Readout durations for each qubit"""
 
 
 @dataclass
-class ZenoResults(Results):
+class ZenoResults(ZenoSignalResults):
     """Zeno outputs."""
 
-    zeno_t1: dict[QubitId, int]
-    """T1 for each qubit."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
     chi2: dict[QubitId, tuple[float, Optional[float]]]
     """Chi squared estimate mean value and error."""
 
 
 def _acquisition(
     params: ZenoParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> ZenoData:
     """
     In a T1_Zeno experiment, we measure an excited qubit repeatedly. Due to decoherence processes,
     it is possible that, at the time of measurement, the qubit will not be excited anymore.
     The quantum zeno effect consists of measuring allowing a particle's time evolution to be slowed
     down by measuring it frequently enough. However, in the experiments we see that due the QND-ness of the readout
     pulse that the qubit decoheres faster.
@@ -56,15 +49,15 @@
     """
 
     # create sequence of pulses:
     sequence = PulseSequence()
     RX_pulses = {}
     ro_pulses = {}
     ro_pulse_duration = {}
-    for qubit in qubits:
+    for qubit in targets:
         RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         sequence.add(RX_pulses[qubit])
         start = RX_pulses[qubit].finish
         ro_pulses[qubit] = []
         for _ in range(params.readouts):
             ro_pulse = platform.create_qubit_readout_pulse(qubit, start=start)
             start += ro_pulse.duration
@@ -83,16 +76,16 @@
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.DISCRIMINATION,
             averaging_mode=AveragingMode.SINGLESHOT,
         ),
     )
 
     # retrieve and store the results for every qubit
-    probs = {qubit: [] for qubit in qubits}
-    for qubit in qubits:
+    probs = {qubit: [] for qubit in targets}
+    for qubit in targets:
         for ro_pulse in ro_pulses[qubit]:
             probs[qubit].append(results[ro_pulse.serial].probability(state=1))
         errors = [np.sqrt(prob * (1 - prob) / params.nshots) for prob in probs[qubit]]
         data.register_qubit(
             t1.CoherenceProbType,
             (qubit),
             dict(
@@ -108,35 +101,24 @@
     """
     Fitting routine for T1 experiment. The used model is
 
         .. math::
 
             y = p_0-p_1 e^{-x p_2}.
     """
-    t1s, fitted_parameters = utils.exponential_fit_probability(data)
-    chi2 = {
-        qubit: (
-            chi2_reduced(
-                data[qubit].prob,
-                utils.exp_decay(data[qubit].wait, *fitted_parameters[qubit]),
-                data[qubit].error,
-            ),
-            np.sqrt(2 / len(data[qubit].prob)),
-        )
-        for qubit in data.qubits
-    }
+    t1s, fitted_parameters, chi2 = utils.exponential_fit_probability(data)
     return ZenoResults(t1s, fitted_parameters, chi2)
 
 
-def _plot(data: ZenoData, fit: ZenoResults, qubit):
+def _plot(data: ZenoData, fit: ZenoResults, target: QubitId):
     """Plotting function for T1 experiment."""
 
     figures = []
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     probs = qubit_data.prob
     error_bars = qubit_data.error
     readouts = np.arange(1, len(qubit_data.prob) + 1)
 
     fig = go.Figure(
         [
             go.Scatter(
@@ -163,31 +145,31 @@
     if fit is not None:
         fitting_report = ""
         waitrange = np.linspace(
             min(readouts),
             max(readouts),
             2 * len(qubit_data),
         )
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=utils.exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["T1 [ns]", "Readout Pulse [ns]", "chi2 reduced"],
                 [
-                    fit.zeno_t1[qubit],
-                    np.array(fit.zeno_t1[qubit]) * data.readout_duration[qubit],
-                    fit.chi2[qubit],
+                    fit.zeno_t1[target],
+                    np.array(fit.zeno_t1[target]) * data.readout_duration[target],
+                    fit.chi2[target],
                 ],
                 display_error=True,
             )
         )
         # FIXME: Pulse duration (+ time of flight ?)
 
     # last part
@@ -198,12 +180,8 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ZenoResults, platform: Platform, qubit: QubitId):
-    update.t1(results.zeno_t1[qubit], platform, qubit)
-
-
 zeno = Routine(_acquisition, _fit, _plot, _update)
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/coherence/zeno_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/coherence/zeno_signal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,145 +1,141 @@
 from dataclasses import dataclass, field
-from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from ..utils import table_dict, table_html
 from . import utils
 
 
 @dataclass
-class ZenoParameters(Parameters):
+class ZenoSignalParameters(Parameters):
     """Zeno runcard inputs."""
 
     readouts: int
     "Number of readout pulses"
-    nshots: Optional[int] = None
-    """Number of shots."""
-    relaxation_time: Optional[int] = None
-    """Relaxation time [ns]."""
 
 
-ZenoType = np.dtype([("signal", np.float64), ("phase", np.float64)])
+ZenoSignalType = np.dtype([("signal", np.float64), ("phase", np.float64)])
 """Custom dtype for Zeno."""
 
 
 @dataclass
-class ZenoData(Data):
+class ZenoSignalData(Data):
+
     readout_duration: dict[QubitId, float] = field(default_factory=dict)
     """Readout durations for each qubit"""
     data: dict[QubitId, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
     def register_qubit(self, qubit, signal, phase):
         """Store output for single qubit."""
-        ar = np.empty((1,), dtype=ZenoType)
+        ar = np.empty((1,), dtype=ZenoSignalType)
         ar["signal"] = signal
         ar["phase"] = phase
         if qubit in self.data:
             self.data[qubit] = np.rec.array(np.concatenate((self.data[qubit], ar)))
         else:
             self.data[qubit] = np.rec.array(ar)
 
 
 @dataclass
-class ZenoResults(Results):
+class ZenoSignalResults(Results):
     """Zeno outputs."""
 
     zeno_t1: dict[QubitId, int]
     """T1 for each qubit."""
     fitted_parameters: dict[QubitId, dict[str, float]]
     """Raw fitting output."""
 
 
 def _acquisition(
-    params: ZenoParameters,
+    params: ZenoSignalParameters,
     platform: Platform,
-    qubits: Qubits,
-) -> ZenoData:
+    targets: list[QubitId],
+) -> ZenoSignalData:
     """
     In a T1_Zeno experiment, we measure an excited qubit repeatedly. Due to decoherence processes,
     it is possible that, at the time of measurement, the qubit will not be excited anymore.
     The quantum zeno effect consists of measuring allowing a particle's time evolution to be slowed
     down by measuring it frequently enough. However, in the experiments we see that due the QND-ness of the readout
     pulse that the qubit decoheres faster.
     Reference: https://link.aps.org/accepted/10.1103/PhysRevLett.118.240401.
     """
 
     # create sequence of pulses:
     sequence = PulseSequence()
     RX_pulses = {}
     ro_pulses = {}
     ro_pulse_duration = {}
-    for qubit in qubits:
+    for qubit in targets:
         RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         sequence.add(RX_pulses[qubit])
         start = RX_pulses[qubit].finish
         ro_pulses[qubit] = []
         for _ in range(params.readouts):
             ro_pulse = platform.create_qubit_readout_pulse(qubit, start=start)
             start += ro_pulse.duration
             sequence.add(ro_pulse)
             ro_pulses[qubit].append(ro_pulse)
         ro_pulse_duration[qubit] = ro_pulse.duration
 
     # create a DataUnits object to store the results
-    data = ZenoData(readout_duration=ro_pulse_duration)
+    data = ZenoSignalData(readout_duration=ro_pulse_duration)
 
     # execute the first pulse sequence
     results = platform.execute_pulse_sequence(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
             averaging_mode=AveragingMode.CYCLIC,
         ),
     )
 
     # retrieve and store the results for every qubit
-    for qubit in qubits:
+    for qubit in targets:
         for ro_pulse in ro_pulses[qubit]:
             result = results[ro_pulse.serial]
             data.register_qubit(
                 qubit=qubit, signal=result.magnitude, phase=result.phase
             )
     return data
 
 
-def _fit(data: ZenoData) -> ZenoResults:
+def _fit(data: ZenoSignalData) -> ZenoSignalResults:
     """
     Fitting routine for T1 experiment. The used model is
 
         .. math::
 
             y = p_0-p_1 e^{-x p_2}.
     """
 
-    t1s, fitted_parameters = utils.exponential_fit(data, zeno=True)
+    t1s, fitted_parameters, _ = utils.exponential_fit(data, zeno=True)
 
-    return ZenoResults(t1s, fitted_parameters)
+    return ZenoSignalResults(t1s, fitted_parameters)
 
 
-def _plot(data: ZenoData, fit: ZenoResults, qubit):
+def _plot(data: ZenoSignalData, fit: ZenoSignalResults, target: QubitId):
     """Plotting function for T1 experiment."""
     figures = []
     fig = go.Figure()
 
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     readouts = np.arange(1, len(qubit_data.signal) + 1)
 
     fig.add_trace(
         go.Scatter(
             x=readouts,
             y=qubit_data.signal,
             opacity=1,
@@ -152,30 +148,30 @@
     if fit is not None:
         fitting_report = ""
         waitrange = np.linspace(
             min(readouts),
             max(readouts),
             2 * len(qubit_data),
         )
-        params = fit.fitted_parameters[qubit]
+        params = fit.fitted_parameters[target]
         fig.add_trace(
             go.Scatter(
                 x=waitrange,
                 y=utils.exp_decay(waitrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["T1", "Readout Pulse"],
                 [
-                    np.round(fit.zeno_t1[qubit]),
-                    np.round(fit.zeno_t1[qubit] * data.readout_duration[qubit]),
+                    np.round(fit.zeno_t1[target]),
+                    np.round(fit.zeno_t1[target] * data.readout_duration[target]),
                 ],
             )
         )
         # FIXME: Pulse duration (+ time of flight ?)
 
     # last part
     fig.update_layout(
@@ -185,12 +181,12 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ZenoResults, platform: Platform, qubit: QubitId):
+def _update(results: ZenoSignalResults, platform: Platform, qubit: QubitId):
     update.t1(results.zeno_t1[qubit], platform, qubit)
 
 
 zeno_signal = Routine(_acquisition, _fit, _plot, _update)
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_qubit_spectroscopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,63 @@
 from typing import Optional
 
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
+from ..flux_dependence import resonator_flux_dependence
 from ..two_qubit_interaction.utils import order_pair
 from .coupler_resonator_spectroscopy import _fit, _plot, _update
 from .utils import CouplerSpectroscopyData, CouplerSpectroscopyParameters
 
 
 class CouplerSpectroscopyParametersQubit(CouplerSpectroscopyParameters):
     drive_duration: Optional[int] = 2000
     """Drive pulse duration to excite the qubit before the measurement"""
 
 
 def _acquisition(
-    params: CouplerSpectroscopyParametersQubit, platform: Platform, qubits: Qubits
+    params: CouplerSpectroscopyParametersQubit,
+    platform: Platform,
+    targets: list[QubitPairId],
 ) -> CouplerSpectroscopyData:
     """
     Data acquisition for CouplerQubit spectroscopy.
 
     This consist on a frequency sweep on the qubit frequency while we change the flux coupler pulse amplitude of
     the coupler pulse. We expect to enable the coupler during the amplitude sweep and detect an avoided crossing
     that will be followed by the frequency sweep. This needs the qubits at resonance, the routine assumes a sweetspot
     value for the higher frequency qubit that moves it to the lower frequency qubit instead of trying to calibrate both pulses at once. This should be run after
     qubit_spectroscopy to further adjust the coupler sweetspot if needed and get some information
     on the flux coupler pulse amplitude requiered to enable 2q interactions.
 
     """
 
     # TODO: Do we  want to measure both qubits on the pair ?
-    # Different acquisition, for now only measure one and reduce possible crosstalk.
 
     # create a sequence of pulses for the experiment:
     # Coupler pulse while Drive pulse - MZ
 
+    if params.measured_qubits is None:
+        params.measured_qubits = [order_pair(pair, platform)[0] for pair in targets]
+
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
     couplers = []
-    for i, pair in enumerate(qubits):
-        qubit = platform.qubits[params.measured_qubits[i]].name
-        # TODO: Qubit pair patch
-        ordered_pair = order_pair(pair, platform.qubits)
+    for i, pair in enumerate(targets):
+        ordered_pair = order_pair(pair, platform)
+        measured_qubit = params.measured_qubits[i]
+
+        qubit = platform.qubits[measured_qubit].name
         couplers.append(platform.pairs[tuple(sorted(ordered_pair))].coupler)
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=params.drive_duration
         )
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
@@ -69,54 +76,63 @@
     sweeper_freq = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[qd_pulses[qubit] for qubit in params.measured_qubits],
         type=SweeperType.OFFSET,
     )
 
-    # define the parameter to sweep and its range:
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
-
-    # This sweeper is implemented in the flux pulse amplitude and we need it to be that way.
-    sweeper_bias = Sweeper(
-        Parameter.bias,
-        delta_bias_range,
-        couplers=couplers,
-        type=SweeperType.ABSOLUTE,
-    )
+    if params.flux_pulses:
+        (
+            delta_bias_flux_range,
+            sweepers,
+        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
+            params, platform, couplers, sequence
+        )
+    else:
+        delta_bias_flux_range = np.arange(
+            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        )
+        sweepers = [
+            Sweeper(
+                Parameter.bias,
+                delta_bias_flux_range,
+                qubits=couplers,
+                type=SweeperType.OFFSET,
+            )
+        ]
 
     data = CouplerSpectroscopyData(
         resonator_type=platform.resonator_type,
+        flux_pulses=params.flux_pulses,
     )
 
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        sweeper_bias,
-        sweeper_freq,
-    )
+    for bias_sweeper in sweepers:
+        results = platform.sweep(
+            sequence,
+            ExecutionParameters(
+                nshots=params.nshots,
+                relaxation_time=params.relaxation_time,
+                acquisition_type=AcquisitionType.INTEGRATION,
+                averaging_mode=AveragingMode.CYCLIC,
+            ),
+            bias_sweeper,
+            sweeper_freq,
+        )
 
     # retrieve the results for every qubit
-    for i, pair in enumerate(qubits):
+    for i, pair in enumerate(targets):
         # TODO: May measure both qubits on the pair
         qubit = platform.qubits[params.measured_qubits[i]].name
         result = results[ro_pulses[qubit].serial]
         # store the results
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
             freq=delta_frequency_range + qd_pulses[qubit].frequency,
-            bias=delta_bias_range,
+            bias=delta_bias_flux_range,
         )
     return data
 
 
 coupler_qubit_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
 """CouplerQubitSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/coupler_resonator_spectroscopy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,62 @@
-from typing import Optional
-
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
-from qibolab.qubits import QubitId
+from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
+from ..flux_dependence import resonator_flux_dependence
 from ..flux_dependence.utils import flux_dependence_plot
 from ..two_qubit_interaction.utils import order_pair
 from .utils import (
     CouplerSpectroscopyData,
     CouplerSpectroscopyParameters,
     CouplerSpectroscopyResults,
 )
 
 
-class CouplerSpectroscopyParametersResonator(CouplerSpectroscopyParameters):
-    readout_delay: Optional[int] = 1000
-    """Readout delay before the measurement is done to let the flux coupler pulse act"""
-
-
 def _acquisition(
-    params: CouplerSpectroscopyParametersResonator, platform: Platform, qubits: Qubits
+    params: CouplerSpectroscopyParameters,
+    platform: Platform,
+    targets: list[QubitPairId],
 ) -> CouplerSpectroscopyData:
     """
     Data acquisition for CouplerResonator spectroscopy.
 
     This consist on a frequency sweep on the readout frequency while we change the flux coupler pulse amplitude of
     the coupler pulse. We expect to enable the coupler during the amplitude sweep and detect an avoided crossing
     that will be followed by the frequency sweep. No need to have the qubits at resonance. This should be run after
     resonator_spectroscopy to detect couplers and adjust the coupler sweetspot if needed and get some information
     on the flux coupler pulse amplitude requiered to enable 2q interactions.
 
     """
 
     # TODO: Do we  want to measure both qubits on the pair ?
-    # Different acquisition, for now only measure one and reduce possible crosstalk.
 
     # create a sequence of pulses for the experiment:
     # Coupler pulse while MZ
 
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
+    if params.measured_qubits is None:
+        params.measured_qubits = [order_pair(pair, platform)[0] for pair in targets]
+
     sequence = PulseSequence()
     ro_pulses = {}
-    fx_pulses = {}
     couplers = []
+    for i, pair in enumerate(targets):
+        ordered_pair = order_pair(pair, platform)
+        measured_qubit = params.measured_qubits[i]
 
-    for i, pair in enumerate(qubits):
-        qubit = platform.qubits[params.measured_qubits[i]].name
-        # TODO: Qubit pair patch
-        ordered_pair = order_pair(pair, platform.qubits)
+        qubit = platform.qubits[measured_qubit].name
         coupler = platform.pairs[tuple(sorted(ordered_pair))].coupler
         couplers.append(coupler)
-
         # TODO: May measure both qubits on the pair
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=params.readout_delay
-        )
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         if params.amplitude is not None:
             ro_pulses[qubit].amplitude = params.amplitude
 
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
@@ -73,113 +66,115 @@
     sweeper_freq = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
         pulses=[ro_pulses[qubit] for qubit in params.measured_qubits],
         type=SweeperType.OFFSET,
     )
 
-    # define the parameter to sweep and its range:
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
-
-    # This sweeper is implemented in the flux pulse amplitude and we need it to be that way.
-    sweeper_bias = Sweeper(
-        Parameter.bias,
-        delta_bias_range,
-        couplers=couplers,
-        type=SweeperType.ABSOLUTE,
-    )
+    if params.flux_pulses:
+        # TODO: Add delay
+        (
+            delta_bias_flux_range,
+            sweepers,
+        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
+            params, platform, couplers, sequence
+        )
+    else:
+        delta_bias_flux_range = np.arange(
+            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        )
+        sweepers = [
+            Sweeper(
+                Parameter.bias,
+                delta_bias_flux_range,
+                qubits=couplers,
+                type=SweeperType.OFFSET,
+            )
+        ]
 
     data = CouplerSpectroscopyData(
         resonator_type=platform.resonator_type,
+        flux_pulses=params.flux_pulses,
     )
 
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        sweeper_bias,
-        sweeper_freq,
-    )
+    for bias_sweeper in sweepers:
+        results = platform.sweep(
+            sequence,
+            ExecutionParameters(
+                nshots=params.nshots,
+                relaxation_time=params.relaxation_time,
+                acquisition_type=AcquisitionType.INTEGRATION,
+                averaging_mode=AveragingMode.CYCLIC,
+            ),
+            bias_sweeper,
+            sweeper_freq,
+        )
 
     # retrieve the results for every qubit
-    for i, pair in enumerate(qubits):
+    for i, pair in enumerate(targets):
         # TODO: May measure both qubits on the pair
         qubit = platform.qubits[params.measured_qubits[i]].name
         result = results[ro_pulses[qubit].serial]
         # store the results
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
             freq=delta_frequency_range + ro_pulses[qubit].frequency,
-            bias=delta_bias_range,
+            bias=delta_bias_flux_range,
         )
     return data
 
 
 def _fit(data: CouplerSpectroscopyData) -> CouplerSpectroscopyResults:
     """Post-processing function for CouplerResonatorSpectroscopy."""
     qubits = data.qubits
     pulse_amp = {}
     sweetspot = {}
     fitted_parameters = {}
 
-    for qubit in qubits:
-        # TODO: Implement fit
-        """It should get two things:
-        Coupler sweetspot: the value that makes both features centered and symmetric
-        Pulse_amp: That turn on the feature taking into account the shift introduced by the coupler sweetspot
-
-        Issues:  Coupler sweetspot it measured in volts while pulse_amp is a pulse amplitude, this routine just sweeps pulse amplitude
-        and relies on manual shifting of that sweetspot by repeated scans as current chips are already symmetric for this feature.
-        Maybe another routine sweeping the bias in volts would be needed and that sweeper implement on Zurich driver.
-        """
-        # spot, amp, fitted_params = coupler_fit(data[qubit])
-
-        sweetspot[qubit] = 0
-        pulse_amp[qubit] = 0
-        fitted_parameters[qubit] = {}
+    # TODO: Implement fit
+    """It should get two things:
+    Coupler sweetspot: the value that makes both features centered and symmetric
+    Pulse_amp: That turn on the feature taking into account the shift introduced by the coupler sweetspot
+    """
 
     return CouplerSpectroscopyResults(
         pulse_amp=pulse_amp,
         sweetspot=sweetspot,
         fitted_parameters=fitted_parameters,
     )
 
 
 def _plot(
     data: CouplerSpectroscopyData,
-    qubit,
+    target: QubitPairId,
     fit: CouplerSpectroscopyResults,
 ):
     """
     We may want to measure both qubits on the pair,
     that will require a different plotting that takes both.
     """
-    qubit_pair = qubit  # TODO: Patch for 2q gate routines
+    qubit_pair = target  # TODO: Patch for 2q gate routines
 
     for qubit in qubit_pair:
         if qubit in data.data.keys():
             fig = flux_dependence_plot(data, fit, qubit)[0]
-            fig.update_yaxes(title_text="Pulse Amplitude [a.u.]", row=1, col=1)
+
             fig.layout.annotations[0].update(
                 text="Signal [a.u.] Qubit" + str(qubit),
             )
             fig.layout.annotations[1].update(
                 text="Phase [rad] Qubit" + str(qubit),
             )
 
-            return [fig], ""
+    return [fig], ""
 
 
-def _update(results: CouplerSpectroscopyResults, platform: Platform, qubit: QubitId):
+def _update(
+    results: CouplerSpectroscopyResults, platform: Platform, target: QubitPairId
+):
     pass
 
 
 coupler_resonator_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
 """CouplerResonatorSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/couplers/utils.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/couplers/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,29 @@
 from dataclasses import dataclass, field
-from typing import Optional
+from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Results
+from qibocal.auto.operation import Data, Results
 
+from ..flux_dependence.resonator_flux_dependence import ResonatorFluxParameters
 from ..flux_dependence.utils import create_data_array
 
 
 @dataclass
-class CouplerSpectroscopyParameters(Parameters):
+class CouplerSpectroscopyParameters(ResonatorFluxParameters):
     """CouplerResonatorSpectroscopy and CouplerQubitSpectroscopy runcard inputs."""
 
-    bias_width: int
-    """Width for bias [a.u.]."""
-    bias_step: int
-    """Frequency step for bias sweep [a.u.]."""
-    freq_width: int
-    """Width for frequency sweep relative  to the readout frequency [Hz]."""
-    freq_step: int
-    """Frequency step for frequency sweep [Hz]."""
-    # TODO: It may be better not to use readout multiplex to avoid readout crosstalk
-    measured_qubits: list[QubitId]
-    """Qubit to readout from the pair"""
-    amplitude: Optional[float] = None
+    measured_qubits: Optional[list[QubitId]] = None
+    """Qubit to measure from the pair"""
+    amplitude: Optional[Union[int, float]] = None
     """Readout or qubit drive amplitude (optional). If defined, same amplitude will be used in all qubits.
     Otherwise the default amplitude defined on the platform runcard will be used"""
-    nshots: Optional[int] = None
-    """Number of shots."""
-    relaxation_time: Optional[int] = None
-    """Relaxation time [ns]."""
 
 
 CouplerSpecType = np.dtype(
     [
         ("freq", np.float64),
         ("bias", np.float64),
         ("signal", np.float64),
@@ -59,14 +47,16 @@
 
 @dataclass
 class CouplerSpectroscopyData(Data):
     """Data structure for CouplerResonatorSpectroscopy or CouplerQubitSpectroscopy."""
 
     resonator_type: str
     """Resonator type."""
+    flux_pulses: bool
+    """True if sweeping flux pulses, False if sweeping bias."""
     data: dict[QubitId, npt.NDArray[CouplerSpecType]] = field(default_factory=dict)
     """Raw data acquired."""
 
     def register_qubit(self, qubit, freq, bias, signal, phase):
         """Store output for single qubit."""
         self.data[qubit] = create_data_array(
             freq, bias, signal, phase, dtype=CouplerSpecType
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/dispersive_shift.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.utils import (
     HZ_TO_GHZ,
     lorentzian,
     lorentzian_fit,
     table_dict,
     table_html,
 )
@@ -75,38 +75,38 @@
     """Resonator type."""
     data: dict[tuple[QubitId, int], npt.NDArray[DispersiveShiftType]] = field(
         default_factory=dict
     )
 
 
 def _acquisition(
-    params: DispersiveShiftParameters, platform: Platform, qubits: Qubits
+    params: DispersiveShiftParameters, platform: Platform, targets: list[QubitId]
 ) -> DispersiveShiftData:
     r"""
     Data acquisition for dispersive shift experiment.
     Perform spectroscopy on the readout resonator, with the qubit in ground and excited state, showing
     the resonator shift produced by the coupling between the resonator and the qubit.
 
     Args:
         params (DispersiveShiftParameters): experiment's parameters
         platform (Platform): Qibolab platform object
-        qubits (dict): list of target qubits to perform the action
+        targets (list): list of target qubits to perform the action
 
     """
 
     # create 2 sequences of pulses for the experiment:
     # sequence_0: I  - MZ
     # sequence_1: RX - MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence_0 = PulseSequence()
     sequence_1 = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].duration
         )
         sequence_0.add(ro_pulses[qubit])
         sequence_1.add(qd_pulses[qubit])
         sequence_1.add(ro_pulses[qubit])
@@ -117,15 +117,15 @@
     )
 
     # create a DataUnits objects to store the results
     data = DispersiveShiftData(resonator_type=platform.resonator_type)
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[ro_pulses[qubit] for qubit in qubits],
+        pulses=[ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
     results_0 = platform.sweep(
         sequence_0,
         ExecutionParameters(
             nshots=params.nshots,
@@ -144,15 +144,15 @@
             acquisition_type=AcquisitionType.INTEGRATION,
             averaging_mode=AveragingMode.CYCLIC,
         ),
         sweeper,
     )
 
     # retrieve the results for every qubit
-    for qubit in qubits:
+    for qubit in targets:
         for i, results in enumerate([results_0, results_1]):
             result = results[ro_pulses[qubit].serial]
             # store the results
             data.register_qubit(
                 DispersiveShiftType,
                 (qubit, i),
                 dict(
@@ -169,53 +169,55 @@
 def _fit(data: DispersiveShiftData) -> DispersiveShiftResults:
     """Post-Processing for dispersive shift"""
     qubits = data.qubits
     iq_couples = [[], []]  # axis 0: states, axis 1: qubit
 
     frequency_0 = {}
     frequency_1 = {}
+    best_freqs = {}
     fitted_parameters_0 = {}
     fitted_parameters_1 = {}
 
     for i in range(2):
         for qubit in qubits:
             data_i = data[qubit, i]
-            freq, fitted_params = lorentzian_fit(
+            fit_result = lorentzian_fit(
                 data_i, resonator_type=data.resonator_type, fit="resonator"
             )
-            if i == 0:
-                frequency_0[qubit] = freq
-                fitted_parameters_0[qubit] = fitted_params
-            else:
-                frequency_1[qubit] = freq
-                fitted_parameters_1[qubit] = fitted_params
+            if fit_result is not None:
+                if i == 0:
+                    frequency_0[qubit], fitted_parameters_0[qubit], _ = fit_result
+                else:
+                    frequency_1[qubit], fitted_parameters_1[qubit], _ = fit_result
+
             i_measures = data_i.i
             q_measures = data_i.q
 
             iq_couples[i].append(np.stack((i_measures, q_measures), axis=-1))
-    # for each qubit find the iq couple of 0-1 states that maximize the distance
+        # for each qubit find the iq couple of 0-1 states that maximize the distance
     iq_couples = np.array(iq_couples)
-    best_freqs = {}
+
     for idx, qubit in enumerate(qubits):
         frequencies = data[qubit, 0].freq
 
         max_index = np.argmax(
             np.linalg.norm(iq_couples[0][idx] - iq_couples[1][idx], axis=-1)
         )
         best_freqs[qubit] = frequencies[max_index]
+
     return DispersiveShiftResults(
         frequency_state_zero=frequency_0,
         frequency_state_one=frequency_1,
         fitted_parameters_state_one=fitted_parameters_1,
         fitted_parameters_state_zero=fitted_parameters_0,
         best_freq=best_freqs,
     )
 
 
-def _plot(data: DispersiveShiftData, qubit, fit: DispersiveShiftResults):
+def _plot(data: DispersiveShiftData, target: QubitId, fit: DispersiveShiftResults):
     """Plotting function for dispersive shift."""
     figures = []
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
@@ -224,16 +226,16 @@
             "phase [rad]",
         ),
     )
     # iterate over multiple data folders
 
     fitting_report = ""
 
-    data_0 = data[qubit, 0]
-    data_1 = data[qubit, 1]
+    data_0 = data[target, 0]
+    data_1 = data[target, 1]
     fit_data_0 = fit.state_zero if fit is not None else None
     fit_data_1 = fit.state_one if fit is not None else None
 
     for i, label, q_data, data_fit in list(
         zip(
             (0, 1),
             ("State 0", "State 1"),
@@ -275,67 +277,70 @@
             )
             params = data_fit[
                 (
                     "fitted_parameters_state_zero"
                     if i == 0
                     else "fitted_parameters_state_one"
                 )
-            ][qubit]
+            ][target]
             fig.add_trace(
                 go.Scatter(
                     x=freqrange,
                     y=lorentzian(freqrange, *params),
                     name=f"{label} Fit",
                     line=go.scatter.Line(dash="dot"),
                 ),
                 row=1,
                 col=1,
             )
 
     if fit is not None:
         fig.add_trace(
             go.Scatter(
-                x=[fit.best_freq[qubit] * HZ_TO_GHZ, fit.best_freq[qubit] * HZ_TO_GHZ],
+                x=[
+                    fit.best_freq[target] * HZ_TO_GHZ,
+                    fit.best_freq[target] * HZ_TO_GHZ,
+                ],
                 y=[
                     np.min(np.concatenate((data_0.signal, data_1.signal))),
                     np.max(np.concatenate((data_0.signal, data_1.signal))),
                 ],
                 mode="lines",
                 line=go.scatter.Line(color="orange", width=3, dash="dash"),
                 name="Best frequency",
             ),
             row=1,
             col=1,
         )
 
         fig.add_vline(
-            x=fit.best_freq[qubit] * HZ_TO_GHZ,
+            x=fit.best_freq[target] * HZ_TO_GHZ,
             line=dict(color="orange", width=3, dash="dash"),
             row=1,
             col=1,
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "State Zero Frequency [Hz]",
                     "State One Frequency [Hz]",
                     "Chi [Hz]",
                     "Best Frequency [Hz]",
                 ],
                 np.round(
                     [
-                        fit_data_0["frequency_state_zero"][qubit],
-                        fit_data_1["frequency_state_one"][qubit],
+                        fit_data_0["frequency_state_zero"][target],
+                        fit_data_1["frequency_state_one"][target],
                         (
-                            fit_data_0["frequency_state_zero"][qubit]
-                            - fit_data_1["frequency_state_one"][qubit]
+                            fit_data_0["frequency_state_zero"][target]
+                            - fit_data_1["frequency_state_one"][target]
                         )
                         / 2,
-                        fit.best_freq[qubit],
+                        fit.best_freq[target],
                     ]
                 ),
             )
         )
     fig.update_layout(
         showlegend=True,
         xaxis_title="Frequency [GHz]",
@@ -345,13 +350,13 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: DispersiveShiftResults, platform: Platform, qubit: QubitId):
-    update.readout_frequency(results.best_freq[qubit], platform, qubit)
+def _update(results: DispersiveShiftResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.best_freq[target], platform, target)
 
 
 dispersive_shift = Routine(_acquisition, _fit, _plot, _update)
 """Dispersive shift Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/dispersive_shift_qutrit.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Results, Routine
+from qibocal.auto.operation import Results, Routine
 from qibocal.protocols.characterization.utils import (
     GHZ_TO_HZ,
     HZ_TO_GHZ,
     lorentzian,
     lorentzian_fit,
     table_dict,
     table_html,
@@ -64,39 +64,39 @@
 
 @dataclass
 class DispersiveShiftQutritData(DispersiveShiftData):
     """Dipsersive shift acquisition outputs."""
 
 
 def _acquisition(
-    params: DispersiveShiftParameters, platform: Platform, qubits: Qubits
+    params: DispersiveShiftParameters, platform: Platform, targets: list[QubitId]
 ) -> DispersiveShiftQutritData:
     r"""
     Data acquisition for dispersive shift experiment.
     Perform spectroscopy on the readout resonator, with the qubit in ground and excited state, showing
     the resonator shift produced by the coupling between the resonator and the qubit.
 
     Args:
         params (DispersiveShiftParameters): experiment's parameters
         platform (Platform): Qibolab platform object
-        qubits (dict): list of target qubits to perform the action
+        targets (list): list of target qubits to perform the action
 
     """
 
     # create 3 sequences of pulses for the experiment:
     # sequence_0: I  - MZ
     # sequence_1: RX - MZ
     # sequence_2: RX - RX12 - MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence_0 = PulseSequence()
     sequence_1 = PulseSequence()
     sequence_2 = PulseSequence()
 
-    for qubit in qubits:
+    for qubit in targets:
         rx_pulse = platform.create_RX_pulse(qubit, start=0)
         rx_12_pulse = platform.create_RX12_pulse(qubit, start=rx_pulse.finish)
         ro_pulse = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence_1.add(rx_pulse)
         sequence_2.add(rx_pulse, rx_12_pulse)
         for sequence in [sequence_0, sequence_1, sequence_2]:
             readout_pulse = deepcopy(ro_pulse)
@@ -125,15 +125,15 @@
                 relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
             sweeper,
         )
 
-        for qubit in qubits:
+        for qubit in targets:
             result = results[qubit]
             # store the results
             data.register_qubit(
                 ResSpecType,
                 (qubit, state),
                 dict(
                     freq=sequence.get_qubit_pulses(qubit).ro_pulses[0].frequency
@@ -156,38 +156,38 @@
     fitted_parameters_0 = {}
     fitted_parameters_1 = {}
     fitted_parameters_2 = {}
 
     for i in range(3):
         for qubit in qubits:
             data_i = data[qubit, i]
-            freq, fitted_params = lorentzian_fit(
+            fit_result = lorentzian_fit(
                 data_i, resonator_type=data.resonator_type, fit="resonator"
             )
-            if i == 0:
-                frequency_0[qubit] = freq
-                fitted_parameters_0[qubit] = fitted_params
-            elif i == 1:
-                frequency_1[qubit] = freq
-                fitted_parameters_1[qubit] = fitted_params
-            else:
-                frequency_2[qubit] = freq
-                fitted_parameters_2[qubit] = fitted_params
+            if fit_result is not None:
+                if i == 0:
+                    frequency_0[qubit], fitted_parameters_0[qubit], _ = fit_result
+                elif i == 1:
+                    frequency_1[qubit], fitted_parameters_1[qubit], _ = fit_result
+                else:
+                    frequency_2[qubit], fitted_parameters_2[qubit], _ = fit_result
 
     return DispersiveShiftQutritResults(
         frequency_state_zero=frequency_0,
         frequency_state_one=frequency_1,
         frequency_state_two=frequency_2,
         fitted_parameters_state_one=fitted_parameters_1,
         fitted_parameters_state_zero=fitted_parameters_0,
         fitted_parameters_state_two=fitted_parameters_2,
     )
 
 
-def _plot(data: DispersiveShiftQutritData, qubit, fit: DispersiveShiftQutritResults):
+def _plot(
+    data: DispersiveShiftQutritData, target: QubitId, fit: DispersiveShiftQutritResults
+):
     """Plotting function for dispersive shift."""
     figures = []
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
@@ -196,17 +196,17 @@
             "phase [rad]",
         ),
     )
     # iterate over multiple data folders
 
     fitting_report = ""
 
-    data_0 = data[qubit, 0]
-    data_1 = data[qubit, 1]
-    data_2 = data[qubit, 2]
+    data_0 = data[target, 0]
+    data_1 = data[target, 1]
+    data_2 = data[target, 2]
     fit_data_0 = fit.state_zero if fit is not None else None
     fit_data_1 = fit.state_one if fit is not None else None
     fit_data_2 = fit.state_two if fit is not None else None
     for i, label, q_data, data_fit in list(
         zip(
             (0, 1, 2),
             ("State 0", "State 1", "State 2"),
@@ -252,40 +252,40 @@
                     if i == 0
                     else (
                         "fitted_parameters_state_one"
                         if i == 1
                         else "fitted_parameters_state_two"
                     )
                 )
-            ][qubit]
+            ][target]
             fig.add_trace(
                 go.Scatter(
                     x=freqrange,
                     y=lorentzian(freqrange, *params),
                     name=f"{label} Fit",
                     line=go.scatter.Line(dash="dot"),
                 ),
                 row=1,
                 col=1,
             )
 
     if fit is not None:
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "State Zero Frequency [Hz]",
                     "State One Frequency [Hz]",
                     "State Two Frequency [Hz]",
                 ],
                 np.round(
                     [
-                        fit_data_0["frequency_state_zero"][qubit] * GHZ_TO_HZ,
-                        fit_data_1["frequency_state_one"][qubit] * GHZ_TO_HZ,
-                        fit_data_2["frequency_state_two"][qubit] * GHZ_TO_HZ,
+                        fit_data_0["frequency_state_zero"][target] * GHZ_TO_HZ,
+                        fit_data_1["frequency_state_one"][target] * GHZ_TO_HZ,
+                        fit_data_2["frequency_state_two"][target] * GHZ_TO_HZ,
                     ]
                 ),
             )
         )
     fig.update_layout(
         showlegend=True,
         xaxis_title="Frequency [GHz]",
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/fast_reset/fast_reset.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/fast_reset/fast_reset.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
 # TODO: IBM Fast Reset until saturation loop
 # https://quantum-computing.ibm.com/lab/docs/iql/manage/systems/reset/backend_reset
 
 
 @dataclass
@@ -48,27 +48,27 @@
     """FastReset acquisition outputs."""
 
     data: dict[tuple, npt.NDArray[FastResetType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: FastResetParameters, platform: Platform, qubits: Qubits
+    params: FastResetParameters, platform: Platform, targets: list[QubitId]
 ) -> FastResetData:
     """Data acquisition for resonator spectroscopy."""
 
     data = FastResetData()
     for state in [0, 1]:
         for fast_reset in [True, False]:
             # Define the pulse sequences
             if state == 1:
                 RX_pulses = {}
             ro_pulses = {}
             sequence = PulseSequence()
-            for qubit in qubits:
+            for qubit in targets:
                 if state == 1:
                     RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
                     ro_pulses[qubit] = platform.create_qubit_readout_pulse(
                         qubit, start=RX_pulses[qubit].finish
                     )
                     sequence.add(RX_pulses[qubit])
                 else:
@@ -150,15 +150,15 @@
         fidelity_fr[qubit] = (
             1 - (state1_count_0fr / nshots + state0_count_1fr / nshots) / 2
         )
 
     return FastResetResults(fidelity_nfr, Lambda_M_nfr, fidelity_fr, Lambda_M_fr)
 
 
-def _plot(data: FastResetData, fit: FastResetResults, qubit):
+def _plot(data: FastResetData, fit: FastResetResults, target: QubitId):
     """Plotting function for FastReset."""
 
     # Maybe the plot can just be something like a confusion matrix between 0s and 1s ???
 
     figures = []
     fitting_report = ""
     fig = make_subplots(
@@ -171,42 +171,42 @@
             "Relaxation Time [ns]",
         ),
     )
 
     if fit is not None:
         fig.add_trace(
             go.Heatmap(
-                z=fit.Lambda_M_fr[qubit],
+                z=fit.Lambda_M_fr[target],
                 coloraxis="coloraxis",
             ),
             row=1,
             col=1,
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["Fidelity [Fast Reset]", "Fidelity [Relaxation Time]"],
                 [
-                    np.round(fit.fidelity_fr[qubit], 6),
-                    np.round(fit.fidelity_nfr[qubit], 6),
+                    np.round(fit.fidelity_fr[target], 6),
+                    np.round(fit.fidelity_nfr[target], 6),
                 ],
             )
         )
 
         fig.add_trace(
             go.Heatmap(
-                z=fit.Lambda_M_nfr[qubit],
+                z=fit.Lambda_M_nfr[target],
                 coloraxis="coloraxis",
             ),
             row=1,
             col=2,
         )
 
     fig.update_xaxes(
-        title_text=f"{qubit}: Fast Reset",
+        title_text=f"{target}: Fast Reset",
         row=1,
         col=1,
     )
     fig.update_yaxes(title_text="State", row=1, col=1)
     fig.update_yaxes(tickvals=[0, 1])
     fig.update_xaxes(tickvals=[0, 1])
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flipping.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flipping.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,67 +6,67 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from scipy.optimize import curve_fit
 
-from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 from qibocal.config import log
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
+from .flipping_signal import (
+    FlippingSignalData,
+    FlippingSignalParameters,
+    FlippingSignalResults,
+    _update,
+    flipping_fit,
+)
 from .utils import COLORBAND, COLORBAND_LINE, chi2_reduced
 
 
 @dataclass
-class FlippingParameters(Parameters):
+class FlippingParameters(FlippingSignalParameters):
     """Flipping runcard inputs."""
 
     nflips_max: int
     """Maximum number of flips ([RX(pi) - RX(pi)] sequences). """
     nflips_step: int
     """Flip step."""
+    unrolling: bool = False
+    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
+    Defaults to ``False``."""
 
 
 @dataclass
-class FlippingResults(Results):
+class FlippingResults(FlippingSignalResults):
     """Flipping outputs."""
 
-    amplitude: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive amplitude for each qubit."""
-    amplitude_factors: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive amplitude correction factor for each qubit."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
     chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
     """Chi squared estimate mean value and error. """
 
 
 FlippingType = np.dtype(
     [("flips", np.float64), ("prob", np.float64), ("error", np.float64)]
 )
 
 
 @dataclass
-class FlippingData(Data):
+class FlippingData(FlippingSignalData):
     """Flipping acquisition outputs."""
 
-    resonator_type: str
-    """Resonator type."""
-    pi_pulse_amplitudes: dict[QubitId, float]
     """Pi pulse amplitudes for each qubit."""
     data: dict[QubitId, npt.NDArray[FlippingType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
     params: FlippingParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> FlippingData:
     r"""
     Data acquisition for flipping.
 
     The flipping experiment correct the delta amplitude in the qubit drive pulse. We measure a qubit after applying
     a Rx(pi/2) and N flips (Rx(pi) rotations). After fitting we can obtain the delta amplitude to refine pi pulses.
 
@@ -78,23 +78,33 @@
     Returns:
         data (:class:`FlippingData`)
     """
 
     data = FlippingData(
         resonator_type=platform.resonator_type,
         pi_pulse_amplitudes={
-            qubit: qubits[qubit].native_gates.RX.amplitude for qubit in qubits
+            qubit: platform.qubits[qubit].native_gates.RX.amplitude for qubit in targets
         },
     )
+
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.DISCRIMINATION,
+        averaging_mode=AveragingMode.SINGLESHOT,
+    )
+
     # sweep the parameter
-    for flips in range(0, params.nflips_max, params.nflips_step):
+    sequences, all_ro_pulses = [], []
+    flips_sweep = range(0, params.nflips_max, params.nflips_step)
+    for flips in flips_sweep:
         # create a sequence of pulses for the experiment
         sequence = PulseSequence()
         ro_pulses = {}
-        for qubit in qubits:
+        for qubit in targets:
             RX90_pulse = platform.create_RX90_pulse(qubit, start=0)
             sequence.add(RX90_pulse)
             # execute sequence RX(pi/2) - [RX(pi) - RX(pi)] from 0...flips times - RO
             start1 = RX90_pulse.duration
             for _ in range(flips):
                 RX_pulse1 = platform.create_RX_pulse(qubit, start=start1)
                 start2 = start1 + RX_pulse1.duration
@@ -102,43 +112,49 @@
                 sequence.add(RX_pulse1)
                 sequence.add(RX_pulse2)
                 start1 = start2 + RX_pulse2.duration
 
             # add ro pulse at the end of the sequence
             ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=start1)
             sequence.add(ro_pulses[qubit])
-        # execute the pulse sequence
-        results = platform.execute_pulse_sequence(
-            sequence,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.DISCRIMINATION,
-                averaging_mode=AveragingMode.SINGLESHOT,
-            ),
-        )
-        for qubit in qubits:
-            prob = results[qubit].probability(state=1)
+
+        sequences.append(sequence)
+        all_ro_pulses.append(ro_pulses)
+
+    # execute the pulse sequence
+    if params.unrolling:
+        results = platform.execute_pulse_sequences(sequences, options)
+
+    elif not params.unrolling:
+        results = [
+            platform.execute_pulse_sequence(sequence, options) for sequence in sequences
+        ]
+
+    for ig, (flips, ro_pulses) in enumerate(zip(flips_sweep, all_ro_pulses)):
+        for qubit in targets:
+            serial = ro_pulses[qubit].serial
+            if params.unrolling:
+                result = results[serial][0]
+            else:
+                result = results[ig][serial]
+            prob = result.probability(state=1)
+            error = np.sqrt(prob * (1 - prob) / params.nshots)
             data.register_qubit(
                 FlippingType,
                 (qubit),
                 dict(
-                    flips=[flips],
-                    prob=prob.tolist(),
-                    error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
+                    flips=np.array([flips]),
+                    prob=np.array([prob]),
+                    error=np.array([error]),
                 ),
             )
 
     return data
 
 
-def flipping_fit(x, offset, amplitude, omega, phase, gamma):
-    return np.sin(x * omega + phase) * amplitude * np.exp(-x * gamma) + offset
-
-
 def _fit(data: FlippingData) -> FlippingResults:
     r"""Post-processing function for Flipping.
 
     The used model is
 
     .. math::
 
@@ -168,16 +184,16 @@
                 ),
                 sigma=qubit_data.error,
             )
             perr = np.sqrt(np.diag(perr)).tolist()
             popt = popt.tolist()
         except:
             log.warning("flipping_fit: the fitting was not succesful")
-            popt = [0] * 4
-            perr = [1] * 4
+            popt = [0] * 5
+            perr = [1] * 5
 
         if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
             signed_correction = -popt[2] / 2
         else:
             signed_correction = popt[2] / 2
         # The amplitude is directly proportional to the rotation angle
         corrected_amplitudes[qubit] = (
@@ -206,22 +222,22 @@
         )
 
     return FlippingResults(
         corrected_amplitudes, amplitude_correction_factors, fitted_parameters, chi2
     )
 
 
-def _plot(data: FlippingData, qubit, fit: FlippingResults = None):
+def _plot(data: FlippingData, target: QubitId, fit: FlippingResults = None):
     """Plotting function for Flipping."""
 
     figures = []
     fig = go.Figure()
 
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
 
     probs = qubit_data.prob
     error_bars = qubit_data.error
 
     fig.add_trace(
         go.Scatter(
             x=qubit_data.flips,
@@ -252,36 +268,36 @@
         )
 
         fig.add_trace(
             go.Scatter(
                 x=flips_range,
                 y=flipping_fit(
                     flips_range,
-                    float(fit.fitted_parameters[qubit][0]),
-                    float(fit.fitted_parameters[qubit][1]),
-                    float(fit.fitted_parameters[qubit][2]),
-                    float(fit.fitted_parameters[qubit][3]),
-                    float(fit.fitted_parameters[qubit][4]),
+                    float(fit.fitted_parameters[target][0]),
+                    float(fit.fitted_parameters[target][1]),
+                    float(fit.fitted_parameters[target][2]),
+                    float(fit.fitted_parameters[target][3]),
+                    float(fit.fitted_parameters[target][4]),
                 ),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             ),
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "Amplitude correction factor",
                     "Corrected amplitude [a.u.]",
                     "chi2 reduced",
                 ],
                 [
-                    np.round(fit.amplitude_factors[qubit], 4),
-                    np.round(fit.amplitude[qubit], 4),
-                    fit.chi2[qubit],
+                    np.round(fit.amplitude_factors[target], 4),
+                    np.round(fit.amplitude[target], 4),
+                    fit.chi2[target],
                 ],
                 display_error=True,
             )
         )
 
     # last part
     fig.update_layout(
@@ -291,13 +307,9 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: FlippingResults, platform: Platform, qubit: QubitId):
-    update.drive_amplitude(results.amplitude[qubit], platform, qubit)
-
-
 flipping = Routine(_acquisition, _fit, _plot, _update)
 """Flipping Routine  object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flipping_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey_signal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,268 +1,302 @@
 from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from scipy.optimize import curve_fit
-from scipy.signal import find_peaks
+from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.flipping import (
-    FlippingData,
-    FlippingParameters,
-    FlippingResults,
-    flipping_fit,
-)
-from qibocal.protocols.characterization.utils import table_dict, table_html
+
+from ..utils import GHZ_TO_HZ, table_dict, table_html
+from .utils import fitting, ramsey_fit, ramsey_sequence
 
 
 @dataclass
-class FlippingSignalParameters(FlippingParameters):
-    """Flipping runcard inputs."""
+class RamseySignalParameters(Parameters):
+    """Ramsey runcard inputs."""
+
+    delay_between_pulses_start: int
+    """Initial delay between RX(pi/2) pulses in ns."""
+    delay_between_pulses_end: int
+    """Final delay between RX(pi/2) pulses in ns."""
+    delay_between_pulses_step: int
+    """Step delay between RX(pi/2) pulses in ns."""
+    detuning: Optional[int] = 0
+    """Frequency detuning [Hz] (optional).
+        If 0 standard Ramsey experiment is performed."""
+    unrolling: bool = False
+    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
+    Defaults to ``False``."""
 
 
 @dataclass
-class FlippingSignalResults(FlippingResults):
-    """Flipping outputs."""
+class RamseySignalResults(Results):
+    """Ramsey outputs."""
+
+    frequency: dict[QubitId, tuple[float, Optional[float]]]
+    """Drive frequency [GHz] for each qubit."""
+    t2: dict[QubitId, tuple[float, Optional[float]]]
+    """T2 for each qubit [ns]."""
+    delta_phys: dict[QubitId, tuple[float, Optional[float]]]
+    """Drive frequency [Hz] correction for each qubit."""
+    delta_fitting: dict[QubitId, tuple[float, Optional[float]]]
+    """Raw drive frequency [Hz] correction for each qubit.
+       including the detuning."""
+    fitted_parameters: dict[QubitId, list[float]]
+    """Raw fitting output."""
 
 
-FlippingType = np.dtype([("flips", np.float64), ("signal", np.float64)])
+RamseySignalType = np.dtype([("wait", np.float64), ("signal", np.float64)])
+"""Custom dtype for coherence routines."""
 
 
 @dataclass
-class FlippingSignalData(FlippingData):
-    """Flipping acquisition outputs."""
+class RamseySignalData(Data):
+    """Ramsey acquisition outputs."""
 
-    data: dict[QubitId, npt.NDArray[FlippingType]] = field(default_factory=dict)
+    detuning: int
+    """Frequency detuning [Hz]."""
+    qubit_freqs: dict[QubitId, float] = field(default_factory=dict)
+    """Qubit freqs for each qubit."""
+    data: dict[QubitId, npt.NDArray[RamseySignalType]] = field(default_factory=dict)
     """Raw data acquired."""
 
+    @property
+    def waits(self):
+        """
+        Return a list with the waiting times without repetitions.
+        """
+        qubit = next(iter(self.data))
+        return np.unique(self.data[qubit].wait)
+
 
 def _acquisition(
-    params: FlippingSignalParameters,
+    params: RamseySignalParameters,
     platform: Platform,
-    qubits: Qubits,
-) -> FlippingSignalData:
-    r"""
-    Data acquisition for flipping.
-
-    The flipping experiment correct the delta amplitude in the qubit drive pulse. We measure a qubit after applying
-    a Rx(pi/2) and N flips (Rx(pi) rotations). After fitting we can obtain the delta amplitude to refine pi pulses.
-
-    Args:
-        params (:class:`FlippingSignalParameters`): input parameters
-        platform (:class:`Platform`): Qibolab's platform
-        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+    targets: list[QubitId],
+) -> RamseySignalData:
+    """Data acquisition for Ramsey Experiment (detuned)."""
+    # create a sequence of pulses for the experiment
+    # RX90 - t - RX90 - MZ
+    # define the parameter to sweep and its range:
+
+    waits = np.arange(
+        # wait time between RX90 pulses
+        params.delay_between_pulses_start,
+        params.delay_between_pulses_end,
+        params.delay_between_pulses_step,
+    )
 
-    Returns:
-        data (:class:`FlippingSignalData`)
-    """
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.INTEGRATION,
+        averaging_mode=AveragingMode.CYCLIC,
+    )
 
-    data = FlippingSignalData(
-        resonator_type=platform.resonator_type,
-        pi_pulse_amplitudes={
-            qubit: qubits[qubit].native_gates.RX.amplitude for qubit in qubits
+    data = RamseySignalData(
+        detuning=params.detuning,
+        qubit_freqs={
+            qubit: platform.qubits[qubit].native_gates.RX.frequency for qubit in targets
         },
     )
-    # sweep the parameter
-    for flips in range(0, params.nflips_max, params.nflips_step):
-        # create a sequence of pulses for the experiment
+
+    if not params.unrolling:
         sequence = PulseSequence()
-        ro_pulses = {}
-        for qubit in qubits:
-            RX90_pulse = platform.create_RX90_pulse(qubit, start=0)
-            sequence.add(RX90_pulse)
-            # execute sequence RX(pi/2) - [RX(pi) - RX(pi)] from 0...flips times - RO
-            start1 = RX90_pulse.duration
-            for _ in range(flips):
-                RX_pulse1 = platform.create_RX_pulse(qubit, start=start1)
-                start2 = start1 + RX_pulse1.duration
-                RX_pulse2 = platform.create_RX_pulse(qubit, start=start2)
-                sequence.add(RX_pulse1)
-                sequence.add(RX_pulse2)
-                start1 = start2 + RX_pulse2.duration
-
-            # add ro pulse at the end of the sequence
-            ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=start1)
-            sequence.add(ro_pulses[qubit])
-        # execute the pulse sequence
-        results = platform.execute_pulse_sequence(
+        for qubit in targets:
+            sequence += ramsey_sequence(
+                platform=platform, qubit=qubit, detuning=params.detuning
+            )
+        sweeper = Sweeper(
+            Parameter.start,
+            waits,
+            [
+                sequence.get_qubit_pulses(qubit).qd_pulses[-1] for qubit in targets
+            ],  # TODO: check if it is correct
+            type=SweeperType.ABSOLUTE,
+        )
+
+        # execute the sweep
+        results = platform.sweep(
             sequence,
-            ExecutionParameters(
-                nshots=params.nshots,
-                relaxation_time=params.relaxation_time,
-                acquisition_type=AcquisitionType.INTEGRATION,
-                averaging_mode=AveragingMode.CYCLIC,
-            ),
+            options,
+            sweeper,
         )
-        for qubit in qubits:
-            result = results[ro_pulses[qubit].serial]
+        for qubit in targets:
+            result = results[sequence.get_qubit_pulses(qubit).ro_pulses[0].serial]
+            # The probability errors are the standard errors of the binomial distribution
             data.register_qubit(
-                FlippingType,
+                RamseySignalType,
                 (qubit),
                 dict(
-                    flips=np.array([flips]),
-                    signal=np.array([result.magnitude]),
+                    wait=waits,
+                    signal=result.magnitude,
                 ),
             )
 
-    return data
-
+    else:
+        sequences, all_ro_pulses = [], []
+        for wait in waits:
+            sequence = PulseSequence()
+            for qubit in targets:
+                sequence += ramsey_sequence(
+                    platform=platform, qubit=qubit, wait=wait, detuning=params.detuning
+                )
+
+            sequences.append(sequence)
+            all_ro_pulses.append(sequence.ro_pulses)
+
+        results = platform.execute_pulse_sequences(sequences, options)
+
+        # We dont need ig as everty serial is different
+        for ig, (wait, ro_pulses) in enumerate(zip(waits, all_ro_pulses)):
+            for qubit in targets:
+                serial = ro_pulses[qubit].serial
+                if params.unrolling:
+                    result = results[serial][0]
+                else:
+                    result = results[ig][serial]
+                data.register_qubit(
+                    RamseySignalType,
+                    (qubit),
+                    dict(
+                        wait=np.array([wait]),
+                        signal=np.array([result.magnitude]),
+                    ),
+                )
 
-def _fit(data: FlippingSignalData) -> FlippingSignalResults:
-    r"""Post-processing function for Flipping.
+    return data
 
-    The used model is
 
+def _fit(data: RamseySignalData) -> RamseySignalResults:
+    r"""
+    Fitting routine for Ramsey experiment. The used model is
     .. math::
-
-        y = p_0 sin\Big(\frac{2 \pi x}{p_2} + p_3\Big)*\exp{-x*p4} + p_1.
+        y = p_0 + p_1 sin \Big(p_2 x + p_3 \Big) e^{-x p_4}.
     """
     qubits = data.qubits
-    corrected_amplitudes = {}
-    fitted_parameters = {}
-    amplitude_correction_factors = {}
+    waits = data.waits
+    popts = {}
+    freq_measure = {}
+    t2_measure = {}
+    delta_phys_measure = {}
+    delta_fitting_measure = {}
     for qubit in qubits:
         qubit_data = data[qubit]
-        pi_pulse_amplitude = data.pi_pulse_amplitudes[qubit]
-        voltages = qubit_data.signal
-        flips = qubit_data.flips
-        y_min = np.min(voltages)
-        # Guessing period using Fourier transform
-        ft = np.fft.rfft(voltages)
-        # Remove the zero frequency mode
-        mags = abs(ft)[1:]
-        local_maxima = find_peaks(mags, height=0)
-        peak_heights = local_maxima[1]["peak_heights"]
-        # Select the frequency with the highest peak
-        index = (
-            int(local_maxima[0][np.argmax(peak_heights)] + 1)
-            if len(local_maxima[0]) > 0
-            else None
-        )
-        f = flips[index] / (flips[1] - flips[0]) if index is not None else 1
-        y_max = np.max(voltages)
-        x_min = np.min(flips)
-        x_max = np.max(flips)
-        x = (flips - x_min) * 2 * np.pi * f / (x_max - x_min)
-        y = (voltages - y_min) / (y_max - y_min)
-
-        pguess = [0.5, 0.5, 1, np.pi, 0]
+        qubit_freq = data.qubit_freqs[qubit]
+        signal = qubit_data["signal"]
         try:
-            popt, _ = curve_fit(
-                flipping_fit,
-                x,
-                y,
-                p0=pguess,
-                maxfev=2000000,
-                bounds=(
-                    [0, 0, -np.inf, 0, 0],
-                    [1, np.inf, np.inf, 2 * np.pi, np.inf],
-                ),
+            popt, perr = fitting(waits, signal)
+            delta_fitting = popt[2] / (2 * np.pi)
+            sign = np.sign(data.detuning) if data.detuning != 0 else 1
+            delta_phys = int(sign * (delta_fitting * GHZ_TO_HZ - np.abs(data.detuning)))
+            corrected_qubit_frequency = int(qubit_freq - delta_phys)
+            t2 = 1 / popt[4]
+            freq_measure[qubit] = (
+                corrected_qubit_frequency,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
             )
-        except:
-            log.warning("flipping_fit: the fitting was not succesful")
-            popt = [0, 0, 0, 0]
-
-        translated_popt = [
-            y_min + (y_max - y_min) * popt[0],
-            (y_max - y_min)
-            * popt[1]
-            * np.exp(x_min * popt[4] * 2 * np.pi * f / (x_max - x_min)),
-            popt[2] * 2 * np.pi * f / (x_max - x_min),
-            popt[3] - x_min * 2 * np.pi * f / (x_max - x_min) * popt[2],
-            popt[4] * 2 * np.pi * f / (x_max - x_min),
-        ]
-        if popt[3] > np.pi / 2 and popt[3] < 3 * np.pi / 2:
-            signed_correction = -translated_popt[2] / 2
-        else:
-            signed_correction = translated_popt[2] / 2
-        # The amplitude is directly proportional to the rotation angle
-        corrected_amplitudes[qubit] = (pi_pulse_amplitude * np.pi) / (
-            np.pi + signed_correction
-        )
-        fitted_parameters[qubit] = translated_popt
-        amplitude_correction_factors[qubit] = (
-            signed_correction / np.pi * pi_pulse_amplitude
-        )
+            t2_measure[qubit] = (t2, perr[4] * (t2**2))
+            popts[qubit] = popt
+            delta_phys_measure[qubit] = (
+                delta_phys,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
+            )
+            delta_fitting_measure[qubit] = (
+                delta_fitting * GHZ_TO_HZ,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
+            )
+        except Exception as e:
+            log.warning(f"Ramsey fitting failed for qubit {qubit} due to {e}.")
 
-    return FlippingSignalResults(
-        corrected_amplitudes, amplitude_correction_factors, fitted_parameters
+    return RamseySignalResults(
+        frequency=freq_measure,
+        t2=t2_measure,
+        delta_phys=delta_phys_measure,
+        delta_fitting=delta_fitting_measure,
+        fitted_parameters=popts,
     )
 
 
-def _plot(data: FlippingSignalData, qubit, fit: FlippingSignalResults = None):
-    """Plotting function for Flipping."""
+def _plot(data: RamseySignalData, target: QubitId, fit: RamseySignalResults = None):
+    """Plotting function for Ramsey Experiment."""
 
     figures = []
     fig = go.Figure()
     fitting_report = ""
-    qubit_data = data[qubit]
 
-    fig.add_trace(
-        go.Scatter(
-            x=qubit_data.flips,
-            y=qubit_data.signal,
-            opacity=1,
-            name="Signal",
-            showlegend=True,
-            legendgroup="Signal",
-        ),
+    qubit_data = data.data[target]
+    waits = data.waits
+    signal = qubit_data["signal"]
+    fig = go.Figure(
+        [
+            go.Scatter(
+                x=waits,
+                y=signal,
+                opacity=1,
+                name="Signal",
+                showlegend=True,
+                legendgroup="Signal",
+                mode="lines",
+            ),
+        ]
     )
 
     if fit is not None:
-        flips_range = np.linspace(
-            min(qubit_data.flips),
-            max(qubit_data.flips),
-            2 * len(qubit_data),
-        )
-
         fig.add_trace(
             go.Scatter(
-                x=flips_range,
-                y=flipping_fit(
-                    flips_range,
-                    float(fit.fitted_parameters[qubit][0]),
-                    float(fit.fitted_parameters[qubit][1]),
-                    float(fit.fitted_parameters[qubit][2]),
-                    float(fit.fitted_parameters[qubit][3]),
-                    float(fit.fitted_parameters[qubit][4]),
+                x=waits,
+                y=ramsey_fit(
+                    waits,
+                    float(fit.fitted_parameters[target][0]),
+                    float(fit.fitted_parameters[target][1]),
+                    float(fit.fitted_parameters[target][2]),
+                    float(fit.fitted_parameters[target][3]),
+                    float(fit.fitted_parameters[target][4]),
                 ),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
-            ),
+            )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
-                ["Amplitude correction factor", "Corrected amplitude [a.u.]"],
+                target,
+                [
+                    "Delta Frequency [Hz]",
+                    "Delta Frequency (with detuning) [Hz]",
+                    "Drive Frequency [Hz]",
+                    "T2* [ns]",
+                ],
                 [
-                    np.round(fit.amplitude_factors[qubit], 4),
-                    np.round(fit.amplitude[qubit], 4),
+                    np.round(fit.delta_phys[target][0], 3),
+                    np.round(fit.delta_fitting[target][0], 3),
+                    np.round(fit.frequency[target][0], 3),
+                    np.round(fit.t2[target][0], 3),
                 ],
             )
         )
 
-    # last part
     fig.update_layout(
         showlegend=True,
-        xaxis_title="Flips",
+        xaxis_title="Time [ns]",
         yaxis_title="Signal [a.u.]",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: FlippingSignalResults, platform: Platform, qubit: QubitId):
-    update.drive_amplitude(results.amplitude[qubit], platform, qubit)
+def _update(results: RamseySignalResults, platform: Platform, target: QubitId):
+    update.drive_frequency(results.frequency[target][0], platform, target)
 
 
-flipping_signal = Routine(_acquisition, _fit, _plot, _update)
-"""Flipping Routine  object."""
+ramsey_signal = Routine(_acquisition, _fit, _plot, _update)
+"""Ramsey Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/avoided_crossing.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.platform import Platform
-from qibolab.qubits import QubitId
+from qibolab.qubits import QubitId, QubitPairId
 
-from qibocal.auto.operation import Data, QubitsPairs, Results, Routine
+from qibocal.auto.operation import Data, Results, Routine
 from qibocal.protocols.characterization.two_qubit_interaction.utils import order_pair
 from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
 
 from .qubit_flux_dependence import QubitFluxParameters, QubitFluxType
 from .qubit_flux_dependence import _acquisition as flux_acquisition
 
 STEP = 60
@@ -53,42 +53,41 @@
     )
     """Raw data acquired."""
 
 
 def _acquisition(
     params: AvoidedCrossingParameters,
     platform: Platform,
-    qubits: QubitsPairs,  # qubit pairs
+    targets: list[QubitPairId],  # qubit pairs
 ) -> AvoidedCrossingData:
     """
     Data acquisition for avoided crossing.
     This routine performs the qubit flux dependency for the "01" and "02" transition
     on the qubit pair. It returns the bias and frequency values to perform a CZ
     and a iSwap gate.
 
     Args:
         params (AvoidedCrossingParameters): experiment's parameters.
         platform (Platform): Qibolab platform object.
         qubits (dict): list of targets qubit pairs to perform the action.
     """
-    qubit_pairs = list(qubits.keys())
-    order_pairs = np.array([order_pair(pair, platform.qubits) for pair in qubit_pairs])
+    order_pairs = np.array([order_pair(pair, platform) for pair in targets])
     data = AvoidedCrossingData(qubit_pairs=order_pairs.tolist())
     # Extract the qubits in the qubits pairs and evaluate their flux dep
     unique_qubits = np.unique(
         order_pairs[:, 1]
     )  # select qubits with high freq in each couple
     new_qubits = {key: platform.qubits[key] for key in unique_qubits}
     excitations = [Excitations.ge, Excitations.gf]
     for transition in excitations:
         params.transition = transition
         data_transition = flux_acquisition(
             params=params,
             platform=platform,
-            qubits=new_qubits,
+            targets=new_qubits,
         )
         for qubit in unique_qubits:
             qubit_data = data_transition.data[qubit]
             freq = qubit_data["freq"]
             bias = qubit_data["bias"]
             signal = qubit_data["signal"]
             phase = qubit_data["phase"]
@@ -151,24 +150,29 @@
         fit_pars[2] -= line_val
         x1, x2 = solve_eq(fit_pars)
         iswap[qubit_pair] = [[x1, line_val], [x2, line_val]]
 
     return AvoidedCrossingResults(curves, fits, cz, iswap)
 
 
-def _plot(data: AvoidedCrossingData, fit: Optional[AvoidedCrossingResults], qubit):
+def _plot(
+    data: AvoidedCrossingData,
+    fit: Optional[AvoidedCrossingResults],
+    target: QubitPairId,
+):
     """Plotting function for avoided crossing"""
     fitting_report = ""
     figures = []
-    order_pair = tuple(index(data.qubit_pairs, qubit))
+    order_pair = tuple(index(data.qubit_pairs, target))
     heatmaps = make_subplots(
         rows=1,
         cols=2,
         subplot_titles=[
-            f"{i} transition qubit {qubit[0]}" for i in [Excitations.ge, Excitations.gf]
+            f"{i} transition qubit {target[0]}"
+            for i in [Excitations.ge, Excitations.gf]
         ],
     )
     parabolas = make_subplots(rows=1, cols=1, subplot_titles=["Parabolas"])
     for i, transition in enumerate([Excitations.ge, Excitations.gf]):
         data_high = data.data[order_pair[1], transition]
         bias_unique = np.unique(data_high.bias)
         min_bias = min(bias_unique)
@@ -203,15 +207,15 @@
             yaxis_title="Bias[V]",
             xaxis2_title="Frequency[GHz]",
             yaxis2_title="Bias[V]",
         )
         figures.append(parabolas)
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["CZ bias", "iSwap bias"],
                 [np.round(cz[:, 0], 3), np.round(iswap[:, 0], 3)],
             )
         )
     return figures, fitting_report
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_crosstalk.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Results, Routine
+from qibocal.auto.operation import Results, Routine
 
 from ..qubit_spectroscopy_ef import DEFAULT_ANHARMONICITY
 from . import utils
 from .qubit_flux_dependence import (
     QubitFluxData,
     QubitFluxParameters,
     QubitFluxResults,
     QubitFluxType,
 )
+from .resonator_flux_dependence import create_flux_pulse_sweepers
 
 
 @dataclass
 class QubitCrosstalkParameters(QubitFluxParameters):
     """Crosstalk runcard inputs."""
 
     flux_qubits: Optional[list[QubitId]] = None
@@ -59,30 +60,30 @@
     Qubit Crosstalk outputs.
     """
 
 
 def _acquisition(
     params: QubitCrosstalkParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> QubitCrosstalkData:
     """Data acquisition for Crosstalk Experiment."""
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
 
         if params.transition == "02":
-            if qubits[qubit].anharmonicity:
-                qd_pulses[qubit].frequency -= qubits[qubit].anharmonicity / 2
+            if platform.qubits[qubit].anharmonicity:
+                qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
             else:
                 qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
 
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
@@ -94,68 +95,74 @@
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in qubits],
+        pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
     # TODO : abstract common lines with qubit flux dep routine
     if params.flux_qubits is None:
         flux_qubits = list(platform.qubits.keys())
     else:
         flux_qubits = params.flux_qubits
-    bias_sweepers = [
-        Sweeper(
-            Parameter.bias,
-            delta_bias_range,
-            qubits=[platform.qubits[flux_qubit]],
-            type=SweeperType.OFFSET,
+    if params.flux_pulses:
+        delta_bias_flux_range, sweepers = create_flux_pulse_sweepers(
+            params, platform, targets, sequence
+        )
+    else:
+        delta_bias_flux_range = np.arange(
+            -params.bias_width / 2, params.bias_width / 2, params.bias_step
         )
-        for flux_qubit in flux_qubits
-    ]
-    data = QubitCrosstalkData(resonator_type=platform.resonator_type)
+        sweepers = [
+            Sweeper(
+                Parameter.bias,
+                delta_bias_flux_range,
+                qubits=[platform.qubits[flux_qubit]],
+                type=SweeperType.OFFSET,
+            )
+            for flux_qubit in flux_qubits
+        ]
+    data = QubitCrosstalkData(
+        resonator_type=platform.resonator_type, flux_pulses=params.flux_pulses
+    )
 
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.INTEGRATION,
         averaging_mode=AveragingMode.CYCLIC,
     )
-    for flux_qubit, bias_sweeper in zip(flux_qubits, bias_sweepers):
+    for flux_qubit, bias_sweeper in zip(flux_qubits, sweepers):
         results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
         # retrieve the results for every qubit
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             if flux_qubit is None:
-                sweetspot = qubits[qubit].sweetspot
+                sweetspot = platform.qubits[qubit].sweetspot
             else:
                 sweetspot = platform.qubits[flux_qubit].sweetspot
             data.register_qubit(
                 qubit,
                 flux_qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=delta_bias_range + sweetspot,
+                bias=delta_bias_flux_range + sweetspot,
             )
 
     return data
 
 
 def _fit(data: QubitCrosstalkData) -> QubitCrosstalkResult:
     return QubitCrosstalkResult()
 
 
-def _plot(data: QubitFluxData, fit: QubitFluxResults, qubit):
+def _plot(data: QubitFluxData, fit: QubitFluxResults, target: QubitId):
     """Plotting function for Crosstalk Experiment."""
-    return utils.flux_crosstalk_plot(data, qubit)
+    return utils.flux_crosstalk_plot(data, target)
 
 
 qubit_crosstalk = Routine(_acquisition, _fit, _plot)
 """Qubit crosstalk Routine object"""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_dependence.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,36 +7,29 @@
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Results, Routine
 from qibocal.config import log
 from qibocal.protocols.characterization.qubit_spectroscopy_ef import (
     DEFAULT_ANHARMONICITY,
 )
 
 from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, table_dict, table_html
-from . import utils
+from . import resonator_flux_dependence, utils
+from .resonator_flux_dependence import ResonatorFluxParameters
 
 
 @dataclass
-class QubitFluxParameters(Parameters):
+class QubitFluxParameters(ResonatorFluxParameters):
     """QubitFlux runcard inputs."""
 
-    freq_width: int
-    """Width for frequency sweep relative to the qubit frequency [Hz]."""
-    freq_step: int
-    """Frequency step for sweep [Hz]."""
-    bias_width: float
-    """Width for bias sweep [V]."""
-    bias_step: float
-    """Bias step for sweep [a.u.]."""
     drive_amplitude: Optional[float] = None
     """Drive amplitude (optional). If defined, same amplitude will be used in all qubits.
     Otherwise the default amplitude defined on the platform runcard will be used"""
     transition: Optional[str] = "01"
     """Flux spectroscopy transition type ("01" or "02"). Default value is 01"""
     drive_duration: int = 2000
     """Duration of the drive pulse."""
@@ -72,14 +65,17 @@
 @dataclass
 class QubitFluxData(Data):
     """QubitFlux acquisition outputs."""
 
     resonator_type: str
     """Resonator type."""
 
+    flux_pulses: bool
+    """True if sweeping flux pulses, False if sweeping bias."""
+
     qubit_frequency: dict[QubitId, float] = field(default_factory=dict)
     """Qubit frequencies."""
 
     data: dict[QubitId, npt.NDArray[QubitFluxType]] = field(default_factory=dict)
     """Raw data acquired."""
 
     def register_qubit(self, qubit, freq, bias, signal, phase):
@@ -88,32 +84,32 @@
             freq, bias, signal, phase, dtype=QubitFluxType
         )
 
 
 def _acquisition(
     params: QubitFluxParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> QubitFluxData:
     """Data acquisition for QubitFlux Experiment."""
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
     qubit_frequency = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
         qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
 
         if params.transition == "02":
-            if qubits[qubit].anharmonicity:
-                qd_pulses[qubit].frequency -= qubits[qubit].anharmonicity / 2
+            if platform.qubits[qubit].anharmonicity:
+                qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
             else:
                 qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
 
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
@@ -125,51 +121,60 @@
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in qubits],
+        pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
-    bias_sweepers = [
-        Sweeper(
-            Parameter.bias,
-            delta_bias_range,
-            qubits=list(qubits.values()),
-            type=SweeperType.OFFSET,
+    if params.flux_pulses:
+        (
+            delta_bias_flux_range,
+            sweepers,
+        ) = resonator_flux_dependence.create_flux_pulse_sweepers(
+            params, platform, targets, sequence
         )
-    ]
+    else:
+        delta_bias_flux_range = np.arange(
+            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        )
+        sweepers = [
+            Sweeper(
+                Parameter.bias,
+                delta_bias_flux_range,
+                qubits=[platform.qubits[qubit] for qubit in targets],
+                type=SweeperType.OFFSET,
+            )
+        ]
     data = QubitFluxData(
-        resonator_type=platform.resonator_type, qubit_frequency=qubit_frequency
+        resonator_type=platform.resonator_type,
+        flux_pulses=params.flux_pulses,
+        qubit_frequency=qubit_frequency,
     )
 
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.INTEGRATION,
         averaging_mode=AveragingMode.CYCLIC,
     )
-    for bias_sweeper in bias_sweepers:
+    for bias_sweeper in sweepers:
         results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
         # retrieve the results for every qubit
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
-            sweetspot = qubits[qubit].sweetspot
+            sweetspot = platform.qubits[qubit].sweetspot
             data.register_qubit(
                 qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=delta_bias_range + sweetspot,
+                bias=delta_bias_flux_range + sweetspot,
             )
     return data
 
 
 def _fit(data: QubitFluxData) -> QubitFluxResults:
     """
     Post-processing for QubitFlux Experiment. See arxiv:0703002
@@ -187,26 +192,15 @@
     for qubit in qubits:
         qubit_data = data[qubit]
 
         biases = qubit_data.bias
         frequencies = qubit_data.freq
         signal = qubit_data.signal
 
-        if data.resonator_type == "3D":
-            frequencies, biases = utils.extract_min_feature(
-                frequencies,
-                biases,
-                signal,
-            )
-        else:
-            frequencies, biases = utils.extract_max_feature(
-                frequencies,
-                biases,
-                signal,
-            )
+        frequencies, biases = utils.extract_feature(frequencies, biases, signal, "max")
 
         try:
             popt = curve_fit(
                 utils.transmon_frequency,
                 biases,
                 frequencies * HZ_TO_GHZ,
                 bounds=utils.qubit_flux_dependence_fit_bounds(
@@ -232,34 +226,38 @@
         sweetspot=sweetspot,
         asymmetry=asymmetry,
         matrix_element=matrix_element,
         fitted_parameters=fitted_parameters,
     )
 
 
-def _plot(data: QubitFluxData, fit: QubitFluxResults, qubit):
+def _plot(data: QubitFluxData, fit: QubitFluxResults, target: QubitId):
     """Plotting function for QubitFlux Experiment."""
     figures = utils.flux_dependence_plot(
-        data, fit, qubit, fit_function=utils.transmon_frequency
+        data, fit, target, fit_function=utils.transmon_frequency
     )
+    if data.flux_pulses:
+        bias_flux_unit = "a.u."
+    else:
+        bias_flux_unit = "V"
     if fit is not None:
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
-                    "Sweetspot [V]",
+                    f"Sweetspot [{bias_flux_unit}]",
                     "Qubit Frequency at Sweetspot [Hz]",
                     "Asymmetry d",
                     "V_ii [V]",
                 ],
                 [
-                    np.round(fit.sweetspot[qubit], 4),
-                    np.round(fit.frequency[qubit], 4),
-                    np.round(fit.asymmetry[qubit], 4),
-                    np.round(fit.matrix_element[qubit], 4),
+                    np.round(fit.sweetspot[target], 4),
+                    np.round(fit.frequency[target], 4),
+                    np.round(fit.asymmetry[target], 4),
+                    np.round(fit.matrix_element[target], 4),
                 ],
             )
         )
         return figures, fitting_report
     return figures, ""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/qubit_flux_tracking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass
 
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 from qibocal.config import raise_error
 
 from ..qubit_spectroscopy_ef import DEFAULT_ANHARMONICITY
 from . import qubit_flux_dependence, utils
 
 
 @dataclass
@@ -41,33 +42,33 @@
         else:
             self.data[qubit] = np.rec.array(ar)
 
 
 def _acquisition(
     params: QubitFluxTrackResults,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> QubitFluxTrackData:
     """Data acquisition for QubitFlux Experiment."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
     qubit_frequency = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
         qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
         if params.transition == "02":
-            if qubits[qubit].anharmonicity != 0:
-                qd_pulses[qubit].frequency -= qubits[qubit].anharmonicity / 2
+            if platform.qubits[qubit].anharmonicity != 0:
+                qd_pulses[qubit].frequency -= platform.qubits[qubit].anharmonicity / 2
             else:
                 qd_pulses[qubit].frequency -= DEFAULT_ANHARMONICITY / 2
 
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
@@ -84,67 +85,69 @@
     delta_bias_range = np.arange(
         -params.bias_width / 2, params.bias_width / 2, params.bias_step
     )
 
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in qubits],
+        pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
     data = QubitFluxTrackData(
-        resonator_type=platform.resonator_type, qubit_frequency=qubit_frequency
+        resonator_type=platform.resonator_type,
+        flux_pulses=params.flux_pulses,
+        qubit_frequency=qubit_frequency,
     )
 
     for bias in delta_bias_range:
-        for qubit in qubits:
+        for qubit in targets:
             try:
                 freq_resonator = utils.transmon_readout_frequency(
                     bias,
-                    qubits[qubit].drive_frequency,
-                    qubits[qubit].asymmetry,
-                    qubits[qubit].Cii,
-                    qubits[qubit].sweetspot,
-                    qubits[qubit].bare_resonator_frequency,
-                    qubits[qubit].g,
+                    platform.qubits[qubit].drive_frequency,
+                    platform.qubits[qubit].asymmetry,
+                    platform.qubits[qubit].crosstalk_matrix[qubit],
+                    platform.qubits[qubit].sweetspot,
+                    platform.qubits[qubit].bare_resonator_frequency,
+                    platform.qubits[qubit].g,
                 )
                 # modify qubit resonator frequency
-                qubits[qubit].readout_frequency = freq_resonator
+                platform.qubits[qubit].readout_frequency = freq_resonator
             except:
                 raise_error
                 (
                     RuntimeError,
                     "qubit_flux_track: Not enough parameters to estimate the resonator freq for the given bias. Please run resonator spectroscopy flux and update the runcard",
                 )
 
             # modify qubit flux
-            qubits[qubit].flux.offset = bias
+            platform.qubits[qubit].flux.offset = bias
 
             # execute pulse sequence sweeping only qubit resonator
             results = platform.sweep(
                 sequence,
                 ExecutionParameters(
                     nshots=params.nshots,
                     relaxation_time=params.relaxation_time,
                     acquisition_type=AcquisitionType.INTEGRATION,
                     averaging_mode=AveragingMode.CYCLIC,
                 ),
                 freq_sweeper,
             )
 
         # retrieve the results for every qubit
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             data.register_qubit_track(
                 qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
-                bias=bias + qubits[qubit].sweetspot,
+                bias=bias + platform.qubits[qubit].sweetspot,
             )
 
     return data
 
 
 qubit_flux_tracking = Routine(
     _acquisition,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/resonator_crosstalk.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
-from qibocal.auto.operation import Qubits, Results, Routine
+from qibocal.auto.operation import Results, Routine
 from qibocal.protocols.characterization.flux_dependence.resonator_flux_dependence import (
     ResFluxType,
     ResonatorFluxData,
     ResonatorFluxParameters,
+    create_flux_pulse_sweepers,
 )
 
 from . import utils
 
 
 @dataclass
 class ResCrosstalkParameters(ResonatorFluxParameters):
@@ -53,26 +54,26 @@
                 np.concatenate((self.data[qubit, flux_qubit], ar))
             )
         else:
             self.data[qubit, flux_qubit] = ar
 
 
 def _acquisition(
-    params: ResCrosstalkParameters, platform: Platform, qubits: Qubits
+    params: ResCrosstalkParameters, platform: Platform, targets: list[QubitId]
 ) -> ResonatorFluxData:
     """Data acquisition for ResonatorFlux experiment."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     bare_resonator_frequency = {}
     qubit_frequency = {}
-    for qubit in qubits:
+    for qubit in targets:
         bare_resonator_frequency[qubit] = platform.qubits[
             qubit
         ].bare_resonator_frequency
         qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
@@ -80,73 +81,78 @@
     # define the parameters to sweep and their range:
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        [ro_pulses[qubit] for qubit in qubits],
+        [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
     if params.flux_qubits is None:
         flux_qubits = list(platform.qubits.keys())
 
     else:
         flux_qubits = params.flux_qubits
-
-    bias_sweepers = [
-        Sweeper(
-            Parameter.bias,
-            delta_bias_range,
-            qubits=[platform.qubits[flux_qubit]],
-            type=SweeperType.OFFSET,
+    if params.flux_pulses:
+        delta_bias_flux_range, sweepers = create_flux_pulse_sweepers(
+            params, platform, targets, sequence
         )
-        for flux_qubit in flux_qubits
-    ]
+    else:
+        delta_bias_flux_range = np.arange(
+            -params.bias_width / 2, params.bias_width / 2, params.bias_step
+        )
+        sweepers = [
+            Sweeper(
+                Parameter.bias,
+                delta_bias_flux_range,
+                qubits=[platform.qubits[flux_qubit]],
+                type=SweeperType.OFFSET,
+            )
+            for flux_qubit in flux_qubits
+        ]
 
     data = ResCrosstalkData(
         resonator_type=platform.resonator_type,
+        flux_pulses=params.flux_pulses,
         qubit_frequency=qubit_frequency,
         bare_resonator_frequency=bare_resonator_frequency,
     )
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.INTEGRATION,
         averaging_mode=AveragingMode.CYCLIC,
     )
-    for flux_qubit, bias_sweeper in zip(flux_qubits, bias_sweepers):
+    for flux_qubit, bias_sweeper in zip(flux_qubits, sweepers):
         results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
         # retrieve the results for every qubit
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             if flux_qubit is None:
-                sweetspot = qubits[qubit].sweetspot
+                sweetspot = platform.qubits[qubit].sweetspot
             else:
                 sweetspot = platform.qubits[flux_qubit].sweetspot
             data.register_qubit(
                 qubit,
                 flux_qubit,
                 signal=result.magnitude,
                 phase=result.phase,
                 freq=delta_frequency_range + ro_pulses[qubit].frequency,
-                bias=delta_bias_range + sweetspot,
+                bias=delta_bias_flux_range + sweetspot,
             )
 
     return data
 
 
 def _fit(data: ResCrosstalkData) -> ResCrosstalkResults:
     return ResCrosstalkResults()
 
 
-def _plot(data: ResCrosstalkData, fit: ResCrosstalkResults, qubit):
+def _plot(data: ResCrosstalkData, fit: ResCrosstalkResults, target: QubitId):
     """Plotting function for ResonatorFlux Experiment."""
-    return utils.flux_crosstalk_plot(data, qubit)
+    return utils.flux_crosstalk_plot(data, target)
 
 
 resonator_crosstalk = Routine(_acquisition, _fit, _plot)
 """Resonator crosstalk Routine object"""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/resonator_flux_dependence.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_spectroscopy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,287 +1,274 @@
-from dataclasses import dataclass, field
+from dataclasses import dataclass, field, fields
+from typing import Optional, Union
 
 import numpy as np
 import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
-from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
-from qibocal.config import log
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
-from ..utils import GHZ_TO_HZ, HZ_TO_GHZ, table_dict, table_html
-from . import utils
+from .utils import (
+    PowerLevel,
+    chi2_reduced,
+    lorentzian,
+    lorentzian_fit,
+    spectroscopy_plot,
+)
+
+ResSpecType = np.dtype(
+    [
+        ("freq", np.float64),
+        ("signal", np.float64),
+        ("phase", np.float64),
+        ("error_signal", np.float64),
+        ("error_phase", np.float64),
+    ]
+)
+"""Custom dtype for resonator spectroscopy."""
 
 
 @dataclass
-class ResonatorFluxParameters(Parameters):
-    """ResonatorFlux runcard inputs."""
+class ResonatorSpectroscopyParameters(Parameters):
+    """ResonatorSpectroscopy runcard inputs."""
 
     freq_width: int
-    """Width for frequency sweep relative to the readout frequency [Hz]."""
+    """Width for frequency sweep relative  to the readout frequency [Hz]."""
     freq_step: int
     """Frequency step for sweep [Hz]."""
-    bias_width: float
-    """Width for bias sweep [V]."""
-    bias_step: float
-    """Bias step for sweep [a.u.]."""
+    power_level: Union[PowerLevel, str]
+    """Power regime (low or high). If low the readout frequency will be updated.
+    If high both the readout frequency and the bare resonator frequency will be updated."""
+    amplitude: Optional[float] = None
+    """Readout amplitude (optional). If defined, same amplitude will be used in all qubits.
+    Otherwise the default amplitude defined on the platform runcard will be used"""
+    attenuation: Optional[int] = None
+    """Readout attenuation (optional). If defined, same attenuation will be used in all qubits.
+    Otherwise the default attenuation defined on the platform runcard will be used"""
+
+    def __post_init__(self):
+        if isinstance(self.power_level, str):
+            self.power_level = PowerLevel(self.power_level)
 
 
 @dataclass
-class ResonatorFluxResults(Results):
-    """ResonatoFlux outputs."""
+class ResonatorSpectroscopyResults(Results):
+    """ResonatorSpectroscopy outputs."""
 
     frequency: dict[QubitId, float]
-    """Readout frequency for each qubit."""
-    sweetspot: dict[QubitId, float]
-    """Sweetspot for each qubit."""
-    asymmetry: dict[QubitId, float]
-    """Asymmetry between junctions."""
-    bare_frequency: dict[QubitId, float]
-    """Resonator bare frequency."""
-    drive_frequency: dict[QubitId, float]
-    """Qubit frequency at sweetspot."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitting output."""
-    coupling: dict[QubitId, float]
-    """Qubit-resonator coupling."""
-    matrix_element: dict[QubitId, float]
-    """C_ii coefficient."""
-
+    """Readout frequency [Hz] for each qubit."""
+    fitted_parameters: dict[QubitId, list[float]]
+    """Raw fitted parameters."""
+    bare_frequency: Optional[dict[QubitId, float]] = field(
+        default_factory=dict,
+    )
+    """Bare resonator frequency [Hz] for each qubit."""
+    error_fit_pars: dict[QubitId, list] = field(default_factory=dict)
+    """Errors of the fit parameters."""
+    chi2_reduced: dict[QubitId, tuple[float, Optional[float]]] = field(
+        default_factory=dict
+    )
+    """Chi2 reduced."""
+    amplitude: Optional[dict[QubitId, float]] = field(
+        default_factory=dict,
+    )
+    """Readout amplitude for each qubit."""
+    attenuation: Optional[dict[QubitId, int]] = field(
+        default_factory=dict,
+    )
+    """Readout attenuation [dB] for each qubit."""
 
-ResFluxType = np.dtype(
-    [
-        ("freq", np.float64),
-        ("bias", np.float64),
-        ("signal", np.float64),
-        ("phase", np.float64),
-    ]
-)
-"""Custom dtype for resonator flux dependence."""
+    def __contains__(self, key: QubitId):
+        return all(
+            key in getattr(self, field.name)
+            for field in fields(self)
+            if isinstance(getattr(self, field.name), dict)
+            and field.name != "bare_frequency"
+        )
 
 
 @dataclass
-class ResonatorFluxData(Data):
-    """ResonatorFlux acquisition outputs."""
+class ResonatorSpectroscopyData(Data):
+    """Data structure for resonator spectroscopy with attenuation."""
 
-    """Resonator type."""
     resonator_type: str
-
-    qubit_frequency: dict[QubitId, float] = field(default_factory=dict)
-    """Qubit frequencies."""
-
-    bare_resonator_frequency: dict[QubitId, int] = field(default_factory=dict)
-    """Qubit bare resonator frequency power provided by the user."""
-
-    data: dict[QubitId, npt.NDArray[ResFluxType]] = field(default_factory=dict)
+    """Resonator type."""
+    amplitudes: dict[QubitId, float]
+    """Amplitudes provided by the user."""
+    data: dict[QubitId, npt.NDArray[ResSpecType]] = field(default_factory=dict)
     """Raw data acquired."""
-
-    def register_qubit(self, qubit, freq, bias, signal, phase):
-        """Store output for single qubit."""
-        self.data[qubit] = utils.create_data_array(
-            freq, bias, signal, phase, dtype=ResFluxType
-        )
+    power_level: Optional[PowerLevel] = None
+    """Power regime of the resonator."""
+    attenuations: Optional[dict[QubitId, int]] = field(default_factory=dict)
+    """Readout attenuation [dB] for each qubit"""
+
+    @classmethod
+    def load(cls, path):
+        obj = super().load(path)
+        # Instantiate PowerLevel object
+        if obj.power_level is not None:  # pylint: disable=E1101
+            obj.power_level = PowerLevel(obj.power_level)  # pylint: disable=E1101
+        return obj
 
 
 def _acquisition(
-    params: ResonatorFluxParameters, platform: Platform, qubits: Qubits
-) -> ResonatorFluxData:
-    """Data acquisition for ResonatorFlux experiment."""
+    params: ResonatorSpectroscopyParameters, platform: Platform, targets: list[QubitId]
+) -> ResonatorSpectroscopyData:
+    """Data acquisition for resonator spectroscopy."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
-    qubit_frequency = {}
-    bare_resonator_frequency = {}
-    for qubit in qubits:
-        qubit_frequency[qubit] = platform.qubits[qubit].drive_frequency
-        bare_resonator_frequency[qubit] = platform.qubits[
-            qubit
-        ].bare_resonator_frequency
+    amplitudes = {}
+    attenuations = {}
 
+    for qubit in targets:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
+
+        if params.amplitude is not None:
+            ro_pulses[qubit].amplitude = params.amplitude
+
+        amplitudes[qubit] = ro_pulses[qubit].amplitude
+
+        if params.attenuation is not None:
+            platform.qubits[qubit].readout.attenuation = params.attenuation
+
+        try:
+            attenuation = platform.qubits[qubit].readout.attenuation
+        except AttributeError:
+            attenuation = None
+
+        attenuations[qubit] = attenuation
         sequence.add(ro_pulses[qubit])
 
-    # define the parameters to sweep and their range:
+    # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
-    freq_sweeper = Sweeper(
+    sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        [ro_pulses[qubit] for qubit in qubits],
+        pulses=[ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
-
-    delta_bias_range = np.arange(
-        -params.bias_width / 2, params.bias_width / 2, params.bias_step
-    )
-    bias_sweepers = [
-        Sweeper(
-            Parameter.bias,
-            delta_bias_range,
-            qubits=list(qubits.values()),
-            type=SweeperType.OFFSET,
-        )
-    ]
-
-    data = ResonatorFluxData(
+    data = ResonatorSpectroscopyData(
         resonator_type=platform.resonator_type,
-        qubit_frequency=qubit_frequency,
-        bare_resonator_frequency=bare_resonator_frequency,
+        power_level=params.power_level,
+        amplitudes=amplitudes,
+        attenuations=attenuations,
     )
 
-    options = ExecutionParameters(
-        nshots=params.nshots,
-        relaxation_time=params.relaxation_time,
-        acquisition_type=AcquisitionType.INTEGRATION,
-        averaging_mode=AveragingMode.CYCLIC,
+    results = platform.sweep(
+        sequence,
+        ExecutionParameters(
+            nshots=params.nshots,
+            relaxation_time=params.relaxation_time,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=AveragingMode.SINGLESHOT,
+        ),
+        sweeper,
     )
-    for bias_sweeper in bias_sweepers:
-        results = platform.sweep(sequence, options, bias_sweeper, freq_sweeper)
-        # retrieve the results for every qubit
-        for qubit in qubits:
-            result = results[ro_pulses[qubit].serial]
-            sweetspot = qubits[qubit].sweetspot
-            data.register_qubit(
-                qubit,
-                signal=result.magnitude,
-                phase=result.phase,
-                freq=delta_frequency_range + ro_pulses[qubit].frequency,
-                bias=delta_bias_range + sweetspot,
-            )
 
+    # retrieve the results for every qubit
+    for qubit in targets:
+        result = results[ro_pulses[qubit].serial]
+        # store the results
+        data.register_qubit(
+            ResSpecType,
+            (qubit),
+            dict(
+                signal=np.abs(result.average.voltage),
+                phase=np.mean(result.phase, axis=0),
+                freq=delta_frequency_range + ro_pulses[qubit].frequency,
+                error_signal=result.average.std,
+                error_phase=np.std(result.phase, axis=0, ddof=1),
+            ),
+        )
+    # finally, save the remaining data
     return data
 
 
-def _fit(data: ResonatorFluxData) -> ResonatorFluxResults:
-    """
-    Post-processing for QubitFlux Experiment. See arxiv:0703002
-    Fit frequency as a function of current for the flux qubit spectroscopy
-    data (QubitFluxData): data object with information on the feature response at each current point.
-    """
-
+def _fit(
+    data: ResonatorSpectroscopyData,
+) -> ResonatorSpectroscopyResults:
+    """Post-processing function for ResonatorSpectroscopy."""
+    # TODO: change data.qubits
     qubits = data.qubits
-    frequency = {}
-    sweetspot = {}
-    asymmetry = {}
     bare_frequency = {}
-    drive_frequency = {}
+    frequency = {}
     fitted_parameters = {}
-    matrix_element = {}
-    coupling = {}
-
+    error_fit_pars = {}
+    chi2 = {}
+    amplitudes = {}
     for qubit in qubits:
-        qubit_data = data[qubit]
+        fit_result = lorentzian_fit(
+            data[qubit], resonator_type=data.resonator_type, fit="resonator"
+        )
 
-        biases = qubit_data.bias
-        frequencies = qubit_data.freq
-        signal = qubit_data.signal
-
-        if data.resonator_type == "3D":
-            frequencies, biases = utils.extract_max_feature(
-                frequencies,
-                biases,
-                signal,
-            )
-        else:
-            frequencies, biases = utils.extract_min_feature(
-                frequencies,
-                biases,
-                signal,
+        if fit_result is not None:
+            frequency[qubit], fitted_parameters[qubit], error_fit_pars[qubit] = (
+                fit_result
             )
-
-        try:
-            popt = curve_fit(
-                utils.transmon_readout_frequency,
-                biases,
-                frequencies * HZ_TO_GHZ,
-                bounds=utils.resonator_flux_dependence_fit_bounds(
-                    data.qubit_frequency[qubit],
-                    qubit_data.bias,
-                    data.bare_resonator_frequency[qubit],
+            if data.power_level is PowerLevel.high:
+                bare_frequency[qubit] = frequency[qubit]
+            chi2[qubit] = (
+                chi2_reduced(
+                    data[qubit].signal,
+                    lorentzian(data[qubit].freq, *fitted_parameters[qubit]),
+                    data[qubit].error_signal,
                 ),
-                maxfev=100000,
-            )[0]
-            fitted_parameters[qubit] = popt.tolist()
-
-            # frequency corresponds to transmon readout frequency
-            # at the sweetspot popt[3]
-            frequency[qubit] = (
-                utils.transmon_readout_frequency(popt[3], *popt) * GHZ_TO_HZ
-            )
-            sweetspot[qubit] = popt[3]
-            asymmetry[qubit] = popt[1]
-            bare_frequency[qubit] = popt[4] * GHZ_TO_HZ
-            drive_frequency[qubit] = popt[0] * GHZ_TO_HZ
-            coupling[qubit] = popt[5]
-            matrix_element[qubit] = popt[2]
-        except ValueError as e:
-            log.error(
-                f"Error in resonator_flux protocol fit: {e} "
-                "The threshold for the SNR mask is probably too high. "
-                "Lowering the value of `threshold` in `extract_*_feature`"
-                "should fix the problem."
+                np.sqrt(2 / len(data[qubit].freq)),
             )
+            amplitudes[qubit] = fitted_parameters[qubit][0]
 
-    return ResonatorFluxResults(
-        frequency=frequency,
-        sweetspot=sweetspot,
-        asymmetry=asymmetry,
-        bare_frequency=bare_frequency,
-        drive_frequency=drive_frequency,
-        coupling=coupling,
-        matrix_element=matrix_element,
-        fitted_parameters=fitted_parameters,
-    )
-
-
-def _plot(data: ResonatorFluxData, fit: ResonatorFluxResults, qubit):
-    """Plotting function for ResonatorFlux Experiment."""
-    figures = utils.flux_dependence_plot(
-        data, fit, qubit, utils.transmon_readout_frequency
-    )
-    if fit is not None:
-        fitting_report = table_html(
-            table_dict(
-                qubit,
-                [
-                    "Sweetspot [V]",
-                    "Bare Resonator Frequency [Hz]",
-                    "Readout Frequency [Hz]",
-                    "Qubit Frequency at Sweetspot [Hz]",
-                    "Asymmetry d",
-                    "Coupling g",
-                    "V_ii [V]",
-                ],
-                [
-                    np.round(fit.sweetspot[qubit], 4),
-                    np.round(fit.bare_frequency[qubit], 4),
-                    np.round(fit.frequency[qubit], 4),
-                    np.round(fit.drive_frequency[qubit], 4),
-                    np.round(fit.asymmetry[qubit], 4),
-                    np.round(fit.coupling[qubit], 4),
-                    np.round(fit.matrix_element[qubit], 4),
-                ],
-            )
+    if data.power_level is PowerLevel.high:
+        return ResonatorSpectroscopyResults(
+            frequency=frequency,
+            fitted_parameters=fitted_parameters,
+            bare_frequency=bare_frequency,
+            error_fit_pars=error_fit_pars,
+            chi2_reduced=chi2,
+            amplitude=data.amplitudes,
+            attenuation=data.attenuations,
+        )
+    else:
+        return ResonatorSpectroscopyResults(
+            frequency=frequency,
+            fitted_parameters=fitted_parameters,
+            error_fit_pars=error_fit_pars,
+            chi2_reduced=chi2,
+            amplitude=data.amplitudes,
+            attenuation=data.attenuations,
         )
-        return figures, fitting_report
-    return figures, ""
 
 
-def _update(results: ResonatorFluxResults, platform: Platform, qubit: QubitId):
-    update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
-    update.readout_frequency(results.frequency[qubit], platform, qubit)
-    update.drive_frequency(results.drive_frequency[qubit], platform, qubit)
-    update.asymmetry(results.asymmetry[qubit], platform, qubit)
-    update.coupling(results.coupling[qubit], platform, qubit)
+def _plot(
+    data: ResonatorSpectroscopyData, target: QubitId, fit: ResonatorSpectroscopyResults
+):
+    """Plotting function for ResonatorSpectroscopy."""
+    return spectroscopy_plot(data, target, fit)
+
+
+def _update(results: ResonatorSpectroscopyResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.frequency[target], platform, target)
+
+    # if this condition is satifisfied means that we are in the low power regime
+    # therefore we update also the readout amplitude
+    if len(results.bare_frequency) == 0:
+        update.readout_amplitude(results.amplitude[target], platform, target)
+        if results.attenuation[target] is not None:
+            update.readout_attenuation(results.attenuation[target], platform, target)
+    else:
+        update.bare_resonator_frequency(
+            results.bare_frequency[target], platform, target
+        )
 
 
-resonator_flux = Routine(_acquisition, _fit, _plot, _update)
-"""ResonatorFlux Routine object."""
+resonator_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
+"""ResonatorSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/flux_dependence/utils.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/flux_dependence/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 import numpy as np
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 
 from ..utils import HZ_TO_GHZ
 
+CONFIDENCE_INTERVAL_FIRST_MASK = 99
+"""Confidence interval used to mask flux data."""
+CONFIDENCE_INTERVAL_SECOND_MASK = 70
+"""Confidence interval used to clean outliers."""
+
 
 def is_crosstalk(data):
     """Check if keys are tuple which corresponds to crosstalk data structure."""
     return all(isinstance(key, tuple) for key in data.data.keys())
 
 
 def create_data_array(freq, bias, signal, phase, dtype):
@@ -73,15 +78,18 @@
 
     fig.update_xaxes(
         title_text=f"Frequency [GHz]",
         row=1,
         col=1,
     )
 
-    fig.update_yaxes(title_text="Bias [V]", row=1, col=1)
+    if data.flux_pulses:
+        fig.update_yaxes(title_text="Flux [a.u.]", row=1, col=1)
+    else:
+        fig.update_yaxes(title_text="Bias [V]", row=1, col=1)
 
     fig.add_trace(
         go.Heatmap(
             x=qubit_data.freq * HZ_TO_GHZ,
             y=qubit_data.bias,
             z=qubit_data.phase,
             colorbar_x=1.01,
@@ -142,17 +150,22 @@
 
         fig.update_xaxes(
             title_text="Frequency [GHz]",
             row=1,
             col=col + 1,
         )
 
-        fig.update_yaxes(
-            title_text=f"Qubit {flux_qubit[1]}: Bias [V]", row=1, col=col + 1
-        )
+        if data.flux_pulses:
+            fig.update_yaxes(
+                title_text=f"Qubit {flux_qubit[1]}: Flux [a.u.]", row=1, col=col + 1
+            )
+        else:
+            fig.update_yaxes(
+                title_text=f"Qubit {flux_qubit[1]}: Bias [V]", row=1, col=col + 1
+            )
 
     fig.update_layout(xaxis1=dict(range=[np.min(frequencies), np.max(frequencies)]))
     fig.update_traces(showscale=False)  # disable colorbar
     fig.update_layout(
         showlegend=False,
     )
 
@@ -219,30 +232,41 @@
          (float): resonator frequency as a function of bias.
     """
     return resonator_freq + g**2 * G_f_d(x, offset, d, element) / (
         resonator_freq - transmon_frequency(x, w_max, d, element, offset)
     )
 
 
-def extract_min_feature(freq, bias, signal, threshold=1.5):
-    """Extract min feature using SNR."""
-    mean_signal = np.mean(signal)
-    std_signal = np.std(signal)
-    snr_map = (signal - mean_signal) / std_signal
-    binary_mask = snr_map < -threshold
-    return freq[binary_mask], bias[binary_mask]
-
-
-def extract_max_feature(freq, bias, signal, threshold=1.5):
-    """Extract max feature using SNR."""
-    mean_signal = np.mean(signal)
-    std_signal = np.std(signal)
-    snr_map = (signal - mean_signal) / std_signal
-    binary_mask = snr_map > threshold
-    return freq[binary_mask], bias[binary_mask]
+def extract_feature(freq: np.ndarray, bias: np.ndarray, signal: np.ndarray, feat: str):
+    """Extract feature using confidence intervals.
+
+    A first mask is construct by looking at 99% confidence interval for each bias bin.
+    A second mask is applied by looking at 70% confidence interval to remove outliers.
+    """
+
+    masks = []
+    for bias_bin in np.unique(bias):
+        signal_fixed_bias = signal[bias == bias_bin]
+        min, max = np.percentile(
+            signal_fixed_bias,
+            [100 - CONFIDENCE_INTERVAL_FIRST_MASK, CONFIDENCE_INTERVAL_FIRST_MASK],
+        )
+        masks.append(
+            signal_fixed_bias < min if feat == "min" else signal_fixed_bias > max
+        )
+
+    first_mask = np.vstack(masks).ravel()
+    min, max = np.percentile(
+        signal[first_mask],
+        [100 - CONFIDENCE_INTERVAL_SECOND_MASK, CONFIDENCE_INTERVAL_SECOND_MASK],
+    )
+    second_mask = (
+        signal[first_mask] < max if feat == "min" else signal[first_mask] > min
+    )
+    return freq[first_mask][second_mask], bias[first_mask][second_mask]
 
 
 def qubit_flux_dependence_fit_bounds(qubit_frequency: float, bias: np.array):
     """Returns bounds for qubit flux fit."""
     return (
         [
             qubit_frequency * HZ_TO_GHZ - 1,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/qubit_spectroscopy.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Parameters, Results, Routine
 
 from .resonator_spectroscopy import ResonatorSpectroscopyData, ResSpecType
-from .utils import lorentzian_fit, spectroscopy_plot
+from .utils import chi2_reduced, lorentzian, lorentzian_fit, spectroscopy_plot
 
 
 @dataclass
 class QubitSpectroscopyParameters(Parameters):
     """QubitSpectroscopy runcard inputs."""
 
     freq_width: int
@@ -35,33 +35,39 @@
 
     frequency: dict[QubitId, dict[str, float]]
     """Drive frequecy [GHz] for each qubit."""
     amplitude: dict[QubitId, float]
     """Input drive amplitude. Same for all qubits."""
     fitted_parameters: dict[QubitId, list[float]]
     """Raw fitting output."""
+    chi2_reduced: dict[QubitId, tuple[float, Optional[float]]] = field(
+        default_factory=dict
+    )
+    """Chi2 reduced."""
+    error_fit_pars: dict[QubitId, list] = field(default_factory=dict)
+    """Errors of the fit parameters."""
 
 
 class QubitSpectroscopyData(ResonatorSpectroscopyData):
     """QubitSpectroscopy acquisition outputs."""
 
 
 def _acquisition(
-    params: QubitSpectroscopyParameters, platform: Platform, qubits: Qubits
+    params: QubitSpectroscopyParameters, platform: Platform, targets: list[QubitId]
 ) -> QubitSpectroscopyData:
     """Data acquisition for qubit spectroscopy."""
     # create a sequence of pulses for the experiment:
     # long drive probing pulse - MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
     amplitudes = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.drive_duration
         )
         if params.drive_amplitude is not None:
             qd_pulses[qubit].amplitude = params.drive_amplitude
 
         amplitudes[qubit] = qd_pulses[qubit].amplitude
@@ -75,73 +81,88 @@
     # define the parameter to sweep and its range:
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in qubits],
+        pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
     # Create data structure for data acquisition.
     data = QubitSpectroscopyData(
         resonator_type=platform.resonator_type, amplitudes=amplitudes
     )
 
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
+            averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
 
     # retrieve the results for every qubit
     for qubit, ro_pulse in ro_pulses.items():
         result = results[ro_pulse.serial]
         # store the results
         data.register_qubit(
             ResSpecType,
             (qubit),
             dict(
-                signal=result.magnitude,
-                phase=result.phase,
+                signal=np.abs(result.average.voltage),
+                phase=np.mean(result.phase, axis=0),
                 freq=delta_frequency_range + qd_pulses[qubit].frequency,
+                error_signal=result.average.std,
+                error_phase=np.std(result.phase, axis=0, ddof=1),
             ),
         )
     return data
 
 
 def _fit(data: QubitSpectroscopyData) -> QubitSpectroscopyResults:
     """Post-processing function for QubitSpectroscopy."""
     qubits = data.qubits
     frequency = {}
     fitted_parameters = {}
+    error_fit_pars = {}
+    chi2 = {}
     for qubit in qubits:
-        freq, fitted_params = lorentzian_fit(
+        fit_result = lorentzian_fit(
             data[qubit], resonator_type=data.resonator_type, fit="qubit"
         )
-        frequency[qubit] = freq
-        fitted_parameters[qubit] = fitted_params
-
+        if fit_result is not None:
+            frequency[qubit], fitted_parameters[qubit], error_fit_pars[qubit] = (
+                fit_result
+            )
+            chi2[qubit] = (
+                chi2_reduced(
+                    data[qubit].signal,
+                    lorentzian(data[qubit].freq, *fitted_parameters[qubit]),
+                    data[qubit].error_signal,
+                ),
+                np.sqrt(2 / len(data[qubit].freq)),
+            )
     return QubitSpectroscopyResults(
         frequency=frequency,
         fitted_parameters=fitted_parameters,
         amplitude=data.amplitudes,
+        error_fit_pars=error_fit_pars,
+        chi2_reduced=chi2,
     )
 
 
-def _plot(data: QubitSpectroscopyData, qubit, fit: QubitSpectroscopyResults):
+def _plot(data: QubitSpectroscopyData, target: QubitId, fit: QubitSpectroscopyResults):
     """Plotting function for QubitSpectroscopy."""
-    return spectroscopy_plot(data, qubit, fit)
+    return spectroscopy_plot(data, target, fit)
 
 
-def _update(results: QubitSpectroscopyResults, platform: Platform, qubit: QubitId):
-    update.drive_frequency(results.frequency[qubit], platform, qubit)
+def _update(results: QubitSpectroscopyResults, platform: Platform, target: QubitId):
+    update.drive_frequency(results.frequency[target], platform, target)
 
 
 qubit_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
 """QubitSpectroscopy Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,180 +1,182 @@
-from dataclasses import asdict, dataclass, field
+from dataclasses import dataclass, field
 
 import numpy as np
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
+import numpy.typing as npt
+import plotly.graph_objects as go
 from qibolab.platform import Platform
-from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
-
-from .qubit_spectroscopy import (
-    QubitSpectroscopyData,
-    QubitSpectroscopyParameters,
-    QubitSpectroscopyResults,
-    _fit,
+from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.protocols.characterization import classification
+from qibocal.protocols.characterization.readout_optimization.resonator_frequency import (
+    ResonatorFrequencyType,
 )
-from .resonator_spectroscopy import ResSpecType
-from .utils import spectroscopy_plot, table_dict, table_html
-
-DEFAULT_ANHARMONICITY = 300e6
-"""Initial guess for anharmonicity."""
+from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
-class QubitSpectroscopyEFParameters(QubitSpectroscopyParameters):
-    """QubitSpectroscopyEF runcard inputs."""
+class TwpaFrequencyParameters(Parameters):
+    """TwpaFrequency runcard inputs."""
 
-
-@dataclass
-class QubitSpectroscopyEFResults(QubitSpectroscopyResults):
-    """QubitSpectroscopyEF outputs."""
-
-    anharmonicity: dict[QubitId, float] = field(default_factory=dict)
+    frequency_width: float
+    """Relative frequency width [Hz]"""
+    frequency_step: float
+    """Frequency step [Hz]"""
 
 
 @dataclass
-class QubitSpectroscopyEFData(QubitSpectroscopyData):
-    """QubitSpectroscopy acquisition outputs."""
+class TwpaFrequencyData(Data):
+    """TwpaFrequency acquisition outputs."""
 
-    drive_frequencies: dict[QubitId, float] = field(default_factory=dict)
+    data: dict[
+        tuple[QubitId, float], npt.NDArray[classification.ClassificationType]
+    ] = field(default_factory=dict)
+    """Raw data acquired."""
+    frequencies: dict[QubitId, float] = field(default_factory=dict)
+    """Frequencies for each qubit."""
 
 
-def _fit_ef(data: QubitSpectroscopyEFData) -> QubitSpectroscopyEFResults:
-    results = _fit(data)
-    anharmoncities = {
-        qubit: data.drive_frequencies[qubit] - results.frequency[qubit]
-        for qubit in data.qubits
-    }
-    params = asdict(results)
-    params.update({"anharmonicity": anharmoncities})
+@dataclass
+class TwpaFrequencyResults(Results):
+    """TwpaFrequency outputs."""
 
-    return QubitSpectroscopyEFResults(**params)
+    best_freqs: dict[QubitId, float] = field(default_factory=dict)
+    best_fidelities: dict[QubitId, float] = field(default_factory=dict)
+    best_angles: dict[QubitId, float] = field(default_factory=dict)
+    best_thresholds: dict[QubitId, float] = field(default_factory=dict)
 
 
 def _acquisition(
-    params: QubitSpectroscopyEFParameters, platform: Platform, qubits: Qubits
-) -> QubitSpectroscopyEFData:
-    """Data acquisition for qubit spectroscopy ef protocol.
-
-    Similar to a qubit spectroscopy with the difference that the qubit is first
-    excited to the state 1. This protocols aims at finding the transition frequency between
-    state 1 and the state 2. The anharmonicity is also computed.
-
-    If the RX12 frequency is not present in the runcard the sweep is performed around the
-    qubit drive frequency shifted by DEFAULT_ANHARMONICITY, an hardcoded parameter editable
-    in this file.
+    params: TwpaFrequencyParameters,
+    platform: Platform,
+    targets: list[QubitId],
+) -> TwpaFrequencyData:
+    r"""
+    Data acquisition for TWPA power optmization.
+    This protocol perform a classification protocol for twpa frequencies
+    in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
+    with step frequency_step.
+
+    Args:
+        params (:class:`TwpaFrequencyParameters`): input parameters
+        platform (:class:`Platform`): Qibolab's platform
+        qubits (dict): dict of target :class:`Qubit` objects to be characterized
 
+    Returns:
+        data (:class:`TwpaFrequencyData`)
     """
-    # create a sequence of pulses for the experiment:
-    # long drive probing pulse - MZ
 
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence = PulseSequence()
-    ro_pulses = {}
-    qd_pulses = {}
-    rx_pulses = {}
-    amplitudes = {}
-    drive_frequencies = {}
-    for qubit in qubits:
-        rx_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
-        drive_frequencies[qubit] = rx_pulses[qubit].frequency
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=rx_pulses[qubit].finish, duration=params.drive_duration
-        )
-        if platform.qubits[qubit].native_gates.RX12.frequency is None:
-            qd_pulses[qubit].frequency = (
-                rx_pulses[qubit].frequency - DEFAULT_ANHARMONICITY
-            )
-        else:
-            qd_pulses[qubit].frequency = platform.qubits[
-                qubit
-            ].native_gates.RX12.frequency
-
-        if params.drive_amplitude is not None:
-            qd_pulses[qubit].amplitude = params.drive_amplitude
-
-        amplitudes[qubit] = qd_pulses[qubit].amplitude
-
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=qd_pulses[qubit].finish
-        )
-        sequence.add(rx_pulses[qubit])
-        sequence.add(qd_pulses[qubit])
-        sequence.add(ro_pulses[qubit])
-
-    # define the parameter to sweep and its range:
-    # sweep only before qubit frequency
-    delta_frequency_range = np.arange(
-        -params.freq_width, params.freq_width, params.freq_step
-    )
-    sweeper = Sweeper(
-        Parameter.frequency,
-        delta_frequency_range,
-        pulses=[qd_pulses[qubit] for qubit in qubits],
-        type=SweeperType.OFFSET,
-    )
+    data = TwpaFrequencyData()
 
-    # Create data structure for data acquisition.
-    data = QubitSpectroscopyEFData(
-        resonator_type=platform.resonator_type,
-        amplitudes=amplitudes,
-        drive_frequencies=drive_frequencies,
-    )
+    freq_range = np.arange(
+        -params.frequency_width / 2, params.frequency_width / 2, params.frequency_step
+    ).astype(int)
+
+    initial_twpa_freq = {}
+    for qubit in targets:
+        initial_twpa_freq[qubit] = float(
+            platform.qubits[qubit].twpa.local_oscillator.frequency
+        )
+        data.frequencies[qubit] = list(
+            float(platform.qubits[qubit].twpa.local_oscillator.frequency) + freq_range
+        )
 
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        sweeper,
-    )
+    for freq in freq_range:
+        for qubit in targets:
+            platform.qubits[qubit].twpa.local_oscillator.frequency = (
+                initial_twpa_freq[qubit] + freq
+            )
 
-    # retrieve the results for every qubit
-    for qubit, ro_pulse in ro_pulses.items():
-        result = results[ro_pulse.serial]
-        # store the results
-        data.register_qubit(
-            ResSpecType,
-            (qubit),
-            dict(
-                signal=result.magnitude,
-                phase=result.phase,
-                freq=delta_frequency_range + qd_pulses[qubit].frequency,
+        classification_data = classification._acquisition(
+            classification.SingleShotClassificationParameters.load(
+                {"nshots": params.nshots}
             ),
+            platform,
+            targets,
         )
+        classification_result = classification._fit(classification_data)
+        for qubit in targets:
+            data.register_qubit(
+                ResonatorFrequencyType,
+                (qubit),
+                dict(
+                    freq=np.array(
+                        [platform.qubits[qubit].twpa.local_oscillator.frequency],
+                        dtype=np.float64,
+                    ),
+                    assignment_fidelity=np.array(
+                        [classification_result.assignment_fidelity[qubit]],
+                    ),
+                    angle=np.array([classification_result.rotation_angle[qubit]]),
+                    threshold=np.array([classification_result.threshold[qubit]]),
+                ),
+            )
     return data
 
 
-def _plot(data: QubitSpectroscopyEFData, qubit, fit: QubitSpectroscopyEFResults):
-    """Plotting function for QubitSpectroscopy."""
-    figures, report = spectroscopy_plot(data, qubit, fit)
+def _fit(data: TwpaFrequencyData) -> TwpaFrequencyResults:
+    """Extract fidelity for each configuration qubit / param.
+    Where param can be either frequency or power."""
+
+    qubits = data.qubits
+    best_freq = {}
+    best_fidelity = {}
+    best_angle = {}
+    best_threshold = {}
+    for qubit in qubits:
+        data_qubit = data[qubit]
+        index_best_err = np.argmax(data_qubit["assignment_fidelity"])
+        best_fidelity[qubit] = data_qubit["assignment_fidelity"][index_best_err]
+        best_freq[qubit] = data_qubit["freq"][index_best_err]
+        best_angle[qubit] = data_qubit["angle"][index_best_err]
+        best_threshold[qubit] = data_qubit["threshold"][index_best_err]
+
+    return TwpaFrequencyResults(
+        best_freq, best_fidelity, best_thresholds=best_threshold, best_angles=best_angle
+    )
+
+
+def _plot(data: TwpaFrequencyData, fit: TwpaFrequencyResults, target: QubitId):
+    """Plotting function that shows the assignment fidelity
+    for different values of the twpa frequency for a single qubit"""
+
+    figures = []
+    fitting_report = ""
     if fit is not None:
-        report = table_html(
+        qubit_data = data.data[target]
+        fidelities = qubit_data["assignment_fidelity"]
+        frequencies = qubit_data["freq"]
+        fitting_report = table_html(
             table_dict(
-                qubit,
-                ["Frequency 1->2 [Hz]", "Amplitude [a.u.]", "Anharmonicity [Hz]"],
+                target,
+                ["Best assignment fidelity", "TWPA Frequency [Hz]"],
                 [
-                    np.round(fit.frequency[qubit], 0),
-                    fit.amplitude[qubit],
-                    np.round(fit.anharmonicity[qubit], 0),
+                    np.round(fit.best_fidelities[target], 3),
+                    fit.best_freqs[target],
                 ],
             )
         )
+        fig = go.Figure(
+            [go.Scatter(x=frequencies * HZ_TO_GHZ, y=fidelities, name="Fidelity")]
+        )
+
+        fig.update_layout(
+            showlegend=True,
+            xaxis_title="TWPA Frequency [GHz]",
+            yaxis_title="Assignment Fidelity",
+        )
+
+        figures.append(fig)
 
-    return figures, report
+    return figures, fitting_report
 
 
-def _update(results: QubitSpectroscopyEFResults, platform: Platform, qubit: QubitId):
-    """Update w12 frequency"""
-    update.frequency_12_transition(results.frequency[qubit], platform, qubit)
-    update.anharmonicity(results.anharmonicity[qubit], platform, qubit)
+def _update(results: TwpaFrequencyResults, platform: Platform, target: QubitId):
+    update.twpa_frequency(results.best_freqs[target], platform, target)
+    update.iq_angle(results.best_angles[target], platform, target)
+    update.threshold(results.best_thresholds[target], platform, target)
 
 
-qubit_spectroscopy_ef = Routine(_acquisition, _fit_ef, _plot, _update)
-"""QubitSpectroscopyEF Routine object."""
+twpa_frequency = Routine(_acquisition, _fit, _plot, _update)
+"""Twpa frequency Routine  object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/qutrit_classification.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/qutrit_classification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 from qibocal.fitting.classifier import run
 from qibocal.protocols.characterization.classification import (
     ClassificationType,
     SingleShotClassificationData,
     SingleShotClassificationParameters,
     SingleShotClassificationResults,
 )
@@ -44,15 +45,15 @@
     )
     """List of models to classify the qubit states"""
 
 
 def _acquisition(
     params: QutritClassificationParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> QutritClassificationData:
     """
     This Routine prepares the qubits in 0,1 and 2 states and measures their
     respective I, Q values.
 
     Args:
         nshots (int): number of times the pulse sequence will be repeated.
@@ -66,15 +67,15 @@
         If not given, the dumping folder will be the report one.
         relaxation_time (float): Relaxation time.
     """
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     states_sequences = [PulseSequence() for _ in range(3)]
     ro_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         rx_pulse = platform.create_RX_pulse(qubit, start=0)
         rx12_pulse = platform.create_RX12_pulse(qubit, start=rx_pulse.finish)
         drive_pulses = [rx_pulse, rx12_pulse]
         ro_pulses[qubit] = []
         for i, sequence in enumerate(states_sequences):
             sequence.add(*drive_pulses[:i])
             start = drive_pulses[i - 1].finish if i != 0 else 0
@@ -97,15 +98,15 @@
                     nshots=params.nshots,
                     relaxation_time=params.relaxation_time,
                     acquisition_type=AcquisitionType.INTEGRATION,
                 ),
             )
         )
 
-    for qubit in qubits:
+    for qubit in targets:
         for state, state_result in enumerate(states_results):
             result = state_result[ro_pulses[qubit][state].serial]
             data.register_qubit(
                 ClassificationType,
                 (qubit),
                 dict(
                     state=[state] * params.nshots,
@@ -161,15 +162,19 @@
         models=models_dict,
         savedir=data.savedir,
         y_preds=y_test_predict,
         grid_preds=grid_preds_dict,
     )
 
 
-def _plot(data: QutritClassificationData, qubit, fit: SingleShotClassificationResults):
-    figures = plot_results(data, qubit, 3, fit)
+def _plot(
+    data: QutritClassificationData,
+    target: QubitId,
+    fit: SingleShotClassificationResults,
+):
+    figures = plot_results(data, target, 3, fit)
     fitting_report = ""
     return figures, fitting_report
 
 
 qutrit_classification = Routine(_acquisition, _fit, _plot)
 """Qutrit classification Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/amplitude.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/amplitude.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,45 +8,31 @@
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Routine
 from qibocal.config import log
 
 from ..utils import chi2_reduced
 from . import utils
+from .amplitude_signal import RabiAmplitudeVoltParameters, RabiAmplitudeVoltResults
 
 
 @dataclass
-class RabiAmplitudeParameters(Parameters):
+class RabiAmplitudeParameters(RabiAmplitudeVoltParameters):
     """RabiAmplitude runcard inputs."""
 
-    min_amp_factor: float
-    """Minimum amplitude multiplicative factor."""
-    max_amp_factor: float
-    """Maximum amplitude multiplicative factor."""
-    step_amp_factor: float
-    """Step amplitude multiplicative factor."""
-    pulse_length: Optional[float]
-    """RX pulse duration [ns]."""
-
 
 @dataclass
-class RabiAmplitudeResults(Results):
+class RabiAmplitudeResults(RabiAmplitudeVoltResults):
     """RabiAmplitude outputs."""
 
-    amplitude: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive amplitude for each qubit."""
-    length: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive pulse duration. Same for all qubits."""
-    fitted_parameters: dict[QubitId, dict[str, float]]
-    """Raw fitted parameters."""
     chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
 
 
 RabiAmpType = np.dtype(
     [("amp", np.float64), ("prob", np.float64), ("error", np.float64)]
 )
 """Custom dtype for rabi amplitude."""
@@ -59,28 +45,28 @@
     durations: dict[QubitId, float] = field(default_factory=dict)
     """Pulse durations provided by the user."""
     data: dict[QubitId, npt.NDArray[RabiAmpType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: RabiAmplitudeParameters, platform: Platform, qubits: Qubits
+    params: RabiAmplitudeParameters, platform: Platform, targets: list[QubitId]
 ) -> RabiAmplitudeData:
     r"""
     Data acquisition for Rabi experiment sweeping amplitude.
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse amplitude
     to find the drive pulse amplitude that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
     durations = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         if params.pulse_length is not None:
             qd_pulses[qubit].duration = params.pulse_length
 
         durations[qubit] = qd_pulses[qubit].duration
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].finish
@@ -94,15 +80,15 @@
         params.min_amp_factor,
         params.max_amp_factor,
         params.step_amp_factor,
     )
     sweeper = Sweeper(
         Parameter.amplitude,
         qd_pulse_amplitude_range,
-        [qd_pulses[qubit] for qubit in qubits],
+        [qd_pulses[qubit] for qubit in targets],
         type=SweeperType.FACTOR,
     )
 
     data = RabiAmplitudeData(durations=durations)
 
     # sweep the parameter
     results = platform.sweep(
@@ -111,15 +97,15 @@
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.DISCRIMINATION,
             averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
-    for qubit in qubits:
+    for qubit in targets:
         prob = results[qubit].probability(state=1)
         data.register_qubit(
             RabiAmpType,
             (qubit),
             dict(
                 amp=qd_pulses[qubit].amplitude * qd_pulse_amplitude_range,
                 prob=prob.tolist(),
@@ -131,14 +117,15 @@
 
 def _fit(data: RabiAmplitudeData) -> RabiAmplitudeResults:
     """Post-processing for RabiAmplitude."""
     qubits = data.qubits
 
     pi_pulse_amplitudes = {}
     fitted_parameters = {}
+    durations = {}
     chi2 = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
 
         x = qubit_data.amp
         y = qubit_data.prob
@@ -164,39 +151,35 @@
                 ),
                 sigma=qubit_data.error,
             )
             perr = np.sqrt(np.diag(perr))
             pi_pulse_parameter = (
                 popt[2] / 2 * utils.period_correction_factor(phase=popt[3])
             )
+            pi_pulse_amplitudes[qubit] = (pi_pulse_parameter, perr[2] / 2)
+            fitted_parameters[qubit] = popt.tolist()
+            durations = {key: (value, 0) for key, value in data.durations.items()}
+            chi2[qubit] = (
+                chi2_reduced(
+                    y,
+                    utils.rabi_amplitude_function(x, *popt),
+                    qubit_data.error,
+                ),
+                np.sqrt(2 / len(y)),
+            )
 
-        except:
-            log.warning("rabi_fit: the fitting was not succesful")
-            pi_pulse_parameter = 0
-            popt = [0] * 4
-            perr = [1] * 4
-
-        pi_pulse_amplitudes[qubit] = (pi_pulse_parameter, perr[2] / 2)
-        fitted_parameters[qubit] = popt.tolist()
-        durations = {key: (value, 0) for key, value in data.durations.items()}
-        chi2[qubit] = (
-            chi2_reduced(
-                y,
-                utils.rabi_amplitude_function(x, *popt),
-                qubit_data.error,
-            ),
-            np.sqrt(2 / len(y)),
-        )
+        except Exception as e:
+            log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
     return RabiAmplitudeResults(pi_pulse_amplitudes, durations, fitted_parameters, chi2)
 
 
-def _plot(data: RabiAmplitudeData, qubit, fit: RabiAmplitudeResults = None):
+def _plot(data: RabiAmplitudeData, target: QubitId, fit: RabiAmplitudeResults = None):
     """Plotting function for RabiAmplitude."""
-    return utils.plot_probabilities(data, qubit, fit)
+    return utils.plot_probabilities(data, target, fit)
 
 
-def _update(results: RabiAmplitudeResults, platform: Platform, qubit: QubitId):
-    update.drive_amplitude(results.amplitude[qubit], platform, qubit)
+def _update(results: RabiAmplitudeResults, platform: Platform, target: QubitId):
+    update.drive_amplitude(results.amplitude[target], platform, target)
 
 
 rabi_amplitude = Routine(_acquisition, _fit, _plot, _update)
 """RabiAmplitude Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/amplitude_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,187 +1,214 @@
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Optional
 
 import numpy as np
+import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Parameters, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.rabi.amplitude import (
-    RabiAmplitudeData,
-    RabiAmplitudeParameters,
-    RabiAmplitudeResults,
+from qibocal.protocols.characterization.rabi.length_signal import (
+    RabiLengthVoltData,
+    RabiLengthVoltResults,
 )
 
+from ..utils import chi2_reduced
 from . import utils
 
 
 @dataclass
-class RabiAmplitudeVoltParameters(RabiAmplitudeParameters):
-    """RabiAmplitude runcard inputs."""
+class RabiLengthParameters(Parameters):
+    """RabiLength runcard inputs."""
+
+    pulse_duration_start: float
+    """Initial pi pulse duration [ns]."""
+    pulse_duration_end: float
+    """Final pi pulse duration [ns]."""
+    pulse_duration_step: float
+    """Step pi pulse duration [ns]."""
+    pulse_amplitude: Optional[float] = None
+    """Pi pulse amplitude. Same for all qubits."""
 
 
 @dataclass
-class RabiAmplitudeVoltResults(RabiAmplitudeResults):
-    """RabiAmplitude outputs."""
+class RabiLengthResults(RabiLengthVoltResults):
+    """RabiLength outputs."""
+
+    chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
 
 
-RabiAmpVoltType = np.dtype(
-    [("amp", np.float64), ("signal", np.float64), ("phase", np.float64)]
+RabiLenType = np.dtype(
+    [("length", np.float64), ("prob", np.float64), ("error", np.float64)]
 )
 """Custom dtype for rabi amplitude."""
 
 
 @dataclass
-class RabiAmplitudeVoltData(RabiAmplitudeData):
-    """RabiAmplitude data acquisition."""
+class RabiLengthData(RabiLengthVoltData):
+    """RabiLength acquisition outputs."""
+
+    data: dict[QubitId, npt.NDArray[RabiLenType]] = field(default_factory=dict)
+    """Raw data acquired."""
 
 
 def _acquisition(
-    params: RabiAmplitudeVoltParameters, platform: Platform, qubits: Qubits
-) -> RabiAmplitudeVoltData:
+    params: RabiLengthParameters, platform: Platform, targets: list[QubitId]
+) -> RabiLengthData:
     r"""
-    Data acquisition for Rabi experiment sweeping amplitude.
-    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse amplitude
-    to find the drive pulse amplitude that creates a rotation of a desired angle.
+    Data acquisition for RabiLength Experiment.
+    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
+    to find the drive pulse length that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
-    durations = {}
-    for qubit in qubits:
-        qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
-        if params.pulse_length is not None:
-            qd_pulses[qubit].duration = params.pulse_length
+    amplitudes = {}
+    for qubit in targets:
+        # TODO: made duration optional for qd pulse?
+        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
+            qubit, start=0, duration=params.pulse_duration_start
+        )
+        if params.pulse_amplitude is not None:
+            qd_pulses[qubit].amplitude = params.pulse_amplitude
+        amplitudes[qubit] = qd_pulses[qubit].amplitude
 
-        durations[qubit] = qd_pulses[qubit].duration
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].finish
         )
         sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
-    # qubit drive pulse amplitude
-    qd_pulse_amplitude_range = np.arange(
-        params.min_amp_factor,
-        params.max_amp_factor,
-        params.step_amp_factor,
+    # qubit drive pulse duration time
+    qd_pulse_duration_range = np.arange(
+        params.pulse_duration_start,
+        params.pulse_duration_end,
+        params.pulse_duration_step,
     )
+
     sweeper = Sweeper(
-        Parameter.amplitude,
-        qd_pulse_amplitude_range,
-        [qd_pulses[qubit] for qubit in qubits],
-        type=SweeperType.FACTOR,
+        Parameter.duration,
+        qd_pulse_duration_range,
+        [qd_pulses[qubit] for qubit in targets],
+        type=SweeperType.ABSOLUTE,
     )
 
-    data = RabiAmplitudeVoltData(durations=durations)
+    data = RabiLengthData(amplitudes=amplitudes)
 
-    # sweep the parameter
+    # execute the sweep
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
+            acquisition_type=AcquisitionType.DISCRIMINATION,
+            averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
-    for qubit in qubits:
-        result = results[ro_pulses[qubit].serial]
+
+    for qubit in targets:
+        prob = results[qubit].probability(state=1)
         data.register_qubit(
-            RabiAmpVoltType,
+            RabiLenType,
             (qubit),
             dict(
-                amp=qd_pulses[qubit].amplitude * qd_pulse_amplitude_range,
-                signal=result.magnitude,
-                phase=result.phase,
+                length=qd_pulse_duration_range,
+                prob=prob,
+                error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
             ),
         )
     return data
 
 
-def _fit(data: RabiAmplitudeVoltData) -> RabiAmplitudeVoltResults:
-    """Post-processing for RabiAmplitude."""
-    qubits = data.qubits
+def _fit(data: RabiLengthData) -> RabiLengthResults:
+    """Post-processing for RabiLength experiment."""
 
-    pi_pulse_amplitudes = {}
+    qubits = data.qubits
     fitted_parameters = {}
+    durations = {}
+    amplitudes = {}
+    chi2 = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
+        raw_x = qubit_data.length
+        min_x = np.min(raw_x)
+        max_x = np.max(raw_x)
+        y = qubit_data.prob
 
-        rabi_parameter = qubit_data.amp
-        voltages = qubit_data.signal
-
-        y_min = np.min(voltages)
-        y_max = np.max(voltages)
-        x_min = np.min(rabi_parameter)
-        x_max = np.max(rabi_parameter)
-        x = (rabi_parameter - x_min) / (x_max - x_min)
-        y = (voltages - y_min) / (y_max - y_min)
-
+        x = (raw_x - min_x) / (max_x - min_x)
         # Guessing period using fourier transform
         ft = np.fft.rfft(y)
         mags = abs(ft)
-        local_maxima = find_peaks(mags, threshold=10)[0]
+        local_maxima = find_peaks(mags, threshold=1)[0]
         index = local_maxima[0] if len(local_maxima) > 0 else None
         # 0.5 hardcoded guess for less than one oscillation
         f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-        pguess = [0.5, 1, 1 / f, 0]
+        pguess = [0.5, 0.5, 1 / f, 0, 0]
+
         try:
-            popt, _ = curve_fit(
-                utils.rabi_amplitude_function,
+            popt, perr = curve_fit(
+                utils.rabi_length_function,
                 x,
                 y,
                 p0=pguess,
                 maxfev=100000,
                 bounds=(
-                    [0, 0, 0, -np.pi],
-                    [1, 1, np.inf, np.pi],
+                    [0, 0, 0, -np.pi, 0],
+                    [1, 1, np.inf, np.pi, np.inf],
                 ),
+                sigma=qubit_data.error,
             )
-            translated_popt = [  # Change it according to fit function changes
-                y_min + (y_max - y_min) * popt[0],
-                (y_max - y_min) * popt[1],
-                popt[2] * (x_max - x_min),
-                popt[3] - 2 * np.pi * x_min / (x_max - x_min) / popt[2],
+
+            translated_popt = [
+                popt[0],
+                popt[1] * np.exp(min_x * popt[4] / (max_x - min_x)),
+                popt[2] * (max_x - min_x),
+                popt[3] - 2 * np.pi * min_x / popt[2] / (max_x - min_x),
+                popt[4] / (max_x - min_x),
             ]
+
+            perr = np.sqrt(np.diag(perr))
             pi_pulse_parameter = (
                 translated_popt[2]
                 / 2
                 * utils.period_correction_factor(phase=translated_popt[3])
             )
+            durations[qubit] = (pi_pulse_parameter, perr[2] * (max_x - min_x) / 2)
+            fitted_parameters[qubit] = translated_popt
+            amplitudes = {key: (value, 0) for key, value in data.amplitudes.items()}
+            chi2[qubit] = (
+                chi2_reduced(
+                    y,
+                    utils.rabi_length_function(raw_x, *translated_popt),
+                    qubit_data.error,
+                ),
+                np.sqrt(2 / len(y)),
+            )
+        except Exception as e:
+            log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
 
-        except:
-            log.warning("rabi_fit: the fitting was not succesful")
-            pi_pulse_parameter = 0
-            fitted_parameters = [0] * 4
-
-        pi_pulse_amplitudes[qubit] = pi_pulse_parameter
-        fitted_parameters[qubit] = translated_popt
-
-    return RabiAmplitudeVoltResults(
-        pi_pulse_amplitudes, data.durations, fitted_parameters
-    )
+    return RabiLengthResults(durations, amplitudes, fitted_parameters, chi2)
 
 
-def _plot(data: RabiAmplitudeVoltData, qubit, fit: RabiAmplitudeVoltResults = None):
-    """Plotting function for RabiAmplitude."""
-    return utils.plot(data, qubit, fit)
+def _update(results: RabiLengthResults, platform: Platform, target: QubitId):
+    update.drive_duration(results.length[target], platform, target)
 
 
-def _update(results: RabiAmplitudeVoltResults, platform: Platform, qubit: QubitId):
-    update.drive_amplitude(results.amplitude[qubit], platform, qubit)
+def _plot(data: RabiLengthData, fit: RabiLengthResults, target: QubitId):
+    """Plotting function for RabiLength experiment."""
+    return utils.plot_probabilities(data, target, fit)
 
 
-rabi_amplitude_signal = Routine(_acquisition, _fit, _plot, _update)
-"""RabiAmplitude Routine object."""
+rabi_length = Routine(_acquisition, _fit, _plot, _update)
+"""RabiLength Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/ef.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/ef.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
 from . import amplitude_signal, utils
 
 
 @dataclass
 class RabiAmplitudeEFParameters(amplitude_signal.RabiAmplitudeVoltParameters):
     """RabiAmplitudeEF runcard inputs."""
@@ -25,15 +25,15 @@
 
 @dataclass
 class RabiAmplitudeEFData(amplitude_signal.RabiAmplitudeVoltData):
     """RabiAmplitude data acquisition."""
 
 
 def _acquisition(
-    params: RabiAmplitudeEFParameters, platform: Platform, qubits: Qubits
+    params: RabiAmplitudeEFParameters, platform: Platform, targets: list[QubitId]
 ) -> RabiAmplitudeEFData:
     r"""
     Data acquisition for Rabi EF experiment sweeping amplitude.
 
     The rabi protocol is performed after exciting the qubit to state 1.
     This protocol allows to compute the amplitude of the RX12 pulse to excite
     the qubit to state 2 starting from state 1.
@@ -42,15 +42,15 @@
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
     rx_pulses = {}
     durations = {}
-    for qubit in qubits:
+    for qubit in targets:
         rx_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         qd_pulses[qubit] = platform.create_RX_pulse(
             qubit, start=rx_pulses[qubit].finish
         )
         if params.pulse_length is not None:
             qd_pulses[qubit].duration = params.pulse_length
 
@@ -68,15 +68,15 @@
         params.min_amp_factor,
         params.max_amp_factor,
         params.step_amp_factor,
     )
     sweeper = Sweeper(
         Parameter.amplitude,
         qd_pulse_amplitude_range,
-        [qd_pulses[qubit] for qubit in qubits],
+        [qd_pulses[qubit] for qubit in targets],
         type=SweeperType.FACTOR,
     )
 
     data = RabiAmplitudeEFData(durations=durations)
 
     # sweep the parameter
     results = platform.sweep(
@@ -85,36 +85,38 @@
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
             averaging_mode=AveragingMode.CYCLIC,
         ),
         sweeper,
     )
-    for qubit in qubits:
+    for qubit in targets:
         result = results[ro_pulses[qubit].serial]
         data.register_qubit(
             amplitude_signal.RabiAmpVoltType,
             (qubit),
             dict(
                 amp=qd_pulses[qubit].amplitude * qd_pulse_amplitude_range,
                 signal=result.magnitude,
                 phase=result.phase,
             ),
         )
     return data
 
 
-def _plot(data: RabiAmplitudeEFData, qubit, fit: RabiAmplitudeEFResults = None):
+def _plot(
+    data: RabiAmplitudeEFData, target: QubitId, fit: RabiAmplitudeEFResults = None
+):
     """Plotting function for RabiAmplitude."""
-    figures, report = utils.plot(data, qubit, fit)
+    figures, report = utils.plot(data, target, fit)
     if report is not None:
         report = report.replace("Pi pulse", "Pi pulse 12")
     return figures, report
 
 
-def _update(results: RabiAmplitudeEFResults, platform: Platform, qubit: QubitId):
+def _update(results: RabiAmplitudeEFResults, platform: Platform, target: QubitId):
     """Update RX2 amplitude_signal"""
-    update.drive_12_amplitude(results.amplitude[qubit], platform, qubit)
+    update.drive_12_amplitude(results.amplitude[target], platform, target)
 
 
 rabi_amplitude_ef = Routine(_acquisition, amplitude_signal._fit, _plot, _update)
 """RabiAmplitudeEF Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_signal.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,79 +8,77 @@
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
 
-from ..utils import chi2_reduced
 from . import utils
 
 
 @dataclass
-class RabiLengthParameters(Parameters):
-    """RabiLength runcard inputs."""
+class RabiLengthVoltParameters(Parameters):
+    """RabiLengthVolt runcard inputs."""
 
     pulse_duration_start: float
     """Initial pi pulse duration [ns]."""
     pulse_duration_end: float
     """Final pi pulse duration [ns]."""
     pulse_duration_step: float
     """Step pi pulse duration [ns]."""
     pulse_amplitude: Optional[float] = None
     """Pi pulse amplitude. Same for all qubits."""
 
 
 @dataclass
-class RabiLengthResults(Results):
-    """RabiLength outputs."""
+class RabiLengthVoltResults(Results):
+    """RabiLengthVolt outputs."""
 
     length: dict[QubitId, tuple[int, Optional[float]]]
     """Pi pulse duration for each qubit."""
     amplitude: dict[QubitId, tuple[float, Optional[float]]]
     """Pi pulse amplitude. Same for all qubits."""
     fitted_parameters: dict[QubitId, dict[str, float]]
     """Raw fitting output."""
-    chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
 
 
-RabiLenType = np.dtype(
-    [("length", np.float64), ("prob", np.float64), ("error", np.float64)]
+RabiLenVoltType = np.dtype(
+    [("length", np.float64), ("signal", np.float64), ("phase", np.float64)]
 )
 """Custom dtype for rabi amplitude."""
 
 
 @dataclass
-class RabiLengthData(Data):
+class RabiLengthVoltData(Data):
     """RabiLength acquisition outputs."""
 
     amplitudes: dict[QubitId, float] = field(default_factory=dict)
     """Pulse durations provided by the user."""
-    data: dict[QubitId, npt.NDArray[RabiLenType]] = field(default_factory=dict)
+    data: dict[QubitId, npt.NDArray[RabiLenVoltType]] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: RabiLengthParameters, platform: Platform, qubits: Qubits
-) -> RabiLengthData:
+    params: RabiLengthVoltParameters, platform: Platform, targets: list[QubitId]
+) -> RabiLengthVoltData:
     r"""
     Data acquisition for RabiLength Experiment.
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
     to find the drive pulse length that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
     amplitudes = {}
-    for qubit in qubits:
+    for qubit in targets:
         # TODO: made duration optional for qd pulse?
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(
             qubit, start=0, duration=params.pulse_duration_start
         )
         if params.pulse_amplitude is not None:
             qd_pulses[qubit].amplitude = params.pulse_amplitude
         amplitudes[qubit] = qd_pulses[qubit].amplitude
@@ -98,106 +96,111 @@
         params.pulse_duration_end,
         params.pulse_duration_step,
     )
 
     sweeper = Sweeper(
         Parameter.duration,
         qd_pulse_duration_range,
-        [qd_pulses[qubit] for qubit in qubits],
+        [qd_pulses[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
-    data = RabiLengthData(amplitudes=amplitudes)
+    data = RabiLengthVoltData(amplitudes=amplitudes)
 
     # execute the sweep
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.DISCRIMINATION,
-            averaging_mode=AveragingMode.SINGLESHOT,
+            acquisition_type=AcquisitionType.INTEGRATION,
+            averaging_mode=AveragingMode.CYCLIC,
         ),
         sweeper,
     )
 
-    for qubit in qubits:
-        prob = results[qubit].probability(state=1)
+    for qubit in targets:
+        result = results[ro_pulses[qubit].serial]
         data.register_qubit(
-            RabiLenType,
+            RabiLenVoltType,
             (qubit),
             dict(
                 length=qd_pulse_duration_range,
-                prob=prob,
-                error=np.sqrt(prob * (1 - prob) / params.nshots).tolist(),
+                signal=result.magnitude,
+                phase=result.phase,
             ),
         )
     return data
 
 
-def _fit(data: RabiLengthData) -> RabiLengthResults:
+def _fit(data: RabiLengthVoltData) -> RabiLengthVoltResults:
     """Post-processing for RabiLength experiment."""
 
     qubits = data.qubits
     fitted_parameters = {}
     durations = {}
-    chi2 = {}
 
     for qubit in qubits:
         qubit_data = data[qubit]
-        x = qubit_data.length
-        y = qubit_data.prob
+        rabi_parameter = qubit_data.length
+        voltages = qubit_data.signal
+
+        y_min = np.min(voltages)
+        y_max = np.max(voltages)
+        x_min = np.min(rabi_parameter)
+        x_max = np.max(rabi_parameter)
+        x = (rabi_parameter - x_min) / (x_max - x_min)
+        y = (voltages - y_min) / (y_max - y_min) - 1 / 2
 
         # Guessing period using fourier transform
         ft = np.fft.rfft(y)
         mags = abs(ft)
         local_maxima = find_peaks(mags, threshold=1)[0]
         index = local_maxima[0] if len(local_maxima) > 0 else None
         # 0.5 hardcoded guess for less than one oscillation
         f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-        pguess = [0.5, 0.5, np.max(x) / f, 0, 0]
+
+        pguess = [0, np.sign(y[0]) * 0.5, 1 / f, 0, 0]
         try:
-            popt, perr = curve_fit(
+            popt, _ = curve_fit(
                 utils.rabi_length_function,
                 x,
                 y,
                 p0=pguess,
                 maxfev=100000,
                 bounds=(
-                    [0, 0, 0, -np.pi, 0],
+                    [0, -1, 0, -np.pi, 0],
                     [1, 1, np.inf, np.pi, np.inf],
                 ),
-                sigma=qubit_data.error,
             )
-            perr = np.sqrt(np.diag(perr))
+            translated_popt = [  # change it according to the fit function
+                (y_max - y_min) * (popt[0] + 1 / 2) + y_min,
+                (y_max - y_min) * popt[1] * np.exp(x_min * popt[4] / (x_max - x_min)),
+                popt[2] * (x_max - x_min),
+                popt[3] - 2 * np.pi * x_min / popt[2] / (x_max - x_min),
+                popt[4] / (x_max - x_min),
+            ]
             pi_pulse_parameter = (
-                popt[2] / 2 * utils.period_correction_factor(phase=popt[3])
+                translated_popt[2]
+                / 2
+                * utils.period_correction_factor(phase=translated_popt[3])
             )
-        except:
-            log.warning("rabi_fit: the fitting was not succesful")
-            pi_pulse_parameter = 0
-            popt = [0] * 4 + [1]
-        durations[qubit] = (pi_pulse_parameter, perr[2] / 2)
-        fitted_parameters[qubit] = popt.tolist()
-        amplitudes = {key: (value, 0) for key, value in data.amplitudes.items()}
-        chi2[qubit] = (
-            chi2_reduced(
-                y,
-                utils.rabi_length_function(x, *popt),
-                qubit_data.error,
-            ),
-            np.sqrt(2 / len(y)),
-        )
-    return RabiLengthResults(durations, amplitudes, fitted_parameters, chi2)
+            durations[qubit] = pi_pulse_parameter
+            fitted_parameters[qubit] = translated_popt
+
+        except Exception as e:
+            log.warning(f"Rabi fit failed for qubit {qubit} due to {e}.")
+
+    return RabiLengthVoltResults(durations, data.amplitudes, fitted_parameters)
 
 
-def _update(results: RabiLengthResults, platform: Platform, qubit: QubitId):
-    update.drive_duration(results.length[qubit], platform, qubit)
+def _update(results: RabiLengthVoltResults, platform: Platform, target: QubitId):
+    update.drive_duration(results.length[target], platform, target)
 
 
-def _plot(data: RabiLengthData, fit: RabiLengthResults, qubit):
+def _plot(data: RabiLengthVoltData, fit: RabiLengthVoltResults, target: QubitId):
     """Plotting function for RabiLength experiment."""
-    return utils.plot_probabilities(data, qubit, fit)
+    return utils.plot(data, target, fit)
 
 
-rabi_length = Routine(_acquisition, _fit, _plot, _update)
+rabi_length_signal = Routine(_acquisition, _fit, _plot, _update)
 """RabiLength Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length_sequences.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/length_sequences.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import numpy as np
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
+from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Qubits, Routine
+from qibocal.auto.operation import Routine
 
 from .length_signal import (
     RabiLengthVoltData,
     RabiLengthVoltParameters,
     RabiLenVoltType,
     _fit,
     _plot,
     _update,
 )
 
 
 def _acquisition(
-    params: RabiLengthVoltParameters, platform: Platform, qubits: Qubits
+    params: RabiLengthVoltParameters, platform: Platform, targets: list[QubitId]
 ) -> RabiLengthVoltData:
     r"""
     Data acquisition for RabiLength Experiment.
     In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
     to find the drive pulse length that creates a rotation of a desired angle.
     """
 
     # create a sequence of pulses for the experiment
     sequence = PulseSequence()
     qd_pulses = {}
     ro_pulses = {}
     amplitudes = {}
-    for qubit in qubits:
+    for qubit in targets:
         # TODO: made duration optional for qd pulse?
         qd_pulses[qubit] = platform.create_qubit_drive_pulse(qubit, start=0, duration=4)
         if params.pulse_amplitude is not None:
             qd_pulses[qubit].amplitude = params.pulse_amplitude
         amplitudes[qubit] = qd_pulses[qubit].amplitude
 
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
@@ -50,30 +51,30 @@
         params.pulse_duration_step,
     )
 
     data = RabiLengthVoltData(amplitudes=amplitudes)
 
     # sweep the parameter
     for duration in qd_pulse_duration_range:
-        for qubit in qubits:
+        for qubit in targets:
             qd_pulses[qubit].duration = duration
             ro_pulses[qubit].start = qd_pulses[qubit].finish
 
         # execute the pulse sequence
         results = platform.execute_pulse_sequence(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
                 relaxation_time=params.relaxation_time,
                 acquisition_type=AcquisitionType.INTEGRATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
         )
 
-        for qubit in qubits:
+        for qubit in targets:
             result = results[ro_pulses[qubit].serial]
             data.register_qubit(
                 RabiLenVoltType,
                 (qubit),
                 dict(
                     length=np.array([duration]),
                     signal=np.array([result.magnitude]),
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/rabi/length_signal.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/rabi/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,190 +1,217 @@
-from dataclasses import dataclass
-
 import numpy as np
-from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
-from qibolab.platform import Platform
-from qibolab.pulses import PulseSequence
-from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
-from scipy.optimize import curve_fit
-from scipy.signal import find_peaks
-
-from qibocal import update
-from qibocal.auto.operation import Qubits, Routine
-from qibocal.config import log
-from qibocal.protocols.characterization.rabi.length import (
-    RabiLengthData,
-    RabiLengthParameters,
-    RabiLengthResults,
-)
-
-from . import utils
-
-
-@dataclass
-class RabiLengthVoltParameters(RabiLengthParameters):
-    """RabiLength runcard inputs."""
-
-
-@dataclass
-class RabiLengthVoltResults(RabiLengthResults):
-    """RabiLength outputs."""
-
-
-RabiLenVoltType = np.dtype(
-    [("length", np.float64), ("signal", np.float64), ("phase", np.float64)]
-)
-"""Custom dtype for rabi amplitude."""
-
-
-@dataclass
-class RabiLengthVoltData(RabiLengthData):
-    """RabiLength acquisition outputs."""
-
-
-def _acquisition(
-    params: RabiLengthVoltParameters, platform: Platform, qubits: Qubits
-) -> RabiLengthVoltData:
-    r"""
-    Data acquisition for RabiLength Experiment.
-    In the Rabi experiment we apply a pulse at the frequency of the qubit and scan the drive pulse length
-    to find the drive pulse length that creates a rotation of a desired angle.
-    """
-
-    # create a sequence of pulses for the experiment
-    sequence = PulseSequence()
-    qd_pulses = {}
-    ro_pulses = {}
-    amplitudes = {}
-    for qubit in qubits:
-        # TODO: made duration optional for qd pulse?
-        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
-            qubit, start=0, duration=params.pulse_duration_start
-        )
-        if params.pulse_amplitude is not None:
-            qd_pulses[qubit].amplitude = params.pulse_amplitude
-        amplitudes[qubit] = qd_pulses[qubit].amplitude
-
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-            qubit, start=qd_pulses[qubit].finish
-        )
-        sequence.add(qd_pulses[qubit])
-        sequence.add(ro_pulses[qubit])
-
-    # define the parameter to sweep and its range:
-    # qubit drive pulse duration time
-    qd_pulse_duration_range = np.arange(
-        params.pulse_duration_start,
-        params.pulse_duration_end,
-        params.pulse_duration_step,
+import plotly.graph_objects as go
+from plotly.subplots import make_subplots
+
+from ..utils import COLORBAND, COLORBAND_LINE, table_dict, table_html
+
+
+def rabi_amplitude_function(x, offset, amplitude, period, phase):
+    """
+    Fit function of Rabi amplitude signal experiment.
+
+    Args:
+        x: Input data.
+    """
+    return offset + amplitude * np.cos(2 * np.pi * x / period + phase)
+
+
+def rabi_length_function(x, offset, amplitude, period, phase, t2_inv):
+    """
+    Fit function of Rabi length signal experiment.
+
+    Args:
+        x: Input data.
+    """
+    return offset + amplitude * np.cos(2 * np.pi * x / period + phase) * np.exp(
+        -x * t2_inv
     )
 
-    sweeper = Sweeper(
-        Parameter.duration,
-        qd_pulse_duration_range,
-        [qd_pulses[qubit] for qubit in qubits],
-        type=SweeperType.ABSOLUTE,
+
+def plot(data, qubit, fit):
+    quantity, title, fitting = extract_rabi(data)
+    figures = []
+    fitting_report = ""
+
+    fig = make_subplots(
+        rows=1,
+        cols=2,
+        horizontal_spacing=0.1,
+        vertical_spacing=0.1,
+        subplot_titles=(
+            "Signal [a.u.]",
+            "phase [rad]",
+        ),
     )
 
-    data = RabiLengthVoltData(amplitudes=amplitudes)
+    qubit_data = data[qubit]
 
-    # execute the sweep
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
+    rabi_parameters = getattr(qubit_data, quantity)
+    fig.add_trace(
+        go.Scatter(
+            x=rabi_parameters,
+            y=qubit_data.signal,
+            opacity=1,
+            name="Signal",
+            showlegend=True,
+            legendgroup="Signal",
         ),
-        sweeper,
+        row=1,
+        col=1,
+    )
+    fig.add_trace(
+        go.Scatter(
+            x=rabi_parameters,
+            y=qubit_data.phase,
+            opacity=1,
+            name="Phase",
+            showlegend=True,
+            legendgroup="Phase",
+        ),
+        row=1,
+        col=2,
     )
 
-    for qubit in qubits:
-        result = results[ro_pulses[qubit].serial]
-        data.register_qubit(
-            RabiLenVoltType,
-            (qubit),
-            dict(
-                length=qd_pulse_duration_range,
-                signal=result.magnitude,
-                phase=result.phase,
+    if fit is not None:
+        rabi_parameter_range = np.linspace(
+            min(rabi_parameters),
+            max(rabi_parameters),
+            2 * len(rabi_parameters),
+        )
+        params = fit.fitted_parameters[qubit]
+        fig.add_trace(
+            go.Scatter(
+                x=rabi_parameter_range,
+                y=fitting(rabi_parameter_range, *params),
+                name="Fit",
+                line=go.scatter.Line(dash="dot"),
+                marker_color="rgb(255, 130, 67)",
             ),
+            row=1,
+            col=1,
         )
-    return data
 
+        fitting_report = table_html(
+            table_dict(
+                qubit,
+                ["Pi pulse amplitude [a.u.]", "Pi pulse length [ns]"],
+                [np.round(fit.amplitude[qubit], 3), np.round(fit.length[qubit], 3)],
+            )
+        )
 
-def _fit(data: RabiLengthVoltData) -> RabiLengthVoltResults:
-    """Post-processing for RabiLength experiment."""
+        fig.update_layout(
+            showlegend=True,
+            xaxis_title=title,
+            yaxis_title="Signal [a.u.]",
+            xaxis2_title=title,
+            yaxis2_title="Phase [rad]",
+        )
 
-    qubits = data.qubits
-    fitted_parameters = {}
-    durations = {}
-
-    for qubit in qubits:
-        qubit_data = data[qubit]
-        rabi_parameter = qubit_data.length
-        voltages = qubit_data.signal
-
-        y_min = np.min(voltages)
-        y_max = np.max(voltages)
-        x_min = np.min(rabi_parameter)
-        x_max = np.max(rabi_parameter)
-        x = (rabi_parameter - x_min) / (x_max - x_min)
-        y = (voltages - y_min) / (y_max - y_min) - 1 / 2
-
-        # Guessing period using fourier transform
-        ft = np.fft.rfft(y)
-        mags = abs(ft)
-        local_maxima = find_peaks(mags, threshold=1)[0]
-        index = local_maxima[0] if len(local_maxima) > 0 else None
-        # 0.5 hardcoded guess for less than one oscillation
-        f = x[index] / (x[1] - x[0]) if index is not None else 0.5
-
-        pguess = [0, np.sign(y[0]) * 0.5, 1 / f, 0, 0]
-        try:
-            popt, _ = curve_fit(
-                utils.rabi_length_function,
-                x,
-                y,
-                p0=pguess,
-                maxfev=100000,
-                bounds=(
-                    [0, -1, 0, -np.pi, 0],
-                    [1, 1, np.inf, np.pi, np.inf],
-                ),
-            )
-            translated_popt = [  # change it according to the fit function
-                (y_max - y_min) * (popt[0] + 1 / 2) + y_min,
-                (y_max - y_min) * popt[1] * np.exp(x_min * popt[4] / (x_max - x_min)),
-                popt[2] * (x_max - x_min),
-                popt[3] - 2 * np.pi * x_min / popt[2] / (x_max - x_min),
-                popt[4] / (x_max - x_min),
-            ]
-            pi_pulse_parameter = (
-                translated_popt[2]
-                / 2
-                * utils.period_correction_factor(phase=translated_popt[3])
+    figures.append(fig)
+
+    return figures, fitting_report
+
+
+def plot_probabilities(data, qubit, fit):
+    quantity, title, fitting = extract_rabi(data)
+    figures = []
+    fitting_report = ""
+
+    qubit_data = data[qubit]
+    probs = qubit_data.prob
+    error_bars = qubit_data.error
+
+    rabi_parameters = getattr(qubit_data, quantity)
+    fig = go.Figure(
+        [
+            go.Scatter(
+                x=rabi_parameters,
+                y=qubit_data.prob,
+                opacity=1,
+                name="Probability",
+                showlegend=True,
+                legendgroup="Probability",
+                mode="lines",
+            ),
+            go.Scatter(
+                x=np.concatenate((rabi_parameters, rabi_parameters[::-1])),
+                y=np.concatenate((probs + error_bars, (probs - error_bars)[::-1])),
+                fill="toself",
+                fillcolor=COLORBAND,
+                line=dict(color=COLORBAND_LINE),
+                showlegend=True,
+                name="Errors",
+            ),
+        ]
+    )
+
+    if fit is not None:
+        rabi_parameter_range = np.linspace(
+            min(rabi_parameters),
+            max(rabi_parameters),
+            2 * len(rabi_parameters),
+        )
+        params = fit.fitted_parameters[qubit]
+        fig.add_trace(
+            go.Scatter(
+                x=rabi_parameter_range,
+                y=fitting(rabi_parameter_range, *params),
+                name="Fit",
+                line=go.scatter.Line(dash="dot"),
+                marker_color="rgb(255, 130, 67)",
+            ),
+        )
+
+        fitting_report = table_html(
+            table_dict(
+                qubit,
+                ["Pi pulse amplitude [a.u.]", "Pi pulse length [ns]", "chi2 reduced"],
+                [fit.amplitude[qubit], fit.length[qubit], fit.chi2[qubit]],
+                display_error=True,
             )
+        )
 
-        except:
-            log.warning("rabi_fit: the fitting was not succesful")
-            pi_pulse_parameter = 0
-            translated_popt = [0, 0, 1, 0, 0]
-        durations[qubit] = pi_pulse_parameter
-        fitted_parameters[qubit] = translated_popt
+        fig.update_layout(
+            showlegend=True,
+            xaxis_title=title,
+            yaxis_title="Excited state probability",
+        )
+
+    figures.append(fig)
+
+    return figures, fitting_report
 
-    return RabiLengthVoltResults(durations, data.amplitudes, fitted_parameters)
+
+def extract_rabi(data):
+    """
+    Extract Rabi fit info.
+    """
+    if "RabiAmplitude" in data.__class__.__name__:
+        return "amp", "Amplitude [dimensionless]", rabi_amplitude_function
+    if "RabiLength" in data.__class__.__name__:
+        return "length", "Time [ns]", rabi_length_function
+    raise RuntimeError("Data has to be a data structure of the Rabi routines.")
 
 
-def _update(results: RabiLengthVoltResults, platform: Platform, qubit: QubitId):
-    update.drive_duration(results.length[qubit], platform, qubit)
+def period_correction_factor(phase: float):
+    r"""Correct period by taking phase into account.
 
+    https://github.com/qiboteam/qibocal/issues/656
 
-def _plot(data: RabiLengthVoltData, fit: RabiLengthVoltResults, qubit):
-    """Plotting function for RabiLength experiment."""
-    return utils.plot(data, qubit, fit)
+    We want to find the first maximum or minimum which will
+    correspond to an exchange of population between 0 and 1.
+    To find it we need to solve the following equation
+    :math:`\cos(2 \pi x / T + \phi) = \pm 1` which will give us
+    the following solution
 
+    .. math::
+
+        x = ( k - \phi / \pi) T / 2
+
+
+    for integer :math:`k`, which is chosen such that we get the smallest
+    multiplicative correction compared to :math:`T/2`.
+
+    """
 
-rabi_length_signal = Routine(_acquisition, _fit, _plot, _update)
-"""RabiLength Routine object."""
+    x = phase / np.pi
+    return np.round(1 + x) - x
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/ramsey.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/ramsey/ramsey.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,226 +5,156 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
-from scipy.optimize import curve_fit
-from scipy.signal import find_peaks
 
-from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
+from qibocal.config import log
 
-from .utils import GHZ_TO_HZ, chi2_reduced, table_dict, table_html
+from ..utils import GHZ_TO_HZ, chi2_reduced, table_dict, table_html
+from .ramsey_signal import (
+    RamseySignalData,
+    RamseySignalParameters,
+    RamseySignalResults,
+    _update,
+)
+from .utils import fitting, ramsey_fit, ramsey_sequence
 
-POPT_EXCEPTION = [0, 0, 0, 0, 0]
-"""Fit parameters output to handle exceptions"""
-PERR_EXCEPTION = [1] * 5
-"""Fit errors to handle exceptions; their choice has no physical meaning
-and is meant to avoid breaking the code."""
 COLORBAND = "rgba(0,100,80,0.2)"
 COLORBAND_LINE = "rgba(255,255,255,0)"
 
 
 @dataclass
-class RamseyParameters(Parameters):
+class RamseyParameters(RamseySignalParameters):
     """Ramsey runcard inputs."""
 
-    delay_between_pulses_start: int
-    """Initial delay between RX(pi/2) pulses in ns."""
-    delay_between_pulses_end: int
-    """Final delay between RX(pi/2) pulses in ns."""
-    delay_between_pulses_step: int
-    """Step delay between RX(pi/2) pulses in ns."""
-    n_osc: Optional[int] = 0
-    """Number of oscillations to induce detuning (optional).
-        If 0 standard Ramsey experiment is performed."""
-    unrolling: bool = False
-    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
-    Defaults to ``False``."""
-
 
 @dataclass
-class RamseyResults(Results):
+class RamseyResults(RamseySignalResults):
     """Ramsey outputs."""
 
-    frequency: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive frequency [GHz] for each qubit."""
-    t2: dict[QubitId, tuple[float, Optional[float]]]
-    """T2 for each qubit [ns]."""
-    delta_phys: dict[QubitId, tuple[float, Optional[float]]]
-    """Drive frequency [Hz] correction for each qubit."""
-    fitted_parameters: dict[QubitId, list[float]]
-    """Raw fitting output."""
     chi2: dict[QubitId, tuple[float, Optional[float]]]
     """Chi squared estimate mean value and error. """
 
 
 RamseyType = np.dtype(
     [("wait", np.float64), ("prob", np.float64), ("errors", np.float64)]
 )
 """Custom dtype for coherence routines."""
 
 
 @dataclass
-class RamseyData(Data):
+class RamseyData(RamseySignalData):
     """Ramsey acquisition outputs."""
 
-    n_osc: int
-    """Number of oscillations for detuning."""
-    t_max: int
-    """Final delay between RX(pi/2) pulses in ns."""
-    detuning_sign: int
-    """Sign for induced detuning."""
-    qubit_freqs: dict[QubitId, float] = field(default_factory=dict)
-    """Qubit freqs for each qubit."""
-    data: dict[QubitId, npt.NDArray] = field(default_factory=dict)
+    data: dict[QubitId, npt.NDArray[RamseyType]] = field(default_factory=dict)
     """Raw data acquired."""
 
-    @property
-    def waits(self):
-        """
-        Return a list with the waiting times without repetitions.
-        """
-        qubit = next(iter(self.data))
-        return np.unique(self.data[qubit].wait)
-
 
 def _acquisition(
     params: RamseyParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> RamseyData:
-    """Data acquisition for Ramsey Experiment (detuned)."""
-    # create a sequence of pulses for the experiment
-    # RX90 - t - RX90 - MZ
-    # define the parameter to sweep and its range:
+    """Data acquisition for Ramsey Experiment (detuned).
+
+    The protocol consists in applying the following pulse sequence
+    RX90 - wait - RX90 - MZ
+    for different waiting times `wait`.
+    The range of waiting times is defined through the attributes
+    `delay_between_pulses_*` available in `RamseyParameters`. The final range
+    will be constructed using `np.arange`.
+    It is possible to detune the drive frequency using the parameter `detuning` in
+    RamseyParameters which will increment the drive frequency accordingly.
+    Currently when `detuning==0` it will be performed a sweep over the waiting values
+    if `detuning` is not zero, all sequences with different waiting value will be
+    executed sequentially. By providing the option `unrolling=True` in RamseyParameters
+    the sequences will be unrolled when the frequency is detuned.
+    The following protocol will display on the y-axis the probability of finding the ground
+    state, therefore it is advise to execute it only after having performed the single
+    shot classification. Error bars are provided as binomial distribution error.
+    """
+
     waits = np.arange(
         # wait time between RX90 pulses
         params.delay_between_pulses_start,
         params.delay_between_pulses_end,
         params.delay_between_pulses_step,
     )
 
     options = ExecutionParameters(
         nshots=params.nshots,
         relaxation_time=params.relaxation_time,
         acquisition_type=AcquisitionType.DISCRIMINATION,
         averaging_mode=AveragingMode.SINGLESHOT,
     )
 
-    if params.n_osc == 0:
-        ro_pulses = {}
-        RX90_pulses1 = {}
-        RX90_pulses2 = {}
-        freqs = {}
+    sequence = PulseSequence()
+
+    data = RamseyData(
+        detuning=params.detuning,
+        qubit_freqs={
+            qubit: platform.qubits[qubit].native_gates.RX.frequency for qubit in targets
+        },
+    )
+
+    if not params.unrolling:
         sequence = PulseSequence()
-        for qubit in qubits:
-            RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
-            RX90_pulses2[qubit] = platform.create_RX90_pulse(
-                qubit,
-                start=RX90_pulses1[qubit].finish,
+        for qubit in targets:
+            sequence += ramsey_sequence(
+                platform=platform, qubit=qubit, detuning=params.detuning
             )
-            ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-                qubit, start=RX90_pulses2[qubit].finish
-            )
-            freqs[qubit] = qubits[qubit].drive_frequency
-            sequence.add(RX90_pulses1[qubit])
-            sequence.add(RX90_pulses2[qubit])
-            sequence.add(ro_pulses[qubit])
-
-        data = RamseyData(
-            n_osc=params.n_osc,
-            t_max=params.delay_between_pulses_end,
-            detuning_sign=+1,
-            qubit_freqs=freqs,
-        )
 
         sweeper = Sweeper(
             Parameter.start,
             waits,
-            [RX90_pulses2[qubit] for qubit in qubits],
+            [sequence.get_qubit_pulses(qubit).qd_pulses[-1] for qubit in targets],
             type=SweeperType.ABSOLUTE,
         )
 
         # execute the sweep
         results = platform.sweep(
             sequence,
             options,
             sweeper,
         )
-        for qubit in qubits:
+        for qubit in targets:
             probs = results[qubit].probability()
             # The probability errors are the standard errors of the binomial distribution
             errors = [np.sqrt(prob * (1 - prob) / params.nshots) for prob in probs]
             data.register_qubit(
                 RamseyType,
                 (qubit),
                 dict(
                     wait=waits,
                     prob=probs,
                     errors=errors,
                 ),
             )
-    if params.n_osc != 0:
+
+    if params.unrolling:
         sequences, all_ro_pulses = [], []
         for wait in waits:
-            ro_pulses = {}
-            RX90_pulses1 = {}
-            RX90_pulses2 = {}
-            freqs = {}
             sequence = PulseSequence()
-            for qubit in qubits:
-                RX90_pulses1[qubit] = platform.create_RX90_pulse(qubit, start=0)
-                RX90_pulses2[qubit] = platform.create_RX90_pulse(
-                    qubit,
-                    start=RX90_pulses1[qubit].finish,
-                )
-                ro_pulses[qubit] = platform.create_qubit_readout_pulse(
-                    qubit, start=RX90_pulses2[qubit].finish
-                )
-
-                RX90_pulses2[qubit].start = RX90_pulses1[qubit].finish + wait
-                ro_pulses[qubit].start = RX90_pulses2[qubit].finish
-
-                RX90_pulses2[qubit].relative_phase = (
-                    RX90_pulses2[qubit].start
-                    * (-2 * np.pi)
-                    * (params.n_osc)
-                    / params.delay_between_pulses_end
+            for qubit in targets:
+                sequence += ramsey_sequence(
+                    platform=platform, qubit=qubit, wait=wait, detuning=params.detuning
                 )
 
-                freqs[qubit] = qubits[qubit].drive_frequency
-                sequence.add(RX90_pulses1[qubit])
-                sequence.add(RX90_pulses2[qubit])
-                sequence.add(ro_pulses[qubit])
-
             sequences.append(sequence)
-            all_ro_pulses.append(ro_pulses)
-
-        data = RamseyData(
-            n_osc=params.n_osc,
-            t_max=params.delay_between_pulses_end,
-            detuning_sign=+1,
-            qubit_freqs=freqs,
-        )
+            all_ro_pulses.append(sequence.ro_pulses)
 
-        if params.unrolling:
-            results = platform.execute_pulse_sequences(sequences, options)
+        results = platform.execute_pulse_sequences(sequences, options)
 
-        elif not params.unrolling:
-            results = [
-                platform.execute_pulse_sequence(sequence, options)
-                for sequence in sequences
-            ]
-
-        # We dont need ig as everty serial is different
+        # We dont need ig as every serial is different
         for ig, (wait, ro_pulses) in enumerate(zip(waits, all_ro_pulses)):
-            for qubit in qubits:
+            for qubit in targets:
                 serial = ro_pulses[qubit].serial
                 if params.unrolling:
                     result = results[serial][0]
                 else:
                     result = results[ig][serial]
                 prob = result.probability()
                 error = np.sqrt(prob * (1 - prob) / params.nshots)
@@ -237,82 +167,84 @@
                         errors=np.array([error]),
                     ),
                 )
 
     return data
 
 
-def ramsey_fit(x, p0, p1, p2, p3, p4):
-    # A fit to Superconducting Qubit Rabi Oscillation
-    #   Offset                       : p[0]
-    #   Oscillation amplitude        : p[1]
-    #   DeltaFreq                    : p[2]
-    #   Phase                        : p[3]
-    #   Arbitrary parameter T_2      : 1/p[4]
-    return p0 + p1 * np.sin(x * p2 + p3) * np.exp(-x * p4)
-
-
 def _fit(data: RamseyData) -> RamseyResults:
     r"""
     Fitting routine for Ramsey experiment. The used model is
     .. math::
         y = p_0 + p_1 sin \Big(p_2 x + p_3 \Big) e^{-x p_4}.
     """
     qubits = data.qubits
     waits = data.waits
     popts = {}
     freq_measure = {}
     t2_measure = {}
     delta_phys_measure = {}
+    delta_fitting_measure = {}
     chi2 = {}
     for qubit in qubits:
         qubit_data = data[qubit]
         qubit_freq = data.qubit_freqs[qubit]
         probs = qubit_data["prob"]
         try:
             popt, perr = fitting(waits, probs, qubit_data.errors)
-        except:
-            popt = POPT_EXCEPTION
-            perr = PERR_EXCEPTION
-
-        delta_fitting = popt[2] / (2 * np.pi)
-        delta_phys = data.detuning_sign * int(
-            (delta_fitting - data.n_osc / data.t_max) * GHZ_TO_HZ
-        )
-        corrected_qubit_frequency = int(qubit_freq - delta_phys)
-        t2 = popt[4]
-        freq_measure[qubit] = (
-            corrected_qubit_frequency,
-            perr[2] * GHZ_TO_HZ / (2 * np.pi * data.t_max),
-        )
-        t2_measure[qubit] = (t2, perr[4])
-        popts[qubit] = popt
-        delta_phys_measure[qubit] = (
-            delta_phys,
-            popt[2] * GHZ_TO_HZ / (2 * np.pi * data.t_max),
-        )
-        chi2[qubit] = (
-            chi2_reduced(
-                probs,
-                ramsey_fit(waits, *popts[qubit]),
-                qubit_data.errors,
-            ),
-            np.sqrt(2 / len(probs)),
-        )
-    return RamseyResults(freq_measure, t2_measure, delta_phys_measure, popts, chi2)
+
+            delta_fitting = popt[2] / (2 * np.pi)
+            sign = np.sign(data.detuning) if data.detuning != 0 else 1
+            delta_phys = int(sign * (delta_fitting * GHZ_TO_HZ - np.abs(data.detuning)))
+            corrected_qubit_frequency = int(qubit_freq - delta_phys)
+            t2 = 1 / popt[4]
+            # TODO: check error formula
+            freq_measure[qubit] = (
+                corrected_qubit_frequency,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
+            )
+            t2_measure[qubit] = (t2, perr[4] * (t2**2))
+            popts[qubit] = popt
+            # TODO: check error formula
+            delta_phys_measure[qubit] = (
+                delta_phys,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
+            )
+            delta_fitting_measure[qubit] = (
+                delta_fitting * GHZ_TO_HZ,
+                perr[2] * GHZ_TO_HZ / (2 * np.pi),
+            )
+            chi2[qubit] = (
+                chi2_reduced(
+                    probs,
+                    ramsey_fit(waits, *popts[qubit]),
+                    qubit_data.errors,
+                ),
+                np.sqrt(2 / len(probs)),
+            )
+        except Exception as e:
+            log.warning(f"Ramsey fitting failed for qubit {qubit} due to {e}.")
+    return RamseyResults(
+        frequency=freq_measure,
+        t2=t2_measure,
+        delta_phys=delta_phys_measure,
+        delta_fitting=delta_fitting_measure,
+        fitted_parameters=popts,
+        chi2=chi2,
+    )
 
 
-def _plot(data: RamseyData, qubit, fit: RamseyResults = None):
+def _plot(data: RamseyData, target: QubitId, fit: RamseyResults = None):
     """Plotting function for Ramsey Experiment."""
 
     figures = []
     fig = go.Figure()
     fitting_report = ""
 
-    qubit_data = data.data[qubit]
+    qubit_data = data.data[target]
     waits = data.waits
     probs = qubit_data["prob"]
     error_bars = qubit_data["errors"]
     fig = go.Figure(
         [
             go.Scatter(
                 x=waits,
@@ -337,38 +269,40 @@
 
     if fit is not None:
         fig.add_trace(
             go.Scatter(
                 x=waits,
                 y=ramsey_fit(
                     waits,
-                    float(fit.fitted_parameters[qubit][0]),
-                    float(fit.fitted_parameters[qubit][1]),
-                    float(fit.fitted_parameters[qubit][2]),
-                    float(fit.fitted_parameters[qubit][3]),
-                    float(fit.fitted_parameters[qubit][4]),
+                    float(fit.fitted_parameters[target][0]),
+                    float(fit.fitted_parameters[target][1]),
+                    float(fit.fitted_parameters[target][2]),
+                    float(fit.fitted_parameters[target][3]),
+                    float(fit.fitted_parameters[target][4]),
                 ),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "Delta Frequency [Hz]",
+                    "Delta Frequency (with detuning) [Hz]",
                     "Drive Frequency [Hz]",
                     "T2* [ns]",
                     "chi2 reduced",
                 ],
                 [
-                    fit.delta_phys[qubit],
-                    fit.frequency[qubit],
-                    fit.t2[qubit],
-                    fit.chi2[qubit],
+                    fit.delta_phys[target],
+                    fit.delta_fitting[target],
+                    fit.frequency[target],
+                    fit.t2[target],
+                    fit.chi2[target],
                 ],
                 display_error=True,
             )
         )
 
     fig.update_layout(
         showlegend=True,
@@ -377,73 +311,9 @@
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: RamseyResults, platform: Platform, qubit: QubitId):
-    update.drive_frequency(results.frequency[qubit][0], platform, qubit)
-
-
 ramsey = Routine(_acquisition, _fit, _plot, _update)
 """Ramsey Routine object."""
-
-
-def fitting(x: list, y: list, errors: list = None) -> list:
-    """
-    Given the inputs list `x` and outputs one `y`, this function fits the
-    `ramsey_fit` function and returns a list with the fit parameters.
-    """
-    y_max = np.max(y)
-    y_min = np.min(y)
-    x_max = np.max(x)
-    x_min = np.min(x)
-    delta_y = y_max - y_min
-    delta_x = x_max - x_min
-    y = (y - y_min) / delta_y
-    x = (x - x_min) / delta_x
-    err = errors / delta_y if errors is not None else None
-    ft = np.fft.rfft(y)
-    freqs = np.fft.rfftfreq(len(y), x[1] - x[0])
-    mags = abs(ft)
-    local_maxima = find_peaks(mags, threshold=10)[0]
-    index = local_maxima[0] if len(local_maxima) > 0 else None
-    # 0.5 hardcoded guess for less than one oscillation
-    f = freqs[index] * 2 * np.pi if index is not None else 0.5
-    p0 = [
-        0.5,
-        0.5,
-        f,
-        0,
-        1,
-    ]
-    popt, perr = curve_fit(
-        ramsey_fit,
-        x,
-        y,
-        p0=p0,
-        maxfev=5000,
-        bounds=(
-            [0, 0, 0, -np.pi, 0],
-            [1, 1, np.inf, np.pi, np.inf],
-        ),
-        sigma=err,
-    )
-    popt = [
-        delta_y * popt[0] + y_min,
-        delta_y * popt[1] * np.exp(x_min * popt[4] / delta_x),
-        popt[2] / delta_x,
-        popt[3] - x_min * popt[2] / delta_x,
-        popt[4] / delta_x,
-    ]
-    perr = np.sqrt(np.diag(perr))
-    perr = [
-        delta_y * perr[0],
-        delta_y
-        * np.exp(x_min * popt[4] / delta_x)
-        * np.sqrt(perr[1] ** 2 + (popt[1] * x_min * perr[4] / delta_x) ** 2),
-        perr[2] / delta_x,
-        np.sqrt(perr[3] ** 2 + (perr[2] * x_min / delta_x) ** 2),
-        perr[4] / delta_x,
-    ]
-    return popt, perr
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/fitting.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,31 +29,14 @@
     """Return :math:`A_1\\cdot f_1^x+A_2\\cdot f_2^x` where ``x`` is an ``np.ndarray`` and
     ``A1``, ``f1``, ``A2``, ``f2`` are floats. There is no linear offsett B.
     """
     x = np.array(x, dtype=complex)
     return A1 * f1**x + A2 * f2**x
 
 
-def expn_func(x: Union[np.ndarray, list], *args) -> np.ndarray:
-    """Compute the sum of exponentials :math:`\\sum A_i\\cdot f_i^x`
-
-    Args:
-        x (np.ndarray | list): list of exponents.
-        *args: Parameters of type `float` in the order
-            :math:`A_1`, :math:`A_2`, :math:`f_1`, :math:`f_2`,...
-
-    Returns:
-        The resulting sum of exponentials.
-    """
-    A_list = np.array(args[: len(args) // 2], dtype=complex)
-    f_list = np.array(args[len(args) // 2 :], dtype=complex)
-    sum_of_exponentials = np.vectorize(lambda m: np.sum(A_list * (f_list**m)))
-    return sum_of_exponentials(np.real(x))
-
-
 def esprit(
     xdata: np.ndarray,
     ydata: np.ndarray,
     num_decays: int,
     hankel_dim: Optional[int] = None,
 ) -> np.ndarray:
     """Implements the ESPRIT algorithm for peak detection.
@@ -162,15 +145,17 @@
             log.warning("Ap^x fit: the fitting was not succesful. %s", e)
             popt, perr = (0, 0), (0, 0)
 
     return popt, perr
 
 
 def fit_expn_func(
-    xdata: Union[np.ndarray, list], ydata: Union[np.ndarray, list], n: int = 2, **kwargs
+    xdata: Union[np.ndarray, list],
+    ydata: Union[np.ndarray, list],
+    n: int = 2,
 ) -> tuple[tuple, tuple]:
     """Calculate n exponentials on top of each other, fit to the given ydata.
     No linear offset, the ESPRIT algorithm is used to identify ``n`` exponential decays.
 
     Args:
         xdata (Union[np.ndarray, list]): The x-labels.
         ydata (Union[np.ndarray, list]): The data to be fitted.
@@ -185,15 +170,16 @@
     decays = esprit(np.array(xdata), np.array(ydata), n)
     vandermonde = np.array([decays**x for x in xdata])
     alphas = np.linalg.pinv(vandermonde) @ np.array(ydata).reshape(-1, 1).flatten()
     return tuple([*alphas, *decays]), (0,) * (len(alphas) + len(decays))
 
 
 def fit_exp2_func(
-    xdata: Union[np.ndarray, list], ydata: Union[np.ndarray, list], **kwargs
+    xdata: Union[np.ndarray, list],
+    ydata: Union[np.ndarray, list],
 ) -> tuple[tuple, tuple]:
     """Calculate 2 exponentials on top of each other, fit to the given ydata.
 
     No linear offset, the ESPRIT algorithm is used to identify the two exponential decays.
 
     Args:
         xdata (Union[np.ndarray, list]): The x-labels.
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/noisemodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     def __init__(self, probabilities: Optional[list] = None) -> None:
         super().__init__()
         # Check if number of arguments is 0 or 1 and if it's equal to None
         if not probabilities:
             # Assign random values to params.
             self.params = np.random.uniform(0, 0.25, size=3).round(3)
         elif len(probabilities) == 3:
-            self.params = probabilities
+            self.params = np.array(probabilities)
         else:
             # Raise ValueError if given paramters are wrong.
             raise_error(
                 ValueError,
                 f"Wrong number of error parameters, 3 != {len(probabilities)}.",
             )
         self.build()
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/randomized_benchmarking/standard_rb.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,26 @@
+from collections import defaultdict
 from dataclasses import dataclass, field
 from typing import Iterable, Optional, TypedDict, Union
 
 import numpy as np
-import pandas as pd
+import numpy.typing as npt
 import plotly.graph_objects as go
-import qibo
 from qibo.backends import GlobalBackend
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
-from qibocal.bootstrap import bootstrap, data_uncertainties
-from qibocal.config import log, raise_error
+from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.config import raise_error
 from qibocal.protocols.characterization.randomized_benchmarking import noisemodels
 
-from .circuit_tools import (
-    add_inverse_layer,
-    add_measurement_layer,
-    embed_circuit,
-    layer_circuit,
-)
-from .data import RBData
+from ..utils import table_dict, table_html
+from .circuit_tools import add_inverse_layer, add_measurement_layer, layer_circuit
 from .fitting import exp1B_func, fit_exp1B_func
-from .utils import extract_from_data, number_to_str, random_clifford
+from .utils import data_uncertainties, number_to_str, random_clifford
 
 NPULSES_PER_CLIFFORD = 1.875
 
 
 class Depthsdict(TypedDict):
     """dictionary used to build a list of depths as ``range(start, stop, step)``."""
 
@@ -39,147 +33,166 @@
 class StandardRBParameters(Parameters):
     """Standard Randomized Benchmarking runcard inputs."""
 
     depths: Union[list, Depthsdict]
     """A list of depths/sequence lengths. If a dictionary is given the list will be build."""
     niter: int
     """Sets how many iterations over the same depth value."""
-    uncertainties: Union[str, float] = 95
+    uncertainties: Optional[float] = None
     """Method of computing the error bars of the signal and uncertainties of the fit. If ``None``,
-    does not compute them. If ``"std"``, computes the standard deviation. If ``float`` or ``int``
-    between 0 and 100, computes the corresponding confidence interval. Defaults to ``95``."""
-    n_bootstrap: int = 100
-    """Number of bootstrap iterations for the fit uncertainties and error bars.
-    If ``0``, gets the fit uncertainties from the fitting function and the error bars
-    from the distribution of the measurements. Defaults to ``100``."""
+    it computes the standard deviation. Otherwise it computes the corresponding confidence interval. Defaults `None`."""
     unrolling: bool = False
     """If ``True`` it uses sequence unrolling to deploy multiple circuits in a single instrument call.
     Defaults to ``False``."""
     seed: Optional[int] = None
     """A fixed seed to initialize ``np.random.Generator``. If ``None``, uses a random seed.
     Defaults is ``None``."""
-    noise_model: str = ""
+    noise_model: Optional[str] = None
     """For simulation purposes, string has to match what is in
     :mod:`qibocal.protocols.characterization.randomized_benchmarking.noisemodels`"""
     noise_params: Optional[list] = field(default_factory=list)
     """With this the noise model will be initialized, if not given random values will be used."""
+    nshots: int = 10
+    """Just to add the default value"""
 
     def __post_init__(self):
         if isinstance(self.depths, dict):
             self.depths = list(
                 range(self.depths["start"], self.depths["stop"], self.depths["step"])
             )
 
 
-# TODO: uniform RB to implement results as dictionaries
+RBType = np.dtype(
+    [
+        ("samples", np.int32),
+    ]
+)
+"""Custom dtype for RB."""
+
+
+@dataclass
+class RBData(Data):
+    """The output of the acquisition function."""
+
+    depths: list
+    """Circuits depths."""
+    uncertainties: Optional[float]
+    """Parameters uncertainties."""
+    seed: Optional[int]
+    nshots: int
+    """Number of shots."""
+    niter: int
+    """Number of iterations for each depth."""
+    data: dict[QubitId, npt.NDArray[RBType]] = field(default_factory=dict)
+    """Raw data acquired."""
+    circuits: dict[QubitId, list[list[int]]] = field(default_factory=dict)
+    """Clifford gate indexes executed."""
+
+    def extract_probabilities(self, qubit):
+        """Extract the probabilities given `qubit`"""
+        probs = []
+        for depth in self.depths:
+            data_list = np.array(self.data[qubit, depth].tolist())
+            data_list = data_list.reshape((-1, self.nshots))
+            probs.append(np.count_nonzero(1 - data_list, axis=1) / data_list.shape[1])
+        return probs
+
+
 @dataclass
 class StandardRBResult(Results):
     """Standard RB outputs."""
 
-    fidelity: float
+    fidelity: dict[QubitId, float]
     """The overall fidelity of this qubit."""
-    pulse_fidelity: float
+    pulse_fidelity: dict[QubitId, float]
     """The pulse fidelity of the gates acting on this qubit."""
-    fit_parameters: tuple[float, float, float]
+    fit_parameters: dict[QubitId, tuple[float, float, float]]
     """Raw fitting parameters."""
-    fit_uncertainties: tuple[float, float, float]
+    fit_uncertainties: dict[QubitId, tuple[float, float, float]]
     """Fitting parameters uncertainties."""
-    error_bars: Optional[Union[float, list[float]]] = None
+    error_bars: dict[QubitId, Optional[Union[float, list[float]]]] = None
     """Error bars for y."""
 
+    # FIXME: fix this after https://github.com/qiboteam/qibocal/pull/597
+    def __contains__(self, qubit: QubitId):
+        return True
 
-def samples_to_p0(samples_list):
-    """Computes the probabilitiy of 0 from the list of samples.
 
-    Args:
-        samples_list (list or np.ndarray): 3d array with ``ncircuits`` rows containing
-            ``nshots`` lists with ``nqubits`` amount of ``0`` and ``1`` samples.
-            e.g. ``samples_list`` for 1 circuit, 3 shots and 2 qubits looks like
-            ``[[[0, 0], [0, 1], [1, 0]]]`` and ``p0=1/3``.
-
-    Returns:
-        list: list of probabilities corresponding to each row.
+class RB_Generator:
     """
-
-    ground = np.array([0] * len(samples_list[0][0]))
-    return np.count_nonzero((samples_list == ground).all(axis=2), axis=1) / len(
-        samples_list[0]
-    )
-
-
-def resample_p0(data, sample_size=100, homogeneous: bool = True):
-    """Preforms parametric resampling of shots with binomial distribution
-        and returns a list of "corrected" probabilites.
-
-    Args:
-        data (list or np.ndarray): list of probabilities for the binomial distribution.
-        nshots (int): sample size for one probability distribution.
-
-    Returns:
-        list: resampled probabilities.
+    This class generates random single qubit cliffords for randomized benchmarking.
     """
-    if homogeneous:
-        return np.apply_along_axis(
-            lambda p: samples_to_p0(
-                np.random.binomial(n=1, p=1 - p, size=(1, sample_size, len(p))).T
-            ),
-            0,
-            data,
-        )
-    resampled_data = []
-    for row in data:
-        resampled_data.append([])
-        for p in row:
-            samples_corrected = np.random.binomial(
-                n=1, p=1 - p, size=(1, sample_size, *p.shape)
-            ).T
-            resampled_data[-1].append(samples_to_p0(samples_corrected))
-    return resampled_data
 
+    def __init__(self, seed):
+        self.seed = seed
+        self.local_state = (
+            np.random.default_rng(seed)
+            if seed is None or isinstance(seed, int)
+            else seed
+        )
 
-def setup_scan(
-    params: StandardRBParameters, qubits: Union[Qubits, list[QubitId]], nqubits: int
+    def random_index(self, gate_list):
+        """
+        Generates a random index within the range of the given gate list.
+
+        Parameters:
+        - gate_list (list): Dict of gates.
+
+        Returns:
+        - int: Random index.
+        """
+        return self.local_state.integers(0, len(gate_list), 1)
+
+    def layer_gen(self):
+        """
+        Returns:
+        - Gate: Random single-qubit clifford .
+        """
+        return random_clifford(self.random_index)
+
+
+def random_circuits(
+    depth: int,
+    targets: list[QubitId],
+    niter,
+    rb_gen,
+    noise_model=None,
 ) -> Iterable:
-    """Returns an iterator of single-qubit random self-inverting Clifford circuits.
+    """Returns single-qubit random self-inverting Clifford circuits.
 
     Args:
         params (StandardRBParameters): Parameters of the RB protocol.
-        qubits (dict[int, Union[str, int]] or list[Union[str, int]]):
+        targets (list[QubitId]):
             list of qubits the circuit is executed on.
         nqubits (int, optional): Number of qubits of the resulting circuits.
             If ``None``, sets ``len(qubits)``. Defaults to ``None``.
 
     Returns:
         Iterable: The iterator of circuits.
     """
 
-    qubit_ids = list(qubits) if isinstance(qubits, dict) else qubits
-
-    def make_circuit(depth):
-        """Returns a random Clifford circuit with inverse of ``depth``."""
-
-        # This function is needed so that the inside of the layer_circuit function layer_gen()
-        # can be called for each layer of the circuit, and it returns a random layer of
-        # Clifford gates. Could also be a generator, it just has to be callable.
-        def layer_gen():
-            """Returns a circuit with a random single-qubit clifford unitary."""
-            return random_clifford(len(qubit_ids), params.seed)
-
-        circuit = layer_circuit(layer_gen, depth)
-        add_inverse_layer(circuit)
-        add_measurement_layer(circuit)
-        return embed_circuit(circuit, nqubits, qubit_ids)
+    circuits = []
+    indexes = defaultdict(list)
+    for _ in range(niter):
+        for target in targets:
+            circuit, random_index = layer_circuit(rb_gen, depth, target)
+            add_inverse_layer(circuit)
+            add_measurement_layer(circuit)
+            if noise_model is not None:
+                circuit = noise_model.apply(circuit)
+            circuits.append(circuit)
+            indexes[target].append(random_index)
 
-    return map(make_circuit, params.depths * params.niter)
+    return circuits, indexes
 
 
 def _acquisition(
     params: StandardRBParameters,
     platform: Platform,
-    qubits: Union[Qubits, list[QubitId]],
+    targets: list[QubitId],
 ) -> RBData:
     """The data acquisition stage of Standard Randomized Benchmarking.
 
     1. Set up the scan
     2. Execute the scan
     3. Post process the data and initialize a standard rb data object with it.
 
@@ -188,202 +201,172 @@
         platform (Platform): Platform the experiment is executed on.
         qubits (dict[int, Union[str, int]] or list[Union[str, int]]): list of qubits the experiment is executed on.
 
     Returns:
         RBData: The depths, samples and ground state probability of each experiment in the scan.
     """
 
+    backend = GlobalBackend()
     # For simulations, a noise model can be added.
     noise_model = None
-    if params.noise_model:
-        # FIXME implement this check outside acquisition
-        if platform and platform.name != "dummy":
+    if params.noise_model is not None:
+        if backend.name == "qibolab":
             raise_error(
-                NotImplementedError,
-                f"Backend qibolab ({platform}) does not perform noise models simulation.",
+                ValueError,
+                "Backend qibolab (%s) does not perform noise models simulation. ",
             )
-        elif platform:
-            log.warning(
-                (
-                    "Backend qibolab (%s) does not perform noise models simulation. "
-                    "Setting backend to ``NumpyBackend`` instead."
-                ),
-                platform.name,
-            )
-            qibo.set_backend("numpy")
-            platform = None
 
         noise_model = getattr(noisemodels, params.noise_model)(params.noise_params)
-        params.noise_params = noise_model.params
-
-    # Grab activated qibo backend
-    backend = GlobalBackend()
-
+        params.noise_params = noise_model.params.tolist()
     # 1. Set up the scan (here an iterator of circuits of random clifford gates with an inverse).
-    nqubits = platform.nqubits if platform else max(qubits) + 1
-    scan = setup_scan(params, qubits, nqubits)
+    nqubits = len(targets)
+    data = RBData(
+        depths=params.depths,
+        uncertainties=params.uncertainties,
+        seed=params.seed,
+        nshots=params.nshots,
+        niter=params.niter,
+    )
 
-    # Iterate through the scan and create circuits
     circuits = []
-    depths = []
-    for circuit in scan:
-        # The inverse and measurement gate don't count for the depth.
-        depths.append((circuit.depth - 2) if circuit.depth > 1 else 0)
-        if noise_model is not None:
-            circuit = noise_model.apply(circuit)
-        circuits.append(circuit)
-
+    indexes = {}
+    samples = []
+    qubits_ids = targets
+    rb_gen = RB_Generator(params.seed)
+    for depth in params.depths:
+        # TODO: This does not generate multi qubit circuits
+        circuits_depth, random_indexes = random_circuits(
+            depth, qubits_ids, params.niter, rb_gen, noise_model
+        )
+        circuits.extend(circuits_depth)
+        for qubit in random_indexes.keys():
+            indexes[(qubit, depth)] = random_indexes[qubit]
     # Execute the circuits
     if params.unrolling:
-        results = backend.execute_circuits(circuits, nshots=params.nshots)
+        executed_circuits = backend.execute_circuits(circuits, nshots=params.nshots)
     else:
-        results = [
+        executed_circuits = [
             backend.execute_circuit(circuit, nshots=params.nshots)
             for circuit in circuits
         ]
 
-    # Every executed circuit gets a row where the data is stored.
-    data_list = [
-        {"depth": depth, "samples": result.samples()}
-        for depth, result in zip(depths, results)
-    ]
-
-    # Build the data object which will be returned and later saved.
-    data = pd.DataFrame(data_list)
+    for circ in executed_circuits:
+        samples.extend(circ.samples())
+    samples = np.reshape(samples, (-1, nqubits, params.nshots))
+
+    for i, depth in enumerate(params.depths):
+        index = (i * params.niter, (i + 1) * params.niter)
+        for nqubit, qubit_id in enumerate(targets):
+            data.register_qubit(
+                RBType,
+                (qubit_id, depth),
+                dict(
+                    samples=samples[index[0] : index[1]][:, nqubit],
+                ),
+            )
+    data.circuits = indexes
 
-    # The signal here is the survival probability.
-    standardrb_data = RBData(
-        data.assign(signal=lambda x: samples_to_p0(x.samples.to_list()))
-    )
-    # Store the parameters to display them later.
-    standardrb_data.attrs = params.__dict__
-    return standardrb_data
+    return data
 
 
 def _fit(data: RBData) -> StandardRBResult:
     """Takes a data frame, extracts the depths and the signal and fits it with an
     exponential function y = Ap^x+B.
 
     Args:
         data (RBData): Data from the data acquisition stage.
 
     Returns:
         StandardRBResult: Aggregated and processed data.
     """
-    # Extract depths and probabilities
-    x, y_scatter = extract_from_data(data, "signal", "depth", list)
-    homogeneous = all(len(y_scatter[0]) == len(row) for row in y_scatter)
-
-    # Extract fitting and bootstrap parameters if given
-    uncertainties = data.attrs.get("uncertainties", None)
-    n_bootstrap = data.attrs.get("n_bootstrap", 0)
-
-    y_estimates, popt_estimates = y_scatter, []
-    if uncertainties and n_bootstrap:
-        # Non-parametric bootstrap resampling
-        bootstrap_y = bootstrap(
-            y_scatter,
-            n_bootstrap,
-            homogeneous=homogeneous,
-            seed=data.attrs.get("seed", None),
-        )
+    qubits = data.qubits
 
-        # Parametric bootstrap resampling of "corrected" probabilites from binomial distribution
-        bootstrap_y = resample_p0(
-            bootstrap_y, data.attrs.get("nshots", 1), homogeneous=homogeneous
+    fidelity, pulse_fidelity = {}, {}
+    popts, perrs = {}, {}
+    error_barss = {}
+    for qubit in qubits:
+        # Extract depths and probabilities
+        x = data.depths
+        probs = data.extract_probabilities(qubit)
+        samples_mean = np.mean(probs, axis=1)
+        # TODO: Should we use the median or the mean?
+        median = np.median(probs, axis=1)
+
+        error_bars = data_uncertainties(
+            probs,
+            method=data.uncertainties,
+            data_median=median,
         )
 
-        # Compute y and popt estimates for each bootstrap iteration
-        y_estimates = (
-            np.mean(bootstrap_y, axis=1)
-            if homogeneous
-            else [np.mean(y_iter, axis=0) for y_iter in bootstrap_y]
-        )
-        popt_estimates = np.apply_along_axis(
-            lambda y_iter: fit_exp1B_func(x, y_iter, bounds=[0, 1])[0],
-            axis=0,
-            arr=np.array(y_estimates),
-        )
-
-    # Fit the initial data and compute error bars
-    y = [np.mean(y_row) for y_row in y_scatter]
-
-    # If bootstrap was not performed, y_estimates can be inhomogeneous
-    error_bars = data_uncertainties(
-        y_estimates,
-        uncertainties,
-        data_median=y,
-        homogeneous=(homogeneous or n_bootstrap != 0),
-    )
-    # Generate symmetric non-zero uncertainty of y for the fit
-    sigma = None
-    if error_bars is not None:
         sigma = (
-            np.max(error_bars, axis=0)
-            if isinstance(error_bars[0], Iterable)
-            else error_bars
-        ) + 0.1
-
-    popt, perr = fit_exp1B_func(x, y, sigma=sigma, bounds=[0, 1])
-
-    # Compute fit uncertainties
-    if len(popt_estimates):
-        perr = data_uncertainties(popt_estimates, uncertainties, data_median=popt)
-        perr = perr.T if perr is not None else (0,) * len(popt)
-
-    # Compute the fidelities
-    infidelity = (1 - popt[1]) / 2
-    fidelity = 1 - infidelity
-    pulse_fidelity = 1 - infidelity / NPULSES_PER_CLIFFORD
-
-    # conversion from np.array to list/tuple
-    error_bars = error_bars.tolist() if error_bars is not None else error_bars
-    perr = perr if isinstance(perr, tuple) else perr.tolist()
-    return StandardRBResult(fidelity, pulse_fidelity, popt, perr, error_bars)
-
+            np.max(error_bars, axis=0) if data.uncertainties is not None else error_bars
+        )
 
-def _plot(data: RBData, fit: StandardRBResult, qubit) -> tuple[list[go.Figure], str]:
+        popt, perr = fit_exp1B_func(x, samples_mean, sigma=sigma, bounds=[0, 1])
+        # Compute the fidelities
+        infidelity = (1 - popt[1]) / 2
+        fidelity[qubit] = 1 - infidelity
+        pulse_fidelity[qubit] = 1 - infidelity / NPULSES_PER_CLIFFORD
+
+        # conversion from np.array to list/tuple
+        error_bars = error_bars.tolist()
+        error_barss[qubit] = error_bars
+        perrs[qubit] = perr
+        popts[qubit] = popt
+
+    return StandardRBResult(fidelity, pulse_fidelity, popts, perrs, error_barss)
+
+
+def _plot(
+    data: RBData, fit: StandardRBResult, target: QubitId
+) -> tuple[list[go.Figure], str]:
     """Builds the table for the qq pipe, calls the plot function of the result object
     and returns the figure es list.
 
     Args:
         data (RBData): Data object used for the table.
         fit (StandardRBResult): Is called for the plot.
-        qubit (_type_): Not used yet.
+        target (_type_): Not used yet.
 
     Returns:
         tuple[list[go.Figure], str]:
     """
-    x, y_scatter = extract_from_data(data, "signal", "depth", list)
-    y = [np.mean(y_row) for y_row in y_scatter]
 
+    qubit = target
     fig = go.Figure()
+    fitting_report = ""
+    x = data.depths
+    raw_data = data.extract_probabilities(qubit)
+    y = np.mean(raw_data, axis=1)
+    raw_depths = [[depth] * data.niter for depth in data.depths]
+
     fig.add_trace(
         go.Scatter(
-            x=data.depth.tolist(),
-            y=data.signal.tolist(),
+            x=np.hstack(raw_depths),
+            y=np.hstack(raw_data),
             line=dict(color="#6597aa"),
             mode="markers",
             marker={"opacity": 0.2, "symbol": "square"},
             name="iterations",
         )
     )
+
     fig.add_trace(
         go.Scatter(
             x=x,
             y=y,
             line=dict(color="#aa6464"),
             mode="markers",
             name="average",
         )
     )
     # Create a dictionary for the error bars
     error_y_dict = None
     if fit is not None:
-        popt, perr = fit.fit_parameters, fit.fit_uncertainties
+        popt, perr = fit.fit_parameters[qubit], fit.fit_uncertainties[qubit]
         label = "Fit: y=Ap^x<br>A: {}<br>p: {}<br>B: {}".format(
             number_to_str(popt[0], perr[0]),
             number_to_str(popt[1], perr[1]),
             number_to_str(popt[2], perr[2]),
         )
         x_fit = np.linspace(min(x), max(x), len(x) * 20)
         y_fit = exp1B_func(x_fit, *popt)
@@ -392,66 +375,64 @@
                 x=x_fit,
                 y=y_fit,
                 name=label,
                 line=go.scatter.Line(dash="dot", color="#00cc96"),
             )
         )
         if fit.error_bars is not None:
+            error_bars = fit.error_bars[qubit]
             # Constant error bars
-            if isinstance(fit.error_bars, Iterable) is False:
-                error_y_dict = {"type": "constant", "value": fit.error_bars}
+            if isinstance(error_bars, Iterable) is False:
+                error_y_dict = {"type": "constant", "value": error_bars}
             # Symmetric error bars
-            elif isinstance(fit.error_bars[0], Iterable) is False:
-                error_y_dict = {"type": "data", "array": fit.error_bars}
+            elif isinstance(error_bars[0], Iterable) is False:
+                error_y_dict = {"type": "data", "array": error_bars}
             # Asymmetric error bars
             else:
                 error_y_dict = {
                     "type": "data",
                     "symmetric": False,
-                    "array": fit.error_bars[1],
-                    "arrayminus": fit.error_bars[0],
+                    "array": error_bars[1],
+                    "arrayminus": error_bars[0],
                 }
             fig.add_trace(
                 go.Scatter(
                     x=x,
                     y=y,
                     error_y=error_y_dict,
                     line={"color": "#aa6464"},
                     mode="markers",
                     name="error bars",
                 )
             )
-
-    # TODO: fix this mess
-    # meta_data = deepcopy(data.attrs)
-    # meta_data.pop("depths")
-    # if not meta_data["noise_model"]:
-    #     meta_data.pop("noise_model")
-    #     meta_data.pop("noise_params")
-
-    table_str = ""
-    # TODO: and this mess
-    # table_str = "".join(
-    #     [
-    #         f" | {key}: {value}<br>"
-    #         for key, value in {
-    #             **meta_data,
-    #             "fidelity": number_to_str(fit.fidelity, np.array(perr[1]) / 2),
-    #             "pulse_fidelity": number_to_str(
-    #                 fit.pulse_fidelity,
-    #                 np.array(perr[1]) / (2 * NPULSES_PER_CLIFFORD),
-    #             ),
-    #         }.items()
-    #     ]
-    # )
+    if fit is not None:
+        fitting_report = table_html(
+            table_dict(
+                qubit,
+                ["niter", "nshots", "uncertainties", "fidelity", "pulse_fidelity"],
+                [
+                    data.niter,
+                    data.nshots,
+                    data.uncertainties,
+                    number_to_str(
+                        fit.fidelity[qubit],
+                        np.array(fit.fit_uncertainties[qubit][1]) / 2,
+                    ),
+                    number_to_str(
+                        fit.pulse_fidelity[qubit],
+                        np.array(fit.fit_uncertainties[qubit][1])
+                        / (2 * NPULSES_PER_CLIFFORD),
+                    ),
+                ],
+            )
+        )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Circuit depth",
         yaxis_title="Survival Probability",
     )
 
-    return [fig], table_str
+    return [fig], fitting_report
 
 
-# Build the routine object which is used by qq-auto.
 standard_rb = Routine(_acquisition, _fit, _plot)
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_characterization.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_characterization.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.utils import (
     effective_qubit_temperature,
     format_error_single_cell,
     round_report,
     table_dict,
     table_html,
 )
@@ -60,33 +60,35 @@
     )
     """Raw data acquired."""
     samples: dict[tuple, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: ReadoutCharacterizationParameters, platform: Platform, qubits: Qubits
+    params: ReadoutCharacterizationParameters,
+    platform: Platform,
+    targets: list[QubitId],
 ) -> ReadoutCharacterizationData:
     """Data acquisition for resonator spectroscopy."""
 
     data = ReadoutCharacterizationData(
         qubit_frequencies={
-            qubit: platform.qubits[qubit].drive_frequency for qubit in qubits
+            qubit: platform.qubits[qubit].drive_frequency for qubit in targets
         }
     )
 
     # FIXME: ADD 1st measurament and post_selection for accurate state preparation ?
 
     for state in [0, 1]:
         # Define the pulse sequences
         if state == 1:
             RX_pulses = {}
         ro_pulses = {}
         sequence = PulseSequence()
-        for qubit in qubits:
+        for qubit in targets:
             start = 0
             if state == 1:
                 RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
                 sequence.add(RX_pulses[qubit])
                 start = RX_pulses[qubit].finish
             ro_pulses[qubit] = []
             for _ in range(2):
@@ -109,15 +111,15 @@
             ExecutionParameters(
                 nshots=params.nshots,
                 relaxation_time=params.relaxation_time,
             ),
         )
 
         # Save the data
-        for qubit in qubits:
+        for qubit in targets:
             for i, ro_pulse in enumerate(ro_pulses[qubit]):
                 result = results[ro_pulse.serial]
                 data.register_qubit(
                     ReadoutCharacterizationType,
                     (qubit, state, i),
                     dict(i=result.voltage_i, q=result.voltage_q),
                 )
@@ -191,26 +193,28 @@
 
     return ReadoutCharacterizationResults(
         fidelity, assignment_fidelity, qnd, effective_temperature, Lambda_M
     )
 
 
 def _plot(
-    data: ReadoutCharacterizationData, fit: ReadoutCharacterizationResults, qubit
+    data: ReadoutCharacterizationData,
+    fit: ReadoutCharacterizationResults,
+    target: QubitId,
 ):
     """Plotting function for ReadoutCharacterization."""
 
     # Maybe the plot can just be something like a confusion matrix between 0s and 1s ???
 
     figures = []
     fitting_report = ""
     fig = go.Figure()
     for state in range(2):
         for measure in range(2):
-            shots = data.data[qubit, state, measure]
+            shots = data.data[target, state, measure]
 
             fig.add_trace(
                 go.Scatter(
                     x=shots.i,
                     y=shots.q,
                     name=f"state {state} measure {measure}",
                     mode="markers",
@@ -221,42 +225,42 @@
             )
     figures.append(fig)
     if fit is not None:
         fig2 = go.Figure()
 
         fig2.add_trace(
             go.Heatmap(
-                z=fit.Lambda_M[qubit],
+                z=fit.Lambda_M[target],
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "Assignment Fidelity",
                     "Fidelity",
                     "QND",
                     "Effective Qubit Temperature [K]",
                 ],
                 [
-                    np.round(fit.assignment_fidelity[qubit], 6),
-                    np.round(fit.fidelity[qubit], 6),
-                    np.round(fit.qnd[qubit], 6),
+                    np.round(fit.assignment_fidelity[target], 6),
+                    np.round(fit.fidelity[target], 6),
+                    np.round(fit.qnd[target], 6),
                     format_error_single_cell(
-                        round_report([fit.effective_temperature[qubit]])
+                        round_report([fit.effective_temperature[target]])
                     ),
                 ],
             )
         )
         figures.append(fig2)
     return figures, fitting_report
 
 
 def _update(
-    results: ReadoutCharacterizationResults, platform: Platform, qubit: QubitId
+    results: ReadoutCharacterizationResults, platform: Platform, target: QubitId
 ):
-    update.readout_fidelity(results.fidelity[qubit], platform, qubit)
-    update.assignment_fidelity(results.assignment_fidelity[qubit], platform, qubit)
+    update.readout_fidelity(results.fidelity[target], platform, target)
+    update.assignment_fidelity(results.assignment_fidelity[target], platform, target)
 
 
 readout_characterization = Routine(_acquisition, _fit, _plot, _update)
 """ReadoutCharacterization Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_mitigation_matrix.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_mitigation_matrix.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from qibo import gates
 from qibo.models import Circuit
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
 
 from .utils import calculate_frequencies
 
 
 @dataclass
 class ReadoutMitigationMatrixParameters(Parameters):
@@ -41,15 +41,15 @@
     """Matrix containing measurement matrices for each state."""
 
 
 @dataclass
 class ReadoutMitigationMatrixData(Data):
     """ReadoutMitigationMatrix acquisition outputs."""
 
-    qubits_list: list
+    qubit_list: list[QubitId]
     """List of qubit ids"""
     nshots: int
     """Number of shots"""
     data: dict = field(default_factory=dict)
     """Raw data acquited."""
 
     def add(self, qubits, state, freqs):
@@ -86,59 +86,61 @@
             if qubits == list(index[: len(index) - 2])
         }
 
 
 def _acquisition(
     params: ReadoutMitigationMatrixParameters,
     platform: Platform,
-    qubits: list[Qubits],
+    targets: list[list[QubitId]],
 ) -> ReadoutMitigationMatrixData:
     data = ReadoutMitigationMatrixData(
-        nshots=params.nshots, qubits_list=[list(qq) for qq in qubits]
+        nshots=params.nshots, qubit_list=[list(qq) for qq in targets]
     )
-    for qubit_list in qubits:
-        nqubits = len(qubit_list)
+    for qubits in targets:
+        nqubits = len(qubits)
         for i in range(2**nqubits):
             state = format(i, f"0{nqubits}b")
             if params.pulses:
                 sequence = PulseSequence()
                 for q, bit in enumerate(state):
                     if bit == "1":
                         sequence.add(
                             platform.create_RX_pulse(
-                                qubit_list[q], start=0, relative_phase=0
+                                qubits[q], start=0, relative_phase=0
                             )
                         )
                 measurement_start = sequence.finish
                 for q in range(len(state)):
                     MZ_pulse = platform.create_MZ_pulse(
-                        qubit_list[q], start=measurement_start
+                        qubits[q], start=measurement_start
                     )
                     sequence.add(MZ_pulse)
                 results = platform.execute_pulse_sequence(
                     sequence, ExecutionParameters(nshots=params.nshots)
                 )
-                data.add(qubit_list, state, calculate_frequencies(results, qubit_list))
+                data.add(
+                    tuple(qubits), state, calculate_frequencies(results, tuple(qubits))
+                )
             else:
                 c = Circuit(platform.nqubits)
                 for q, bit in enumerate(state):
                     if bit == "1":
-                        c.add(gates.X(qubit_list[q]))
-                    c.add(gates.M(qubit_list[q]))
+                        c.add(gates.X(qubits[q]))
+                    c.add(gates.M(qubits[q]))
                 results = c(nshots=params.nshots)
 
-                data.add(qubit_list, state, dict(results.frequencies()))
+                data.add(tuple(qubits), state, dict(results.frequencies()))
     return data
 
 
 def _fit(data: ReadoutMitigationMatrixData) -> ReadoutMitigationMatrixResults:
     """Post processing for readout mitigation matrix protocol."""
     readout_mitigation_matrix = {}
     measurement_matrix = {}
-    for qubit in data.qubits_list:
+    for qubit in data.qubit_list:
         qubit_data = data[qubit]
         matrix = np.zeros((2 ** len(qubit), 2 ** len(qubit)))
         computational_basis = [
             format(i, f"0{len(qubit)}b") for i in range(2 ** len(qubit))
         ]
         for state in computational_basis:
             column = np.zeros(2 ** len(qubit))
@@ -152,35 +154,34 @@
             matrix[:, int(state, 2)] = np.flip(column)
 
         measurement_matrix[tuple(qubit)] = matrix.tolist()
         try:
             readout_mitigation_matrix[tuple(qubit)] = np.linalg.inv(matrix).tolist()
         except np.linalg.LinAlgError as e:
             log.warning(f"ReadoutMitigationMatrix: the fitting was not succesful. {e}")
-            readout_mitigation_matrix[tuple(qubit)] = np.zeros(
-                (2 ** len(qubit), 2 ** len(qubit))
-            ).tolist()
 
     return ReadoutMitigationMatrixResults(
         readout_mitigation_matrix=readout_mitigation_matrix,
         measurement_matrix=measurement_matrix,
     )
 
 
 def _plot(
-    data: ReadoutMitigationMatrixData, fit: ReadoutMitigationMatrixResults, qubit
+    data: ReadoutMitigationMatrixData,
+    fit: ReadoutMitigationMatrixResults,
+    target: list[QubitId],
 ):
     """Plotting function for readout mitigation matrix."""
     fitting_report = ""
     figs = []
     if fit is not None:
         computational_basis = [
-            format(i, f"0{len(qubit)}b") for i in range(2 ** len(qubit))
+            format(i, f"0{len(target)}b") for i in range(2 ** len(target))
         ]
-        z = fit.measurement_matrix[tuple(qubit)]
+        z = fit.measurement_matrix[tuple(target)]
 
         fig = px.imshow(
             z,
             x=computational_basis,
             y=computational_basis[::-1],
             text_auto=True,
             labels={
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_amplitude.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.fitting.classifier.qubit_fit import QubitFit
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
 
 @dataclass
 class ResonatorAmplitudeParameters(Parameters):
     """ResonatorAmplitude runcard inputs."""
@@ -61,33 +61,33 @@
     best_threshold: dict[QubitId, float]
     """Thershold that gives lower error."""
 
 
 def _acquisition(
     params: ResonatorAmplitudeParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> ResonatorAmplitudeData:
     r"""
     Data acquisition for resoantor amplitude optmization.
     This protocol sweeps the readout amplitude performing a classification routine
     and evaluating the error probability at each step. The sweep will be interrupted
     if the probability error is less than the `error_threshold`.
 
     Args:
         params (:class:`ResonatorAmplitudeParameters`): input parameters
         platform (:class:`Platform`): Qibolab's platform
-        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+        targets (list): list of QubitIds to be characterized
 
     Returns:
         data (:class:`ResonatorAmplitudeData`)
     """
 
     data = ResonatorAmplitudeData()
-    for qubit in qubits:
+    for qubit in targets:
         error = 1
         old_amp = platform.qubits[qubit].native_gates.MZ.amplitude
         new_amp = params.amplitude_start
         while error > params.error_threshold and new_amp <= params.amplitude_stop:
             platform.qubits[qubit].native_gates.MZ.amplitude = new_amp
             sequence_0 = PulseSequence()
             sequence_1 = PulseSequence()
@@ -156,56 +156,58 @@
         best_amps[qubit] = data_qubit["amp"][index_best_err]
         best_angle[qubit] = data_qubit["angle"][index_best_err]
         best_threshold[qubit] = data_qubit["threshold"][index_best_err]
 
     return ResonatorAmplitudeResults(lowest_err, best_amps, best_angle, best_threshold)
 
 
-def _plot(data: ResonatorAmplitudeData, fit: ResonatorAmplitudeResults, qubit):
+def _plot(
+    data: ResonatorAmplitudeData, fit: ResonatorAmplitudeResults, target: QubitId
+):
     """Plotting function for Optimization RO amplitude."""
     figures = []
     opacity = 1
     fitting_report = None
     fig = make_subplots(
         rows=1,
         cols=1,
     )
     if fit is not None:
         fig.add_trace(
             go.Scatter(
-                x=data[qubit]["amp"],
-                y=data[qubit]["error"],
+                x=data[target]["amp"],
+                y=data[target]["error"],
                 opacity=opacity,
                 showlegend=True,
                 mode="lines+markers",
             ),
             row=1,
             col=1,
         )
 
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 "Best Readout Amplitude [a.u.]",
-                np.round(fit.best_amp[qubit], 4),
+                np.round(fit.best_amp[target], 4),
             )
         )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Readout Amplitude [a.u.]",
         yaxis_title="Probability Error",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ResonatorAmplitudeResults, platform: Platform, qubit: QubitId):
-    update.readout_amplitude(results.best_amp[qubit], platform, qubit)
-    update.iq_angle(results.best_angle[qubit], platform, qubit)
-    update.threshold(results.best_threshold[qubit], platform, qubit)
+def _update(results: ResonatorAmplitudeResults, platform: Platform, target: QubitId):
+    update.readout_amplitude(results.best_amp[target], platform, target)
+    update.iq_angle(results.best_angle[target], platform, target)
+    update.threshold(results.best_threshold[target], platform, target)
 
 
 resonator_amplitude = Routine(_acquisition, _fit, _plot, _update)
 """Resonator Amplitude Routine  object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/resonator_frequency.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from qibolab import AcquisitionType, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.fitting.classifier.qubit_fit import QubitFit
 from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
 class ResonatorFrequencyParameters(Parameters):
     """Optimization RO frequency inputs."""
@@ -62,40 +62,40 @@
     )
 
     def unique_freqs(self, qubit: QubitId) -> np.ndarray:
         return np.unique(self.data[qubit]["freq"])
 
 
 def _acquisition(
-    params: ResonatorFrequencyParameters, platform: Platform, qubits: Qubits
+    params: ResonatorFrequencyParameters, platform: Platform, targets: list[QubitId]
 ) -> ResonatorFrequencyData:
     r"""
     Data acquisition for readout frequency optimization.
     While sweeping the readout frequency, the routine performs a single shot
     classification and evaluates the assignement fidelity.
     At the end, the readout frequency is updated, choosing the one that has
     the highest assignment fidelity.
 
     Args:
         params (ResonatorFrequencyParameters): experiment's parameters
         platform (Platform): Qibolab platform object
-        qubits (dict): list of target qubits to perform the action
+        qubits (list): list of target qubits to perform the action
 
     """
 
     # create 2 sequences of pulses for the experiment:
     # sequence_0: I  - MZ
     # sequence_1: RX - MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence_0 = PulseSequence()
     sequence_1 = PulseSequence()
     ro_pulses = {}
     qd_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         qd_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=qd_pulses[qubit].finish
         )
         sequence_0.add(ro_pulses[qubit])
         sequence_1.add(qd_pulses[qubit])
         sequence_1.add(ro_pulses[qubit])
@@ -105,15 +105,15 @@
         -params.freq_width / 2, params.freq_width / 2, params.freq_step
     )
 
     data = ResonatorFrequencyData(resonator_type=platform.resonator_type)
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[ro_pulses[qubit] for qubit in qubits],
+        pulses=[ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
     results_0 = platform.sweep(
         sequence_0,
         ExecutionParameters(
             nshots=params.nshots,
@@ -130,15 +130,15 @@
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
         ),
         sweeper,
     )
 
     # retrieve the results for every qubit
-    for qubit in qubits:
+    for qubit in targets:
         for k, freq in enumerate(delta_frequency_range):
             i_values = []
             q_values = []
             states = []
             for i, results in enumerate([results_0, results_1]):
                 result = results[ro_pulses[qubit].serial]
                 i_values.extend(result.voltage_i[k])
@@ -179,56 +179,58 @@
         fidelities=highest_fidelity,
         best_freq=best_freq,
         best_angle=best_angle,
         best_threshold=best_threshold,
     )
 
 
-def _plot(data: ResonatorFrequencyData, fit: ResonatorFrequencyResults, qubit):
+def _plot(
+    data: ResonatorFrequencyData, fit: ResonatorFrequencyResults, target: QubitId
+):
     """Plotting function for Optimization RO frequency."""
     figures = []
-    freqs = data[qubit]["freq"]
+    freqs = data[target]["freq"]
     opacity = 1
     fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=1,
     )
     if fit is not None:
         fig.add_trace(
             go.Scatter(
                 x=freqs,
-                y=data[qubit]["assignment_fidelity"],
+                y=data[target]["assignment_fidelity"],
                 opacity=opacity,
                 showlegend=True,
             ),
             row=1,
             col=1,
         )
 
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 "Best Resonator Frequency [Hz]",
-                np.round(fit.best_freq[qubit], 4),
+                np.round(fit.best_freq[target], 4),
             )
         )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Resonator Frequencies [GHz]",
         yaxis_title="Assignment Fidelities",
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ResonatorFrequencyResults, platform: Platform, qubit: QubitId):
-    update.readout_frequency(results.best_freq[qubit], platform, qubit)
-    update.threshold(results.best_threshold[qubit], platform, qubit)
-    update.iq_angle(results.best_angle[qubit], platform, qubit)
+def _update(results: ResonatorFrequencyResults, platform: Platform, target: QubitId):
+    update.readout_frequency(results.best_freq[target], platform, target)
+    update.threshold(results.best_threshold[target], platform, target)
+    update.iq_angle(results.best_angle[target], platform, target)
 
 
 resonator_frequency = Routine(_acquisition, _fit, _plot, _update)
 """"Optimization RO frequency Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_SNR.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.resonator_spectroscopy import (
     resonator_spectroscopy,
 )
 from qibocal.protocols.characterization.utils import (
     HZ_TO_GHZ,
     PowerLevel,
     table_dict,
@@ -87,15 +87,15 @@
             obj.power_level = PowerLevel(obj.power_level)  # pylint: disable=E1101
         return obj
 
 
 def _acquisition(
     params: ResonatorTWPAFrequencyParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> ResonatorTWPAFrequencyData:
     r"""
     Data acquisition for TWPA frequency optmization using SNR.
     This protocol perform a classification protocol for twpa frequencies
     in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
     with step frequency_step.
 
@@ -114,39 +114,39 @@
     )
 
     TWPAFrequency_range = np.arange(
         -params.twpa_freq_width // 2, params.twpa_freq_width // 2, params.twpa_freq_step
     )
 
     initial_twpa_freq = {}
-    for qubit in qubits:
+    for qubit in targets:
         initial_twpa_freq[qubit] = float(
             platform.qubits[qubit].twpa.local_oscillator.frequency
         )
 
     for _freq in TWPAFrequency_range:
-        for qubit in qubits:
-            qubits[qubit].twpa.local_oscillator.frequency = (
+        for qubit in targets:
+            platform.qubits[qubit].twpa.local_oscillator.frequency = (
                 initial_twpa_freq[qubit] + _freq
             )
 
         resonator_spectroscopy_data, _ = resonator_spectroscopy.acquisition(
             resonator_spectroscopy.parameters_type.load(
                 {
                     "freq_width": params.freq_width,
                     "freq_step": params.freq_step,
                     "power_level": params.power_level,
                     "nshots": params.nshots,
                 }
             ),
             platform,
-            qubits,
+            targets,
         )
 
-        for qubit in qubits:
+        for qubit in targets:
             data.register_qubit(
                 ResonatorTWPAFrequencyType,
                 (qubit),
                 dict(
                     signal=resonator_spectroscopy_data[qubit].signal,
                     phase=resonator_spectroscopy_data[qubit].phase,
                     freq=resonator_spectroscopy_data[qubit].freq,
@@ -184,15 +184,15 @@
     else:
         return ResonatorTWPAFrequencyResults(
             twpa_frequency=twpa_frequency,
             frequency=frequency,
         )
 
 
-def _plot(data: ResonatorTWPAFrequencyData, fit: ResonatorTWPAFrequencyResults, qubit):
+def _plot(data: ResonatorTWPAFrequencyData, fit: ResonatorTWPAFrequencyResults, target):
     """Plotting for ResonatorTWPAFrequency."""
 
     figures = []
     fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=2,
@@ -201,15 +201,15 @@
         subplot_titles=(
             "Signal [a.u.]",
             "Phase [rad]",
         ),
     )
 
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     resonator_frequencies = qubit_data.freq * HZ_TO_GHZ
     twpa_frequencies = qubit_data.twpa_freq * HZ_TO_GHZ
 
     fig.add_trace(
         go.Heatmap(
             x=resonator_frequencies,
             y=twpa_frequencies,
@@ -232,24 +232,24 @@
         col=2,
     )
     fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
     fig.update_yaxes(title_text="TWPA Frequency [GHz]", row=1, col=2)
 
     if fit is not None:
         label_1 = "TWPA Frequency [Hz]"
-        twpa_frequency = np.round(fit.twpa_frequency[qubit])
-        if qubit in fit.bare_frequency:
+        twpa_frequency = np.round(fit.twpa_frequency[target])
+        if target in fit.bare_frequency:
             label_2 = "High Power Resonator Frequency [Hz]"
-            resonator_frequency = np.round(fit.bare_frequency[qubit])
+            resonator_frequency = np.round(fit.bare_frequency[target])
         else:
             label_2 = "Low Power Resonator Frequency [Hz]"
-            resonator_frequency = np.round(fit.frequency[qubit])
+            resonator_frequency = np.round(fit.frequency[target])
 
         summary = table_dict(
-            qubit,
+            target,
             [
                 label_2,
                 label_1,
             ],
             [
                 resonator_frequency,
                 twpa_frequency,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/frequency_power.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization import classification
 from qibocal.protocols.characterization.utils import HZ_TO_GHZ, table_dict, table_html
 
 
 @dataclass
 class TwpaFrequencyPowerParameters(Parameters):
     """Twpa Frequency Power runcard inputs."""
@@ -61,26 +61,26 @@
     best_angles: dict[QubitId, float] = field(default_factory=dict)
     best_thresholds: dict[QubitId, float] = field(default_factory=dict)
 
 
 def _acquisition(
     params: TwpaFrequencyPowerParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> TwpaFrequencyPowerData:
     r"""
     Data acquisition for TWPA frequency vs. power optmization.
     This protocol perform a classification protocol for twpa frequencies
     in the range [twpa_frequency - frequency_width / 2, twpa_frequency + frequency_width / 2]
     with step frequency_step and powers in the range [twpa_power - power_width / 2, twpa_power + power_width / 2]
 
     Args:
         params (:class:`TwpaFrequencyPowerParameters`): input parameters
         platform (:class:`Platform`): Qibolab's platform
-        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+        targets (list): list of qubit to be characterized
 
     Returns:
         data (:class:`TwpaFrequencyPowerData`)
     """
 
     data = TwpaFrequencyPowerData()
 
@@ -90,37 +90,37 @@
     power_range = np.arange(
         -params.power_width / 2, params.power_width / 2, params.power_step
     )
     data = TwpaFrequencyPowerData()
 
     initial_twpa_freq = {}
     initial_twpa_power = {}
-    for qubit in qubits:
+    for qubit in targets:
         initial_twpa_freq[qubit] = platform.qubits[
             qubit
         ].twpa.local_oscillator.frequency
         initial_twpa_power[qubit] = platform.qubits[qubit].twpa.local_oscillator.power
 
         for freq in freq_range:
             platform.qubits[qubit].twpa.local_oscillator.frequency = (
                 initial_twpa_freq[qubit] + freq
             )
 
             for power in power_range:
-                for qubit in qubits:
+                for qubit in targets:
                     platform.qubits[qubit].twpa.local_oscillator.power = (
                         initial_twpa_power[qubit] + power
                     )
 
                 classification_data = classification._acquisition(
                     classification.SingleShotClassificationParameters.load(
                         {"nshots": params.nshots}
                     ),
                     platform,
-                    qubits,
+                    targets,
                 )
 
                 classification_result = classification._fit(classification_data)
 
                 data.register_qubit(
                     TwpaFrequencyPowerType,
                     (qubit),
@@ -168,33 +168,35 @@
         best_power,
         best_fidelity,
         best_angles=best_angle,
         best_thresholds=best_threshold,
     )
 
 
-def _plot(data: TwpaFrequencyPowerData, fit: TwpaFrequencyPowerResults, qubit):
+def _plot(
+    data: TwpaFrequencyPowerData, fit: TwpaFrequencyPowerResults, target: QubitId
+):
     """Plotting function that shows the assignment fidelity
     for different values of the twpa frequency for a single qubit"""
 
     figures = []
     fitting_report = ""
     if fit is not None:
-        qubit_data = data.data[qubit]
+        qubit_data = data.data[target]
         fidelities = qubit_data["assignment_fidelity"]
         frequencies = qubit_data["freq"]
         powers = qubit_data["power"]
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["Best assignment fidelity", "TWPA Frequency [Hz]", "TWPA Power [dBm]"],
                 [
-                    np.round(fit.best_fidelities[qubit], 3),
-                    fit.best_freqs[qubit],
-                    np.round(fit.best_powers[qubit], 3),
+                    np.round(fit.best_fidelities[target], 3),
+                    fit.best_freqs[target],
+                    np.round(fit.best_powers[target], 3),
                 ],
             )
         )
 
         fig = go.Figure(
             [
                 go.Heatmap(
@@ -210,16 +212,16 @@
         )
 
         figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: TwpaFrequencyPowerResults, platform: Platform, qubit: QubitId):
-    update.twpa_frequency(results.best_freqs[qubit], platform, qubit)
-    update.twpa_power(results.best_powers[qubit], platform, qubit)
-    update.iq_angle(results.best_angles[qubit], platform, qubit)
-    update.threshold(results.best_thresholds[qubit], platform, qubit)
+def _update(results: TwpaFrequencyPowerResults, platform: Platform, target: QubitId):
+    update.twpa_frequency(results.best_freqs[target], platform, target)
+    update.twpa_power(results.best_powers[target], platform, target)
+    update.iq_angle(results.best_angles[target], platform, target)
+    update.threshold(results.best_thresholds[target], platform, target)
 
 
 twpa_frequency_power = Routine(_acquisition, _fit, _plot, _update)
 """Twpa frequency Routine  object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import plotly.graph_objects as go
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Parameters, Results, Routine
 from qibocal.protocols.characterization import classification
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
 from . import frequency
 
 
 @dataclass
@@ -50,60 +50,60 @@
     best_angles: dict[QubitId, float] = field(default_factory=dict)
     best_thresholds: dict[QubitId, float] = field(default_factory=dict)
 
 
 def _acquisition(
     params: TwpaPowerParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> TwpaPowerData:
     r"""
     Data acquisition for TWPA power optmization.
     This protocol perform a classification protocol for twpa powers
     in the range [twpa_power - power_width / 2, twpa_power + power_width / 2]
     with step power_step.
 
     Args:
         params (:class:`TwpaPowerParameters`): input parameters
         platform (:class:`Platform`): Qibolab's platform
-        qubits (dict): dict of target :class:`Qubit` objects to be characterized
+        targets (list): list of QubitId to be characterized
 
     Returns:
         data (:class:`TwpaFrequencyData`)
     """
 
     data = TwpaPowerData()
 
     power_range = np.arange(
         -params.power_width / 2, params.power_width / 2, params.power_step
     )
 
     initial_twpa_power = {}
-    for qubit in qubits:
+    for qubit in targets:
         initial_twpa_power[qubit] = platform.qubits[qubit].twpa.local_oscillator.power
         data.powers[qubit] = list(
             platform.qubits[qubit].twpa.local_oscillator.power + power_range
         )
 
     for power in power_range:
-        for qubit in qubits:
+        for qubit in targets:
             platform.qubits[qubit].twpa.local_oscillator.power = (
                 initial_twpa_power[qubit] + power
             )
 
         classification_data = classification._acquisition(
             classification.SingleShotClassificationParameters.load(
                 {"nshots": params.nshots}
             ),
             platform,
-            qubits,
+            targets,
         )
         classification_result = classification._fit(classification_data)
 
-        for qubit in qubits:
+        for qubit in targets:
             data.register_qubit(
                 TwpaPowerType,
                 (qubit),
                 dict(
                     power=np.array(
                         [float(platform.qubits[qubit].twpa.local_oscillator.power)]
                     ),
@@ -137,32 +137,32 @@
         best_power,
         best_fidelity,
         best_angles=best_angle,
         best_thresholds=best_threshold,
     )
 
 
-def _plot(data: TwpaPowerData, fit: TwpaPowerResults, qubit):
+def _plot(data: TwpaPowerData, fit: TwpaPowerResults, target: QubitId):
     """Plotting function that shows the assignment fidelity
     for different values of the twpa power for a single qubit."""
 
     figures = []
     fitting_report = ""
 
     if fit is not None:
-        qubit_data = data.data[qubit]
+        qubit_data = data.data[target]
         fidelities = qubit_data["assignment_fidelity"]
         powers = qubit_data["power"]
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 ["Best assignment fidelity", "TWPA Power [dBm]"],
                 [
-                    np.round(fit.best_fidelities[qubit], 3),
-                    np.round(fit.best_powers[qubit], 3),
+                    np.round(fit.best_fidelities[target], 3),
+                    np.round(fit.best_powers[target], 3),
                 ],
             )
         )
         fig = go.Figure([go.Scatter(x=powers, y=fidelities, name="Fidelity")])
         figures.append(fig)
 
         fig.update_layout(
@@ -170,15 +170,15 @@
             xaxis_title="TWPA Power [dB]",
             yaxis_title="Assignment Fidelity",
         )
 
     return figures, fitting_report
 
 
-def _update(results: TwpaPowerResults, platform: Platform, qubit: QubitId):
-    update.twpa_power(results.best_powers[qubit], platform, qubit)
-    update.iq_angle(results.best_angles[qubit], platform, qubit)
-    update.threshold(results.best_thresholds[qubit], platform, qubit)
+def _update(results: TwpaPowerResults, platform: Platform, target: QubitId):
+    update.twpa_power(results.best_powers[target], platform, target)
+    update.iq_angle(results.best_angles[target], platform, target)
+    update.threshold(results.best_thresholds[target], platform, target)
 
 
 twpa_power = Routine(_acquisition, _fit, _plot, _update)
 """Twpa power Routine  object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power_SNR.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/readout_optimization/twpa_calibration/power_SNR.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab.platform import Platform
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.resonator_spectroscopy import (
     resonator_spectroscopy,
 )
 from qibocal.protocols.characterization.utils import (
     HZ_TO_GHZ,
     PowerLevel,
     table_dict,
@@ -87,15 +87,15 @@
             obj.power_level = PowerLevel(obj.power_level)  # pylint: disable=E1101
         return obj
 
 
 def _acquisition(
     params: ResonatorTWPAPowerParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> ResonatorTWPAPowerData:
     r"""
     Data acquisition for TWPA power optmization using SNR.
     This protocol perform a classification protocol for twpa powers
     in the range [twpa_power - frequency_width / 2, twpa_power + frequency_width / 2]
     with step frequency_step.
 
@@ -114,37 +114,39 @@
     )
 
     TWPAPower_range = np.arange(
         -params.twpa_pow_width // 2, params.twpa_pow_width // 2, params.twpa_pow_step
     )
 
     initial_twpa_pow = {}
-    for qubit in qubits:
+    for qubit in targets:
         initial_twpa_pow[qubit] = float(
             platform.qubits[qubit].twpa.local_oscillator.power
         )
 
     for _pow in TWPAPower_range:
-        for qubit in qubits:
-            qubits[qubit].twpa.local_oscillator.power = initial_twpa_pow[qubit] + _pow
+        for qubit in targets:
+            platform.qubits[qubit].twpa.local_oscillator.power = (
+                initial_twpa_pow[qubit] + _pow
+            )
 
         resonator_spectroscopy_data, _ = resonator_spectroscopy.acquisition(
             resonator_spectroscopy.parameters_type.load(
                 {
                     "freq_width": params.freq_width,
                     "freq_step": params.freq_step,
                     "power_level": params.power_level,
                     "nshots": params.nshots,
                 }
             ),
             platform,
-            qubits,
+            targets,
         )
 
-        for qubit in qubits:
+        for qubit in targets:
             data.register_qubit(
                 ResonatorTWPAPowerType,
                 (qubit),
                 dict(
                     signal=resonator_spectroscopy_data.data[qubit].signal,
                     phase=resonator_spectroscopy_data.data[qubit].phase,
                     freq=resonator_spectroscopy_data.data[qubit].freq,
@@ -182,15 +184,15 @@
     else:
         return ResonatorTWPAPowerResults(
             twpa_power=twpa_power,
             frequency=frequency,
         )
 
 
-def _plot(data: ResonatorTWPAPowerData, fit: ResonatorTWPAPowerResults, qubit):
+def _plot(data: ResonatorTWPAPowerData, fit: ResonatorTWPAPowerResults, target):
     """Plotting for ResonatorTWPAPower."""
 
     figures = []
     fitting_report = ""
     fig = make_subplots(
         rows=1,
         cols=2,
@@ -199,15 +201,15 @@
         subplot_titles=(
             "Signal [a.u.]",
             "Phase [rad]",
         ),
     )
 
     fitting_report = ""
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     frequencies = qubit_data.freq * HZ_TO_GHZ
     powers = qubit_data.twpa_pow
 
     fig.add_trace(
         go.Heatmap(
             x=frequencies,
             y=powers,
@@ -230,24 +232,24 @@
         col=2,
     )
     fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
     fig.update_yaxes(title_text="TWPA Power [dBm]", row=1, col=2)
 
     if fit is not None:
         label_1 = "TWPA Power"
-        twpa_power = np.round(fit.twpa_power[qubit])
-        if qubit in fit.bare_frequency:
+        twpa_power = np.round(fit.twpa_power[target])
+        if target in fit.bare_frequency:
             label_2 = "High Power Resonator Frequency [Hz]"
-            resonator_frequency = np.round(fit.bare_frequency[qubit])
+            resonator_frequency = np.round(fit.bare_frequency[target])
         else:
             label_2 = "Low Power Resonator Frequency [Hz]"
-            resonator_frequency = np.round(fit.frequency[qubit])
+            resonator_frequency = np.round(fit.frequency[target])
 
         summary = table_dict(
-            qubit,
+            target,
             [
                 label_2,
                 label_1,
             ],
             [
                 resonator_frequency,
                 twpa_power,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_punchout.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/drag.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,269 +1,282 @@
 from dataclasses import dataclass, field
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
-from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
-from qibolab.sweeper import Parameter, Sweeper, SweeperType
+from scipy.optimize import curve_fit
+from scipy.signal import find_peaks
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
+from qibocal.config import log
 
-from .utils import HZ_TO_GHZ, fit_punchout, norm, table_dict, table_html
+from .utils import COLORBAND, COLORBAND_LINE, chi2_reduced, table_dict, table_html
+
+# TODO: add errors in fitting
 
 
 @dataclass
-class ResonatorPunchoutParameters(Parameters):
-    """ "ResonatorPunchout runcard inputs."""
+class DragTuningParameters(Parameters):
+    """DragTuning runcard inputs."""
 
-    freq_width: int
-    """Width for frequency sweep relative  to the readout frequency [Hz]."""
-    freq_step: int
-    """Frequency step for sweep [Hz]."""
-    min_amp_factor: float
-    """Minimum amplitude multiplicative factor."""
-    max_amp_factor: float
-    """Maximum amplitude multiplicative factor."""
-    step_amp_factor: float
-    """Step amplitude multiplicative factor."""
-    amplitude: float = None
-    """Initial readout amplitude."""
+    beta_start: float
+    """DRAG pulse beta start sweep parameter."""
+    beta_end: float
+    """DRAG pulse beta end sweep parameter."""
+    beta_step: float
+    """DRAG pulse beta sweep step parameter."""
+    unrolling: bool = False
+    """If ``True`` it uses sequence unrolling to deploy multiple sequences in a single instrument call.
+    Defaults to ``False``."""
 
 
 @dataclass
-class ResonatorPunchoutResults(Results):
-    """ResonatorPunchout outputs."""
+class DragTuningResults(Results):
+    """DragTuning outputs."""
+
+    betas: dict[QubitId, float]
+    """Optimal beta paramter for each qubit."""
+    fitted_parameters: dict[QubitId, dict[str, float]]
+    """Raw fitting output."""
+    chi2: dict[QubitId, tuple[float, Optional[float]]] = field(default_factory=dict)
+    """Chi2 calculation."""
+
 
-    readout_frequency: dict[QubitId, float]
-    """Readout frequency [GHz] for each qubit."""
-    bare_frequency: Optional[dict[QubitId, float]]
-    """Bare resonator frequency [GHz] for each qubit."""
-    readout_amplitude: dict[QubitId, float]
-    """Readout amplitude for each qubit."""
-
-
-ResPunchoutType = np.dtype(
-    [
-        ("freq", np.float64),
-        ("amp", np.float64),
-        ("signal", np.float64),
-        ("phase", np.float64),
-    ]
+DragTuningType = np.dtype(
+    [("prob", np.float64), ("error", np.float64), ("beta", np.float64)]
 )
-"""Custom dtype for resonator punchout."""
 
 
 @dataclass
-class ResonatorPunchoutData(Data):
-    """ResonatorPunchout data acquisition."""
+class DragTuningData(Data):
+    """DragTuning acquisition outputs."""
 
-    resonator_type: str
-    """Resonator type."""
-    amplitudes: dict[QubitId, float]
-    """Amplitudes provided by the user."""
-    data: dict[QubitId, npt.NDArray[ResPunchoutType]] = field(default_factory=dict)
+    data: dict[QubitId, npt.NDArray[DragTuningType]] = field(default_factory=dict)
     """Raw data acquired."""
 
-    def register_qubit(self, qubit, freq, amp, signal, phase):
-        """Store output for single qubit."""
-        size = len(freq) * len(amp)
-        frequency, amplitude = np.meshgrid(freq, amp)
-        ar = np.empty(size, dtype=ResPunchoutType)
-        ar["freq"] = frequency.ravel()
-        ar["amp"] = amplitude.ravel()
-        ar["signal"] = signal.ravel()
-        ar["phase"] = phase.ravel()
-        self.data[qubit] = np.rec.array(ar)
-
 
 def _acquisition(
-    params: ResonatorPunchoutParameters,
+    params: DragTuningParameters,
     platform: Platform,
-    qubits: Qubits,
-) -> ResonatorPunchoutData:
-    """Data acquisition for Punchout over amplitude."""
-    # create a sequence of pulses for the experiment:
-    # MZ
-
-    # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
-    sequence = PulseSequence()
+    targets: list[QubitId],
+) -> DragTuningData:
+    r"""
+    Data acquisition for drag pulse tuning experiment.
+    See https://arxiv.org/pdf/1504.06597.pdf Fig. 2 (c).
+    """
+    # define the parameter to sweep and its range:
+    # qubit drive DRAG pulse beta parameter
+    beta_param_range = np.arange(
+        params.beta_start, params.beta_end, params.beta_step
+    ).round(4)
+
+    data = DragTuningData()
+
+    sequences, all_ro_pulses = [], []
+    for beta_param in beta_param_range:
+        sequence = PulseSequence()
+        ro_pulses = {}
+        for qubit in targets:
+            RX_drag_pulse = platform.create_RX_drag_pulse(
+                qubit, start=0, beta=beta_param
+            )
+            RX_drag_pulse_minus = platform.create_RX_drag_pulse(
+                qubit, start=RX_drag_pulse.finish, beta=beta_param, relative_phase=np.pi
+            )
+            ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+                qubit, start=RX_drag_pulse_minus.finish
+            )
 
-    ro_pulses = {}
-    amplitudes = {}
-    for qubit in qubits:
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
-        if params.amplitude is not None:
-            ro_pulses[qubit].amplitude = params.amplitude
-
-        amplitudes[qubit] = ro_pulses[qubit].amplitude
-        sequence.add(ro_pulses[qubit])
-
-    # define the parameters to sweep and their range:
-    # resonator frequency
-    delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
-    )
-    freq_sweeper = Sweeper(
-        Parameter.frequency,
-        delta_frequency_range,
-        [ro_pulses[qubit] for qubit in qubits],
-        type=SweeperType.OFFSET,
+            sequence.add(RX_drag_pulse)
+            sequence.add(RX_drag_pulse_minus)
+            sequence.add(ro_pulses[qubit])
+        sequences.append(sequence)
+        all_ro_pulses.append(ro_pulses)
+
+    options = ExecutionParameters(
+        nshots=params.nshots,
+        relaxation_time=params.relaxation_time,
+        acquisition_type=AcquisitionType.DISCRIMINATION,
+        averaging_mode=AveragingMode.SINGLESHOT,
     )
+    # execute the pulse sequence
+    if params.unrolling:
+        results = platform.execute_pulse_sequences(sequences, options)
+
+    elif not params.unrolling:
+        results = [
+            platform.execute_pulse_sequence(sequence, options) for sequence in sequences
+        ]
+
+    for ig, (beta, ro_pulses) in enumerate(zip(beta_param_range, all_ro_pulses)):
+        for qubit in targets:
+            serial = ro_pulses[qubit].serial
+            if params.unrolling:
+                result = results[serial][ig]
+            else:
+                result = results[ig][serial]
+            prob = result.probability(state=0)
+            # store the results
+            data.register_qubit(
+                DragTuningType,
+                (qubit),
+                dict(
+                    prob=np.array([prob]),
+                    error=np.array([np.sqrt(prob * (1 - prob) / params.nshots)]),
+                    beta=np.array([beta]),
+                ),
+            )
 
-    # amplitude
-    amplitude_range = np.arange(
-        params.min_amp_factor, params.max_amp_factor, params.step_amp_factor
-    )
-    amp_sweeper = Sweeper(
-        Parameter.amplitude,
-        amplitude_range,
-        [ro_pulses[qubit] for qubit in qubits],
-        type=SweeperType.FACTOR,
-    )
+    return data
 
-    data = ResonatorPunchoutData(
-        amplitudes=amplitudes,
-        resonator_type=platform.resonator_type,
-    )
 
-    results = platform.sweep(
-        sequence,
-        ExecutionParameters(
-            nshots=params.nshots,
-            relaxation_time=params.relaxation_time,
-            acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
-        ),
-        amp_sweeper,
-        freq_sweeper,
-    )
+def drag_fit(x, offset, amplitude, period, phase):
+    return offset + amplitude * np.cos(2 * np.pi * x / period + phase)
 
-    # retrieve the results for every qubit
-    for qubit, ro_pulse in ro_pulses.items():
-        # average signal, phase, i and q over the number of shots defined in the runcard
-        result = results[ro_pulse.serial]
-        data.register_qubit(
-            qubit,
-            signal=result.magnitude,
-            phase=result.phase,
-            freq=delta_frequency_range + ro_pulse.frequency,
-            amp=amplitude_range * amplitudes[qubit],
-        )
 
-    return data
+def _fit(data: DragTuningData) -> DragTuningResults:
+    qubits = data.qubits
+    betas_optimal = {}
+    fitted_parameters = {}
+    chi2 = {}
 
+    for qubit in qubits:
+        qubit_data = data[qubit]
+        beta_params = qubit_data.beta
+        prob = qubit_data.prob
+
+        beta_min = np.min(beta_params)
+        beta_max = np.max(beta_params)
+        normalized_beta = (beta_params - beta_min) / (beta_max - beta_min)
+
+        # Guessing period using fourier transform
+        ft = np.fft.rfft(prob)
+        mags = abs(ft)
+        local_maxima = find_peaks(mags, threshold=1)[0]
+        index = local_maxima[0] if len(local_maxima) > 0 else None
+        # 0.5 hardcoded guess for less than one oscillation
+        f = (
+            beta_params[index] / (beta_params[1] - beta_params[0])
+            if index is not None
+            else 0.5
+        )
+        pguess = [0.5, 0.5, 1 / f, 0]
 
-def _fit(data: ResonatorPunchoutData, fit_type="amp") -> ResonatorPunchoutResults:
-    """Fit frequency and attenuation at high and low power for a given resonator."""
+        try:
+            popt, _ = curve_fit(
+                drag_fit,
+                normalized_beta,
+                prob,
+                p0=pguess,
+                maxfev=100000,
+                bounds=(
+                    [0, 0, 0, -np.pi],
+                    [1, 1, np.inf, np.pi],
+                ),
+                sigma=qubit_data.error,
+            )
+            translated_popt = [
+                popt[0],
+                popt[1],
+                popt[2] * (beta_max - beta_min),
+                popt[3] - 2 * np.pi * beta_min / popt[2] / (beta_max - beta_min),
+            ]
+            fitted_parameters[qubit] = translated_popt
+            predicted_prob = drag_fit(beta_params, *translated_popt)
+            betas_optimal[qubit] = beta_params[np.argmax(predicted_prob)]
+            chi2[qubit] = (
+                chi2_reduced(
+                    prob,
+                    predicted_prob,
+                    qubit_data.error,
+                ),
+                np.sqrt(2 / len(prob)),
+            )
+        except Exception as e:
+            log.warning(f"drag_tuning_fit failed for qubit {qubit} due to {e}.")
+
+    return DragTuningResults(betas_optimal, fitted_parameters, chi2=chi2)
 
-    return ResonatorPunchoutResults(*fit_punchout(data, fit_type))
 
+def _plot(data: DragTuningData, target: QubitId, fit: DragTuningResults):
+    """Plotting function for DragTuning."""
 
-def _plot(data: ResonatorPunchoutData, qubit, fit: ResonatorPunchoutResults = None):
-    """Plotting function for ResonatorPunchout."""
     figures = []
     fitting_report = ""
-    fig = make_subplots(
-        rows=1,
-        cols=2,
-        horizontal_spacing=0.1,
-        vertical_spacing=0.2,
-        subplot_titles=(
-            "Normalised Signal [a.u.]",
-            "phase [rad]",
-        ),
-    )
-    qubit_data = data[qubit]
-    frequencies = qubit_data.freq * HZ_TO_GHZ
-    amplitudes = qubit_data.amp
-    n_amps = len(np.unique(qubit_data.amp))
-    n_freq = len(np.unique(qubit_data.freq))
-    for i in range(n_amps):
-        qubit_data.signal[i * n_freq : (i + 1) * n_freq] = norm(
-            qubit_data.signal[i * n_freq : (i + 1) * n_freq]
-        )
 
-    fig.add_trace(
-        go.Heatmap(
-            x=frequencies,
-            y=amplitudes,
-            z=qubit_data.signal,
-            colorbar_x=0.46,
-        ),
-        row=1,
-        col=1,
-    )
-
-    fig.add_trace(
-        go.Heatmap(
-            x=frequencies,
-            y=amplitudes,
-            z=qubit_data.phase,
-            colorbar_x=1.01,
-        ),
-        row=1,
-        col=2,
+    qubit_data = data[target]
+    fig = go.Figure(
+        [
+            go.Scatter(
+                x=qubit_data.beta,
+                y=qubit_data.prob,
+                opacity=1,
+                mode="lines",
+                name="Probability",
+                showlegend=True,
+                legendgroup="Probability",
+            ),
+            go.Scatter(
+                x=np.concatenate((qubit_data.beta, qubit_data.beta[::-1])),
+                y=np.concatenate(
+                    (
+                        qubit_data.prob + qubit_data.error,
+                        (qubit_data.prob - qubit_data.error)[::-1],
+                    )
+                ),
+                fill="toself",
+                fillcolor=COLORBAND,
+                line=dict(color=COLORBAND_LINE),
+                showlegend=True,
+                name="Errors",
+            ),
+        ]
     )
 
+    # add fitting traces
     if fit is not None:
+        beta_range = np.linspace(
+            min(qubit_data.beta),
+            max(qubit_data.beta),
+            20,
+        )
+
         fig.add_trace(
             go.Scatter(
-                x=[
-                    fit.readout_frequency[qubit] * HZ_TO_GHZ,
-                ],
-                y=[
-                    fit.readout_amplitude[qubit],
-                ],
-                mode="markers",
-                marker=dict(
-                    size=8,
-                    color="gray",
-                    symbol="circle",
-                ),
-                name="Estimated readout point",
-                showlegend=True,
-            )
+                x=beta_range,
+                y=drag_fit(beta_range, *fit.fitted_parameters[target]),
+                name="Fit",
+                line=go.scatter.Line(dash="dot"),
+            ),
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
-                [
-                    "Low Power Resonator Frequency [Hz]",
-                    "Low Power readout amplitude [a.u.]",
-                    "High Power Resonator Frequency [Hz]",
-                ],
-                [
-                    np.round(fit.readout_frequency[qubit]),
-                    np.round(fit.readout_amplitude[qubit], 3),
-                    np.round(fit.bare_frequency[qubit]),
-                ],
+                target,
+                ["Optimal Beta Param", "Chi2 reduced"],
+                [(np.round(fit.betas[target], 4), 0), fit.chi2[target]],
+                display_error=True,
             )
         )
 
     fig.update_layout(
         showlegend=True,
-        legend=dict(orientation="h"),
+        xaxis_title="Beta parameter",
+        yaxis_title="Ground State Probability",
     )
 
-    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=1)
-    fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
-    fig.update_yaxes(title_text="Amplitude [a.u.]", row=1, col=1)
-
     figures.append(fig)
 
     return figures, fitting_report
 
 
-def _update(results: ResonatorPunchoutResults, platform: Platform, qubit: QubitId):
-    update.readout_frequency(results.readout_frequency[qubit], platform, qubit)
-    update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
-    update.readout_amplitude(results.readout_amplitude[qubit], platform, qubit)
+def _update(results: DragTuningResults, platform: Platform, target: QubitId):
+    update.drag_pulse_beta(results.betas[target], platform, target)
 
 
-resonator_punchout = Routine(_acquisition, _fit, _plot, _update)
-"""ResonatorPunchout Routine object."""
+drag_tuning = Routine(_acquisition, _fit, _plot, _update)
+"""DragTuning Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/resonator_punchout_attenuation.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from .utils import HZ_TO_GHZ, fit_punchout, norm, table_dict, table_html
 
 
 @dataclass
 class ResonatorPunchoutAttenuationParameters(Parameters):
     """ResonatorPunchoutAttenuation runcard inputs."""
@@ -76,46 +76,46 @@
         ar["phase"] = phase.ravel()
         self.data[qubit] = np.rec.array(ar)
 
 
 def _acquisition(
     params: ResonatorPunchoutAttenuationParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitId],
 ) -> ResonatorPunchoutAttenuationData:
     """Data acquisition for Punchout over attenuation."""
     # create a sequence of pulses for the experiment:
     # MZ
 
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
 
     ro_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
         sequence.add(ro_pulses[qubit])
 
     # define the parameters to sweep and their range:
     # resonator frequency
     delta_frequency_range = np.arange(
         -params.freq_width // 2, params.freq_width // 2, params.freq_step
     )
     freq_sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        [ro_pulses[qubit] for qubit in qubits],
+        [ro_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
     # attenuation
     attenuation_range = np.arange(params.min_att, params.max_att, params.step_att)
     att_sweeper = Sweeper(
         Parameter.attenuation,
         attenuation_range,
-        qubits=list(qubits.values()),
+        qubits=[platform.qubits[qubit] for qubit in targets],
         type=SweeperType.ABSOLUTE,
     )
 
     data = ResonatorPunchoutAttenuationData(resonator_type=platform.resonator_type)
 
     results = platform.sweep(
         sequence,
@@ -126,15 +126,15 @@
             averaging_mode=AveragingMode.CYCLIC,
         ),
         att_sweeper,
         freq_sweeper,
     )
 
     # retrieve the results for every qubit
-    for qubit in qubits:
+    for qubit in targets:
         result = results[ro_pulses[qubit].serial]
         data.register_qubit(
             qubit,
             signal=result.magnitude,
             phase=result.phase,
             freq=delta_frequency_range + ro_pulses[qubit].frequency,
             att=attenuation_range,
@@ -154,15 +154,15 @@
     """Fit frequency and attenuation at high and low power for a given resonator."""
 
     return ResonatorPunchoutAttenuationResults(*fit_punchout(data, fit_type))
 
 
 def _plot(
     data: ResonatorPunchoutAttenuationData,
-    qubit,
+    target: QubitId,
     fit: ResonatorPunchoutAttenuationResults = None,
 ):
     """Plotting for ResonatorPunchoutAttenuation."""
 
     figures = []
     fitting_report = ""
     fig = make_subplots(
@@ -172,15 +172,15 @@
         vertical_spacing=0.2,
         subplot_titles=(
             "Normalised Signal [a.u.]",
             "phase [rad]",
         ),
     )
 
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     frequencies = qubit_data.freq * HZ_TO_GHZ
     attenuations = qubit_data.att
     n_att = len(np.unique(qubit_data.att))
     n_freq = len(np.unique(qubit_data.freq))
     for i in range(n_att):
         qubit_data.signal[i * n_freq : (i + 1) * n_freq] = norm(
             qubit_data.signal[i * n_freq : (i + 1) * n_freq]
@@ -210,57 +210,57 @@
     )
     fig.update_xaxes(title_text="Frequency [GHz]", row=1, col=2)
 
     if fit is not None:
         fig.add_trace(
             go.Scatter(
                 x=[
-                    fit.readout_frequency[qubit] * HZ_TO_GHZ,
+                    fit.readout_frequency[target] * HZ_TO_GHZ,
                 ],
                 y=[
-                    fit.readout_attenuation[qubit],
+                    fit.readout_attenuation[target],
                 ],
                 mode="markers",
                 marker=dict(
                     size=8,
                     color="gray",
                     symbol="circle",
                 ),
                 name="Estimated readout point",
                 showlegend=True,
             )
         )
         fitting_report = table_html(
             table_dict(
-                qubit,
+                target,
                 [
                     "Low Power Resonator Frequency [Hz]",
                     "Readout Attenuation [dB]",
                     "High Power Resonator Frequency [Hz]",
                 ],
                 [
-                    np.round(fit.readout_frequency[qubit], 0),
-                    fit.readout_attenuation[qubit],
-                    np.round(fit.bare_frequency[qubit]),
+                    np.round(fit.readout_frequency[target], 0),
+                    fit.readout_attenuation[target],
+                    np.round(fit.bare_frequency[target]),
                 ],
             )
         )
     fig.update_layout(
         showlegend=True,
         legend=dict(orientation="h"),
     )
 
     figures.append(fig)
 
     return figures, fitting_report
 
 
 def _update(
-    results: ResonatorPunchoutAttenuationResults, platform: Platform, qubit: QubitId
+    results: ResonatorPunchoutAttenuationResults, platform: Platform, target: QubitId
 ):
-    update.readout_frequency(results.readout_frequency[qubit], platform, qubit)
-    update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
-    update.readout_attenuation(results.readout_attenuation[qubit], platform, qubit)
+    update.readout_frequency(results.readout_frequency[target], platform, target)
+    update.bare_resonator_frequency(results.bare_frequency[target], platform, target)
+    update.readout_attenuation(results.readout_attenuation[target], platform, target)
 
 
 resonator_punchout_attenuation = Routine(_acquisition, _fit, _plot, _update)
 """ResonatorPunchoutAttenuation Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/resonator_spectroscopy.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/qubit_spectroscopy_ef.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,200 +1,189 @@
-from dataclasses import dataclass, field
-from typing import Optional
+from dataclasses import asdict, dataclass, field
 
 import numpy as np
-import numpy.typing as npt
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Routine
 
-from .utils import PowerLevel, lorentzian_fit, spectroscopy_plot
+from .qubit_spectroscopy import (
+    QubitSpectroscopyData,
+    QubitSpectroscopyParameters,
+    QubitSpectroscopyResults,
+    _fit,
+)
+from .resonator_spectroscopy import ResSpecType
+from .utils import spectroscopy_plot, table_dict, table_html
 
+DEFAULT_ANHARMONICITY = 300e6
+"""Initial guess for anharmonicity."""
 
-@dataclass
-class ResonatorSpectroscopyParameters(Parameters):
-    """ResonatorSpectroscopy runcard inputs."""
 
-    freq_width: int
-    """Width for frequency sweep relative  to the readout frequency [Hz]."""
-    freq_step: int
-    """Frequency step for sweep [Hz]."""
-    power_level: PowerLevel
-    """Power regime (low or high). If low the readout frequency will be updated.
-    If high both the readout frequency and the bare resonator frequency will be updated."""
-    amplitude: Optional[float] = None
-    """Readout amplitude (optional). If defined, same amplitude will be used in all qubits.
-    Otherwise the default amplitude defined on the platform runcard will be used"""
-
-    def __post_init__(self):
-        # TODO: ask Alessandro if there is a proper way to pass Enum to class
-        self.power_level = PowerLevel(self.power_level)
+@dataclass
+class QubitSpectroscopyEFParameters(QubitSpectroscopyParameters):
+    """QubitSpectroscopyEF runcard inputs."""
 
 
 @dataclass
-class ResonatorSpectroscopyResults(Results):
-    """ResonatorSpectroscopy outputs."""
+class QubitSpectroscopyEFResults(QubitSpectroscopyResults):
+    """QubitSpectroscopyEF outputs."""
 
-    frequency: dict[QubitId, float] = field(metadata=dict(update="readout_frequency"))
-    """Readout frequency [GHz] for each qubit."""
-    fitted_parameters: dict[QubitId, list[float]]
-    """Raw fitted parameters."""
-    bare_frequency: Optional[dict[QubitId, float]] = field(
-        default_factory=dict, metadata=dict(update="bare_resonator_frequency")
-    )
-    """Bare resonator frequency [GHz] for each qubit."""
-    amplitude: Optional[dict[QubitId, float]] = field(
-        default_factory=dict, metadata=dict(update="readout_amplitude")
-    )
-    """Readout amplitude for each qubit."""
-    attenuation: Optional[dict[QubitId, int]] = field(
-        default_factory=dict, metadata=dict(update="readout_attenuation")
-    )
-    """Readout attenuation [dB] for each qubit."""
+    anharmonicity: dict[QubitId, float] = field(default_factory=dict)
 
 
-ResSpecType = np.dtype(
-    [("freq", np.float64), ("signal", np.float64), ("phase", np.float64)]
-)
-"""Custom dtype for resonator spectroscopy."""
+@dataclass
+class QubitSpectroscopyEFData(QubitSpectroscopyData):
+    """QubitSpectroscopy acquisition outputs."""
 
+    drive_frequencies: dict[QubitId, float] = field(default_factory=dict)
 
-@dataclass
-class ResonatorSpectroscopyData(Data):
-    """Data structure for resonator spectroscopy."""
 
-    resonator_type: str
-    """Resonator type."""
-    amplitudes: dict[QubitId, float]
-    """Amplitudes provided by the user."""
-    data: dict[QubitId, npt.NDArray[ResSpecType]] = field(default_factory=dict)
-    """Raw data acquired."""
-    power_level: Optional[PowerLevel] = None
-    """Power regime of the resonator."""
-
-    @classmethod
-    def load(cls, path):
-        obj = super().load(path)
-        # Instantiate PowerLevel object
-        if obj.power_level is not None:  # pylint: disable=E1101
-            obj.power_level = PowerLevel(obj.power_level)  # pylint: disable=E1101
-        return obj
+def _fit_ef(data: QubitSpectroscopyEFData) -> QubitSpectroscopyEFResults:
+    results = _fit(data)
+    anharmoncities = {
+        qubit: data.drive_frequencies[qubit] - results.frequency[qubit]
+        for qubit in data.qubits
+        if qubit in results
+    }
+    params = asdict(results)
+    return QubitSpectroscopyEFResults(anharmonicity=anharmoncities, **params)
 
 
 def _acquisition(
-    params: ResonatorSpectroscopyParameters, platform: Platform, qubits: Qubits
-) -> ResonatorSpectroscopyData:
-    """Data acquisition for resonator spectroscopy."""
-    # create a sequence of pulses for the experiment:
-    # MZ
+    params: QubitSpectroscopyEFParameters, platform: Platform, targets: list[QubitId]
+) -> QubitSpectroscopyEFData:
+    """Data acquisition for qubit spectroscopy ef protocol.
+
+    Similar to a qubit spectroscopy with the difference that the qubit is first
+    excited to the state 1. This protocols aims at finding the transition frequency between
+    state 1 and the state 2. The anharmonicity is also computed.
+
+    If the RX12 frequency is not present in the runcard the sweep is performed around the
+    qubit drive frequency shifted by DEFAULT_ANHARMONICITY, an hardcoded parameter editable
+    in this file.
 
+    """
+    # create a sequence of pulses for the experiment:
+    # long drive probing pulse - MZ
     # taking advantage of multiplexing, apply the same set of gates to all qubits in parallel
     sequence = PulseSequence()
     ro_pulses = {}
+    qd_pulses = {}
+    rx_pulses = {}
     amplitudes = {}
+    drive_frequencies = {}
+    for qubit in targets:
+        rx_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
+        drive_frequencies[qubit] = rx_pulses[qubit].frequency
+        qd_pulses[qubit] = platform.create_qubit_drive_pulse(
+            qubit, start=rx_pulses[qubit].finish, duration=params.drive_duration
+        )
+        if platform.qubits[qubit].native_gates.RX12.frequency is None:
+            qd_pulses[qubit].frequency = (
+                rx_pulses[qubit].frequency - DEFAULT_ANHARMONICITY
+            )
+        else:
+            qd_pulses[qubit].frequency = platform.qubits[
+                qubit
+            ].native_gates.RX12.frequency
+
+        if params.drive_amplitude is not None:
+            qd_pulses[qubit].amplitude = params.drive_amplitude
 
-    for qubit in qubits:
-        ro_pulses[qubit] = platform.create_qubit_readout_pulse(qubit, start=0)
-        if params.amplitude is not None:
-            ro_pulses[qubit].amplitude = params.amplitude
-        amplitudes[qubit] = ro_pulses[qubit].amplitude
+        amplitudes[qubit] = qd_pulses[qubit].amplitude
 
+        ro_pulses[qubit] = platform.create_qubit_readout_pulse(
+            qubit, start=qd_pulses[qubit].finish
+        )
+        sequence.add(rx_pulses[qubit])
+        sequence.add(qd_pulses[qubit])
         sequence.add(ro_pulses[qubit])
 
     # define the parameter to sweep and its range:
+    # sweep only before qubit frequency
     delta_frequency_range = np.arange(
-        -params.freq_width // 2, params.freq_width // 2, params.freq_step
+        -params.freq_width, params.freq_width, params.freq_step
     )
     sweeper = Sweeper(
         Parameter.frequency,
         delta_frequency_range,
-        pulses=[ro_pulses[qubit] for qubit in qubits],
+        pulses=[qd_pulses[qubit] for qubit in targets],
         type=SweeperType.OFFSET,
     )
 
-    data = ResonatorSpectroscopyData(
-        amplitudes=amplitudes,
-        power_level=params.power_level,
+    # Create data structure for data acquisition.
+    data = QubitSpectroscopyEFData(
         resonator_type=platform.resonator_type,
+        amplitudes=amplitudes,
+        drive_frequencies=drive_frequencies,
     )
 
     results = platform.sweep(
         sequence,
         ExecutionParameters(
             nshots=params.nshots,
             relaxation_time=params.relaxation_time,
             acquisition_type=AcquisitionType.INTEGRATION,
-            averaging_mode=AveragingMode.CYCLIC,
+            averaging_mode=AveragingMode.SINGLESHOT,
         ),
         sweeper,
     )
 
     # retrieve the results for every qubit
-    for qubit in qubits:
-        result = results[ro_pulses[qubit].serial]
+    for qubit, ro_pulse in ro_pulses.items():
+        result = results[ro_pulse.serial]
         # store the results
         data.register_qubit(
             ResSpecType,
             (qubit),
             dict(
-                signal=result.magnitude,
-                phase=result.phase,
-                freq=delta_frequency_range + ro_pulses[qubit].frequency,
+                signal=np.abs(result.average.voltage),
+                phase=np.mean(result.phase, axis=0),
+                freq=delta_frequency_range + qd_pulses[qubit].frequency,
+                error_signal=result.average.std,
+                error_phase=np.std(result.phase, axis=0, ddof=1),
             ),
         )
     return data
 
 
-def _fit(data: ResonatorSpectroscopyData) -> ResonatorSpectroscopyResults:
-    """Post-processing function for ResonatorSpectroscopy."""
-    qubits = data.qubits
-    bare_frequency = {}
-    frequency = {}
-    fitted_parameters = {}
-    for qubit in qubits:
-        freq, fitted_params = lorentzian_fit(
-            data[qubit], resonator_type=data.resonator_type, fit="resonator"
+def _plot(
+    data: QubitSpectroscopyEFData, target: QubitId, fit: QubitSpectroscopyEFResults
+):
+    """Plotting function for QubitSpectroscopy."""
+    figures, report = spectroscopy_plot(data, target, fit)
+    if fit is not None:
+        report = table_html(
+            table_dict(
+                target,
+                [
+                    "Frequency 1->2 [Hz]",
+                    "Amplitude [a.u.]",
+                    "Anharmonicity [Hz]",
+                    "Chi2",
+                ],
+                [
+                    (fit.frequency[target], fit.error_fit_pars[target][1]),
+                    (fit.amplitude[target], fit.error_fit_pars[target][0]),
+                    (fit.anharmonicity[target], fit.error_fit_pars[target][2]),
+                    fit.chi2_reduced[target],
+                ],
+                display_error=True,
+            )
         )
-        if data.power_level is PowerLevel.high:
-            bare_frequency[qubit] = freq
-
-        frequency[qubit] = freq
-        fitted_parameters[qubit] = fitted_params
-
-    if data.power_level is PowerLevel.high:
-        return ResonatorSpectroscopyResults(
-            frequency=frequency,
-            fitted_parameters=fitted_parameters,
-            bare_frequency=bare_frequency,
-            amplitude=data.amplitudes,
-        )
-    else:
-        return ResonatorSpectroscopyResults(
-            frequency=frequency,
-            fitted_parameters=fitted_parameters,
-            amplitude=data.amplitudes,
-        )
-
-
-def _plot(data: ResonatorSpectroscopyData, qubit, fit: ResonatorSpectroscopyResults):
-    """Plotting function for ResonatorSpectroscopy."""
-    return spectroscopy_plot(data, qubit, fit)
 
+    return figures, report
 
-def _update(results: ResonatorSpectroscopyResults, platform: Platform, qubit: QubitId):
-    update.readout_frequency(results.frequency[qubit], platform, qubit)
 
-    # if this condition is satifisfied means that we are in the low power regime
-    # therefore we update also the readout amplitude
-    if len(results.bare_frequency) == 0:
-        update.readout_amplitude(results.amplitude[qubit], platform, qubit)
-    else:
-        update.bare_resonator_frequency(results.bare_frequency[qubit], platform, qubit)
+def _update(results: QubitSpectroscopyEFResults, platform: Platform, target: QubitId):
+    """Update w12 frequency"""
+    update.frequency_12_transition(results.frequency[target], platform, target)
+    update.anharmonicity(results.anharmonicity[target], platform, target)
 
 
-resonator_spectroscopy = Routine(_acquisition, _fit, _plot, _update)
-"""ResonatorSpectroscopy Routine object."""
+qubit_spectroscopy_ef = Routine(_acquisition, _fit_ef, _plot, _update)
+"""QubitSpectroscopyEF Routine object."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/calibrate_state_discrimination.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 SAMPLES_FACTOR = 16
 
 
 @dataclass
 class CalibrateStateDiscriminationParameters(Parameters):
     """Calibrate State Discrimination inputs."""
@@ -64,15 +64,17 @@
     """Resonator type."""
     data: dict[tuple[QubitId, int], npt.NDArray[CalibrateStateDiscriminationType]] = (
         field(default_factory=dict)
     )
 
 
 def _acquisition(
-    params: CalibrateStateDiscriminationParameters, platform: Platform, qubits: Qubits
+    params: CalibrateStateDiscriminationParameters,
+    platform: Platform,
+    targets: list[QubitId],
 ) -> CalibrateStateDiscriminationData:
     r"""
     Data acquisition for Calibrate State Discrimination experiment.
     Calculates the optimal kernel for the readout. It has to be run one qubit at a time.
     The kernels are stored in the result.npz generated on the report.
 
     Args:
@@ -85,15 +87,15 @@
     # create 2 sequences of pulses for the experiment:
     # sequence_0: I  - MZ
     # sequence_1: RX - MZ
 
     data = CalibrateStateDiscriminationData(resonator_type=platform.resonator_type)
 
     # TODO: test if qibolab supports multiplex with raw acquisition
-    for qubit in qubits:
+    for qubit in targets:
         sequence_0 = PulseSequence()
         sequence_1 = PulseSequence()
         sequence_1.add(platform.create_RX_pulse(qubit, start=0))
 
         sequence_0.add(
             platform.create_qubit_readout_pulse(qubit, start=sequence_0.finish)
         )
@@ -175,15 +177,15 @@
         kernel_state_zero[qubit] = kernel
 
     return CalibrateStateDiscriminationResults(data=kernel_state_zero)
 
 
 def _plot(
     data: CalibrateStateDiscriminationData,
-    qubit,
+    target,
     fit: CalibrateStateDiscriminationResults,
 ):
     """Plotting function for Calibrate State Discrimination."""
     # Plot kernels
     figures = []
     fitting_report = ""
 
@@ -194,16 +196,16 @@
             horizontal_spacing=0.1,
             vertical_spacing=0.1,
             subplot_titles=("Kernel state 0",),
         )
 
         fig.add_trace(
             go.Scatter(
-                x=np.arange(len(fit.data[qubit])),
-                y=np.abs(fit.data[qubit]),
+                x=np.arange(len(fit.data[target])),
+                y=np.abs(fit.data[target]),
                 opacity=1,
                 name="kernel state 0",
                 showlegend=True,
                 legendgroup="kernel state 0",
             ),
             row=1,
             col=1,
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/signal_experiments/time_of_flight_readout.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
 from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.utils import S_TO_NS, table_dict, table_html
 
 
 @dataclass
 class TimeOfFlightReadoutParameters(Parameters):
     """TimeOfFlightReadout runcard inputs."""
 
@@ -42,23 +42,23 @@
     sampling_rate: int
 
     data: dict[QubitId, npt.NDArray] = field(default_factory=dict)
     """Raw data acquired."""
 
 
 def _acquisition(
-    params: TimeOfFlightReadoutParameters, platform: Platform, qubits: Qubits
+    params: TimeOfFlightReadoutParameters, platform: Platform, targets: list[QubitId]
 ) -> TimeOfFlightReadoutData:
     """Data acquisition for time of flight experiment."""
 
     sequence = PulseSequence()
 
     RX_pulses = {}
     ro_pulses = {}
-    for qubit in qubits:
+    for qubit in targets:
         RX_pulses[qubit] = platform.create_RX_pulse(qubit, start=0)
         ro_pulses[qubit] = platform.create_qubit_readout_pulse(
             qubit, start=RX_pulses[qubit].finish
         )
         if params.readout_amplitude is not None:
             ro_pulses[qubit].amplitude = params.readout_amplitude
         sequence.add(ro_pulses[qubit])
@@ -74,15 +74,15 @@
     )
 
     data = TimeOfFlightReadoutData(
         windows_size=params.window_size, sampling_rate=platform.sampling_rate
     )
 
     # retrieve and store the results for every qubit
-    for qubit in qubits:
+    for qubit in targets:
         samples = results[ro_pulses[qubit].serial].magnitude
         # store the results
         data.register_qubit(TimeOfFlightReadoutType, (qubit), dict(samples=samples))
     return data
 
 
 def _fit(data: TimeOfFlightReadoutData) -> TimeOfFlightReadoutResults:
@@ -106,21 +106,23 @@
         max_average_change = np.argmax(moving_average_deltas)
         time_of_flight_readout = max_average_change / sampling_rate
         fitted_parameters[qubit] = time_of_flight_readout
 
     return TimeOfFlightReadoutResults(fitted_parameters)
 
 
-def _plot(data: TimeOfFlightReadoutData, qubit, fit: TimeOfFlightReadoutResults):
+def _plot(
+    data: TimeOfFlightReadoutData, target: QubitId, fit: TimeOfFlightReadoutResults
+):
     """Plotting function for TimeOfFlightReadout."""
 
     figures = []
     fitting_report = ""
     fig = go.Figure()
-    qubit_data = data[qubit]
+    qubit_data = data[target]
     sampling_rate = data.sampling_rate
     y = qubit_data.samples
 
     fig.add_trace(
         go.Scatter(
             y=y,
             textposition="bottom center",
@@ -133,22 +135,22 @@
     fig.update_layout(
         showlegend=True,
         xaxis_title="Sample",
         yaxis_title="Signal [a.u.]",
     )
     if fit is not None:
         fig.add_vline(
-            x=fit.fitted_parameters[qubit] * sampling_rate,
+            x=fit.fitted_parameters[target] * sampling_rate,
             line_width=2,
             line_dash="dash",
             line_color="grey",
         )
         fitting_report = table_html(
             table_dict(
-                qubit, "Time of flights [ns]", fit.fitted_parameters[qubit] * S_TO_NS
+                target, "Time of flights [ns]", fit.fitted_parameters[target] * S_TO_NS
             )
         )
     fig.update_layout(
         showlegend=True,
         xaxis_title="Sample",
         yaxis_title="Signal [a.u.]",
     )
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chevron.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chevron/chevron.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,59 +5,76 @@
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from plotly.subplots import make_subplots
 from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.platform import Platform
-from qibolab.pulses import PulseSequence
 from qibolab.qubits import QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
-from .utils import fit_flux_amplitude, order_pair
-
-COLORAXIS = ["coloraxis2", "coloraxis1"]
+from ..utils import fit_flux_amplitude, order_pair
+from .utils import COLORAXIS, chevron_fit, chevron_sequence
 
 
 @dataclass
 class ChevronParameters(Parameters):
     """CzFluxTime runcard inputs."""
 
-    amplitude_min: float
+    amplitude_min_factor: float
     """Amplitude minimum."""
-    amplitude_max: float
+    amplitude_max_factor: float
     """Amplitude maximum."""
-    amplitude_step: float
+    amplitude_step_factor: float
     """Amplitude step."""
     duration_min: float
     """Duration minimum."""
     duration_max: float
     """Duration maximum."""
     duration_step: float
     """Duration step."""
     dt: Optional[int] = 0
     """Time delay between flux pulses and readout."""
     parking: bool = True
     """Wether to park non interacting qubits or not."""
 
+    @property
+    def amplitude_range(self):
+        return np.arange(
+            self.amplitude_min_factor,
+            self.amplitude_max_factor,
+            self.amplitude_step_factor,
+        )
+
+    @property
+    def duration_range(self):
+        return np.arange(
+            self.duration_min,
+            self.duration_max,
+            self.duration_step,
+        )
+
 
 @dataclass
 class ChevronResults(Results):
     """CzFluxTime outputs when fitting will be done."""
 
     amplitude: dict[QubitPairId, float]
     """CZ angle."""
     duration: dict[QubitPairId, int]
     """Virtual Z phase correction."""
 
+    def __contains__(self, key: QubitPairId):
+        return super().__contains__(key) | super().__contains__((key[1], key[0]))
+
 
 ChevronType = np.dtype(
     [
         ("amp", np.float64),
         ("length", np.float64),
         ("prob_high", np.float64),
         ("prob_low", np.float64),
@@ -66,236 +83,216 @@
 """Custom dtype for Chevron."""
 
 
 @dataclass
 class ChevronData(Data):
     """Chevron acquisition outputs."""
 
+    native_amplitude: dict[QubitPairId, float] = field(default_factory=dict)
+    """CZ platform amplitude for qubit pair."""
+    sweetspot: dict[QubitPairId, float] = field(default_factory=dict)
+    """Sweetspot value for high frequency qubit."""
     data: dict[QubitPairId, npt.NDArray[ChevronType]] = field(default_factory=dict)
 
     def register_qubit(self, low_qubit, high_qubit, length, amp, prob_low, prob_high):
         """Store output for single qubit."""
         size = len(length) * len(amp)
         amplitude, duration = np.meshgrid(amp, length)
         ar = np.empty(size, dtype=ChevronType)
         ar["length"] = duration.ravel()
         ar["amp"] = amplitude.ravel()
         ar["prob_low"] = prob_low.ravel()
         ar["prob_high"] = prob_high.ravel()
         self.data[low_qubit, high_qubit] = np.rec.array(ar)
 
+    def amplitudes(self, pair):
+        """Unique pair amplitudes"""
+        return np.unique(self[pair].amp)
+
+    def durations(self, pair):
+        """Unique pair durations."""
+        return np.unique(self[pair].length)
+
+    def low_frequency(self, pair):
+        return self[pair].prob_low
+
+    def high_frequency(self, pair):
+        return self[pair].prob_high
+
 
 def _aquisition(
     params: ChevronParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitPairId],
 ) -> ChevronData:
     r"""
-    Perform an iSWAP/CZ experiment between pairs of qubits by changing its frequency.
+    Perform an CZ experiment between pairs of qubits by changing its frequency.
 
     Args:
         platform: Platform to use.
         params: Experiment parameters.
-        qubits: Qubits to use.
+        targets (list): List of pairs to use sequentially.
 
     Returns:
         ChevronData: Acquisition data.
     """
 
     # create a DataUnits object to store the results,
     data = ChevronData()
-    for pair in qubits:
+    for pair in targets:
         # order the qubits so that the low frequency one is the first
-        sequence = PulseSequence()
-        ordered_pair = order_pair(pair, platform.qubits)
-        # initialize in system in 11 state
-        initialize_lowfreq = platform.create_RX_pulse(
-            ordered_pair[0], start=0, relative_phase=0
-        )
-        initialize_highfreq = platform.create_RX_pulse(
-            ordered_pair[1], start=0, relative_phase=0
-        )
-        sequence.add(initialize_highfreq)
-        sequence.add(initialize_lowfreq)
-        cz, _ = platform.create_CZ_pulse_sequence(
-            qubits=(ordered_pair[1], ordered_pair[0]),
-            start=initialize_highfreq.finish,
-        )
-
-        sequence.add(cz.get_qubit_pulses(ordered_pair[0]))
-        sequence.add(cz.get_qubit_pulses(ordered_pair[1]))
-
-        # Patch to get the coupler until the routines use QubitPair
-        if platform.couplers:
-            sequence.add(
-                cz.coupler_pulses(platform.pairs[tuple(ordered_pair)].coupler.name)
-            )
-
-        if params.parking:
-            for pulse in cz:
-                if pulse.qubit not in ordered_pair:
-                    pulse.start = 0
-                    pulse.duration = 100
-                    sequence.add(pulse)
-
-        # add readout
-        measure_lowfreq = platform.create_qubit_readout_pulse(
-            ordered_pair[0],
-            start=initialize_lowfreq.finish + params.duration_max + params.dt,
-        )
-        measure_highfreq = platform.create_qubit_readout_pulse(
-            ordered_pair[1],
-            start=initialize_highfreq.finish + params.duration_max + params.dt,
-        )
-
-        sequence.add(measure_lowfreq)
-        sequence.add(measure_highfreq)
-
-        # define the parameter to sweep and its range:
-        delta_amplitude_range = np.arange(
-            params.amplitude_min,
-            params.amplitude_max,
-            params.amplitude_step,
-        )
-        delta_duration_range = np.arange(
-            params.duration_min, params.duration_max, params.duration_step
+        sequence = chevron_sequence(
+            platform=platform,
+            pair=pair,
+            duration_max=params.duration_max,
+            parking=params.parking,
+            dt=params.dt,
         )
+        ordered_pair = order_pair(pair, platform)
 
+        # TODO: move in function to avoid code duplications
         sweeper_amplitude = Sweeper(
             Parameter.amplitude,
-            delta_amplitude_range,
-            pulses=[cz.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
-            type=SweeperType.ABSOLUTE,
+            params.amplitude_range,
+            pulses=[sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
+            type=SweeperType.FACTOR,
+        )
+
+        data.native_amplitude[ordered_pair] = (
+            sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0].amplitude
         )
+        data.sweetspot[ordered_pair] = platform.qubits[ordered_pair[1]].sweetspot
         sweeper_duration = Sweeper(
             Parameter.duration,
-            delta_duration_range,
-            pulses=[cz.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
+            params.duration_range,
+            pulses=[sequence.get_qubit_pulses(ordered_pair[1]).qf_pulses[0]],
             type=SweeperType.ABSOLUTE,
         )
+
         results = platform.sweep(
             sequence,
             ExecutionParameters(
                 nshots=params.nshots,
-                acquisition_type=AcquisitionType.INTEGRATION,
+                acquisition_type=AcquisitionType.DISCRIMINATION,
                 averaging_mode=AveragingMode.CYCLIC,
             ),
             sweeper_duration,
             sweeper_amplitude,
         )
         data.register_qubit(
             ordered_pair[0],
             ordered_pair[1],
-            delta_duration_range,
-            delta_amplitude_range,
-            results[ordered_pair[0]].magnitude,
-            results[ordered_pair[1]].magnitude,
+            params.duration_range,
+            params.amplitude_range * data.native_amplitude[ordered_pair],
+            results[ordered_pair[0]].probability(state=1),
+            results[ordered_pair[1]].probability(state=1),
         )
     return data
 
 
-# fitting function for single row in chevron plot (rabi-like curve)
-def cos(x, omega, phase, amplitude, offset):
-    return amplitude * np.cos(x * omega + phase) + offset
-
-
 def _fit(data: ChevronData) -> ChevronResults:
     durations = {}
     amplitudes = {}
     for pair in data.data:
         pair_amplitude = []
         pair_duration = []
-        amps = np.unique(data[pair].amp)
-        times = np.unique(data[pair].length)
+        amps = data.amplitudes(pair)
+        times = data.durations(pair)
 
         for qubit in pair:
-            signal = data[pair].prob_low if pair[0] == qubit else data[pair].prob_high
+            signal = (
+                data.low_frequency(pair)
+                if pair[0] == qubit
+                else data.high_frequency(pair)
+            )
             signal_matrix = signal.reshape(len(times), len(amps)).T
 
             # guess amplitude computing FFT
             amplitude, index, delta = fit_flux_amplitude(signal_matrix, amps, times)
             # estimate duration by rabi curve at amplitude previously estimated
             y = signal_matrix[index, :].ravel()
 
-            popt, _ = curve_fit(cos, times, y, p0=[delta, 0, np.mean(y), np.mean(y)])
+            popt, _ = curve_fit(
+                chevron_fit, times, y, p0=[delta, 0, np.mean(y), np.mean(y)]
+            )
 
             # duration can be estimated as the period of the oscillation
             duration = 1 / (popt[0] / 2 / np.pi)
             pair_amplitude.append(amplitude)
             pair_duration.append(duration)
 
         amplitudes[pair] = np.mean(pair_amplitude)
         durations[pair] = int(np.mean(duration))
 
     return ChevronResults(amplitude=amplitudes, duration=durations)
 
 
-def _plot(data: ChevronData, fit: ChevronResults, qubit):
+def _plot(data: ChevronData, fit: ChevronResults, target: QubitPairId):
     """Plot the experiment result for a single pair."""
 
     # reverse qubit order if not found in data
-    if qubit not in data.data:
-        qubit = (qubit[1], qubit[0])
+    if target not in data.data:
+        target = (target[1], target[0])
 
-    pair_data = data[qubit]
+    pair_data = data[target]
 
     fig = make_subplots(
         rows=1,
         cols=2,
         subplot_titles=(
-            f"Qubit {qubit[0]} - Low Frequency",
-            f"Qubit {qubit[1]} - High Frequency",
+            f"Qubit {target[0]} - Low Frequency",
+            f"Qubit {target[1]} - High Frequency",
         ),
     )
     fitting_report = ""
 
     fig.add_trace(
         go.Heatmap(
             x=pair_data.length,
             y=pair_data.amp,
-            z=pair_data.prob_low,
+            z=data.low_frequency(target),
             coloraxis=COLORAXIS[0],
         ),
         row=1,
         col=1,
     )
 
     fig.add_trace(
         go.Heatmap(
             x=pair_data.length,
             y=pair_data.amp,
-            z=pair_data.prob_high,
+            z=data.high_frequency(target),
             coloraxis=COLORAXIS[1],
         ),
         row=1,
         col=2,
     )
 
-    for measured_qubit in qubit:
+    for measured_qubit in target:
         if fit is not None:
             fig.add_trace(
                 go.Scatter(
                     x=[
-                        fit.duration[qubit],
+                        fit.duration[target],
                     ],
                     y=[
-                        fit.amplitude[qubit],
+                        fit.amplitude[target],
                     ],
                     mode="markers",
                     marker=dict(
                         size=8,
                         color="black",
                         symbol="cross",
                     ),
-                    name="CZ estimate",
-                    showlegend=True if measured_qubit == qubit[0] else False,
+                    name="CZ estimate",  #  Change name from the params
+                    showlegend=True if measured_qubit == target[0] else False,
                     legendgroup="Voltage",
                 ),
                 row=1,
-                col=1 if measured_qubit == qubit[0] else 2,
+                col=1 if measured_qubit == target[0] else 2,
             )
 
     fig.update_layout(
         xaxis_title="Duration [ns]",
         xaxis2_title="Duration [ns]",
         yaxis_title="Amplitude [a.u.]",
         legend=dict(orientation="h"),
@@ -304,25 +301,29 @@
         coloraxis={"colorscale": "Oryel", "colorbar": {"x": 1.15}},
         coloraxis2={"colorscale": "Darkmint", "colorbar": {"x": -0.15}},
     )
 
     if fit is not None:
         fitting_report = table_html(
             table_dict(
-                qubit[1],
-                ["CZ amplitude", "CZ duration"],
-                [fit.amplitude[qubit], fit.duration[qubit]],
+                target[1],
+                ["CZ amplitude", "CZ duration", "Bias point"],
+                [
+                    fit.amplitude[target],
+                    fit.duration[target],
+                    fit.amplitude[target] + data.sweetspot[target],
+                ],
             )
         )
 
     return [fig], fitting_report
 
 
-def _update(results: ChevronResults, platform: Platform, qubit_pair: QubitPairId):
-    if qubit_pair not in results.duration:
-        qubit_pair = (qubit_pair[1], qubit_pair[0])
-    update.CZ_duration(results.duration[qubit_pair], platform, qubit_pair)
-    update.CZ_amplitude(results.amplitude[qubit_pair], platform, qubit_pair)
+def _update(results: ChevronResults, platform: Platform, target: QubitPairId):
+    if target not in results.duration:
+        target = (target[1], target[0])
+    update.CZ_duration(results.duration[target], platform, target)
+    update.CZ_amplitude(results.amplitude[target], platform, target)
 
 
 chevron = Routine(_aquisition, _fit, _plot, _update, two_qubit_gates=True)
 """Chevron routine."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/circuits.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/protocol.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 """Protocol for CHSH experiment using both circuits and pulses."""
 
+import json
 from dataclasses import dataclass, field
+from pathlib import Path
 from typing import Optional
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objects as go
 from qibolab import ExecutionParameters
 from qibolab.platform import Platform
-from qibolab.qubits import QubitId
+from qibolab.qubits import QubitId, QubitPairId
 
-from qibocal.auto.operation import Data, Parameters, Qubits, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 
 from ...readout_mitigation_matrix import (
     ReadoutMitigationMatrixParameters as mitigation_params,
 )
 from ...readout_mitigation_matrix import _acquisition as mitigation_acquisition
 from ...readout_mitigation_matrix import _fit as mitigation_fit
 from ...utils import calculate_frequencies
 from .circuits import create_chsh_circuits
 from .pulses import create_chsh_sequences
 from .utils import READOUT_BASIS, compute_chsh
 
 COMPUTATIONAL_BASIS = ["00", "01", "10", "11"]
 
+CLASSICAL_BOUND = 2
+"""Classical limit of CHSH,"""
+QUANTUM_BOUND = 2 * np.sqrt(2)
+"""Quantum limit of CHSH."""
+
+
+MITIGATION_MATRIX_FILE = "mitigation_matrix"
+"""File where readout mitigation matrix is stored."""
+
 
 @dataclass
 class CHSHParameters(Parameters):
     """CHSH runcard inputs."""
 
     bell_states: list
     """List with Bell states to compute CHSH.
@@ -43,25 +54,50 @@
     """If True a circuit will be created using only GPI2 and CZ gates."""
     apply_error_mitigation: Optional[bool] = False
     """Error mitigation model"""
 
 
 @dataclass
 class CHSHData(Data):
+    """CHSH Data structure."""
+
     bell_states: list
     """Bell states list."""
     thetas: list
     """Angles probed."""
     data: dict[QubitId, QubitId, int, tuple, str] = field(default_factory=dict)
     """Raw data acquired."""
     mitigation_matrix: dict[tuple[QubitId, ...], npt.NDArray] = field(
         default_factory=dict
     )
     """Mitigation matrix computed using the readout_mitigation_matrix protocol."""
 
+    def save(self, path: Path):
+        """Saving data including mitigation matrix."""
+
+        np.savez(
+            path / f"{MITIGATION_MATRIX_FILE}.npz",
+            **{
+                json.dumps((control, target)): self.mitigation_matrix[control, target]
+                for control, target, _, _, _ in self.data
+            },
+        )
+        super().save(path=path)
+
+    @classmethod
+    def load(cls, path: Path):
+        """Custom loading to acco   modate mitigation matrix"""
+        instance = super().load(path=path)
+        # load readout mitigation matrix
+        mitigation_matrix = super().load_data(
+            path=path, filename=MITIGATION_MATRIX_FILE
+        )
+        instance.mitigation_matrix = mitigation_matrix
+        return instance
+
     def register_basis(self, pair, bell_state, basis, frequencies):
         """Store output for single qubit."""
 
         # Add zero is state do not appear in state
         # could be removed by using high number of shots
         for i in COMPUTATIONAL_BASIS:
             if i not in frequencies:
@@ -102,37 +138,48 @@
         data_dict.pop("mitigation_matrix")
 
         return data_dict
 
 
 @dataclass
 class CHSHResults(Results):
-    chsh: dict[tuple[QubitId, QubitId, int], float] = field(default_factory=dict)
-    chsh_mitigated: dict[tuple[QubitId, QubitId, int], float] = field(
-        default_factory=dict
-    )
+    """CHSH Results class."""
+
+    chsh: dict[tuple[QubitPairId, int], float] = field(default_factory=dict)
+    """Raw CHSH value."""
+    chsh_mitigated: dict[tuple[QubitPairId, int], float] = field(default_factory=dict)
+    """Mitigated CHSH value."""
+
+    def __contains__(self, key: QubitPairId):
+        """Check if key is in class.
+
+        While key is a QubitPairId both chsh and chsh_mitigated contain
+        an additional key which represents the basis chosen.
+
+        """
+
+        return key in [(target, control) for target, control, _ in self.chsh]
 
 
 def _acquisition_pulses(
     params: CHSHParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[list[QubitId]],
 ) -> CHSHData:
     r"""Data acquisition for CHSH protocol using pulse sequences."""
-
     thetas = np.linspace(0, 2 * np.pi, params.ntheta)
     data = CHSHData(bell_states=params.bell_states, thetas=thetas.tolist())
 
     if params.apply_error_mitigation:
         mitigation_data = mitigation_acquisition(
-            mitigation_params(pulses=True, nshots=params.nshots), platform, qubits
+            mitigation_params(pulses=True, nshots=params.nshots), platform, targets
         )
         mitigation_results = mitigation_fit(mitigation_data)
 
-    for pair in qubits:
+    for pair in targets:
         if params.apply_error_mitigation:
             data.mitigation_matrix[pair] = mitigation_results.readout_mitigation_matrix[
                 pair
             ]
         for bell_state in params.bell_states:
             for theta in thetas:
                 chsh_sequences = create_chsh_sequences(
@@ -149,29 +196,29 @@
                     data.register_basis(pair, bell_state, basis, frequencies)
     return data
 
 
 def _acquisition_circuits(
     params: CHSHParameters,
     platform: Platform,
-    qubits: Qubits,
+    targets: list[QubitPairId],
 ) -> CHSHData:
     """Data acquisition for CHSH protocol using circuits."""
     thetas = np.linspace(0, 2 * np.pi, params.ntheta)
     data = CHSHData(
         bell_states=params.bell_states,
         thetas=thetas.tolist(),
     )
 
     if params.apply_error_mitigation:
         mitigation_data = mitigation_acquisition(
-            mitigation_params(pulses=False, nshots=params.nshots), platform, qubits
+            mitigation_params(pulses=False, nshots=params.nshots), platform, targets
         )
         mitigation_results = mitigation_fit(mitigation_data)
-    for pair in qubits:
+    for pair in targets:
         if params.apply_error_mitigation:
             data.mitigation_matrix[pair] = mitigation_results.readout_mitigation_matrix[
                 pair
             ]
         for bell_state in params.bell_states:
             for theta in thetas:
                 chsh_circuits = create_chsh_circuits(
@@ -185,70 +232,93 @@
                     result = circuit(nshots=params.nshots)
                     frequencies = result.frequencies()
                     data.register_basis(pair, bell_state, basis, frequencies)
 
     return data
 
 
-def _plot(data: CHSHData, fit: CHSHResults, qubit):
+def _plot(data: CHSHData, fit: CHSHResults, target: QubitPairId):
     """Plotting function for CHSH protocol."""
     figures = []
 
     for bell_state in data.bell_states:
         fig = go.Figure(layout_yaxis_range=[-3, 3])
         if fit is not None:
             fig.add_trace(
                 go.Scatter(
                     x=data.thetas,
-                    y=fit.chsh[qubit[0], qubit[1], bell_state],
+                    y=fit.chsh[target[0], target[1], bell_state],
                     name="Bare",
                 )
             )
             if fit.chsh_mitigated:
                 fig.add_trace(
                     go.Scatter(
                         x=data.thetas,
-                        y=fit.chsh_mitigated[qubit[0], qubit[1], bell_state],
+                        y=fit.chsh_mitigated[target[0], target[1], bell_state],
                         name="Mitigated",
                     )
                 )
 
-        # classical bounds
-        fig.add_hline(
-            y=2,
-            line_width=2,
-            line_color="red",
+        fig.add_trace(
+            go.Scatter(
+                mode="lines",
+                x=data.thetas,
+                y=[+CLASSICAL_BOUND] * len(data.thetas),
+                line_color="gray",
+                name="Classical limit",
+                line_dash="dash",
+                legendgroup="classic",
+            )
         )
-        fig.add_hline(
-            y=-2,
-            line_width=2,
-            line_color="red",
+
+        fig.add_trace(
+            go.Scatter(
+                mode="lines",
+                x=data.thetas,
+                y=[-CLASSICAL_BOUND] * len(data.thetas),
+                line_color="gray",
+                name="Classical limit",
+                legendgroup="classic",
+                line_dash="dash",
+                showlegend=False,
+            )
         )
 
-        # maximum values
-        fig.add_hline(
-            y=2 * np.sqrt(2),
-            line_width=2,
-            line_dash="dash",
-            line_color="grey",
+        fig.add_trace(
+            go.Scatter(
+                mode="lines",
+                x=data.thetas,
+                y=[+QUANTUM_BOUND] * len(data.thetas),
+                line_color="gray",
+                name="Quantum limit",
+                legendgroup="quantum",
+            )
         )
-        fig.add_hline(
-            y=-2 * np.sqrt(2),
-            line_width=2,
-            line_dash="dash",
-            line_color="grey",
+
+        fig.add_trace(
+            go.Scatter(
+                mode="lines",
+                x=data.thetas,
+                y=[-QUANTUM_BOUND] * len(data.thetas),
+                line_color="gray",
+                name="Quantum limit",
+                legendgroup="quantum",
+                showlegend=False,
+            )
         )
 
         fig.update_layout(
             xaxis_title="Theta [rad]",
             yaxis_title="CHSH value",
+            xaxis=dict(range=[min(data.thetas), max(data.thetas)]),
         )
         figures.append(fig)
 
-    return figures, None
+    return figures, ""
 
 
 def _fit(data: CHSHData) -> CHSHResults:
     """Fitting for CHSH protocol."""
     results = {}
     mitigated_results = {}
     for pair in data.pairs:
@@ -264,15 +334,14 @@
                         freq_array = np.zeros(4)
                         for k, v in freq_basis.items():
                             freq_array[int(k, 2)] = v[i]
                         freq_array = freq_array.reshape(-1, 1)
                         for j, val in enumerate(matrix @ freq_array):
                             mitigated_freq[format(j, f"0{2}b")].append(float(val))
                     mitigated_freq_list.append(mitigated_freq)
-
             results[pair[0], pair[1], bell_state] = [
                 compute_chsh(freq, bell_state, l) for l in range(len(data.thetas))
             ]
 
             if data.mitigation_matrix:
                 mitigated_results[pair[0], pair[1], bell_state] = [
                     compute_chsh(mitigated_freq_list, bell_state, l)
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/pulses.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/chsh/utils.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/cz_virtualz.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,32 +11,35 @@
 from qibolab.platform import Platform
 from qibolab.pulses import Pulse, PulseSequence
 from qibolab.qubits import QubitId, QubitPairId
 from qibolab.sweeper import Parameter, Sweeper, SweeperType
 from scipy.optimize import curve_fit
 
 from qibocal import update
-from qibocal.auto.operation import Data, Parameters, QubitsPairs, Results, Routine
+from qibocal.auto.operation import Data, Parameters, Results, Routine
 from qibocal.config import log
-from qibocal.protocols.characterization.two_qubit_interaction.chevron import order_pair
 from qibocal.protocols.characterization.utils import table_dict, table_html
 
+from .utils import order_pair
+
 
 @dataclass
 class CZVirtualZParameters(Parameters):
     """CzVirtualZ runcard inputs."""
 
     theta_start: float
     """Initial angle for the low frequency qubit measurement in radians."""
     theta_end: float
     """Final angle for the low frequency qubit measurement in radians."""
     theta_step: float
     """Step size for the theta sweep in radians."""
     flux_pulse_amplitude: Optional[float] = None
     """Amplitude of flux pulse implementing CZ."""
+    flux_pulse_duration: Optional[float] = None
+    """Duration of flux pulse implementing CZ."""
     dt: Optional[float] = 20
     """Time delay between flux pulses and readout."""
     parking: bool = True
     """Wether to park non interacting qubits or not."""
 
 
 @dataclass
@@ -45,27 +48,40 @@
 
     fitted_parameters: dict[tuple[str, QubitId],]
     """Fitted parameters"""
     cz_angle: dict[QubitPairId, float]
     """CZ angle."""
     virtual_phase: dict[QubitPairId, dict[QubitId, float]]
     """Virtual Z phase correction."""
+    leakage: dict[QubitPairId, dict[QubitId, float]]
+    """Leakage on control qubit for pair."""
+
+    def __contains__(self, key: QubitPairId):
+        """Check if key is in class.
+        While key is a QubitPairId both chsh and chsh_mitigated contain
+        an additional key which represents the basis chosen.
+        """
+
+        return key in [
+            (target, control) for target, control, _ in self.fitted_parameters
+        ]
 
 
 CZVirtualZType = np.dtype([("target", np.float64), ("control", np.float64)])
 
 
 @dataclass
 class CZVirtualZData(Data):
     """CZVirtualZ data."""
 
     data: dict[tuple, npt.NDArray[CZVirtualZType]] = field(default_factory=dict)
     thetas: list = field(default_factory=list)
     vphases: dict[QubitPairId, dict[QubitId, float]] = field(default_factory=dict)
     amplitudes: dict[tuple[QubitId, QubitId], float] = field(default_factory=dict)
+    durations: dict[tuple[QubitId, QubitId], float] = field(default_factory=dict)
 
     def __getitem__(self, pair):
         return {
             index: value
             for index, value in self.data.items()
             if set(pair).issubset(index)
         }
@@ -76,16 +92,21 @@
     setup: str,
     target_qubit: QubitId,
     control_qubit: QubitId,
     ordered_pair: list[QubitId, QubitId],
     parking: bool,
     dt: float,
     amplitude: float = None,
+    duration: float = None,
 ) -> tuple[
-    PulseSequence, dict[QubitId, Pulse], dict[QubitId, Pulse], dict[QubitId, Pulse]
+    PulseSequence,
+    dict[QubitId, Pulse],
+    dict[QubitId, Pulse],
+    dict[QubitId, Pulse],
+    dict[QubitId, Pulse],
 ]:
     """Create the experiment PulseSequence."""
 
     sequence = PulseSequence()
 
     Y90_pulse = platform.create_RX90_pulse(
         target_qubit, start=0, relative_phase=np.pi / 2
@@ -96,14 +117,17 @@
         (ordered_pair[1], ordered_pair[0]),
         start=max(Y90_pulse.finish, RX_pulse_start.finish),
     )
 
     if amplitude is not None:
         cz.get_qubit_pulses(ordered_pair[1])[0].amplitude = amplitude
 
+    if duration is not None:
+        cz.get_qubit_pulses(ordered_pair[1])[0].duration = duration
+
     theta_pulse = platform.create_RX90_pulse(
         target_qubit,
         start=cz.finish + dt,
         relative_phase=virtual_z_phase[target_qubit],
     )
     RX_pulse_end = platform.create_RX_pulse(
         control_qubit,
@@ -138,21 +162,22 @@
                 sequence.add(pulse)
 
     return (
         sequence,
         virtual_z_phase,
         theta_pulse,
         cz.get_qubit_pulses(ordered_pair[1])[0].amplitude,
+        cz.get_qubit_pulses(ordered_pair[1])[0].duration,
     )
 
 
 def _acquisition(
     params: CZVirtualZParameters,
     platform: Platform,
-    qubits: QubitsPairs,
+    targets: list[QubitPairId],
 ) -> CZVirtualZData:
     r"""
     Acquisition for CZVirtualZ.
 
     Check the two-qubit landscape created by a flux pulse of a given duration
     and amplitude.
     The system is initialized with a Y90 pulse on the low frequency qubit and either
@@ -165,63 +190,64 @@
     remnant single qubit Z phase aquired during the execution to be corrected.
     Population of the high frequency qubit yield the leakage to the non-computational states
     during the execution of the flux pulse.
     """
 
     theta_absolute = np.arange(params.theta_start, params.theta_end, params.theta_step)
     data = CZVirtualZData(thetas=theta_absolute.tolist())
-    for pair in qubits:
+    for pair in targets:
         # order the qubits so that the low frequency one is the first
-        ord_pair = order_pair(pair, platform.qubits)
+        ord_pair = order_pair(pair, platform)
 
         for target_q, control_q in (
             (ord_pair[0], ord_pair[1]),
             (ord_pair[1], ord_pair[0]),
         ):
             for setup in ("I", "X"):
                 (
                     sequence,
                     virtual_z_phase,
                     theta_pulse,
                     data.amplitudes[ord_pair],
+                    data.durations[ord_pair],
                 ) = create_sequence(
                     platform,
                     setup,
                     target_q,
                     control_q,
                     ord_pair,
                     params.dt,
                     params.parking,
                     params.flux_pulse_amplitude,
                 )
                 data.vphases[ord_pair] = dict(virtual_z_phase)
                 theta = np.arange(
-                    virtual_z_phase[target_q] + params.theta_start,
-                    virtual_z_phase[target_q] + params.theta_end,
+                    params.theta_start,
+                    params.theta_end,
                     params.theta_step,
                     dtype=float,
                 )
                 sweeper = Sweeper(
                     Parameter.relative_phase,
-                    theta,
+                    theta - data.vphases[ord_pair][target_q],
                     pulses=[theta_pulse],
                     type=SweeperType.ABSOLUTE,
                 )
                 results = platform.sweep(
                     sequence,
                     ExecutionParameters(
                         nshots=params.nshots,
-                        acquisition_type=AcquisitionType.INTEGRATION,
+                        acquisition_type=AcquisitionType.DISCRIMINATION,
                         averaging_mode=AveragingMode.CYCLIC,
                     ),
                     sweeper,
                 )
 
-                result_target = results[target_q].magnitude
-                result_control = results[control_q].magnitude
+                result_target = results[target_q].probability(1)
+                result_control = results[control_q].probability(1)
 
                 data.register_qubit(
                     CZVirtualZType,
                     (target_q, control_q, setup),
                     dict(
                         target=result_target,
                         control=result_control,
@@ -247,160 +273,197 @@
 
         y = p_0 sin\Big(x + p_2\Big) + p_1.
     """
     fitted_parameters = {}
     pairs = data.pairs
     virtual_phase = {}
     cz_angle = {}
+    leakage = {}
     for pair in pairs:
         virtual_phase[pair] = {}
+        leakage[pair] = {}
         for target, control, setup in data[pair]:
             target_data = data[pair][target, control, setup].target
             pguess = [
                 np.max(target_data) - np.min(target_data),
                 np.mean(target_data),
-                3.14,
+                np.pi,
             ]
-
             try:
                 popt, _ = curve_fit(
                     fit_function,
-                    np.array(data.thetas) + data.vphases[pair][target],
+                    np.array(data.thetas) - data.vphases[pair][target],
                     target_data,
                     p0=pguess,
-                    bounds=((0, 0, 0), (2.5, 2.5, 2 * np.pi)),
+                    bounds=(
+                        (0, -np.max(target_data), 0),
+                        (np.max(target_data), np.max(target_data), 2 * np.pi),
+                    ),
                 )
                 fitted_parameters[target, control, setup] = popt.tolist()
 
-            except:
-                log.warning("landscape_fit: the fitting was not succesful")
-                fitted_parameters[target, control, setup] = [0] * 3
+            except Exception as e:
+                log.warning(f"CZ fit failed for pair ({target, control}) due to {e}.")
 
-        for target_q, control_q in (
-            pair,
-            list(pair)[::-1],
-        ):
-            cz_angle[target_q, control_q] = abs(
-                fitted_parameters[target_q, control_q, "X"][2]
-                - fitted_parameters[target_q, control_q, "I"][2]
-            )
-            virtual_phase[pair][target_q] = -fitted_parameters[
-                target_q, control_q, "I"
-            ][2]
+        try:
+            for target_q, control_q in (
+                pair,
+                list(pair)[::-1],
+            ):
+                cz_angle[target_q, control_q] = abs(
+                    fitted_parameters[target_q, control_q, "X"][2]
+                    - fitted_parameters[target_q, control_q, "I"][2]
+                )
+                virtual_phase[pair][target_q] = fitted_parameters[
+                    target_q, control_q, "I"
+                ][2]
+
+                # leakage estimate: L = m /2
+                # See NZ paper from Di Carlo
+                # approximation which does not need qutrits
+                # https://arxiv.org/pdf/1903.02492.pdf
+                leakage[pair][control_q] = 0.5 * float(
+                    np.mean(
+                        data[pair][target_q, control_q, "X"].control
+                        - data[pair][target_q, control_q, "I"].control
+                    )
+                )
+        except KeyError:
+            pass  # exception covered above
 
     return CZVirtualZResults(
         cz_angle=cz_angle,
         virtual_phase=virtual_phase,
         fitted_parameters=fitted_parameters,
+        leakage=leakage,
     )
 
 
 # TODO: remove str
-def _plot(data: CZVirtualZData, fit: CZVirtualZResults, qubit):
+def _plot(data: CZVirtualZData, fit: CZVirtualZResults, target: QubitPairId):
     """Plot routine for CZVirtualZ."""
-    pair_data = data[qubit]
+    pair_data = data[target]
     qubits = next(iter(pair_data))[:2]
     fig1 = make_subplots(
         rows=1,
         cols=2,
         subplot_titles=(
             f"Qubit {qubits[0]}",
             f"Qubit {qubits[1]}",
         ),
     )
-    reports = []
+    fitting_report = set()
     fig2 = make_subplots(
         rows=1,
         cols=2,
         subplot_titles=(
             f"Qubit {qubits[0]}",
             f"Qubit {qubits[1]}",
         ),
     )
 
-    fitting_report = ""
     thetas = data.thetas
-    for target, control, setup in pair_data:
-        target_prob = pair_data[target, control, setup].target
-        control_prob = pair_data[target, control, setup].control
-        fig = fig1 if (target, control) == qubits else fig2
+    for target_q, control_q, setup in pair_data:
+        target_prob = pair_data[target_q, control_q, setup].target
+        control_prob = pair_data[target_q, control_q, setup].control
+        fig = fig1 if (target_q, control_q) == qubits else fig2
         fig.add_trace(
             go.Scatter(
-                x=np.array(thetas) + data.vphases[qubits][target],
+                x=np.array(thetas) + data.vphases[qubits][target_q],
                 y=target_prob,
                 name=f"{setup} sequence",
                 legendgroup=setup,
             ),
             row=1,
             col=1 if fig == fig1 else 2,
         )
 
         fig.add_trace(
             go.Scatter(
-                x=np.array(thetas) + data.vphases[qubits][control],
+                x=np.array(thetas) + data.vphases[qubits][control_q],
                 y=control_prob,
                 name=f"{setup} sequence",
                 legendgroup=setup,
             ),
             row=1,
             col=2 if fig == fig1 else 1,
         )
         if fit is not None:
             angle_range = np.linspace(thetas[0], thetas[-1], 100)
-            fitted_parameters = fit.fitted_parameters[target, control, setup]
+            fitted_parameters = fit.fitted_parameters[target_q, control_q, setup]
             fig.add_trace(
                 go.Scatter(
-                    x=angle_range + data.vphases[qubits][target],
+                    x=angle_range + data.vphases[qubits][target_q],
                     y=fit_function(
-                        angle_range + data.vphases[qubits][target],
+                        angle_range - data.vphases[qubits][target_q],
                         *fitted_parameters,
                     ),
                     name="Fit",
                     line=go.scatter.Line(dash="dot"),
                 ),
                 row=1,
                 col=1 if fig == fig1 else 2,
             )
 
-            fitting_report = table_html(
-                table_dict(
-                    [target, target, qubits[1]],
-                    [
-                        "CZ angle [rad]",
-                        "Virtual Z phase [rad]",
-                        "Flux pulse amplitude [a.u.]",
-                    ],
-                    [
-                        np.round(fit.cz_angle[target, control], 4),
-                        np.round(fit.virtual_phase[tuple(sorted(qubit))][target], 4),
-                        np.round(data.amplitudes[qubits]),
-                    ],
+            fitting_report.add(
+                table_html(
+                    table_dict(
+                        [target_q, target_q, control_q],
+                        [
+                            "CZ angle [rad]",
+                            "Virtual Z phase [rad]",
+                            "Leakage [a.u.]",
+                        ],
+                        [
+                            np.round(fit.cz_angle[target_q, control_q], 4),
+                            np.round(
+                                fit.virtual_phase[tuple(sorted(target))][target_q], 4
+                            ),
+                            np.round(fit.leakage[tuple(sorted(target))][control_q], 4),
+                        ],
+                    )
                 )
             )
+    fitting_report.add(
+        table_html(
+            table_dict(
+                [qubits[1], qubits[1]],
+                [
+                    "Flux pulse amplitude [a.u.]",
+                    "Flux pulse duration [ns]",
+                ],
+                [
+                    np.round(data.amplitudes[qubits], 4),
+                    np.round(data.durations[qubits], 4),
+                ],
+            )
+        )
+    )
 
     fig1.update_layout(
         title_text=f"Phase correction Qubit {qubits[0]}",
         showlegend=True,
-        xaxis1_title="theta [rad] + virtual phase[rad]",
-        xaxis2_title="theta [rad] + virtual phase [rad]",
-        yaxis_title="Signal [a.u.]",
+        xaxis1_title="Virtual phase[rad]",
+        xaxis2_title="Virtual phase [rad]",
+        yaxis_title="State 0 Probability",
     )
 
     fig2.update_layout(
         title_text=f"Phase correction Qubit {qubits[1]}",
         showlegend=True,
-        xaxis1_title="theta [rad] + virtual phase[rad]",
-        xaxis2_title="theta [rad] + virtual phase[rad]",
-        yaxis_title="Signal [a.u.]",
+        xaxis1_title="Virtual phase[rad]",
+        xaxis2_title="Virtual phase[rad]",
+        yaxis_title="State 0 Probability",
     )
 
-    return [fig1, fig2], fitting_report
+    return [fig1, fig2], "".join(fitting_report)  # target and control qubit
 
 
-def _update(results: CZVirtualZResults, platform: Platform, qubit_pair: QubitPairId):
+def _update(results: CZVirtualZResults, platform: Platform, target: QubitPairId):
     # FIXME: quick fix for qubit order
-    qubit_pair = tuple(sorted(qubit_pair))
-    update.virtual_phases(results.virtual_phase[qubit_pair], platform, qubit_pair)
+    qubit_pair = tuple(sorted(target))
+    target = tuple(sorted(target))
+    update.virtual_phases(results.virtual_phase[target], platform, target)
 
 
 cz_virtualz = Routine(_acquisition, _fit, _plot, _update, two_qubit_gates=True)
 """CZ virtual Z correction routine."""
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/two_qubit_interaction/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from statistics import median_high
 
 import numpy as np
-from qibolab.qubits import Qubit, QubitId
+from qibolab.platform import Platform
+from qibolab.qubits import QubitId, QubitPairId
 from scipy.signal import find_peaks
 
 RANDOM_HIGH_VALUE = 1e6
 """High value to avoid None when computing FFT."""
 
 
-def order_pair(pair: list[QubitId, QubitId], qubits: dict[QubitId, Qubit]) -> tuple:
+def order_pair(pair: QubitPairId, platform: Platform) -> tuple[QubitId, QubitId]:
     """Order a pair of qubits by drive frequency."""
-    if qubits[pair[0]].drive_frequency > qubits[pair[1]].drive_frequency:
+    if (
+        platform.qubits[pair[0]].drive_frequency
+        > platform.qubits[pair[1]].drive_frequency
+    ):
         return pair[1], pair[0]
     return pair[0], pair[1]
 
 
 def fit_flux_amplitude(matrix, amps, times):
     """Estimate amplitude for CZ gate.
```

### Comparing `qibocal-0.0.7/src/qibocal/protocols/characterization/utils.py` & `qibocal-0.0.8/src/qibocal/protocols/characterization/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     Returns:
         temp (float): effective temperature
         error (float): error on effective temperature
 
     """
     error_prob_0 = np.sqrt(prob_0 * (1 - prob_0) / nshots)
     error_prob_1 = np.sqrt(prob_1 * (1 - prob_1) / nshots)
+    # TODO: find way to handle this exception
     try:
         temp = -HBAR * qubit_frequency / (np.log(prob_1 / prob_0) * KB)
         dT_dp0 = temp / prob_0 / np.log(prob_1 / prob_0)
         dT_dp1 = -temp / prob_1 / np.log(prob_1 / prob_0)
         error = np.sqrt((dT_dp0 * error_prob_0) ** 2 + (dT_dp1 * error_prob_1) ** 2)
     except ZeroDivisionError:
         temp = np.nan
@@ -124,110 +125,163 @@
         guess_amp,
         guess_center,
         guess_sigma,
         guess_offset,
     ]
     # fit the model with the data and guessed parameters
     try:
-        fit_parameters, _ = curve_fit(
-            lorentzian,
-            frequencies,
-            voltages,
-            p0=model_parameters,
-        )
+        if hasattr(data, "error_signal"):
+            fit_parameters, perr = curve_fit(
+                lorentzian,
+                frequencies,
+                voltages,
+                p0=model_parameters,
+                sigma=data.error_signal,
+            )
+            perr = np.sqrt(np.diag(perr)).tolist()
+        else:
+            fit_parameters, perr = curve_fit(
+                lorentzian,
+                frequencies,
+                voltages,
+                p0=model_parameters,
+            )
+            perr = [0] * 4
         model_parameters = list(fit_parameters)
-    except RuntimeError:
-        log.warning("lorentzian_fit: the fitting was not successful")
-
-    return model_parameters[1] * GHZ_TO_HZ, model_parameters
+        return model_parameters[1] * GHZ_TO_HZ, model_parameters, perr
+    except RuntimeError as e:
+        log.warning(f"Lorentzian fit not successful due to {e}")
 
 
 def spectroscopy_plot(data, qubit, fit: Results = None):
     figures = []
     fig = make_subplots(
         rows=1,
         cols=2,
         horizontal_spacing=0.1,
         vertical_spacing=0.1,
     )
     qubit_data = data[qubit]
     fitting_report = ""
-
     frequencies = qubit_data.freq * HZ_TO_GHZ
+    signal = qubit_data.signal
+    errors_signal = qubit_data.error_signal
+    errors_phase = qubit_data.error_phase
+    phase = qubit_data.phase
     fig.add_trace(
         go.Scatter(
             x=frequencies,
-            y=qubit_data.signal,
+            y=signal,
             opacity=1,
             name="Frequency",
             showlegend=True,
             legendgroup="Frequency",
         ),
         row=1,
         col=1,
     )
     fig.add_trace(
         go.Scatter(
+            x=np.concatenate((frequencies, frequencies[::-1])),
+            y=np.concatenate((signal + errors_signal, (signal - errors_signal)[::-1])),
+            fill="toself",
+            fillcolor=COLORBAND,
+            line=dict(color=COLORBAND_LINE),
+            showlegend=True,
+            name="Signal Errors",
+        ),
+        row=1,
+        col=1,
+    )
+    fig.add_trace(
+        go.Scatter(
             x=frequencies,
-            y=qubit_data.phase,
+            y=phase,
             opacity=1,
             name="Phase",
             showlegend=True,
             legendgroup="Phase",
         ),
         row=1,
         col=2,
     )
-
+    fig.add_trace(
+        go.Scatter(
+            x=np.concatenate((frequencies, frequencies[::-1])),
+            y=np.concatenate((phase + errors_phase, (phase - errors_phase)[::-1])),
+            fill="toself",
+            fillcolor=COLORBAND,
+            line=dict(color=COLORBAND_LINE),
+            showlegend=True,
+            name="Phase Errors",
+        ),
+        row=1,
+        col=2,
+    )
     freqrange = np.linspace(
         min(frequencies),
         max(frequencies),
         2 * len(frequencies),
     )
 
     if fit is not None:
         params = fit.fitted_parameters[qubit]
-
         fig.add_trace(
             go.Scatter(
                 x=freqrange,
                 y=lorentzian(freqrange, *params),
                 name="Fit",
                 line=go.scatter.Line(dash="dot"),
             ),
             row=1,
             col=1,
         )
 
         if data.power_level is PowerLevel.low:
-            label = "readout frequency"
+            label = "readout frequency[Hz]"
             freq = fit.frequency
         elif data.power_level is PowerLevel.high:
-            label = "bare resonator frequency"
+            label = "bare resonator frequency[Hz]"
             freq = fit.bare_frequency
         else:
-            label = "qubit frequency"
+            label = "qubit frequency[Hz]"
             freq = fit.frequency
 
-        if fit.amplitude[qubit] is not None:
+        if data.amplitudes[qubit] is not None:
             fitting_report = table_html(
                 table_dict(
                     qubit,
-                    [label, "amplitude"],
-                    [np.round(freq[qubit], 0), fit.amplitude[qubit]],
+                    [label, "amplitude", "chi2 reduced"],
+                    [
+                        (
+                            freq[qubit],
+                            fit.error_fit_pars[qubit][1],
+                        ),
+                        (data.amplitudes[qubit], 0),
+                        fit.chi2_reduced[qubit],
+                    ],
+                    display_error=True,
                 )
             )
-
-        if data.__class__.__name__ == "ResonatorSpectroscopyAttenuationData":
-            if fit.attenuation[qubit] is not None and fit.attenuation[qubit] != 0:
+        if data.attenuations:
+            if data.attenuations[qubit] is not None:
                 fitting_report = table_html(
                     table_dict(
                         qubit,
-                        [label, "attenuation"],
-                        [np.round(freq[qubit], 0), fit.attenuation[qubit]],
+                        [label, "amplitude", "attenuation", "chi2 reduced"],
+                        [
+                            (
+                                freq[qubit],
+                                fit.error_fit_pars[qubit][1],
+                            ),
+                            (data.amplitudes[qubit], 0),
+                            (data.attenuations[qubit], 0),
+                            fit.chi2_reduced[qubit],
+                        ],
+                        display_error=True,
                     )
                 )
 
     fig.update_layout(
         showlegend=True,
         xaxis_title="Frequency [GHz]",
         yaxis_title="Signal [a.u.]",
```

### Comparing `qibocal-0.0.7/src/qibocal/update.py` & `qibocal-0.0.8/src/qibocal/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,33 +126,33 @@
         if pulse.qubit.name == pair[1]:
             pulse.amplitude = float(amp)
 
 
 def t1(t1: int, platform: Platform, qubit: QubitId):
     """Update t1 value in platform for specific qubit."""
     if isinstance(t1, tuple):
-        platform.qubits[qubit].t1 = int(t1[0])
+        platform.qubits[qubit].T1 = int(t1[0])
     else:
-        platform.qubits[qubit].t1 = int(t1)
+        platform.qubits[qubit].T1 = int(t1)
 
 
 def t2(t2: int, platform: Platform, qubit: QubitId):
     """Update t2 value in platform for specific qubit."""
     if isinstance(t2, tuple):
-        platform.qubits[qubit].t2 = int(t2[0])
+        platform.qubits[qubit].T2 = int(t2[0])
     else:
-        platform.qubits[qubit].t2 = int(t2)
+        platform.qubits[qubit].T2 = int(t2)
 
 
 def t2_spin_echo(t2_spin_echo: float, platform: Platform, qubit: QubitId):
     """Update t2 echo value in platform for specific qubit."""
     if isinstance(t2_spin_echo, tuple):
-        platform.qubits[qubit].t2_spin_echo = int(t2_spin_echo[0])
+        platform.qubits[qubit].T2_spin_echo = int(t2_spin_echo[0])
     else:
-        platform.qubits[qubit].t2_spin_echo = int(t2_spin_echo)
+        platform.qubits[qubit].T2_spin_echo = int(t2_spin_echo)
 
 
 def drag_pulse_beta(beta: float, platform: Platform, qubit: QubitId):
     """Update beta parameter value in platform for specific qubit."""
     pulse = platform.qubits[qubit].native_gates.RX.pulse(start=0)
     rel_sigma = pulse.shape.rel_sigma
     drag_pulse = pulses.Drag(rel_sigma=rel_sigma, beta=beta)
```

### Comparing `qibocal-0.0.7/src/qibocal/web/report.py` & `qibocal-0.0.8/src/qibocal/web/report.py`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/web/static/styles.css` & `qibocal-0.0.8/src/qibocal/web/static/styles.css`

 * *Files identical despite different names*

### Comparing `qibocal-0.0.7/src/qibocal/web/templates/template.html` & `qibocal-0.0.8/src/qibocal/web/templates/template.html`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,15 @@
 
       {% for task_uid in report.history %}
 
       <div id="{{report.routine_name(*task_uid)}}" style="scroll-margin-top: 4em;">
         <h4
           class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
           {{ report.routine_name(*task_uid) }}</h4>
-        {% for qubit in report.routine_qubits(task_uid) %}
+        {% for qubit in report.routine_targets(task_uid) %}
         <div id="{{ routine }}-{{ iteration }}-{{ qubit }}" style="scroll-margin-top: 4em;">
             <h5
               class="d-flex justify-content-between flex-wrap flex-md-nowrap align-items-center pt-3 pb-2 mb-3 border-bottom">
               {{ header }} - Qubit {{ qubit }}</h5>
 
 
             {% set figures, fitting_report = report.single_qubit_plot(task_uid, qubit) %}
```

#### html2text {}

```diff
@@ -25,15 +25,15 @@
 Export to pdf
 Platform: {{ report.metadata.get('platform')}}
 Run date: {{ report.metadata.get('date') }}
 Start time (UTC): {{ report.metadata.get('start-time') }}
 End time (UTC): {{ report.metadata.get('end-time') }}
 {% for task_uid in report.history %}
 ****** {{{{ rreeppoorrtt..rroouuttiinnee__nnaammee((**ttaasskk__uuiidd)) }}}} ******
-{% for qubit in report.routine_qubits(task_uid) %}
+{% for qubit in report.routine_targets(task_uid) %}
 **** {{{{ hheeaaddeerr }}}} -- QQuubbiitt {{{{ qquubbiitt }}}} ****
 {% set figures, fitting_report = report.single_qubit_plot(task_uid, qubit) %} {
 { fitting_report }} {{ figures }}
 {% endfor %}
 {% endfor %} {% endif %}
 ******** SSuummmmaarryy ********
 In the table below we show the libraries and respective versions used in {
```

### Comparing `qibocal-0.0.7/PKG-INFO` & `qibocal-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qibocal
-Version: 0.0.7
+Version: 0.0.8
 Summary: Qibo's quantum calibration, characterization and validation module.
 Home-page: https://qibo.science/
 License: Apache-2.0
 Author: andrea-pasquale
 Author-email: andreapasquale97@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -14,34 +14,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides-Extra: classify
 Provides-Extra: viz
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: dash (>=2.6.0,<3.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: keras-tuner (>=1.3.0,<1.3.1) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "classify")
 Requires-Dist: matplotlib (>=3.7.0,<4.0.0) ; extra == "classify"
-Requires-Dist: networkx (>=3.0,<4.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: onnx (>=1.13.1,<2.0.0) ; extra == "classify"
+Requires-Dist: numpy (>=1.26.4,<2.0.0)
 Requires-Dist: onnxruntime (>=1.14.1,<2.0.0) ; extra == "classify"
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: plotly (>=5.15.0,<6.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
 Requires-Dist: pydot (>=1.4.2,<2.0.0) ; extra == "viz"
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: qibo (>=0.2.1,<0.3.0)
-Requires-Dist: qibolab (>=0.1.5,<0.2.0)
+Requires-Dist: qibo (>=0.2.6,<0.3.0)
+Requires-Dist: qibolab (>=0.1.6,<0.2.0)
 Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0) ; extra == "classify"
 Requires-Dist: setuptools (>=67.8.0,<68.0.0)
 Requires-Dist: skl2onnx (>=1.14.0,<2.0.0) ; extra == "classify"
 Requires-Dist: skops (>=0.6.0,<0.7.0)
-Requires-Dist: tensorflow (>=2.12.0,<3.0.0) ; (sys_platform == "linux" or sys_platform == "darwin") and (extra == "classify")
 Project-URL: Documentation, https://qibo.science/qibocal/stable/
 Project-URL: Repository, https://github.com/qiboteam/qibocal/
 Description-Content-Type: text/markdown
 
 # Qibocal
 [![codecov](https://codecov.io/gh/qiboteam/qibocal/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibocal)
 ![PyPI - Version](https://img.shields.io/pypi/v/qibocal)
```

