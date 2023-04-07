# Comparing `tmp/dkist_processing_cryonirsp-0.0.1rc1.tar.gz` & `tmp/dkist_processing_cryonirsp-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_cryonirsp-0.0.1rc1.tar", last modified: Tue Apr  4 17:23:32 2023, max compression
+gzip compressed data, was "dkist_processing_cryonirsp-0.0.1rc2.tar", last modified: Fri Apr  7 17:53:25 2023, max compression
```

## Comparing `dkist_processing_cryonirsp-0.0.1rc1.tar` & `dkist_processing_cryonirsp-0.0.1rc2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.426401 dkist_processing_cryonirsp-0.0.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4671 2023-04-04 17:23:32.426401 dkist_processing_cryonirsp-0.0.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4153 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2737 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.410401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.414401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5158 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     8824 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     6535 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      755 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/task_name.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.414401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2620 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      886 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     6564 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1872 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/measurements.py
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/modstates.py
--rw-rw-rw-   0 root         (0) root         (0)     1104 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     1754 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/polcal_task.py
--rw-rw-rw-   0 root         (0) root         (0)     2851 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/scan_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1534 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/spectral_line.py
--rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     2496 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.418401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3978 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/bad_pixel_map.py
--rw-rw-rw-   0 root         (0) root         (0)    14150 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/ci_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)     4373 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/ci_science.py
--rw-rw-rw-   0 root         (0) root         (0)     3209 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/cryonirsp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3844 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     7600 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    19346 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     9936 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/linearity_correction.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.418401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1661 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/beam_access.py
--rw-rw-rw-   0 root         (0) root         (0)     5149 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/input_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     7499 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     9099 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     8276 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     8575 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    16769 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/science_base.py
--rw-rw-rw-   0 root         (0) root         (0)    24438 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)     7779 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)     8227 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_science.py
--rw-rw-rw-   0 root         (0) root         (0)    24203 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_solar_gain.py
--rw-rw-rw-   0 root         (0) root         (0)    13302 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.422402 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23554 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/ci_e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)    22348 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     4229 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/e2e_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     6104 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/e2e_linearize.py
--rw-rw-rw-   0 root         (0) root         (0)    22873 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/sp_e2e_test.py
--rw-rw-rw-   0 root         (0) root         (0)     4958 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py
--rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_beam_boundaries.py
--rw-rw-rw-   0 root         (0) root         (0)     4497 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     4587 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    13729 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_ci_science.py
--rw-rw-rw-   0 root         (0) root         (0)     7173 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_cryo_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2190 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_cryo_constants.py
--rw-rw-rw-   0 root         (0) root         (0)    10540 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)    12006 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)    18752 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5220 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_linearity_correction.py
--rw-rw-rw-   0 root         (0) root         (0)     3670 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    27043 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4440 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    10892 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)     4577 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    15816 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9201 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_submit_qualilty.py
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.422402 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3776 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/ci_l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     3785 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/sp_l0_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.410401 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4671 2023-04-04 17:23:32.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4527 2023-04-04 17:23:32.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-04 17:23:32.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-04 17:23:32.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-04 17:23:32.000000 dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.426401 dkist_processing_cryonirsp-0.0.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/ci_l0_to_l1_cryonirsp.rst
--rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      297 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/docs/sp_l0_to_l1_cryonirsp.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-04 17:23:32.426401 dkist_processing_cryonirsp-0.0.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1590 2023-04-04 17:23:32.426401 dkist_processing_cryonirsp-0.0.1rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-04 17:23:21.000000 dkist_processing_cryonirsp-0.0.1rc1/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      804 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4671 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4153 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2737 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.948305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.948305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5158 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     8824 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      755 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/task_name.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.952305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      886 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     6564 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/measurements.py
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/modstates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1104 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/polcal_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2851 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/scan_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1534 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/spectral_line.py
+-rw-rw-rw-   0 root         (0) root         (0)     1530 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     2496 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.952305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5653 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3978 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/bad_pixel_map.py
+-rw-rw-rw-   0 root         (0) root         (0)    14150 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     7408 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/ci_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)     4373 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/ci_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     3209 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/cryonirsp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3844 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     7600 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    19346 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     9936 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/linearity_correction.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.952305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1661 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/beam_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     5149 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/input_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     7499 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     9099 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     8137 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     8575 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    16769 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/science_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24438 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)     7779 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)     8227 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_science.py
+-rw-rw-rw-   0 root         (0) root         (0)    24203 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_solar_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    13302 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23554 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/ci_e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)    22348 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     4229 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/e2e_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6104 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/e2e_linearize.py
+-rw-rw-rw-   0 root         (0) root         (0)    22873 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/sp_e2e_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     4958 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4419 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py
+-rw-rw-rw-   0 root         (0) root         (0)     4867 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_beam_boundaries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4497 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     4587 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    13729 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_ci_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     7173 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_cryo_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2190 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_cryo_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    10540 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    12006 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    18752 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5220 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_linearity_correction.py
+-rw-rw-rw-   0 root         (0) root         (0)     3670 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    27043 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4440 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    10892 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)     4577 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    15816 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9201 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_submit_qualilty.py
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)    11689 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3776 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/ci_l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     3950 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/sp_l0_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.948305 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4671 2023-04-07 17:53:25.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4527 2023-04-07 17:53:25.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-07 17:53:25.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      596 2023-04-07 17:53:25.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       27 2023-04-07 17:53:25.000000 dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/ci_l0_to_l1_cryonirsp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2038 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      297 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/docs/sp_l0_to_l1_cryonirsp.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1590 2023-04-07 17:53:25.956305 dkist_processing_cryonirsp-0.0.1rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-04-07 17:53:19.000000 dkist_processing_cryonirsp-0.0.1rc2/setup.py
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/.gitignore` & `dkist_processing_cryonirsp-0.0.1rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/.pre-commit-config.yaml` & `dkist_processing_cryonirsp-0.0.1rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/PKG-INFO` & `dkist_processing_cryonirsp-0.0.1rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_cryonirsp
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Science processing code for the Cryo-NIRSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist_processing_cryonirsp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/README.rst` & `dkist_processing_cryonirsp-0.0.1rc2/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/bitbucket-pipelines.yml` & `dkist_processing_cryonirsp-0.0.1rc2/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/constants.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/parameters.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/spectral_line.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/tags.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 class CryonirspStemName(str, Enum):
     """Controlled list of Tag Stems."""
 
     linearized = "LINEARIZED"
     beam = "BEAM"
-    arm_id = "ARM_ID"
     scan_step = "SCAN_STEP"
     curr_frame_in_ramp = "CURR_FRAME_IN_RAMP"
     time_obs = "TIME_OBS"
     meas_num = "MEAS_NUM"
     modstate = "MODSTATE"
     map_scan = "MAP_SCAN"
 
@@ -97,30 +96,14 @@
         Returns
         -------
         The formatted tag string
         """
         return cls.format_tag(CryonirspStemName.linearized)
 
     @classmethod
-    def arm_id(cls, arm_id: str) -> str:
-        """
-        Tags based on the CryoNIRSP arm_id from which the data is recorded (SP or CI).
-
-        Parameters
-        ----------
-        arm_id
-            The arm ID in use, SP or CI
-
-        Returns
-        -------
-        The formatted tag string
-        """
-        return cls.format_tag(CryonirspStemName.arm_id, arm_id)
-
-    @classmethod
     def curr_frame_in_ramp(cls, curr_frame_in_ramp: int) -> str:
         """
         Tags based on the current frame number in the ramp.
 
         Parameters
         ----------
         curr_frame_in_ramp
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/models/task_name.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/models/task_name.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/cryonirsp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/cryonirsp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/map_repeats.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/measurements.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/measurements.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/modstates.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/modstates.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/polarimeter_mode.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/polcal_task.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/polcal_task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/scan_step.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/scan_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/spectral_line.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/spectral_line.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/task.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/time.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/parsers/wavelength.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/assemble_movie.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/bad_pixel_map.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/bad_pixel_map.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/beam_boundaries.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/ci_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/ci_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/ci_science.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/ci_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/cryonirsp_base.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/cryonirsp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/dark.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/gain.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/instrument_polarization.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/l1_output_data.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/linearity_correction.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/linearity_correction.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/beam_access.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/beam_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/corrections.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/input_frame.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/input_frame.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/intermediate_frame.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/mixin/linearized_frame.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/parse.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/parse.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,17 +172,14 @@
     @property
     def tag_flowers(self) -> list[S]:
         """Add CryoNIRSP specific tags to common tags."""
         # Items defined here are tags
         return super().tag_flowers + [
             CryonirspTaskTypeFlower(),
             PolcalTaskFlower(),
-            SingleValueSingleKeyFlower(
-                tag_stem_name=CryonirspStemName.arm_id.value, metadata_key="arm_id"
-            ),
             MapScanFlower(),
             ModstateNumberFlower(),
             ExposureTimeFlower(),
             CSStepFlower(max_cs_step_time_sec=self.parameters.max_cs_step_time_sec),
             ScanStepNumberFlower(),
             MeasurementNumberFlower(),
         ]
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/quality_metrics.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/science_base.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/science_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_geometric.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_science.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/sp_solar_gain.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/sp_solar_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tasks/write_l1.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/ci_e2e_test.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/ci_e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/conftest.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/e2e_helpers.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/e2e_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/e2e_linearize.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/e2e_linearize.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/sp_e2e_test.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/sp_e2e_test.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_assemble_movie.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_bad_pixel_maps.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_beam_boundaries.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_beam_boundaries.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_build_quality_report.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_ci_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_ci_science.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_ci_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_cryo_base.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_cryo_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_cryo_constants.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_cryo_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_dark.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_gain.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_instrument_polarization.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_linearity_correction.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_linearity_correction.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_parameters.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_parse.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_quality.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_geometric.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_science.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_sp_solar.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_sp_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_submit_qualilty.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_submit_qualilty.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/tests/test_write_l1.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/ci_l0_processing.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/ci_l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp/workflows/sp_l0_processing.py` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp/workflows/sp_l0_processing.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     SPInstrumentPolarizationCalibration,
 )
 from dkist_processing_cryonirsp.tasks.linearity_correction import LinearityCorrection
 from dkist_processing_cryonirsp.tasks.parse import ParseL0CryonirspLinearizedData
 from dkist_processing_cryonirsp.tasks.parse import ParseL0CryonirspRampData
 from dkist_processing_cryonirsp.tasks.quality_metrics import CryonirspL0QualityMetrics
 from dkist_processing_cryonirsp.tasks.quality_metrics import CryonirspL1QualityMetrics
+from dkist_processing_cryonirsp.tasks.sp_geometric import SPGeometricCalibration
 from dkist_processing_cryonirsp.tasks.sp_make_movie_frames import SPMakeCryonirspMovieFrames
 from dkist_processing_cryonirsp.tasks.sp_science import SPScienceCalibration
 from dkist_processing_cryonirsp.tasks.sp_solar_gain import SPSolarGainCalibration
 from dkist_processing_cryonirsp.tasks.write_l1 import SPWriteL1Frame
 
 l0_pipeline = Workflow(
     category="cryonirsp_sp",
@@ -37,15 +38,16 @@
 l0_pipeline.add_node(task=LinearityCorrection, upstreams=ParseL0CryonirspRampData)
 l0_pipeline.add_node(task=ParseL0CryonirspLinearizedData, upstreams=LinearityCorrection)
 l0_pipeline.add_node(task=CryonirspL0QualityMetrics, upstreams=ParseL0CryonirspLinearizedData)
 l0_pipeline.add_node(task=BadPixelMapCalibration, upstreams=CryonirspL0QualityMetrics)
 l0_pipeline.add_node(task=BeamBoundariesCalibration, upstreams=BadPixelMapCalibration)
 l0_pipeline.add_node(task=DarkCalibration, upstreams=BeamBoundariesCalibration)
 l0_pipeline.add_node(task=LampGainCalibration, upstreams=DarkCalibration)
-l0_pipeline.add_node(task=SPSolarGainCalibration, upstreams=LampGainCalibration)
+l0_pipeline.add_node(task=SPGeometricCalibration, upstreams=LampGainCalibration)
+l0_pipeline.add_node(task=SPSolarGainCalibration, upstreams=SPGeometricCalibration)
 l0_pipeline.add_node(task=SPInstrumentPolarizationCalibration, upstreams=SPSolarGainCalibration)
 l0_pipeline.add_node(task=SPScienceCalibration, upstreams=SPInstrumentPolarizationCalibration)
 l0_pipeline.add_node(task=SPWriteL1Frame, upstreams=SPScienceCalibration)
 l0_pipeline.add_node(task=QualityL1Metrics, upstreams=SPWriteL1Frame)
 l0_pipeline.add_node(task=CryonirspL1QualityMetrics, upstreams=SPWriteL1Frame)
 l0_pipeline.add_node(
     task=SubmitQuality,
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/PKG-INFO` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-cryonirsp
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: Science processing code for the Cryo-NIRSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist_processing_cryonirsp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/SOURCES.txt` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/dkist_processing_cryonirsp.egg-info/requires.txt` & `dkist_processing_cryonirsp-0.0.1rc2/dkist_processing_cryonirsp.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/docs/Makefile` & `dkist_processing_cryonirsp-0.0.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/docs/ci_l0_to_l1_cryonirsp.rst` & `dkist_processing_cryonirsp-0.0.1rc2/docs/ci_l0_to_l1_cryonirsp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/docs/conf.py` & `dkist_processing_cryonirsp-0.0.1rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/docs/make.bat` & `dkist_processing_cryonirsp-0.0.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/docs/sp_l0_to_l1_cryonirsp.rst` & `dkist_processing_cryonirsp-0.0.1rc2/docs/sp_l0_to_l1_cryonirsp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/licenses/LICENSE.rst` & `dkist_processing_cryonirsp-0.0.1rc2/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_cryonirsp-0.0.1rc1/setup.cfg` & `dkist_processing_cryonirsp-0.0.1rc2/setup.cfg`

 * *Files identical despite different names*

