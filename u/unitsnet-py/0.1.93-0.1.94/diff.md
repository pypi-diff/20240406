# Comparing `tmp/unitsnet-py-0.1.93.tar.gz` & `tmp/unitsnet-py-0.1.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitsnet-py-0.1.93.tar", last modified: Thu Apr  4 17:43:34 2024, max compression
+gzip compressed data, was "unitsnet-py-0.1.94.tar", last modified: Sat Apr  6 20:51:32 2024, max compression
```

## Comparing `unitsnet-py-0.1.93.tar` & `unitsnet-py-0.1.94.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:43:34.099506 unitsnet-py-0.1.93/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-04 17:43:14.000000 unitsnet-py-0.1.93/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    29928 2024-04-04 17:43:34.099506 unitsnet-py-0.1.93/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    29375 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:43:34.099506 unitsnet-py-0.1.93/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-04 17:43:27.000000 unitsnet-py-0.1.93/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:43:34.079506 unitsnet-py-0.1.93/unitsnet_py/
--rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-04 17:43:14.000000 unitsnet-py-0.1.93/unitsnet_py/abstract_unit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:43:34.099506 unitsnet-py-0.1.93/unitsnet_py/units/
--rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
--rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/acceleration.py
--rw-r--r--   0 runner    (1001) docker     (127)    24365 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/amount_of_substance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/amplitude_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)    20276 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/angle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/apparent_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/apparent_power.py
--rw-r--r--   0 runner    (1001) docker     (127)    21861 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/area.py
--rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/area_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/area_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/bit_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/brake_specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/capacitance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/coefficient_of_thermal_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/compressibility.py
--rw-r--r--   0 runner    (1001) docker     (127)    82985 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/density.py
--rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/duration.py
--rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/dynamic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_admittance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_conductance.py
--rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_current.py
--rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_current_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_current_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_inductance.py
--rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_potential.py
--rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_ac.py
--rw-r--r--   0 runner    (1001) docker     (127)    34546 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_dc.py
--rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    22246 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_resistivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/electric_surface_charge_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    21082 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/energy_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/force.py
--rw-r--r--   0 runner    (1001) docker     (127)    24886 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/force_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    60392 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/force_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/frequency.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/fuel_efficiency.py
--rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/heat_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/heat_transfer_coefficient.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/illuminance.py
--rw-r--r--   0 runner    (1001) docker     (127)    19586 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/impulse.py
--rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/information.py
--rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/irradiance.py
--rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/irradiation.py
--rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/jerk.py
--rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/kinematic_viscosity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/leak_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    54141 2024-04-04 17:43:24.000000 unitsnet-py-0.1.93/unitsnet_py/units/length.py
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/level.py
--rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/linear_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    39789 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/linear_power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/luminance.py
--rw-r--r--   0 runner    (1001) docker     (127)    18581 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/luminosity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/luminous_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/luminous_intensity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/magnetic_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/magnetic_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/magnetization.py
--rw-r--r--   0 runner    (1001) docker     (127)    38317 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    77865 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)    46027 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    22990 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass_flux.py
--rw-r--r--   0 runner    (1001) docker     (127)    35460 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass_fraction.py
--rw-r--r--   0 runner    (1001) docker     (127)    46516 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/mass_moment_of_inertia.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molality.py
--rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molar_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molar_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molar_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molar_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/molarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/permeability.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/permittivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/porous_medium_permeability.py
--rw-r--r--   0 runner    (1001) docker     (127)    34531 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/power.py
--rw-r--r--   0 runner    (1001) docker     (127)    67957 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/power_density.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/power_ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)    71480 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/pressure.py
--rw-r--r--   0 runner    (1001) docker     (127)    31983 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/pressure_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/radiation_equivalent_dose.py
--rw-r--r--   0 runner    (1001) docker     (127)    13976 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/radiation_exposure.py
--rw-r--r--   0 runner    (1001) docker     (127)    40280 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/radioactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/ratio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/ratio_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/reactive_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/reactive_power.py
--rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/reciprocal_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/reciprocal_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/relative_humidity.py
--rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/rotational_acceleration.py
--rw-r--r--   0 runner    (1001) docker     (127)    21827 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/rotational_speed.py
--rw-r--r--   0 runner    (1001) docker     (127)    59692 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/rotational_stiffness.py
--rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/rotational_stiffness_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/scalar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/solid_angle.py
--rw-r--r--   0 runner    (1001) docker     (127)    48046 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/specific_energy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17122 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/specific_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/specific_fuel_consumption.py
--rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/specific_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    30235 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/specific_weight.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/speed.py
--rw-r--r--   0 runner    (1001) docker     (127)    17586 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/standard_volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)    19399 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/temperature_change_rate.py
--rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/temperature_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/temperature_gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/thermal_conductivity.py
--rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/thermal_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)    36640 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/torque.py
--rw-r--r--   0 runner    (1001) docker     (127)    37174 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/torque_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/turbidity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/vitamin_a.py
--rw-r--r--   0 runner    (1001) docker     (127)    69416 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    32167 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volume_concentration.py
--rw-r--r--   0 runner    (1001) docker     (127)   108994 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volume_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volume_flow_per_area.py
--rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volume_per_length.py
--rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/volumetric_heat_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-04 17:43:25.000000 unitsnet-py-0.1.93/unitsnet_py/units/warping_moment_of_inertia.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:43:34.079506 unitsnet-py-0.1.93/unitsnet_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29928 2024-04-04 17:43:34.000000 unitsnet-py-0.1.93/unitsnet_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-04 17:43:34.000000 unitsnet-py-0.1.93/unitsnet_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:43:34.000000 unitsnet-py-0.1.93/unitsnet_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-04 17:43:34.000000 unitsnet-py-0.1.93/unitsnet_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:51:32.414056 unitsnet-py-0.1.94/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-06 20:51:15.000000 unitsnet-py-0.1.94/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    29928 2024-04-06 20:51:32.414056 unitsnet-py-0.1.94/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    29375 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:51:32.414056 unitsnet-py-0.1.94/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-06 20:51:26.000000 unitsnet-py-0.1.94/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:51:32.390056 unitsnet-py-0.1.94/unitsnet_py/
+-rw-r--r--   0 runner    (1001) docker     (127)    14051 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-06 20:51:15.000000 unitsnet-py-0.1.94/unitsnet_py/abstract_unit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:51:32.414056 unitsnet-py-0.1.94/unitsnet_py/units/
+-rw-r--r--   0 runner    (1001) docker     (127)    25439 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23490 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24365 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/amount_of_substance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7499 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/amplitude_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20276 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-06 20:51:23.000000 unitsnet-py-0.1.94/unitsnet_py/units/apparent_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/apparent_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21861 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/area.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/area_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/area_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20811 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/bit_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7919 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/brake_specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/capacitance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11733 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/coefficient_of_thermal_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12120 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/compressibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82985 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14510 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/duration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16852 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/dynamic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7390 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_admittance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_conductance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11475 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13590 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_current.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7070 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_current_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_current_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3379 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_inductance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9716 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_potential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8701 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34546 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_dc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10791 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22246 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_resistivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/electric_surface_charge_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51988 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21082 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/energy_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24235 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/force.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24886 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/force_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60392 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/force_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17587 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/fuel_efficiency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29449 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/heat_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/heat_transfer_coefficient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/illuminance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19586 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/impulse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18532 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/information.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23997 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/irradiance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16064 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/irradiation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17971 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/jerk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14345 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/kinematic_viscosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/leak_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54141 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4064 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22618 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/linear_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39789 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/linear_power_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/luminance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18581 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/luminosity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3111 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/luminous_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/luminous_intensity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9363 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/magnetic_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/magnetic_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/magnetization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38317 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    77865 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46027 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22990 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass_flux.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35460 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass_fraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46516 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/mass_moment_of_inertia.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6060 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molar_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molar_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14295 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molar_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molar_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17438 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/molarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/permeability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/permittivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9114 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/porous_medium_permeability.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34531 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67957 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/power_ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71480 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/pressure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31983 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/pressure_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11804 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/radiation_equivalent_dose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13976 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/radiation_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40280 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/radioactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9645 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/ratio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5111 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/ratio_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6949 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/reactive_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8173 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/reactive_power.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18779 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/reciprocal_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15917 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/reciprocal_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/relative_humidity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9099 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/rotational_acceleration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21827 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/rotational_speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59692 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/rotational_stiffness.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12178 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/rotational_stiffness_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/solid_angle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48046 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/specific_energy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17122 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/specific_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-04-06 20:51:24.000000 unitsnet-py-0.1.94/unitsnet_py/units/specific_fuel_consumption.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/specific_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30235 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/specific_weight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/speed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17586 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/standard_volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15447 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19399 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/temperature_change_rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14262 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/temperature_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8415 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/temperature_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/thermal_conductivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13301 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/thermal_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36640 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/torque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37174 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/torque_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/turbidity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/vitamin_a.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69416 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32167 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volume_concentration.py
+-rw-r--r--   0 runner    (1001) docker     (127)   108994 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volume_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5845 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volume_flow_per_area.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15469 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volume_per_length.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19509 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/volumetric_heat_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-06 20:51:25.000000 unitsnet-py-0.1.94/unitsnet_py/units/warping_moment_of_inertia.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:51:32.394056 unitsnet-py-0.1.94/unitsnet_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29928 2024-04-06 20:51:32.000000 unitsnet-py-0.1.94/unitsnet_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-04-06 20:51:32.000000 unitsnet-py-0.1.94/unitsnet_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:51:32.000000 unitsnet-py-0.1.94/unitsnet_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:51:32.000000 unitsnet-py-0.1.94/unitsnet_py.egg-info/top_level.txt
```

### Comparing `unitsnet-py-0.1.93/LICENSE` & `unitsnet-py-0.1.94/LICENSE`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/PKG-INFO` & `unitsnet-py-0.1.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.93
+Version: 0.1.94
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 License: MIT
```

### Comparing `unitsnet-py-0.1.93/README.md` & `unitsnet-py-0.1.94/README.md`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/setup.py` & `unitsnet-py-0.1.94/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['unitsnet_py', 'unitsnet_py.units']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'unitsnet-py',
-    'version': '0.1.93',
+    'version': '0.1.94',
     'license': 'MIT',
     'keywords': 'conversion, units-of-measure, units, quantities, unit-converter, converter, unit, measure, measures, measurement, measurements',
     'description': 'A better way to hold unit variables and easily convert to the destination unit',
     'long_description': long_description,
     'long_description_content_type': "text/markdown",
     'author': 'Haim Kastner',
     'author_email': 'haim.kastner@gmail.com',
```

### Comparing `unitsnet-py-0.1.93/unitsnet_py/__init__.py` & `unitsnet-py-0.1.94/unitsnet_py/__init__.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/abstract_unit.py` & `unitsnet-py-0.1.94/unitsnet_py/abstract_unit.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py` & `unitsnet-py-0.1.94/unitsnet_py/units/absorbed_dose_of_ionizing_radiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/acceleration.py` & `unitsnet-py-0.1.94/unitsnet_py/units/acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/amount_of_substance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/amount_of_substance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/amplitude_ratio.py` & `unitsnet-py-0.1.94/unitsnet_py/units/amplitude_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/angle.py` & `unitsnet-py-0.1.94/unitsnet_py/units/angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/apparent_energy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/apparent_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/apparent_power.py` & `unitsnet-py-0.1.94/unitsnet_py/units/apparent_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/area.py` & `unitsnet-py-0.1.94/unitsnet_py/units/area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/area_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/area_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/area_moment_of_inertia.py` & `unitsnet-py-0.1.94/unitsnet_py/units/area_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/bit_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/bit_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/brake_specific_fuel_consumption.py` & `unitsnet-py-0.1.94/unitsnet_py/units/brake_specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/capacitance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/capacitance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/coefficient_of_thermal_expansion.py` & `unitsnet-py-0.1.94/unitsnet_py/units/coefficient_of_thermal_expansion.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/compressibility.py` & `unitsnet-py-0.1.94/unitsnet_py/units/compressibility.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/duration.py` & `unitsnet-py-0.1.94/unitsnet_py/units/duration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/dynamic_viscosity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/dynamic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_admittance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_admittance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_charge.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_charge.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_charge_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_conductance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_conductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_conductivity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_current.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_current.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_current_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_current_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_current_gradient.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_current_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_field.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_inductance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_inductance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_potential.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_potential.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_ac.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_ac.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_change_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_potential_dc.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_potential_dc.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_resistance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_resistivity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_resistivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/electric_surface_charge_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/electric_surface_charge_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/energy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/energy_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/energy_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/entropy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/force.py` & `unitsnet-py-0.1.94/unitsnet_py/units/force.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/force_change_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/force_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/force_per_length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/force_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/frequency.py` & `unitsnet-py-0.1.94/unitsnet_py/units/frequency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/fuel_efficiency.py` & `unitsnet-py-0.1.94/unitsnet_py/units/fuel_efficiency.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/heat_flux.py` & `unitsnet-py-0.1.94/unitsnet_py/units/heat_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/heat_transfer_coefficient.py` & `unitsnet-py-0.1.94/unitsnet_py/units/heat_transfer_coefficient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/illuminance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/illuminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/impulse.py` & `unitsnet-py-0.1.94/unitsnet_py/units/impulse.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/information.py` & `unitsnet-py-0.1.94/unitsnet_py/units/information.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/irradiance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/irradiance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/irradiation.py` & `unitsnet-py-0.1.94/unitsnet_py/units/irradiation.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/jerk.py` & `unitsnet-py-0.1.94/unitsnet_py/units/jerk.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/kinematic_viscosity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/kinematic_viscosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/leak_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/leak_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/level.py` & `unitsnet-py-0.1.94/unitsnet_py/units/level.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/linear_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/linear_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/linear_power_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/linear_power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/luminance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/luminance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/luminosity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/luminosity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/luminous_flux.py` & `unitsnet-py-0.1.94/unitsnet_py/units/luminous_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/luminous_intensity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/luminous_intensity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/magnetic_field.py` & `unitsnet-py-0.1.94/unitsnet_py/units/magnetic_field.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/magnetic_flux.py` & `unitsnet-py-0.1.94/unitsnet_py/units/magnetic_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/magnetization.py` & `unitsnet-py-0.1.94/unitsnet_py/units/magnetization.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass_concentration.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass_flow.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass_flux.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass_flux.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass_fraction.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass_fraction.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/mass_moment_of_inertia.py` & `unitsnet-py-0.1.94/unitsnet_py/units/mass_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molality.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molality.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molar_energy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molar_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molar_entropy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molar_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molar_flow.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molar_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molar_mass.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molar_mass.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/molarity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/molarity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/permeability.py` & `unitsnet-py-0.1.94/unitsnet_py/units/permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/permittivity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/permittivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/porous_medium_permeability.py` & `unitsnet-py-0.1.94/unitsnet_py/units/porous_medium_permeability.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/power.py` & `unitsnet-py-0.1.94/unitsnet_py/units/power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/power_density.py` & `unitsnet-py-0.1.94/unitsnet_py/units/power_density.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/power_ratio.py` & `unitsnet-py-0.1.94/unitsnet_py/units/power_ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/pressure.py` & `unitsnet-py-0.1.94/unitsnet_py/units/pressure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/pressure_change_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/pressure_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/radiation_equivalent_dose.py` & `unitsnet-py-0.1.94/unitsnet_py/units/radiation_equivalent_dose.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/radiation_exposure.py` & `unitsnet-py-0.1.94/unitsnet_py/units/radiation_exposure.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/radioactivity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/radioactivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/ratio.py` & `unitsnet-py-0.1.94/unitsnet_py/units/ratio.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/ratio_change_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/ratio_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/reactive_energy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/reactive_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/reactive_power.py` & `unitsnet-py-0.1.94/unitsnet_py/units/reactive_power.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/reciprocal_area.py` & `unitsnet-py-0.1.94/unitsnet_py/units/reciprocal_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/reciprocal_length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/reciprocal_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/relative_humidity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/relative_humidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/rotational_acceleration.py` & `unitsnet-py-0.1.94/unitsnet_py/units/rotational_acceleration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/rotational_speed.py` & `unitsnet-py-0.1.94/unitsnet_py/units/rotational_speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/rotational_stiffness.py` & `unitsnet-py-0.1.94/unitsnet_py/units/rotational_stiffness.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/rotational_stiffness_per_length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/rotational_stiffness_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/scalar.py` & `unitsnet-py-0.1.94/unitsnet_py/units/scalar.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/solid_angle.py` & `unitsnet-py-0.1.94/unitsnet_py/units/solid_angle.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/specific_energy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/specific_energy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/specific_entropy.py` & `unitsnet-py-0.1.94/unitsnet_py/units/specific_entropy.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/specific_fuel_consumption.py` & `unitsnet-py-0.1.94/unitsnet_py/units/specific_fuel_consumption.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/specific_volume.py` & `unitsnet-py-0.1.94/unitsnet_py/units/specific_volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/specific_weight.py` & `unitsnet-py-0.1.94/unitsnet_py/units/specific_weight.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/speed.py` & `unitsnet-py-0.1.94/unitsnet_py/units/speed.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/standard_volume_flow.py` & `unitsnet-py-0.1.94/unitsnet_py/units/standard_volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/temperature.py` & `unitsnet-py-0.1.94/unitsnet_py/units/temperature.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/temperature_change_rate.py` & `unitsnet-py-0.1.94/unitsnet_py/units/temperature_change_rate.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/temperature_delta.py` & `unitsnet-py-0.1.94/unitsnet_py/units/temperature_delta.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/temperature_gradient.py` & `unitsnet-py-0.1.94/unitsnet_py/units/temperature_gradient.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/thermal_conductivity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/thermal_conductivity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/thermal_resistance.py` & `unitsnet-py-0.1.94/unitsnet_py/units/thermal_resistance.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/torque.py` & `unitsnet-py-0.1.94/unitsnet_py/units/torque.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/torque_per_length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/torque_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/turbidity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/turbidity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/vitamin_a.py` & `unitsnet-py-0.1.94/unitsnet_py/units/vitamin_a.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volume.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volume.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volume_concentration.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volume_concentration.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volume_flow.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volume_flow.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volume_flow_per_area.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volume_flow_per_area.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volume_per_length.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volume_per_length.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/volumetric_heat_capacity.py` & `unitsnet-py-0.1.94/unitsnet_py/units/volumetric_heat_capacity.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py/units/warping_moment_of_inertia.py` & `unitsnet-py-0.1.94/unitsnet_py/units/warping_moment_of_inertia.py`

 * *Files identical despite different names*

### Comparing `unitsnet-py-0.1.93/unitsnet_py.egg-info/PKG-INFO` & `unitsnet-py-0.1.94/unitsnet_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitsnet-py
-Version: 0.1.93
+Version: 0.1.94
 Summary: A better way to hold unit variables and easily convert to the destination unit
 Home-page: https://github.com/haimkastner/unitsnet-py
 Author: Haim Kastner
 Author-email: haim.kastner@gmail.com
 Maintainer: Haim Kastner
 Maintainer-email: haim.kastner@gmail.com
 License: MIT
```

### Comparing `unitsnet-py-0.1.93/unitsnet_py.egg-info/SOURCES.txt` & `unitsnet-py-0.1.94/unitsnet_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

