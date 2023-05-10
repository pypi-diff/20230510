# Comparing `tmp/financepy-0.270.tar.gz` & `tmp/financepy-0.290.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "financepy-0.270.tar", last modified: Mon Feb 13 16:38:27 2023, max compression
+gzip compressed data, was "financepy-0.290.tar", last modified: Wed May 10 16:52:55 2023, max compression
```

## Comparing `financepy-0.270.tar` & `financepy-0.290.tar`

### file list

```diff
@@ -1,292 +1,299 @@
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.568952 financepy-0.270/
--rw-rw-rw-   0        0        0    35823 2020-09-30 09:26:37.000000 financepy-0.270/LICENSE
--rw-rw-rw-   0        0        0     7561 2023-02-13 16:38:27.568952 financepy-0.270/PKG-INFO
--rw-rw-rw-   0        0        0     6923 2022-12-15 08:23:27.000000 financepy-0.270/README.md
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.204925 financepy-0.270/financepy/
--rw-rw-rw-   0        0        0      453 2023-02-13 16:38:27.000000 financepy-0.270/financepy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.213902 financepy-0.270/financepy/market/
--rw-rw-rw-   0        0        0        0 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.226867 financepy-0.270/financepy/market/curves/
--rw-rw-rw-   0        0        0      308 2023-02-13 16:33:55.000000 financepy-0.270/financepy/market/curves/__init__.py
--rw-rw-rw-   0        0        0    17339 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve.py
--rw-rw-rw-   0        0        0     5170 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_flat.py
--rw-rw-rw-   0        0        0     6789 2023-02-13 16:33:55.000000 financepy-0.270/financepy/market/curves/discount_curve_ns.py
--rw-rw-rw-   0        0        0     7392 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_nss.py
--rw-rw-rw-   0        0        0     6281 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_poly.py
--rw-rw-rw-   0        0        0     5982 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_pwf.py
--rw-rw-rw-   0        0        0     5825 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_pwl.py
--rw-rw-rw-   0        0        0     5649 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/curves/discount_curve_zeros.py
--rw-rw-rw-   0        0        0    12495 2021-10-05 08:15:43.000000 financepy-0.270/financepy/market/curves/interpolator.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.228861 financepy-0.270/financepy/market/prices/
--rw-rw-rw-   0        0        0       25 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/prices/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.239833 financepy-0.270/financepy/market/volatility/
--rw-rw-rw-   0        0        0      172 2021-12-22 21:07:08.000000 financepy-0.270/financepy/market/volatility/__init__.py
--rw-rw-rw-   0        0        0     2747 2021-10-05 08:15:43.000000 financepy-0.270/financepy/market/volatility/equity_vol_curve.py
--rw-rw-rw-   0        0        0    29959 2022-08-31 19:10:11.000000 financepy-0.270/financepy/market/volatility/equity_vol_surface.py
--rw-rw-rw-   0        0        0    47487 2022-08-31 19:10:11.000000 financepy-0.270/financepy/market/volatility/fx_vol_surface.py
--rw-rw-rw-   0        0        0    92029 2022-08-31 19:10:11.000000 financepy-0.270/financepy/market/volatility/fx_vol_surface_plus.py
--rw-rw-rw-   0        0        0     7343 2021-11-06 12:48:44.000000 financepy-0.270/financepy/market/volatility/ibor_cap_vol_curve.py
--rw-rw-rw-   0        0        0     1497 2021-10-05 08:15:43.000000 financepy-0.270/financepy/market/volatility/ibor_cap_vol_curve_fn.py
--rw-rw-rw-   0        0        0    36051 2022-08-31 19:10:11.000000 financepy-0.270/financepy/market/volatility/swaption_vol_surface.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.301666 financepy-0.270/financepy/models/
--rw-rw-rw-   0        0        0      837 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/__init__.py
--rw-rw-rw-   0        0        0     2299 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/bachelier.py
--rw-rw-rw-   0        0        0    30528 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/bdt_tree.py
--rw-rw-rw-   0        0        0    39920 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/bk_tree.py
--rw-rw-rw-   0        0        0     7081 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/black.py
--rw-rw-rw-   0        0        0     5580 2022-12-28 17:30:01.000000 financepy-0.270/financepy/models/black_scholes.py
--rw-rw-rw-   0        0        0    16083 2022-06-10 20:46:40.000000 financepy-0.270/financepy/models/black_scholes_analytic.py
--rw-rw-rw-   0        0        0     6944 2021-12-22 21:43:40.000000 financepy-0.270/financepy/models/black_scholes_mc.py
--rw-rw-rw-   0        0        0     3117 2021-12-22 21:35:15.000000 financepy-0.270/financepy/models/black_scholes_mc_tests.py
--rw-rw-rw-   0        0        0     2888 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/black_shifted.py
--rw-rw-rw-   0        0        0        0 2022-11-22 10:41:15.000000 financepy-0.270/financepy/models/bond_analytics.py
--rw-rw-rw-   0        0        0    10102 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/cir_mc.py
--rw-rw-rw-   0        0        0     7178 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/equity_crr_tree.py
--rw-rw-rw-   0        0        0     3560 2022-12-28 14:43:04.000000 financepy-0.270/financepy/models/equity_lsmc.py
--rw-rw-rw-   0        0        0     1725 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/gauss_copula.py
--rw-rw-rw-   0        0        0     6379 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/gauss_copula_lhp.py
--rw-rw-rw-   0        0        0     5638 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/gauss_copula_lhplus.py
--rw-rw-rw-   0        0        0    14108 2022-06-10 20:13:01.000000 financepy-0.270/financepy/models/gauss_copula_onefactor.py
--rw-rw-rw-   0        0        0     7254 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/gbm_process_simulator.py
--rw-rw-rw-   0        0        0    14264 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/heston.py
--rw-rw-rw-   0        0        0    50919 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/hw_tree.py
--rw-rw-rw-   0        0        0    33901 2021-12-22 21:46:06.000000 financepy-0.270/financepy/models/lmm_mc.py
--rw-rw-rw-   0        0        0     4361 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/loss_dbn_builder.py
--rw-rw-rw-   0        0        0     5484 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/merton_firm.py
--rw-rw-rw-   0        0        0     6022 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/merton_firm_mkt.py
--rw-rw-rw-   0        0        0      434 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/model.py
--rw-rw-rw-   0        0        0     1985 2021-12-22 19:57:45.000000 financepy-0.270/financepy/models/option_implied_dbn.py
--rw-rw-rw-   0        0        0    14570 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/process_simulator.py
--rw-rw-rw-   0        0        0     3822 2021-11-06 12:48:44.000000 financepy-0.270/financepy/models/rates_ho_lee.py
--rw-rw-rw-   0        0        0    10494 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/sabr.py
--rw-rw-rw-   0        0        0     8306 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/sabr_shifted.py
--rw-rw-rw-   0        0        0     5321 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/sobol.py
--rw-rw-rw-   0        0        0   120492 2020-12-08 14:37:22.000000 financepy-0.270/financepy/models/sobolcoeff.npz
--rw-rw-rw-   0        0        0     1800 2021-10-05 08:15:43.000000 financepy-0.270/financepy/models/student_t_copula.py
--rw-rw-rw-   0        0        0     3303 2021-11-09 10:39:55.000000 financepy-0.270/financepy/models/vasicek_mc.py
--rw-rw-rw-   0        0        0     8210 2022-06-10 20:10:22.000000 financepy-0.270/financepy/models/volatility_fns.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.302664 financepy-0.270/financepy/products/
--rw-rw-rw-   0        0        0        0 2020-09-30 09:26:37.000000 financepy-0.270/financepy/products/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.320622 financepy-0.270/financepy/products/bonds/
--rw-rw-rw-   0        0        0      367 2022-11-22 10:11:01.000000 financepy-0.270/financepy/products/bonds/__init__.py
--rw-rw-rw-   0        0        0    34520 2023-02-13 16:33:55.000000 financepy-0.270/financepy/products/bonds/bond.py
--rw-rw-rw-   0        0        0     7744 2022-03-20 13:06:59.000000 financepy-0.270/financepy/products/bonds/bond_annuity.py
--rw-rw-rw-   0        0        0     9793 2022-03-20 13:01:16.000000 financepy-0.270/financepy/products/bonds/bond_callable.py
--rw-rw-rw-   0        0        0    26813 2022-03-20 13:14:56.000000 financepy-0.270/financepy/products/bonds/bond_convertible.py
--rw-rw-rw-   0        0        0    19575 2022-03-20 13:03:48.000000 financepy-0.270/financepy/products/bonds/bond_frn.py
--rw-rw-rw-   0        0        0     6067 2022-03-20 13:02:32.000000 financepy-0.270/financepy/products/bonds/bond_future.py
--rw-rw-rw-   0        0        0     5176 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/bonds/bond_market.py
--rw-rw-rw-   0        0        0     6495 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/bonds/bond_mortgage.py
--rw-rw-rw-   0        0        0     5841 2022-03-20 13:04:01.000000 financepy-0.270/financepy/products/bonds/bond_option.py
--rw-rw-rw-   0        0        0    11494 2022-03-20 13:04:21.000000 financepy-0.270/financepy/products/bonds/bond_portfolio.py
--rw-rw-rw-   0        0        0    28018 2022-11-22 10:43:37.000000 financepy-0.270/financepy/products/bonds/bond_zero.py
--rw-rw-rw-   0        0        0     6784 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/bonds/yield_curve.py
--rw-rw-rw-   0        0        0     5746 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/bonds/yield_curve_model.py
--rw-rw-rw-   0        0        0     7056 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/bonds/zero_curve.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.330588 financepy-0.270/financepy/products/credit/
--rw-rw-rw-   0        0        0      197 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/credit/__init__.py
--rw-rw-rw-   0        0        0    34584 2022-08-31 17:54:32.000000 financepy-0.270/financepy/products/credit/cds.py
--rw-rw-rw-   0        0        0    13492 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/credit/cds_basket.py
--rw-rw-rw-   0        0        0     8958 2022-08-31 18:05:32.000000 financepy-0.270/financepy/products/credit/cds_curve.py
--rw-rw-rw-   0        0        0    14463 2022-08-31 18:16:21.000000 financepy-0.270/financepy/products/credit/cds_index_option.py
--rw-rw-rw-   0        0        0    19440 2022-08-31 18:13:43.000000 financepy-0.270/financepy/products/credit/cds_index_portfolio.py
--rw-rw-rw-   0        0        0     6774 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/credit/cds_option.py
--rw-rw-rw-   0        0        0     8960 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/credit/cds_tranche.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.356521 financepy-0.270/financepy/products/equity/
--rw-rw-rw-   0        0        0      754 2022-12-28 17:26:13.000000 financepy-0.270/financepy/products/equity/__init__.py
--rw-rw-rw-   0        0        0     4523 2022-12-24 15:09:21.000000 financepy-0.270/financepy/products/equity/equity_american_option.py
--rw-rw-rw-   0        0        0    30586 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_asian_option.py
--rw-rw-rw-   0        0        0    19031 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_barrier_option.py
--rw-rw-rw-   0        0        0    10048 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_basket_option.py
--rw-rw-rw-   0        0        0     8409 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/equity/equity_binomial_tree.py
--rw-rw-rw-   0        0        0     9434 2022-06-10 19:55:23.000000 financepy-0.270/financepy/products/equity/equity_chooser_option.py
--rw-rw-rw-   0        0        0     7546 2022-06-10 19:56:04.000000 financepy-0.270/financepy/products/equity/equity_cliquet_option.py
--rw-rw-rw-   0        0        0    18066 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_compound_option.py
--rw-rw-rw-   0        0        0     7763 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_digital_option.py
--rw-rw-rw-   0        0        0    10384 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_fixed_lookback_option.py
--rw-rw-rw-   0        0        0     8866 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_float_lookback_option.py
--rw-rw-rw-   0        0        0     4868 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_forward.py
--rw-rw-rw-   0        0        0     1950 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/equity/equity_model_types.py
--rw-rw-rw-   0        0        0    19683 2021-12-25 18:48:58.000000 financepy-0.270/financepy/products/equity/equity_one_touch_option.py
--rw-rw-rw-   0        0        0     6735 2021-12-23 15:44:42.000000 financepy-0.270/financepy/products/equity/equity_option.py
--rw-rw-rw-   0        0        0    12100 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/equity/equity_rainbow_option.py
--rw-rw-rw-   0        0        0    24907 2023-02-13 16:33:55.000000 financepy-0.270/financepy/products/equity/equity_vanilla_option.py
--rw-rw-rw-   0        0        0    10614 2021-12-22 21:00:14.000000 financepy-0.270/financepy/products/equity/equity_variance_swap.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.370481 financepy-0.270/financepy/products/fx/
--rw-rw-rw-   0        0        0      375 2021-12-25 19:13:13.000000 financepy-0.270/financepy/products/fx/__init__.py
--rw-rw-rw-   0        0        0    17295 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_barrier_option.py
--rw-rw-rw-   0        0        0     6174 2021-12-21 13:58:02.000000 financepy-0.270/financepy/products/fx/fx_digital_option.py
--rw-rw-rw-   0        0        0     9113 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_fixed_lookback_option.py
--rw-rw-rw-   0        0        0     7583 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_float_lookback_option.py
--rw-rw-rw-   0        0        0     7198 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_forward.py
--rw-rw-rw-   0        0        0     4868 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/fx/fx_mkt_conventions.py
--rw-rw-rw-   0        0        0    19515 2021-12-23 15:49:15.000000 financepy-0.270/financepy/products/fx/fx_one_touch_option.py
--rw-rw-rw-   0        0        0     5292 2021-12-23 15:43:21.000000 financepy-0.270/financepy/products/fx/fx_option.py
--rw-rw-rw-   0        0        0    11013 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_rainbow_option.py
--rw-rw-rw-   0        0        0    28127 2022-06-10 10:47:18.000000 financepy-0.270/financepy/products/fx/fx_vanilla_option.py
--rw-rw-rw-   0        0        0    10072 2021-12-03 18:08:34.000000 financepy-0.270/financepy/products/fx/fx_variance_swap.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.376467 financepy-0.270/financepy/products/inflation/
--rw-rw-rw-   0        0        0     6647 2023-02-13 16:27:38.000000 financepy-0.270/financepy/products/inflation/FinInflationBond.py
--rw-rw-rw-   0        0        0     4361 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/inflation/FinInflationIndexCurve.py
--rw-rw-rw-   0        0        0     6672 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/inflation/FinInflationSwap.py
--rw-rw-rw-   0        0        0    21176 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/inflation/FinInflationSwapCurve.py
--rw-rw-rw-   0        0        0       33 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/inflation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.400402 financepy-0.270/financepy/products/rates/
--rw-rw-rw-   0        0        0      435 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/__init__.py
--rw-rw-rw-   0        0        0     9390 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/bermudan_swaption.py
--rw-rw-rw-   0        0        0    11427 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/callable_swap.py
--rw-rw-rw-   0        0        0    22970 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/dual_curve.py
--rw-rw-rw-   0        0        0     7979 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_basis_swap.py
--rw-rw-rw-   0        0        0    15095 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_cap_floor.py
--rw-rw-rw-   0        0        0     1246 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_conventions.py
--rw-rw-rw-   0        0        0     6722 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_deposit.py
--rw-rw-rw-   0        0        0     7139 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_fra.py
--rw-rw-rw-   0        0        0     5822 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_future.py
--rw-rw-rw-   0        0        0    17758 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/ibor_lmm_products.py
--rw-rw-rw-   0        0        0    27170 2022-08-31 19:10:11.000000 financepy-0.270/financepy/products/rates/ibor_single_curve.py
--rw-rw-rw-   0        0        0    11620 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/ibor_swap.py
--rw-rw-rw-   0        0        0    17602 2021-10-05 08:15:43.000000 financepy-0.270/financepy/products/rates/ibor_swaption.py
--rw-rw-rw-   0        0        0    10266 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/ois.py
--rw-rw-rw-   0        0        0     7437 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/ois_basis_swap.py
--rw-rw-rw-   0        0        0    24892 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/ois_curve.py
--rw-rw-rw-   0        0        0    11273 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/swap_fixed_leg.py
--rw-rw-rw-   0        0        0    12350 2021-11-06 12:48:44.000000 financepy-0.270/financepy/products/rates/swap_float_leg.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.426334 financepy-0.270/financepy/utils/
--rw-rw-rw-   0        0        0      371 2021-10-05 08:15:43.000000 financepy-0.270/financepy/utils/__init__.py
--rw-rw-rw-   0        0        0     1553 2021-10-05 08:15:43.000000 financepy-0.270/financepy/utils/amount.py
--rw-rw-rw-   0        0        0    33935 2022-03-20 08:54:30.000000 financepy-0.270/financepy/utils/calendar.py
--rw-rw-rw-   0        0        0      630 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/currency.py
--rw-rw-rw-   0        0        0    32484 2023-02-13 16:33:55.000000 financepy-0.270/financepy/utils/date.py
--rw-rw-rw-   0        0        0    10541 2022-10-02 12:44:23.000000 financepy-0.270/financepy/utils/day_count.py
--rw-rw-rw-   0        0        0      888 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/distribution.py
--rw-rw-rw-   0        0        0     1956 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/error.py
--rw-rw-rw-   0        0        0     1601 2022-10-02 12:44:23.000000 financepy-0.270/financepy/utils/frequency.py
--rw-rw-rw-   0        0        0     2497 2021-12-22 17:12:48.000000 financepy-0.270/financepy/utils/global_types.py
--rw-rw-rw-   0        0        0      447 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/global_vars.py
--rw-rw-rw-   0        0        0    15192 2022-11-22 10:17:15.000000 financepy-0.270/financepy/utils/helpers.py
--rw-rw-rw-   0        0        0     2927 2022-03-20 08:29:25.000000 financepy-0.270/financepy/utils/latex.py
--rw-rw-rw-   0        0        0    19248 2022-11-22 09:47:45.000000 financepy-0.270/financepy/utils/math.py
--rw-rw-rw-   0        0        0     2301 2022-12-28 10:41:39.000000 financepy-0.270/financepy/utils/polyfit.py
--rw-rw-rw-   0        0        0    11862 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/schedule.py
--rw-rw-rw-   0        0        0      498 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/singleton.py
--rw-rw-rw-   0        0        0    29377 2022-11-22 11:57:17.000000 financepy-0.270/financepy/utils/solver_1d.py
--rw-rw-rw-   0        0        0    21753 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/solver_cg.py
--rw-rw-rw-   0        0        0    13277 2021-11-06 12:48:44.000000 financepy-0.270/financepy/utils/solver_nm.py
--rw-rw-rw-   0        0        0     2754 2022-06-24 08:40:16.000000 financepy-0.270/financepy/utils/stats.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.212906 financepy-0.270/financepy.egg-info/
--rw-rw-rw-   0        0        0     7561 2023-02-13 16:38:27.000000 financepy-0.270/financepy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    10394 2023-02-13 16:38:27.000000 financepy-0.270/financepy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-13 16:38:27.000000 financepy-0.270/financepy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-02-13 16:38:27.000000 financepy-0.270/financepy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-02-13 16:38:27.000000 financepy-0.270/financepy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-13 16:38:27.569949 financepy-0.270/setup.cfg
--rw-rw-rw-   0        0        0     1996 2021-10-05 08:15:44.000000 financepy-0.270/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-13 16:38:27.566957 financepy-0.270/tests_golden/
--rw-rw-rw-   0        0        0    17690 2022-12-28 17:24:50.000000 financepy-0.270/tests_golden/FinTestCases.py
--rw-rw-rw-   0        0        0      890 2021-12-19 17:01:30.000000 financepy-0.270/tests_golden/TestFinAmount.py
--rw-rw-rw-   0        0        0    20479 2023-02-13 16:06:47.000000 financepy-0.270/tests_golden/TestFinBond.py
--rw-rw-rw-   0        0        0     7598 2022-03-20 13:10:36.000000 financepy-0.270/tests_golden/TestFinBondAnnuity.py
--rw-rw-rw-   0        0        0     4588 2022-06-24 08:59:58.000000 financepy-0.270/tests_golden/TestFinBondConvertible.py
--rw-rw-rw-   0        0        0     6956 2022-06-24 09:00:24.000000 financepy-0.270/tests_golden/TestFinBondEmbeddedOptionBK.py
--rw-rw-rw-   0        0        0     6942 2022-06-24 09:01:06.000000 financepy-0.270/tests_golden/TestFinBondEmbeddedOptionHW.py
--rw-rw-rw-   0        0        0    14054 2022-03-20 12:33:53.000000 financepy-0.270/tests_golden/TestFinBondFRN.py
--rw-rw-rw-   0        0        0     6176 2022-03-20 08:53:51.000000 financepy-0.270/tests_golden/TestFinBondFutures.py
--rw-rw-rw-   0        0        0     2041 2021-12-21 13:16:15.000000 financepy-0.270/tests_golden/TestFinBondMortgage.py
--rw-rw-rw-   0        0        0    15002 2022-06-24 09:01:30.000000 financepy-0.270/tests_golden/TestFinBondOptionBDTModel.py
--rw-rw-rw-   0        0        0    14962 2022-06-24 09:03:01.000000 financepy-0.270/tests_golden/TestFinBondOptionBKModel.py
--rw-rw-rw-   0        0        0    18901 2022-06-24 09:04:04.000000 financepy-0.270/tests_golden/TestFinBondOptionHWModel.py
--rw-rw-rw-   0        0        0     2152 2022-10-02 12:44:23.000000 financepy-0.270/tests_golden/TestFinBondPortfolio.py
--rw-rw-rw-   0        0        0     4514 2022-06-10 21:00:21.000000 financepy-0.270/tests_golden/TestFinBondYieldCurve.py
--rw-rw-rw-   0        0        0     2924 2022-11-22 09:47:45.000000 financepy-0.270/tests_golden/TestFinBondZeroCoupon.py
--rw-rw-rw-   0        0        0     2472 2022-08-11 21:00:13.000000 financepy-0.270/tests_golden/TestFinBondZeroCurve.py
--rw-rw-rw-   0        0        0    23600 2022-01-22 13:18:12.000000 financepy-0.270/tests_golden/TestFinCDS.py
--rw-rw-rw-   0        0        0    13736 2022-06-24 09:26:11.000000 financepy-0.270/tests_golden/TestFinCDSBasket.py
--rw-rw-rw-   0        0        0     5636 2022-08-31 20:01:33.000000 financepy-0.270/tests_golden/TestFinCDSCurve.py
--rw-rw-rw-   0        0        0     5374 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinCDSIndex.py
--rw-rw-rw-   0        0        0    11357 2022-06-24 09:05:07.000000 financepy-0.270/tests_golden/TestFinCDSIndexAdjustHazards.py
--rw-rw-rw-   0        0        0    10646 2022-06-24 09:05:28.000000 financepy-0.270/tests_golden/TestFinCDSIndexAdjustSpreads.py
--rw-rw-rw-   0        0        0     8588 2022-06-24 09:12:38.000000 financepy-0.270/tests_golden/TestFinCDSIndexOption.py
--rw-rw-rw-   0        0        0     8138 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinCDSIndexPortfolio.py
--rw-rw-rw-   0        0        0    10741 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinCDSOption.py
--rw-rw-rw-   0        0        0    10942 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinCDSTranche.py
--rw-rw-rw-   0        0        0     1720 2022-03-20 08:54:04.000000 financepy-0.270/tests_golden/TestFinCalendar.py
--rw-rw-rw-   0        0        0     8660 2022-02-14 09:19:14.000000 financepy-0.270/tests_golden/TestFinDate.py
--rw-rw-rw-   0        0        0     3513 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDateAdjust.py
--rw-rw-rw-   0        0        0     1335 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDayCount.py
--rw-rw-rw-   0        0        0     3504 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurve.py
--rw-rw-rw-   0        0        0     1857 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurveFlat.py
--rw-rw-rw-   0        0        0     7352 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurveNS.py
--rw-rw-rw-   0        0        0     4340 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurveNSS.py
--rw-rw-rw-   0        0        0     1499 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurvePolynomial.py
--rw-rw-rw-   0        0        0     2873 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurveZeros.py
--rw-rw-rw-   0        0        0     6743 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/TestFinDiscountCurves.py
--rw-rw-rw-   0        0        0    11033 2022-12-28 17:23:07.000000 financepy-0.270/tests_golden/TestFinEquityAmericanMC.py
--rw-rw-rw-   0        0        0     7143 2022-12-25 20:34:58.000000 financepy-0.270/tests_golden/TestFinEquityAmericanOption.py
--rw-rw-rw-   0        0        0    14048 2022-01-22 09:41:29.000000 financepy-0.270/tests_golden/TestFinEquityAsianOption.py
--rw-rw-rw-   0        0        0     5763 2022-06-24 09:08:05.000000 financepy-0.270/tests_golden/TestFinEquityBarrierOption.py
--rw-rw-rw-   0        0        0     7653 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinEquityBasketOption.py
--rw-rw-rw-   0        0        0     6414 2022-06-24 09:08:30.000000 financepy-0.270/tests_golden/TestFinEquityBinomialTree.py
--rw-rw-rw-   0        0        0     5534 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinEquityChooserOption.py
--rw-rw-rw-   0        0        0     1996 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinEquityCliquetOption.py
--rw-rw-rw-   0        0        0     5917 2022-06-24 09:08:45.000000 financepy-0.270/tests_golden/TestFinEquityCompoundOption.py
--rw-rw-rw-   0        0        0     5086 2022-06-24 09:16:47.000000 financepy-0.270/tests_golden/TestFinEquityDigitalOption.py
--rw-rw-rw-   0        0        0     2134 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinEquityForward.py
--rw-rw-rw-   0        0        0    16388 2022-01-22 09:40:51.000000 financepy-0.270/tests_golden/TestFinEquityLookbackOption.py
--rw-rw-rw-   0        0        0     6191 2022-01-22 09:44:19.000000 financepy-0.270/tests_golden/TestFinEquityOneTouchOption.py
--rw-rw-rw-   0        0        0    17897 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinEquityRainbowOption.py
--rw-rw-rw-   0        0        0    10841 2022-06-24 10:06:27.000000 financepy-0.270/tests_golden/TestFinEquityVanillaOption.py
--rw-rw-rw-   0        0        0     2341 2021-12-22 21:02:43.000000 financepy-0.270/tests_golden/TestFinEquityVarianceSwap.py
--rw-rw-rw-   0        0        0     4021 2021-12-22 21:03:03.000000 financepy-0.270/tests_golden/TestFinEquityVolSurface.py
--rw-rw-rw-   0        0        0     4803 2022-06-24 09:10:42.000000 financepy-0.270/tests_golden/TestFinFXAmericanOption.py
--rw-rw-rw-   0        0        0     6480 2022-06-24 09:10:55.000000 financepy-0.270/tests_golden/TestFinFXBarrierOption.py
--rw-rw-rw-   0        0        0     2644 2021-12-21 13:53:03.000000 financepy-0.270/tests_golden/TestFinFXDigitalOption.py
--rw-rw-rw-   0        0        0     3170 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinFXForward.py
--rw-rw-rw-   0        0        0    15254 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinFXLookbackOption.py
--rw-rw-rw-   0        0        0     6018 2021-12-25 19:11:30.000000 financepy-0.270/tests_golden/TestFinFXOneTouchOption.py
--rw-rw-rw-   0        0        0     5147 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinFXOptionSABR.py
--rw-rw-rw-   0        0        0    15960 2021-12-03 18:56:33.000000 financepy-0.270/tests_golden/TestFinFXVanillaOption.py
--rw-rw-rw-   0        0        0     9858 2021-12-22 21:05:30.000000 financepy-0.270/tests_golden/TestFinFXVolSurface.py
--rw-rw-rw-   0        0        0    18123 2021-12-22 19:19:05.000000 financepy-0.270/tests_golden/TestFinFXVolSurfacePlus.py
--rw-rw-rw-   0        0        0    28257 2021-12-22 19:15:39.000000 financepy-0.270/tests_golden/TestFinIborBermudanSwaption.py
--rw-rw-rw-   0        0        0    14266 2021-12-22 19:16:48.000000 financepy-0.270/tests_golden/TestFinIborCapFloor.py
--rw-rw-rw-   0        0        0     1921 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinIborCapVolCurve.py
--rw-rw-rw-   0        0        0    25121 2022-06-24 11:50:17.000000 financepy-0.270/tests_golden/TestFinIborDualCurve.py
--rw-rw-rw-   0        0        0     1044 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinIborFuture.py
--rw-rw-rw-   0        0        0     9516 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinIborLMMProducts.py
--rw-rw-rw-   0        0        0    27549 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinIborSingleCurve.py
--rw-rw-rw-   0        0        0    14159 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinIborSwap.py
--rw-rw-rw-   0        0        0    27393 2022-03-20 08:53:09.000000 financepy-0.270/tests_golden/TestFinIborSwaption.py
--rw-rw-rw-   0        0        0    14923 2022-03-20 08:57:37.000000 financepy-0.270/tests_golden/TestFinInflationBond.py
--rw-rw-rw-   0        0        0     1424 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinInflationIndexCurve.py
--rw-rw-rw-   0        0        0     2269 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinInterpolate.py
--rw-rw-rw-   0        0        0     2209 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinInterpolatedForwards.py
--rw-rw-rw-   0        0        0     4299 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinLossDbnBuilder.py
--rw-rw-rw-   0        0        0     2850 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinMath.py
--rw-rw-rw-   0        0        0     1910 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinMathAccruedInterp.py
--rw-rw-rw-   0        0        0     3679 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelBlack.py
--rw-rw-rw-   0        0        0     4958 2021-12-22 20:18:30.000000 financepy-0.270/tests_golden/TestFinModelBlackScholes.py
--rw-rw-rw-   0        0        0     2586 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelBlack_SABR_HW.py
--rw-rw-rw-   0        0        0     2455 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelCIR.py
--rw-rw-rw-   0        0        0     6657 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelHeston.py
--rw-rw-rw-   0        0        0     3595 2022-01-22 13:54:49.000000 financepy-0.270/tests_golden/TestFinModelMerton.py
--rw-rw-rw-   0        0        0    10334 2022-03-20 13:11:37.000000 financepy-0.270/tests_golden/TestFinModelRatesBDT.py
--rw-rw-rw-   0        0        0     5310 2022-03-20 13:06:22.000000 financepy-0.270/tests_golden/TestFinModelRatesBK.py
--rw-rw-rw-   0        0        0    11763 2022-03-20 13:11:16.000000 financepy-0.270/tests_golden/TestFinModelRatesHW.py
--rw-rw-rw-   0        0        0    17835 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelRatesLMM.py
--rw-rw-rw-   0        0        0     3182 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelSABR.py
--rw-rw-rw-   0        0        0     2689 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinModelShiftedSABR.py
--rw-rw-rw-   0        0        0    12233 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinNumbaNumpySpeed.py
--rw-rw-rw-   0        0        0     2302 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinOIS.py
--rw-rw-rw-   0        0        0    19529 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinOISCurve.py
--rw-rw-rw-   0        0        0     3818 2021-12-22 20:46:18.000000 financepy-0.270/tests_golden/TestFinOptionImpliedDbn.py
--rw-rw-rw-   0        0        0     1018 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinPieceCurve.py
--rw-rw-rw-   0        0        0     6178 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinProcessSimulator.py
--rw-rw-rw-   0        0        0    17672 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinSchedule.py
--rw-rw-rw-   0        0        0     1669 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinSobol.py
--rw-rw-rw-   0        0        0     2442 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinStatistics.py
--rw-rw-rw-   0        0        0     8851 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinSwapLegs.py
--rw-rw-rw-   0        0        0     4678 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinSwaptionVolSurface.py
--rw-rw-rw-   0        0        0     1341 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinVasicekRateModel.py
--rw-rw-rw-   0        0        0     1358 2021-12-03 18:08:34.000000 financepy-0.270/tests_golden/TestFinVolatilityCurve.py
--rw-rw-rw-   0        0        0       56 2021-10-05 08:15:44.000000 financepy-0.270/tests_golden/__init__.py
--rw-rw-rw-   0        0        0     2447 2022-09-26 07:54:06.000000 financepy-0.270/tests_golden/runAllTests.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:55.134478 financepy-0.290/
+-rw-rw-rw-   0        0        0    35823 2020-09-30 09:26:37.000000 financepy-0.290/LICENSE
+-rw-rw-rw-   0        0        0     7284 2023-05-10 16:52:55.132487 financepy-0.290/PKG-INFO
+-rw-rw-rw-   0        0        0     6687 2023-04-21 19:06:18.000000 financepy-0.290/README.md
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.211156 financepy-0.290/financepy/
+-rw-rw-rw-   0        0        0      453 2023-05-10 16:52:52.000000 financepy-0.290/financepy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.275505 financepy-0.290/financepy/market/
+-rw-rw-rw-   0        0        0        0 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.306422 financepy-0.290/financepy/market/curves/
+-rw-rw-rw-   0        0        0      308 2023-02-13 16:33:55.000000 financepy-0.290/financepy/market/curves/__init__.py
+-rw-rw-rw-   0        0        0    17339 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve.py
+-rw-rw-rw-   0        0        0     5170 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_flat.py
+-rw-rw-rw-   0        0        0     6789 2023-02-13 16:33:55.000000 financepy-0.290/financepy/market/curves/discount_curve_ns.py
+-rw-rw-rw-   0        0        0     7392 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_nss.py
+-rw-rw-rw-   0        0        0     6281 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_poly.py
+-rw-rw-rw-   0        0        0     5982 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_pwf.py
+-rw-rw-rw-   0        0        0     5825 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_pwl.py
+-rw-rw-rw-   0        0        0     5649 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/curves/discount_curve_zeros.py
+-rw-rw-rw-   0        0        0    12495 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/curves/interpolator.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.308417 financepy-0.290/financepy/market/prices/
+-rw-rw-rw-   0        0        0       25 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/prices/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.336355 financepy-0.290/financepy/market/volatility/
+-rw-rw-rw-   0        0        0      172 2021-12-22 21:07:08.000000 financepy-0.290/financepy/market/volatility/__init__.py
+-rw-rw-rw-   0        0        0     2747 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/volatility/equity_vol_curve.py
+-rw-rw-rw-   0        0        0    29961 2023-04-21 18:35:46.000000 financepy-0.290/financepy/market/volatility/equity_vol_surface.py
+-rw-rw-rw-   0        0        0    47487 2022-08-31 19:10:11.000000 financepy-0.290/financepy/market/volatility/fx_vol_surface.py
+-rw-rw-rw-   0        0        0    92029 2022-08-31 19:10:11.000000 financepy-0.290/financepy/market/volatility/fx_vol_surface_plus.py
+-rw-rw-rw-   0        0        0     7343 2021-11-06 12:48:44.000000 financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve.py
+-rw-rw-rw-   0        0        0     1497 2021-10-05 08:15:43.000000 financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve_fn.py
+-rw-rw-rw-   0        0        0    36053 2023-04-21 18:35:56.000000 financepy-0.290/financepy/market/volatility/swaption_vol_surface.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.464063 financepy-0.290/financepy/models/
+-rw-rw-rw-   0        0        0      837 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/__init__.py
+-rw-rw-rw-   0        0        0     2299 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/bachelier.py
+-rw-rw-rw-   0        0        0    30528 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/bdt_tree.py
+-rw-rw-rw-   0        0        0    39920 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/bk_tree.py
+-rw-rw-rw-   0        0        0    16639 2023-04-14 12:22:10.000000 financepy-0.290/financepy/models/black.py
+-rw-rw-rw-   0        0        0    10633 2023-05-10 16:37:54.000000 financepy-0.290/financepy/models/black_scholes.py
+-rw-rw-rw-   0        0        0    17933 2023-02-25 17:11:47.000000 financepy-0.290/financepy/models/black_scholes_analytic.py
+-rw-rw-rw-   0        0        0     6944 2021-12-22 21:43:40.000000 financepy-0.290/financepy/models/black_scholes_mc.py
+-rw-rw-rw-   0        0        0     3117 2021-12-22 21:35:15.000000 financepy-0.290/financepy/models/black_scholes_mc_tests.py
+-rw-rw-rw-   0        0        0     2888 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/black_shifted.py
+-rw-rw-rw-   0        0        0        0 2022-11-22 10:41:15.000000 financepy-0.290/financepy/models/bond_analytics.py
+-rw-rw-rw-   0        0        0    10102 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/cir_mc.py
+-rw-rw-rw-   0        0        0     8510 2023-03-12 16:15:39.000000 financepy-0.290/financepy/models/equity_barrier_models.py
+-rw-rw-rw-   0        0        0     7178 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/equity_crr_tree.py
+-rw-rw-rw-   0        0        0     5689 2023-05-10 16:33:55.000000 financepy-0.290/financepy/models/equity_lsmc.py
+-rw-rw-rw-   0        0        0     7955 2023-04-21 18:55:08.000000 financepy-0.290/financepy/models/finite_difference.py
+-rw-rw-rw-   0        0        0     4944 2023-04-14 12:22:10.000000 financepy-0.290/financepy/models/finite_difference_PSOR.py
+-rw-rw-rw-   0        0        0     1725 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/gauss_copula.py
+-rw-rw-rw-   0        0        0     6379 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gauss_copula_lhp.py
+-rw-rw-rw-   0        0        0     5638 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gauss_copula_lhplus.py
+-rw-rw-rw-   0        0        0    14108 2022-06-10 20:13:01.000000 financepy-0.290/financepy/models/gauss_copula_onefactor.py
+-rw-rw-rw-   0        0        0     7254 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/gbm_process_simulator.py
+-rw-rw-rw-   0        0        0    14264 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/heston.py
+-rw-rw-rw-   0        0        0    50919 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/hw_tree.py
+-rw-rw-rw-   0        0        0    33901 2021-12-22 21:46:06.000000 financepy-0.290/financepy/models/lmm_mc.py
+-rw-rw-rw-   0        0        0     4361 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/loss_dbn_builder.py
+-rw-rw-rw-   0        0        0     5484 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/merton_firm.py
+-rw-rw-rw-   0        0        0     6022 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/merton_firm_mkt.py
+-rw-rw-rw-   0        0        0      434 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/model.py
+-rw-rw-rw-   0        0        0     1985 2021-12-22 19:57:45.000000 financepy-0.290/financepy/models/option_implied_dbn.py
+-rw-rw-rw-   0        0        0    14570 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/process_simulator.py
+-rw-rw-rw-   0        0        0     3822 2021-11-06 12:48:44.000000 financepy-0.290/financepy/models/rates_ho_lee.py
+-rw-rw-rw-   0        0        0    10574 2023-04-14 13:09:24.000000 financepy-0.290/financepy/models/sabr.py
+-rw-rw-rw-   0        0        0     8306 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/sabr_shifted.py
+-rw-rw-rw-   0        0        0     5321 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/sobol.py
+-rw-rw-rw-   0        0        0   120492 2020-12-08 14:37:22.000000 financepy-0.290/financepy/models/sobolcoeff.npz
+-rw-rw-rw-   0        0        0     1800 2021-10-05 08:15:43.000000 financepy-0.290/financepy/models/student_t_copula.py
+-rw-rw-rw-   0        0        0     3303 2021-11-09 10:39:55.000000 financepy-0.290/financepy/models/vasicek_mc.py
+-rw-rw-rw-   0        0        0     8210 2022-06-10 20:10:22.000000 financepy-0.290/financepy/models/volatility_fns.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.469048 financepy-0.290/financepy/products/
+-rw-rw-rw-   0        0        0        0 2020-09-30 09:26:37.000000 financepy-0.290/financepy/products/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.525896 financepy-0.290/financepy/products/bonds/
+-rw-rw-rw-   0        0        0      367 2023-04-23 13:18:26.000000 financepy-0.290/financepy/products/bonds/__init__.py
+-rw-rw-rw-   0        0        0    40484 2023-04-23 13:34:35.000000 financepy-0.290/financepy/products/bonds/bond.py
+-rw-rw-rw-   0        0        0     7744 2022-03-20 13:06:59.000000 financepy-0.290/financepy/products/bonds/bond_annuity.py
+-rw-rw-rw-   0        0        0     9793 2022-03-20 13:01:16.000000 financepy-0.290/financepy/products/bonds/bond_callable.py
+-rw-rw-rw-   0        0        0    26813 2022-03-20 13:14:56.000000 financepy-0.290/financepy/products/bonds/bond_convertible.py
+-rw-rw-rw-   0        0        0    19575 2022-03-20 13:03:48.000000 financepy-0.290/financepy/products/bonds/bond_frn.py
+-rw-rw-rw-   0        0        0     6067 2022-03-20 13:02:32.000000 financepy-0.290/financepy/products/bonds/bond_future.py
+-rw-rw-rw-   0        0        0     5176 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/bond_market.py
+-rw-rw-rw-   0        0        0     6495 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/bonds/bond_mortgage.py
+-rw-rw-rw-   0        0        0     5841 2022-03-20 13:04:01.000000 financepy-0.290/financepy/products/bonds/bond_option.py
+-rw-rw-rw-   0        0        0    11494 2022-03-20 13:04:21.000000 financepy-0.290/financepy/products/bonds/bond_portfolio.py
+-rw-rw-rw-   0        0        0    28075 2023-02-24 13:55:17.000000 financepy-0.290/financepy/products/bonds/bond_zero.py
+-rw-rw-rw-   0        0        0     6784 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/yield_curve.py
+-rw-rw-rw-   0        0        0     5746 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/bonds/yield_curve_model.py
+-rw-rw-rw-   0        0        0     7056 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/bonds/zero_curve.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.555346 financepy-0.290/financepy/products/credit/
+-rw-rw-rw-   0        0        0      197 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/credit/__init__.py
+-rw-rw-rw-   0        0        0    34584 2022-08-31 17:54:32.000000 financepy-0.290/financepy/products/credit/cds.py
+-rw-rw-rw-   0        0        0    13492 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/credit/cds_basket.py
+-rw-rw-rw-   0        0        0     8958 2022-08-31 18:05:32.000000 financepy-0.290/financepy/products/credit/cds_curve.py
+-rw-rw-rw-   0        0        0    14463 2022-08-31 18:16:21.000000 financepy-0.290/financepy/products/credit/cds_index_option.py
+-rw-rw-rw-   0        0        0    19440 2022-08-31 18:13:43.000000 financepy-0.290/financepy/products/credit/cds_index_portfolio.py
+-rw-rw-rw-   0        0        0     6774 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/credit/cds_option.py
+-rw-rw-rw-   0        0        0     8960 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/credit/cds_tranche.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.620179 financepy-0.290/financepy/products/equity/
+-rw-rw-rw-   0        0        0      814 2023-03-12 15:30:43.000000 financepy-0.290/financepy/products/equity/__init__.py
+-rw-rw-rw-   0        0        0     4523 2022-12-24 15:09:21.000000 financepy-0.290/financepy/products/equity/equity_american_option.py
+-rw-rw-rw-   0        0        0    30586 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_asian_option.py
+-rw-rw-rw-   0        0        0    11033 2023-03-12 16:16:22.000000 financepy-0.290/financepy/products/equity/equity_barrier_option.py
+-rw-rw-rw-   0        0        0     9960 2023-04-21 18:57:50.000000 financepy-0.290/financepy/products/equity/equity_basket_option.py
+-rw-rw-rw-   0        0        0     8409 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/equity/equity_binomial_tree.py
+-rw-rw-rw-   0        0        0     9434 2022-06-10 19:55:23.000000 financepy-0.290/financepy/products/equity/equity_chooser_option.py
+-rw-rw-rw-   0        0        0     7546 2022-06-10 19:56:04.000000 financepy-0.290/financepy/products/equity/equity_cliquet_option.py
+-rw-rw-rw-   0        0        0    18066 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_compound_option.py
+-rw-rw-rw-   0        0        0     7763 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_digital_option.py
+-rw-rw-rw-   0        0        0    10384 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_fixed_lookback_option.py
+-rw-rw-rw-   0        0        0     8866 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_float_lookback_option.py
+-rw-rw-rw-   0        0        0     4868 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_forward.py
+-rw-rw-rw-   0        0        0     9939 2023-04-14 12:22:10.000000 financepy-0.290/financepy/products/equity/equity_index_option.py
+-rw-rw-rw-   0        0        0     1950 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/equity/equity_model_types.py
+-rw-rw-rw-   0        0        0    19683 2021-12-25 18:48:58.000000 financepy-0.290/financepy/products/equity/equity_one_touch_option.py
+-rw-rw-rw-   0        0        0     6735 2021-12-23 15:44:42.000000 financepy-0.290/financepy/products/equity/equity_option.py
+-rw-rw-rw-   0        0        0    12100 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/equity/equity_rainbow_option.py
+-rw-rw-rw-   0        0        0     8584 2023-04-21 18:30:04.000000 financepy-0.290/financepy/products/equity/equity_swap.py
+-rw-rw-rw-   0        0        0    14016 2023-04-21 18:38:13.000000 financepy-0.290/financepy/products/equity/equity_swap_leg.py
+-rw-rw-rw-   0        0        0    24907 2023-02-13 16:33:55.000000 financepy-0.290/financepy/products/equity/equity_vanilla_option.py
+-rw-rw-rw-   0        0        0    10614 2021-12-22 21:00:14.000000 financepy-0.290/financepy/products/equity/equity_variance_swap.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.660595 financepy-0.290/financepy/products/fx/
+-rw-rw-rw-   0        0        0      375 2021-12-25 19:13:13.000000 financepy-0.290/financepy/products/fx/__init__.py
+-rw-rw-rw-   0        0        0    17295 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_barrier_option.py
+-rw-rw-rw-   0        0        0     6174 2021-12-21 13:58:02.000000 financepy-0.290/financepy/products/fx/fx_digital_option.py
+-rw-rw-rw-   0        0        0     9113 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_fixed_lookback_option.py
+-rw-rw-rw-   0        0        0     7583 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_float_lookback_option.py
+-rw-rw-rw-   0        0        0     7198 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_forward.py
+-rw-rw-rw-   0        0        0     4868 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/fx/fx_mkt_conventions.py
+-rw-rw-rw-   0        0        0    19515 2021-12-23 15:49:15.000000 financepy-0.290/financepy/products/fx/fx_one_touch_option.py
+-rw-rw-rw-   0        0        0     5292 2021-12-23 15:43:21.000000 financepy-0.290/financepy/products/fx/fx_option.py
+-rw-rw-rw-   0        0        0    11013 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_rainbow_option.py
+-rw-rw-rw-   0        0        0    28014 2023-05-10 16:06:39.000000 financepy-0.290/financepy/products/fx/fx_vanilla_option.py
+-rw-rw-rw-   0        0        0    10072 2021-12-03 18:08:34.000000 financepy-0.290/financepy/products/fx/fx_variance_swap.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.673555 financepy-0.290/financepy/products/inflation/
+-rw-rw-rw-   0        0        0     6773 2023-02-24 13:55:17.000000 financepy-0.290/financepy/products/inflation/FinInflationBond.py
+-rw-rw-rw-   0        0        0     4361 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/FinInflationIndexCurve.py
+-rw-rw-rw-   0        0        0     6672 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/FinInflationSwap.py
+-rw-rw-rw-   0        0        0    21176 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/inflation/FinInflationSwapCurve.py
+-rw-rw-rw-   0        0        0       33 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/inflation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.722432 financepy-0.290/financepy/products/rates/
+-rw-rw-rw-   0        0        0      435 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/__init__.py
+-rw-rw-rw-   0        0        0     9390 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/bermudan_swaption.py
+-rw-rw-rw-   0        0        0    11427 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/callable_swap.py
+-rw-rw-rw-   0        0        0    22970 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/dual_curve.py
+-rw-rw-rw-   0        0        0     7979 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_basis_swap.py
+-rw-rw-rw-   0        0        0    15095 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_cap_floor.py
+-rw-rw-rw-   0        0        0     1246 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_conventions.py
+-rw-rw-rw-   0        0        0     6722 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_deposit.py
+-rw-rw-rw-   0        0        0     7139 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_fra.py
+-rw-rw-rw-   0        0        0     5822 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_future.py
+-rw-rw-rw-   0        0        0    17758 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ibor_lmm_products.py
+-rw-rw-rw-   0        0        0    27170 2022-08-31 19:10:11.000000 financepy-0.290/financepy/products/rates/ibor_single_curve.py
+-rw-rw-rw-   0        0        0    11620 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ibor_swap.py
+-rw-rw-rw-   0        0        0    17602 2021-10-05 08:15:43.000000 financepy-0.290/financepy/products/rates/ibor_swaption.py
+-rw-rw-rw-   0        0        0    10266 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois.py
+-rw-rw-rw-   0        0        0     7437 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois_basis_swap.py
+-rw-rw-rw-   0        0        0    24892 2021-11-06 12:48:44.000000 financepy-0.290/financepy/products/rates/ois_curve.py
+-rw-rw-rw-   0        0        0    11327 2023-04-14 12:22:10.000000 financepy-0.290/financepy/products/rates/swap_fixed_leg.py
+-rw-rw-rw-   0        0        0    12625 2023-03-12 15:30:43.000000 financepy-0.290/financepy/products/rates/swap_float_leg.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.779804 financepy-0.290/financepy/utils/
+-rw-rw-rw-   0        0        0      371 2021-10-05 08:15:43.000000 financepy-0.290/financepy/utils/__init__.py
+-rw-rw-rw-   0        0        0     1553 2021-10-05 08:15:43.000000 financepy-0.290/financepy/utils/amount.py
+-rw-rw-rw-   0        0        0    33935 2022-03-20 08:54:30.000000 financepy-0.290/financepy/utils/calendar.py
+-rw-rw-rw-   0        0        0      630 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/currency.py
+-rw-rw-rw-   0        0        0    32484 2023-02-13 16:33:55.000000 financepy-0.290/financepy/utils/date.py
+-rw-rw-rw-   0        0        0    10541 2022-10-02 12:44:23.000000 financepy-0.290/financepy/utils/day_count.py
+-rw-rw-rw-   0        0        0      888 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/distribution.py
+-rw-rw-rw-   0        0        0     1956 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/error.py
+-rw-rw-rw-   0        0        0     1601 2022-10-02 12:44:23.000000 financepy-0.290/financepy/utils/frequency.py
+-rw-rw-rw-   0        0        0     2972 2023-03-12 15:57:49.000000 financepy-0.290/financepy/utils/global_types.py
+-rw-rw-rw-   0        0        0      447 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/global_vars.py
+-rw-rw-rw-   0        0        0    15898 2023-03-12 15:30:43.000000 financepy-0.290/financepy/utils/helpers.py
+-rw-rw-rw-   0        0        0     2927 2022-03-20 08:29:25.000000 financepy-0.290/financepy/utils/latex.py
+-rw-rw-rw-   0        0        0    20984 2023-04-14 12:22:10.000000 financepy-0.290/financepy/utils/math.py
+-rw-rw-rw-   0        0        0     2301 2022-12-28 10:41:39.000000 financepy-0.290/financepy/utils/polyfit.py
+-rw-rw-rw-   0        0        0    11970 2023-05-04 07:59:23.000000 financepy-0.290/financepy/utils/schedule.py
+-rw-rw-rw-   0        0        0      498 2021-11-06 12:48:44.000000 financepy-0.290/financepy/utils/singleton.py
+-rw-rw-rw-   0        0        0    29377 2022-11-22 11:57:17.000000 financepy-0.290/financepy/utils/solver_1d.py
+-rw-rw-rw-   0        0        0    21755 2023-04-21 18:36:04.000000 financepy-0.290/financepy/utils/solver_cg.py
+-rw-rw-rw-   0        0        0    13278 2023-04-21 18:38:22.000000 financepy-0.290/financepy/utils/solver_nm.py
+-rw-rw-rw-   0        0        0     2754 2022-06-24 08:40:16.000000 financepy-0.290/financepy/utils/stats.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:54.272513 financepy-0.290/financepy.egg-info/
+-rw-rw-rw-   0        0        0     7284 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    10686 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-10 16:52:53.000000 financepy-0.290/financepy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-10 16:52:55.135478 financepy-0.290/setup.cfg
+-rw-rw-rw-   0        0        0     1996 2021-10-05 08:15:44.000000 financepy-0.290/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-10 16:52:55.127485 financepy-0.290/tests_golden/
+-rw-rw-rw-   0        0        0    17690 2022-12-28 17:24:50.000000 financepy-0.290/tests_golden/FinTestCases.py
+-rw-rw-rw-   0        0        0      890 2023-03-13 18:31:42.000000 financepy-0.290/tests_golden/TestFinAmount.py
+-rw-rw-rw-   0        0        0    22862 2023-05-10 16:07:46.000000 financepy-0.290/tests_golden/TestFinBond.py
+-rw-rw-rw-   0        0        0     7598 2022-03-20 13:10:36.000000 financepy-0.290/tests_golden/TestFinBondAnnuity.py
+-rw-rw-rw-   0        0        0     4588 2022-06-24 08:59:58.000000 financepy-0.290/tests_golden/TestFinBondConvertible.py
+-rw-rw-rw-   0        0        0     6956 2022-06-24 09:00:24.000000 financepy-0.290/tests_golden/TestFinBondEmbeddedOptionBK.py
+-rw-rw-rw-   0        0        0     6942 2022-06-24 09:01:06.000000 financepy-0.290/tests_golden/TestFinBondEmbeddedOptionHW.py
+-rw-rw-rw-   0        0        0    14054 2022-03-20 12:33:53.000000 financepy-0.290/tests_golden/TestFinBondFRN.py
+-rw-rw-rw-   0        0        0     6176 2022-03-20 08:53:51.000000 financepy-0.290/tests_golden/TestFinBondFutures.py
+-rw-rw-rw-   0        0        0     2041 2021-12-21 13:16:15.000000 financepy-0.290/tests_golden/TestFinBondMortgage.py
+-rw-rw-rw-   0        0        0    15002 2022-06-24 09:01:30.000000 financepy-0.290/tests_golden/TestFinBondOptionBDTModel.py
+-rw-rw-rw-   0        0        0    14962 2022-06-24 09:03:01.000000 financepy-0.290/tests_golden/TestFinBondOptionBKModel.py
+-rw-rw-rw-   0        0        0    18901 2022-06-24 09:04:04.000000 financepy-0.290/tests_golden/TestFinBondOptionHWModel.py
+-rw-rw-rw-   0        0        0     2152 2022-10-02 12:44:23.000000 financepy-0.290/tests_golden/TestFinBondPortfolio.py
+-rw-rw-rw-   0        0        0     4514 2022-06-10 21:00:21.000000 financepy-0.290/tests_golden/TestFinBondYieldCurve.py
+-rw-rw-rw-   0        0        0     2924 2022-11-22 09:47:45.000000 financepy-0.290/tests_golden/TestFinBondZeroCoupon.py
+-rw-rw-rw-   0        0        0     2472 2022-08-11 21:00:13.000000 financepy-0.290/tests_golden/TestFinBondZeroCurve.py
+-rw-rw-rw-   0        0        0    23600 2022-01-22 13:18:12.000000 financepy-0.290/tests_golden/TestFinCDS.py
+-rw-rw-rw-   0        0        0    13736 2022-06-24 09:26:11.000000 financepy-0.290/tests_golden/TestFinCDSBasket.py
+-rw-rw-rw-   0        0        0     5636 2022-08-31 20:01:33.000000 financepy-0.290/tests_golden/TestFinCDSCurve.py
+-rw-rw-rw-   0        0        0     5374 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSIndex.py
+-rw-rw-rw-   0        0        0    11357 2022-06-24 09:05:07.000000 financepy-0.290/tests_golden/TestFinCDSIndexAdjustHazards.py
+-rw-rw-rw-   0        0        0    10646 2022-06-24 09:05:28.000000 financepy-0.290/tests_golden/TestFinCDSIndexAdjustSpreads.py
+-rw-rw-rw-   0        0        0     8588 2022-06-24 09:12:38.000000 financepy-0.290/tests_golden/TestFinCDSIndexOption.py
+-rw-rw-rw-   0        0        0     8138 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSIndexPortfolio.py
+-rw-rw-rw-   0        0        0    10741 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSOption.py
+-rw-rw-rw-   0        0        0    10942 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinCDSTranche.py
+-rw-rw-rw-   0        0        0     1720 2022-03-20 08:54:04.000000 financepy-0.290/tests_golden/TestFinCalendar.py
+-rw-rw-rw-   0        0        0     8660 2022-02-14 09:19:14.000000 financepy-0.290/tests_golden/TestFinDate.py
+-rw-rw-rw-   0        0        0     3513 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDateAdjust.py
+-rw-rw-rw-   0        0        0     1335 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDayCount.py
+-rw-rw-rw-   0        0        0     3504 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurve.py
+-rw-rw-rw-   0        0        0     1857 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveFlat.py
+-rw-rw-rw-   0        0        0     7352 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveNS.py
+-rw-rw-rw-   0        0        0     4340 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveNSS.py
+-rw-rw-rw-   0        0        0     1499 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurvePolynomial.py
+-rw-rw-rw-   0        0        0     2873 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurveZeros.py
+-rw-rw-rw-   0        0        0     6743 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/TestFinDiscountCurves.py
+-rw-rw-rw-   0        0        0    11033 2022-12-28 17:23:07.000000 financepy-0.290/tests_golden/TestFinEquityAmericanMC.py
+-rw-rw-rw-   0        0        0     7143 2022-12-25 20:34:58.000000 financepy-0.290/tests_golden/TestFinEquityAmericanOption.py
+-rw-rw-rw-   0        0        0    14048 2022-01-22 09:41:29.000000 financepy-0.290/tests_golden/TestFinEquityAsianOption.py
+-rw-rw-rw-   0        0        0     6546 2023-03-12 16:16:54.000000 financepy-0.290/tests_golden/TestFinEquityBarrierOption.py
+-rw-rw-rw-   0        0        0     7653 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityBasketOption.py
+-rw-rw-rw-   0        0        0     6414 2022-06-24 09:08:30.000000 financepy-0.290/tests_golden/TestFinEquityBinomialTree.py
+-rw-rw-rw-   0        0        0     5534 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityChooserOption.py
+-rw-rw-rw-   0        0        0     1996 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityCliquetOption.py
+-rw-rw-rw-   0        0        0     5917 2022-06-24 09:08:45.000000 financepy-0.290/tests_golden/TestFinEquityCompoundOption.py
+-rw-rw-rw-   0        0        0     5086 2022-06-24 09:16:47.000000 financepy-0.290/tests_golden/TestFinEquityDigitalOption.py
+-rw-rw-rw-   0        0        0     2134 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityForward.py
+-rw-rw-rw-   0        0        0    16388 2022-01-22 09:40:51.000000 financepy-0.290/tests_golden/TestFinEquityLookbackOption.py
+-rw-rw-rw-   0        0        0     6191 2022-01-22 09:44:19.000000 financepy-0.290/tests_golden/TestFinEquityOneTouchOption.py
+-rw-rw-rw-   0        0        0    17897 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinEquityRainbowOption.py
+-rw-rw-rw-   0        0        0     7872 2023-04-14 13:24:43.000000 financepy-0.290/tests_golden/TestFinEquitySwap.py
+-rw-rw-rw-   0        0        0    10841 2023-03-13 18:31:42.000000 financepy-0.290/tests_golden/TestFinEquityVanillaOption.py
+-rw-rw-rw-   0        0        0     2341 2021-12-22 21:02:43.000000 financepy-0.290/tests_golden/TestFinEquityVarianceSwap.py
+-rw-rw-rw-   0        0        0     4021 2021-12-22 21:03:03.000000 financepy-0.290/tests_golden/TestFinEquityVolSurface.py
+-rw-rw-rw-   0        0        0     4803 2022-06-24 09:10:42.000000 financepy-0.290/tests_golden/TestFinFXAmericanOption.py
+-rw-rw-rw-   0        0        0     6480 2022-06-24 09:10:55.000000 financepy-0.290/tests_golden/TestFinFXBarrierOption.py
+-rw-rw-rw-   0        0        0     2644 2021-12-21 13:53:03.000000 financepy-0.290/tests_golden/TestFinFXDigitalOption.py
+-rw-rw-rw-   0        0        0     3170 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXForward.py
+-rw-rw-rw-   0        0        0    15254 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXLookbackOption.py
+-rw-rw-rw-   0        0        0     6018 2021-12-25 19:11:30.000000 financepy-0.290/tests_golden/TestFinFXOneTouchOption.py
+-rw-rw-rw-   0        0        0     5147 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinFXOptionSABR.py
+-rw-rw-rw-   0        0        0    17551 2023-05-10 16:04:00.000000 financepy-0.290/tests_golden/TestFinFXVanillaOption.py
+-rw-rw-rw-   0        0        0     9858 2021-12-22 21:05:30.000000 financepy-0.290/tests_golden/TestFinFXVolSurface.py
+-rw-rw-rw-   0        0        0    18123 2021-12-22 19:19:05.000000 financepy-0.290/tests_golden/TestFinFXVolSurfacePlus.py
+-rw-rw-rw-   0        0        0    28257 2021-12-22 19:15:39.000000 financepy-0.290/tests_golden/TestFinIborBermudanSwaption.py
+-rw-rw-rw-   0        0        0    14266 2021-12-22 19:16:48.000000 financepy-0.290/tests_golden/TestFinIborCapFloor.py
+-rw-rw-rw-   0        0        0     1921 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborCapVolCurve.py
+-rw-rw-rw-   0        0        0    25121 2022-06-24 11:50:45.000000 financepy-0.290/tests_golden/TestFinIborDualCurve.py
+-rw-rw-rw-   0        0        0     1044 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborFuture.py
+-rw-rw-rw-   0        0        0     9516 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborLMMProducts.py
+-rw-rw-rw-   0        0        0    27549 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborSingleCurve.py
+-rw-rw-rw-   0        0        0    14159 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinIborSwap.py
+-rw-rw-rw-   0        0        0    27393 2022-03-20 08:53:09.000000 financepy-0.290/tests_golden/TestFinIborSwaption.py
+-rw-rw-rw-   0        0        0    14923 2022-03-20 08:57:37.000000 financepy-0.290/tests_golden/TestFinInflationBond.py
+-rw-rw-rw-   0        0        0     1424 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInflationIndexCurve.py
+-rw-rw-rw-   0        0        0     2269 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInterpolate.py
+-rw-rw-rw-   0        0        0     2209 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinInterpolatedForwards.py
+-rw-rw-rw-   0        0        0     4299 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinLossDbnBuilder.py
+-rw-rw-rw-   0        0        0     2850 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinMath.py
+-rw-rw-rw-   0        0        0     1910 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinMathAccruedInterp.py
+-rw-rw-rw-   0        0        0     3679 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelBlack.py
+-rw-rw-rw-   0        0        0     4958 2021-12-22 20:18:30.000000 financepy-0.290/tests_golden/TestFinModelBlackScholes.py
+-rw-rw-rw-   0        0        0     2586 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelBlack_SABR_HW.py
+-rw-rw-rw-   0        0        0     2455 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelCIR.py
+-rw-rw-rw-   0        0        0     6657 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelHeston.py
+-rw-rw-rw-   0        0        0     3595 2022-01-22 13:54:49.000000 financepy-0.290/tests_golden/TestFinModelMerton.py
+-rw-rw-rw-   0        0        0    10334 2022-03-20 13:11:37.000000 financepy-0.290/tests_golden/TestFinModelRatesBDT.py
+-rw-rw-rw-   0        0        0     5310 2022-03-20 13:06:22.000000 financepy-0.290/tests_golden/TestFinModelRatesBK.py
+-rw-rw-rw-   0        0        0    11763 2022-03-20 13:11:16.000000 financepy-0.290/tests_golden/TestFinModelRatesHW.py
+-rw-rw-rw-   0        0        0    17835 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelRatesLMM.py
+-rw-rw-rw-   0        0        0     3182 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelSABR.py
+-rw-rw-rw-   0        0        0     2689 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinModelShiftedSABR.py
+-rw-rw-rw-   0        0        0    12233 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinNumbaNumpySpeed.py
+-rw-rw-rw-   0        0        0     2302 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinOIS.py
+-rw-rw-rw-   0        0        0    19529 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinOISCurve.py
+-rw-rw-rw-   0        0        0     3818 2021-12-22 20:46:18.000000 financepy-0.290/tests_golden/TestFinOptionImpliedDbn.py
+-rw-rw-rw-   0        0        0     1018 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinPieceCurve.py
+-rw-rw-rw-   0        0        0     6178 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinProcessSimulator.py
+-rw-rw-rw-   0        0        0    18118 2023-05-03 16:37:45.000000 financepy-0.290/tests_golden/TestFinSchedule.py
+-rw-rw-rw-   0        0        0     1669 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSobol.py
+-rw-rw-rw-   0        0        0     2442 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinStatistics.py
+-rw-rw-rw-   0        0        0     8851 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSwapLegs.py
+-rw-rw-rw-   0        0        0     4678 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinSwaptionVolSurface.py
+-rw-rw-rw-   0        0        0     1341 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinVasicekRateModel.py
+-rw-rw-rw-   0        0        0     1358 2021-12-03 18:08:34.000000 financepy-0.290/tests_golden/TestFinVolatilityCurve.py
+-rw-rw-rw-   0        0        0       56 2021-10-05 08:15:44.000000 financepy-0.290/tests_golden/__init__.py
+-rw-rw-rw-   0        0        0     2443 2023-03-13 10:28:21.000000 financepy-0.290/tests_golden/runAllTests.py
```

### Comparing `financepy-0.270/LICENSE` & `financepy-0.290/LICENSE`

 * *Files identical despite different names*

### Comparing `financepy-0.270/PKG-INFO` & `financepy-0.290/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: financepy
-Version: 0.270
+Version: 0.290
 Summary: A Finance Securities Valuation Library
 Home-page: https://github.com/domokane/FinancePy
 Author: Dominic O'Kane
 Author-email: dominic.okane@edhec.edu
-License: UNKNOWN
 Keywords: FINANCE,OPTIONS,BONDS,VALUATION,DERIVATIVES
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![unit test action](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml/badge.svg)](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml)
-
-![alt text](./images/logo.jpg?raw=true)
-
 # Latest News and Versions
 
 22 Nov 22
 Version 0.260 has been released and pushed to PyPI
 - Create Date from python datetime
 - Zero coupon bond class
 - Fixed bug in bond payment date
@@ -31,15 +25,15 @@
 31-Aug-2022
 Version 0.240 has just been released and pushed to PyPI with changes
 - Negative terms in date class
 - Recovery rates do not default to standard value for CDS curves 
 
 # DISCLAIMER
 
-This software is distributed FREE & WITHOUT ANY WARRANTY. 
+This software is distributed FREE AND WITHOUT ANY WARRANTY. 
 
 Report any bugs or suggestions here as an issue. 
 
 # CONTRIBUTORS WANTED !
 
 If you have a knowledge of Quantitative Finance and a reasonable knowledge of Python, then please consider contributing to this project. There are small tasks and big tasks to be done. Just look in the list of Issues and you may find something you can do. Before you begin, please comment in the issue thread in case someone else may be working on that issue. Or you can contact me directly at dominic.okane at edhec.edu. 
 
@@ -139,9 +133,7 @@
 * Comments are required for every class and function and they should be a clear description.
 * At least one broad test case and a set of unit tests must be provided for every function.
 * Avoid very pythonic constructions. For example a loop is as good as a list comprehension. And with numba it can be faster. Readability is the priority.
 
 ## License
 
  GPL-3.0 License - See the license file in this folder for details.
-
-
```

### Comparing `financepy-0.270/README.md` & `financepy-0.290/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-[![unit test action](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml/badge.svg)](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml)
-
-![alt text](./images/logo.jpg?raw=true)
-
 # Latest News and Versions
 
 22 Nov 22
 Version 0.260 has been released and pushed to PyPI
 - Create Date from python datetime
 - Zero coupon bond class
 - Fixed bug in bond payment date
@@ -13,15 +9,15 @@
 31-Aug-2022
 Version 0.240 has just been released and pushed to PyPI with changes
 - Negative terms in date class
 - Recovery rates do not default to standard value for CDS curves 
 
 # DISCLAIMER
 
-This software is distributed FREE & WITHOUT ANY WARRANTY. 
+This software is distributed FREE AND WITHOUT ANY WARRANTY. 
 
 Report any bugs or suggestions here as an issue. 
 
 # CONTRIBUTORS WANTED !
 
 If you have a knowledge of Quantitative Finance and a reasonable knowledge of Python, then please consider contributing to this project. There are small tasks and big tasks to be done. Just look in the list of Issues and you may find something you can do. Before you begin, please comment in the issue thread in case someone else may be working on that issue. Or you can contact me directly at dominic.okane at edhec.edu.
```

### Comparing `financepy-0.270/financepy/market/curves/discount_curve.py` & `financepy-0.290/financepy/market/curves/discount_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_flat.py` & `financepy-0.290/financepy/market/curves/discount_curve_flat.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_ns.py` & `financepy-0.290/financepy/market/curves/discount_curve_ns.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_nss.py` & `financepy-0.290/financepy/market/curves/discount_curve_nss.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_poly.py` & `financepy-0.290/financepy/market/curves/discount_curve_poly.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_pwf.py` & `financepy-0.290/financepy/market/curves/discount_curve_pwf.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_pwl.py` & `financepy-0.290/financepy/market/curves/discount_curve_pwl.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/discount_curve_zeros.py` & `financepy-0.290/financepy/market/curves/discount_curve_zeros.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/curves/interpolator.py` & `financepy-0.290/financepy/market/curves/interpolator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/equity_vol_curve.py` & `financepy-0.290/financepy/market/volatility/equity_vol_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/equity_vol_surface.py` & `financepy-0.290/financepy/market/volatility/equity_vol_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     # Determine parameters of vol surface using minimisation
     ###########################################################################
 
     tol = 1e-6
 
     args = (s, t, r, q, strikes, timeIndex, volatility_grid, vol_type_value)
 
-    # Nelder-Mead (both SciPy & Numba) is quicker, but occasionally fails
+    # Nelder-Mead (both SciPy and Numba) is quicker, but occasionally fails
     # to converge, so for those cases try again with CG
     # Numba version is quicker, but can be slightly away from CG output
     try:
         if finSolverType == FinSolverTypes.NELDER_MEAD_NUMBA:
             xopt = nelder_mead(_obj, np.array(x_inits),
                                bounds=np.array([[], []]).T,
                                args=args, tol_f=tol,
```

### Comparing `financepy-0.270/financepy/market/volatility/fx_vol_surface.py` & `financepy-0.290/financepy/market/volatility/fx_vol_surface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/fx_vol_surface_plus.py` & `financepy-0.290/financepy/market/volatility/fx_vol_surface_plus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/ibor_cap_vol_curve.py` & `financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/ibor_cap_vol_curve_fn.py` & `financepy-0.290/financepy/market/volatility/ibor_cap_vol_curve_fn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/market/volatility/swaption_vol_surface.py` & `financepy-0.290/financepy/market/volatility/swaption_vol_surface.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     # Determine parameters of vol surface using minimisation
     ###########################################################################
 
     tol = 1e-6
 
     args = (t, f, strikesGrid, timeIndex, volatility_grid, vol_type_value)
 
-    # Nelder-Mead (both SciPy & Numba) is quicker, but occasionally fails
+    # Nelder-Mead (both SciPy amd Numba) is quicker, but occasionally fails
     # to converge, so for those cases try again with CG
     # Numba version is quicker, but can be slightly away from CG output
     try:
         if finSolverType == FinSolverTypes.NELDER_MEAD_NUMBA:
             xopt = nelder_mead(_obj, np.array(x_inits),
                                bounds=np.array([[], []]).T,
                                args=args, tol_f=tol,
```

### Comparing `financepy-0.270/financepy/models/__init__.py` & `financepy-0.290/financepy/models/__init__.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/bachelier.py` & `financepy-0.290/financepy/models/bachelier.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/bdt_tree.py` & `financepy-0.290/financepy/models/bdt_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/bk_tree.py` & `financepy-0.290/financepy/models/bk_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/black_scholes_analytic.py` & `financepy-0.290/financepy/models/black_scholes_analytic.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,17 +182,16 @@
     d1 = np.log(ss/kk) / vsqrtT + vsqrtT / 2.0
     d2 = d1 - vsqrtT
     vanna = np.exp(-q*t) * sqrtT * n_prime_vect(d1) * (d2/v)
     return vanna
 
 ###############################################################################
 
-@njit(fastmath=True, cache=True)
-
 
+@njit(fastmath=True, cache=True)
 def _f(sigma, args):
 
     s = args[0]
     t = args[1]
     k = args[2]
     r = args[3]
     q = args[4]
@@ -201,14 +200,15 @@
 
     bsPrice = bs_value(s, t, k, r, q, sigma, option_type_value)
     obj = bsPrice - price
     return obj
 
 ##############################################################################
 
+
 @njit(fastmath=True, cache=True)
 def _fvega(sigma, args):
 
     s = args[0]
     t = args[1]
     k = args[2]
     r = args[3]
@@ -219,15 +219,15 @@
 
 ###############################################################################
 
 
 @vectorize([float64(float64, float64, float64, float64,
                     float64, int64)], fastmath=True, cache=True)
 def bs_intrinsic(s, t, k, r, q, option_type_value):
-    """ Calculate the Black-Scholes implied volatility of a European 
+    """ Calculate the Black-Scholes implied volatility of a European
     vanilla option using Newton with a fallback to bisection. """
 
     fwd = s * np.exp((r-q)*t)
 
     if option_type_value == OptionTypes.EUROPEAN_CALL.value:
         intrinsic_value = np.exp(-r*t) * max(fwd - k, 0.0)
     else:
@@ -237,15 +237,15 @@
 
 ###############################################################################
 
 
 # @vectorize([float64(float64, float64, float64, float64, float64, float64,
 #                    int64)], fastmath=True, cache=True,  forceobj=True)
 def bs_implied_volatility(s, t, k, r, q, price, option_type_value):
-    """ Calculate the Black-Scholes implied volatility of a European 
+    """ Calculate the Black-Scholes implied volatility of a European
     vanilla option using Newton with a fallback to bisection. """
 
     fwd = s * np.exp((r-q)*t)
 
     if option_type_value == OptionTypes.EUROPEAN_CALL.value:
         intrinsic_value = np.exp(-r*t) * max(fwd - k, 0.0)
     else:
@@ -438,15 +438,15 @@
         W = 2.0 * b / (v*v)
         K = 1.0 - np.exp(-r * t)
         d1 = (np.log(sstar/k) + (b + v*v / 2.0) * t) / (v * np.sqrt(t))
         q2 = (-1.0 * (W - 1.0) + np.sqrt((W - 1.0)**2 + 4.0 * M/K)) / 2.0
         A2 = (sstar / q2) * (1.0 - np.exp(-q * t) * n_vect(d1))
 
         if s < sstar:
-            return bs_value(s, t, k, r, q, v, +1) + A2 * ((s/sstar)**q2)
+            return bs_value(s, t, k, r, q, v, OptionTypes.EUROPEAN_CALL.value) + A2 * ((s/sstar)**q2)
         else:
             return s - k
 
     elif phi == -1:
 
         argtuple = (t, k, r, q, v)
 
@@ -462,25 +462,71 @@
         W = 2.0 * b / v2
         K = 1.0 - np.exp(-r * t)
         d1 = (np.log(sstar / k) + (b + v2 / 2.0) * t) / (v * np.sqrt(t))
         q1 = (-1.0 * (W - 1.0) - np.sqrt((W - 1.0)**2 + 4.0 * M/K)) / 2.0
         a1 = -(sstar / q1) * (1 - np.exp(-q * t) * n_vect(-d1))
 
         if s > sstar:
-            return bs_value(s, t, k, r, q, v, -1) + a1 * ((s/sstar)**q1)
+            return bs_value(s, t, k, r, q, v, OptionTypes.EUROPEAN_PUT.value) + a1 * ((s/sstar)**q1)
         else:
             return k - s
 
     else:
 
         raise FinError("Phi must equal 1 or -1.")
 
 ###############################################################################
 
 
+@njit(fastmath=True)
+def bjerksund_stensland_value(s, t, k, r, q, v, option_type_value):
+    """ Price American Option using the Bjerksund-Stensland
+    approximation (1993) for the Black Scholes Model """
+    if option_type_value == OptionTypes.AMERICAN_CALL.value:
+        pass
+    elif option_type_value == OptionTypes.AMERICAN_PUT.value:
+        # put-call transformation
+        s, k, r, q = k, s, r-q, -q
+    else:
+        return 0.0
+
+    def phi(S, T, gamma, H, X):
+        """ The function corresponding to Eq.(13)
+        in Bjerksund-Stensland approximation (1993)"""
+        nonlocal r, q
+        lambda0 = (-r + gamma * q + 0.5 * gamma * (gamma - 1.0) * v**2) * T
+        d = - (np.log(S/H) + (q + (gamma - 0.5) * v**2) * T) / (v * np.sqrt(t))
+        kappa = (2.0 * gamma - 1.0) + (2.0 * q) / v**2
+        return (
+            np.exp(lambda0) * (S ** gamma)
+            * (N(d) - N(d - (2.0 * np.log(X/S)/v/np.sqrt(T))) * ((X/S)**kappa))
+        )
+    # calc trigger price x_t
+    beta = (0.5 - q/(v**2)) + np.sqrt((0.5 - q/(v**2))**2 + 2.0 * r/(v**2))
+    # avoid division by zero
+    if abs(r-q) < 1.e-10:
+        beta = 1.0
+        x_t = 1.e10
+    else:
+        b_infty = k * beta / (beta - 1.0)
+        b_0 = max(k, k * r/((r-q)))
+        h_t = -(q*t + 2.0 * v * np.sqrt(t)) * (b_0 / (b_infty - b_0))
+        x_t = b_0 + (b_infty - b_0) * (1.0 - np.exp(h_t))
+    # calc option value
+    alpha = (x_t - k) * x_t ** (-beta)
+    value = (
+        alpha * (s**beta) - alpha * phi(s, t, beta, x_t, x_t)
+        + phi(s, t, 1.0, x_t, x_t) - phi(s, t, 1.0, k, x_t)
+        - k * phi(s, t, 0.0, x_t, x_t) + k * phi(s, t, 0.0, k, x_t)
+    )
+    return value
+
+###############################################################################
+
+
 if __name__ == '__main__':
     # spot_price, strike_price, time_to_expiry, r, b, vol, phi
 
     # Checking against table 3-1 in Haug
     k = 100.0
     r = 0.10
     q = 0.10
```

### Comparing `financepy-0.270/financepy/models/black_scholes_mc.py` & `financepy-0.290/financepy/models/black_scholes_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/black_scholes_mc_tests.py` & `financepy-0.290/financepy/models/black_scholes_mc_tests.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/black_shifted.py` & `financepy-0.290/financepy/models/black_shifted.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/cir_mc.py` & `financepy-0.290/financepy/models/cir_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/equity_crr_tree.py` & `financepy-0.290/financepy/models/equity_crr_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/gauss_copula.py` & `financepy-0.290/financepy/models/gauss_copula.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/gauss_copula_lhp.py` & `financepy-0.290/financepy/models/gauss_copula_lhp.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/gauss_copula_lhplus.py` & `financepy-0.290/financepy/models/gauss_copula_lhplus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/gauss_copula_onefactor.py` & `financepy-0.290/financepy/models/gauss_copula_onefactor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/gbm_process_simulator.py` & `financepy-0.290/financepy/models/gbm_process_simulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/heston.py` & `financepy-0.290/financepy/models/heston.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/hw_tree.py` & `financepy-0.290/financepy/models/hw_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/lmm_mc.py` & `financepy-0.290/financepy/models/lmm_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/loss_dbn_builder.py` & `financepy-0.290/financepy/models/loss_dbn_builder.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/merton_firm.py` & `financepy-0.290/financepy/models/merton_firm.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/merton_firm_mkt.py` & `financepy-0.290/financepy/models/merton_firm_mkt.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/option_implied_dbn.py` & `financepy-0.290/financepy/models/option_implied_dbn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/process_simulator.py` & `financepy-0.290/financepy/models/process_simulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/rates_ho_lee.py` & `financepy-0.290/financepy/models/rates_ho_lee.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/sabr.py` & `financepy-0.290/financepy/models/sabr.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 @njit
 def _x(rho, z):
     """ Return function x used in Hagan's 2002 SABR lognormal vol expansion."""
     a = (1.0 - 2.0*rho*z + z**2)**.5 + z - rho
     b = 1.0 - rho
     return np.log(a / b)
 
+##############################################################################
 
 @njit(float64(float64[:], float64, float64, float64),
       fastmath=True, cache=True)
 def vol_function_sabr(params, f, k, t):
     """ Black volatility implied by SABR model. """
 
     alpha = params[0]
```

### Comparing `financepy-0.270/financepy/models/sabr_shifted.py` & `financepy-0.290/financepy/models/sabr_shifted.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/sobol.py` & `financepy-0.290/financepy/models/sobol.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/sobolcoeff.npz` & `financepy-0.290/financepy/models/sobolcoeff.npz`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/student_t_copula.py` & `financepy-0.290/financepy/models/student_t_copula.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/vasicek_mc.py` & `financepy-0.290/financepy/models/vasicek_mc.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/models/volatility_fns.py` & `financepy-0.290/financepy/models/volatility_fns.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond.py` & `financepy-0.290/financepy/products/bonds/bond.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,14 +33,16 @@
 from ...utils.calendar import Calendar
 from ...utils.calendar import CalendarTypes
 from ...utils.calendar import BusDayAdjustTypes
 from ...utils.calendar import DateGenRuleTypes
 from ...utils.helpers import label_to_string, check_argument_types
 from ...utils.math import npv
 from ...market.curves.discount_curve import DiscountCurve
+from ...market.curves.interpolator import InterpTypes
+from .zero_curve import BondZeroCurve
 
 
 # References https://www.dmo.gov.uk/media/15011/yldeqns_v1.pdf
 # DO TRUE YIELD
 # JAPANESE SIMPLE YIELD
 
 ###############################################################################
@@ -94,15 +96,17 @@
     def __init__(self,
                  issue_date: Date,
                  maturity_date: Date,
                  coupon: float,  # Annualised bond coupon
                  freq_type: FrequencyTypes,
                  accrual_type: DayCountTypes,
                  face_amount: float = 100.0,
-                 calendar_type: CalendarTypes = CalendarTypes.WEEKEND):
+                 calendar_type: CalendarTypes = CalendarTypes.WEEKEND,
+                 bus_day_rule_type = BusDayAdjustTypes.FOLLOWING,
+                 date_gen_rule_type = DateGenRuleTypes.BACKWARD):
         """ Create Bond object by providing the issue date, maturity Date,
         coupon frequency, annualised coupon, the accrual convention type, face
         amount and the number of ex-dividend days. A calendar type is used 
         to determine holidays from which coupon dates might be shifted."""
 
         check_argument_types(self.__init__, locals())
 
@@ -136,35 +140,38 @@
         self._payment_dates = []  # Actual payment dates are adjusted
         self._flow_amounts = []
 
         self._accrued_interest = None
         self._accrued_days = 0.0
         self._alpha = 0.0
 
+        self.bus_day_rule_type = bus_day_rule_type
+        self.date_gen_rule_type = date_gen_rule_type
+
         self._calculate_coupon_dates()
         self._calculate_flows()
 
     ###########################################################################
 
     def _calculate_coupon_dates(self):
         """ Determine the bond coupon dates. Note that for analytical 
         calculations these are not usually adjusted and so may fall on a 
         weekend or holiday. 
         """
 
         # This should only be called once from init
-        bus_day_rule_type = BusDayAdjustTypes.FOLLOWING
-        date_gen_rule_type = DateGenRuleTypes.BACKWARD
+        #bus_day_rule_type = BusDayAdjustTypes.FOLLOWING
+        #date_gen_rule_type = DateGenRuleTypes.BACKWARD
 
         self._coupon_dates = Schedule(self._issue_date,
                                     self._maturity_date,
                                     self._freq_type,
                                     CalendarTypes.NONE,
-                                    bus_day_rule_type,
-                                    date_gen_rule_type, 
+                                    self.bus_day_rule_type,
+                                    self.date_gen_rule_type, 
                                     end_of_month = self._end_of_month)._generate()
 
     ###########################################################################
 
     def _calculate_payment_dates(self):
         """ For the actual payment dates, they are adjusted 
         and so we then use the calendar payment dates. Although payments are 
@@ -337,24 +344,159 @@
 
     ###########################################################################
 
     def modified_duration(self,
                           settlement_date: Date,
                           ytm: float,
                           convention: YTMCalcType = YTMCalcType.UK_DMO):
-        """ Calculate the modified duration of the bondon a settlement date
+        """ Calculate the modified duration of the bond on a settlement date
         given its yield to maturity. """
 
         dd = self.dollar_duration(settlement_date, ytm, convention)
         fp = self.full_price_from_ytm(settlement_date, ytm, convention)
         md = dd / fp
         return md
 
     ###########################################################################
 
+    def key_rate_durations(bond,
+                           settlement_date: Date,
+                           ytm: float,
+                           key_rate_tenors: list = None,
+                           shift: float = None,
+                           rates: list = None):
+
+        """
+        Calculates the key rate durations for a bond.
+
+        Parameters
+        ----------
+        bond : FinancePy Bond object
+            
+        settlement_date : FinancePy Date object
+            The settlement date.
+        ytm : float
+            The yield to maturity.
+        key_rate_tenors : list of float, optional
+            The tenors of the key rates, default is None which will generate
+            the tenors from 0.25 to 30 years.
+        shift : float, optional
+            The shift used to calculate the key rate durations, default is None
+            which will set the shift to 0.0001.
+        rates: list of float, optional
+            Corresponding yield curve data in line with key_rate_tenors
+            If None, flat yield curve is used
+
+        Returns
+        -------
+        tuple of (numpy array of float, numpy array of float)
+            A tuple containing the key rate tenors and the key rate durations.
+        """
+
+        # check if key_rate_tenors is None
+        if key_rate_tenors is None:
+        # if it is None, create an array of key rates ranging from 0.5 to 30 years
+            key_rate_tenors = np.array([0.5,  1,  2,  3,  5,  7,  10, 20, 30])
+
+        # set the shift to a small value if not give
+        if not shift:
+            shift = 0.0001
+
+        # initialize an empty list for the key rate durations
+        key_rate_durations = []
+
+        # iterate over each key rate (tenor) and calculate the key rate duration
+        for ind, _ in enumerate(key_rate_tenors):
+            # if rates not given
+            # create an array of rates where each rate is equal to the ytm value
+            if rates is None:
+                rates = np.ones(len(key_rate_tenors)) * ytm
+
+            #Create set of par bonds to be used in BondZeroCurve
+            # ytm and coupons are equal
+            par_bonds = []
+            for tenor, cpn in zip(key_rate_tenors, rates):
+
+                mat_date = settlement_date.add_years(tenor)
+
+                par_bond = Bond(settlement_date, mat_date, cpn,
+                                bond._freq_type, bond._accrual_type)
+
+                par_bonds.append(par_bond)
+
+            clean_prices = [par_bond.clean_price_from_ytm(
+                settlement_date, ytm, YTMCalcType.US_STREET) for par_bond, ytm in zip(par_bonds, rates)]
+
+            par_crv = BondZeroCurve(settlement_date, par_bonds,
+                                    clean_prices, InterpTypes.LINEAR_ZERO_RATES)
+
+            # calculate the full price of the bond using the discount curve
+            p_zero = bond.full_price_from_discount_curve(settlement_date, par_crv)
+
+
+            # shift up by the yield of corresponding par bond
+            rates[ind] += shift
+
+            par_bonds = []
+            for tenor, cpn in zip(key_rate_tenors, rates):
+
+                mat = settlement_date.add_years(tenor)
+
+                par_bond = Bond(settlement_date, mat, cpn,
+                                bond._freq_type, bond._accrual_type)
+
+                par_bonds.append(par_bond)
+
+            clean_prices = [par_bond.clean_price_from_ytm(
+                settlement_date, ytm, YTMCalcType.US_STREET) for par_bond, ytm in zip(par_bonds, rates)]
+
+            par_crv_up = BondZeroCurve(
+                settlement_date, par_bonds, clean_prices, InterpTypes.LINEAR_ZERO_RATES)
+
+            # calculate the full price of the bond
+            # using the discount curve with the key rate shifted up
+            p_up = bond.full_price_from_discount_curve(settlement_date, par_crv_up)
+
+            # create a curve again with the key rate shifted down
+            # by twice the shift value.
+            rates[ind] -= shift * 2
+
+            par_bonds = []
+            for tenor, cpn in zip(key_rate_tenors, rates):
+
+                mat = settlement_date.add_years(tenor)
+
+                par_bond = Bond(settlement_date, mat, cpn,
+                                bond._freq_type, bond._accrual_type)
+
+                par_bonds.append(par_bond)
+
+            clean_prices = [par_bond.clean_price_from_ytm(settlement_date, 
+                                                          ytm, 
+                                                          YTMCalcType.US_STREET) for par_bond, ytm in zip(par_bonds, rates)]
+
+            par_crv_down = BondZeroCurve(settlement_date, 
+                                         par_bonds, 
+                                         clean_prices, 
+                                         InterpTypes.LINEAR_ZERO_RATES)
+
+            # calculate the full price of the bond using
+            p_down = bond.full_price_from_discount_curve(settlement_date, par_crv_down)
+
+            # calculate the key rate duration
+            # using the formula (P_down - P_up) / (2 * shift * P_zero)
+            key_rate_duration = (p_down - p_up) / (2 * shift * p_zero)
+
+            # append the key rate duration to the key_rate_durations list
+            key_rate_durations.append(key_rate_duration)
+            
+        return key_rate_tenors, np.array(key_rate_durations)
+
+    ###########################################################################
+
     def convexity_from_ytm(self,
                            settlement_date: Date,
                            ytm: float,
                            convention: YTMCalcType = YTMCalcType.UK_DMO):
         """ Calculate the bond convexity from the yield to maturity. This
         function is vectorised with respect to the yield input. """
 
@@ -414,16 +556,16 @@
 
         px = 0.0
         df = 1.0
         dfSettle = discount_curve.df(settlement_date)
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on the settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on a settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 flow = self._coupon / self._frequency
                 pv = flow * df
                 px += pv
 
         px += df * self._redemption
         px = px / dfSettle
@@ -496,16 +638,16 @@
 
         num_flows = len(self._coupon_dates)
 
         if num_flows == 0:
             raise FinError("Accrued interest - not enough flow dates.")
 
         for iFlow in range(1, num_flows):
-            # coupons paid on a settlement date are paid
-            if self._coupon_dates[iFlow] >= settlement_date:
+            # coupons paid on a settlement date are paid to the seller
+            if self._coupon_dates[iFlow] > settlement_date:
                 self._pcd = self._coupon_dates[iFlow - 1]
                 self._ncd = self._coupon_dates[iFlow]
                 break
 
         dc = DayCount(self._accrual_type)
         cal = Calendar(calendar_type)
         exDividend_date = cal.add_business_days(
@@ -546,16 +688,16 @@
         bondPrice = clean_price + accrued_amount
         # Calculate the price of the bond discounted on the Ibor curve
         pvIbor = 0.0
         prev_date = self._pcd
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on a settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 pvIbor += df * self._coupon / self._frequency
 
         pvIbor += df * self._redemption
 
         # Calculate the PV01 of the floating leg of the asset swap
         # I assume here that the coupon starts accruing on the settlement date
@@ -592,23 +734,25 @@
         self.calc_accrued_interest(settlement_date)
         f = self._frequency
         c = self._coupon
 
         pv = 0.0
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on a settlement date are paid to the seller
+            if dt > settlement_date:
                 t = (dt - settlement_date) / gDaysInYear
 
                 t = np.maximum(t, gSmall)
 
                 df = discount_curve.df(dt)
+
                 # determine the Ibor implied zero rate
                 r = f * (np.power(df, -1.0 / t / f) - 1.0)
+
                 # determine the OAS adjusted zero rate
                 df_adjusted = np.power(1.0 + (r + oas) / f, -t * f)
                 pv = pv + (c / f) * df_adjusted
 
         pv = pv + df_adjusted * self._redemption
         pv *= self._par
         return pv
@@ -663,20 +807,20 @@
         analytic calculations for the bond. """
 
         flow = self._face_amount * self._coupon / self._frequency
 
         flow_str = ""
 
         for dt in self._coupon_dates[1:-1]:
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
-                flow_str += ("%12s %12.2f \n" % (dt, flow))
+            # coupons paid on a settlement date are paid to the seller
+            if dt > settlement_date:
+                flow_str += ("%12s %12.5f \n" % (dt, flow))
 
         redemption_amount = self._face_amount + flow
-        flow_str += ("%12s %12.2f \n"
+        flow_str += ("%12s %12.5f \n"
                      % (self._coupon_dates[-1], redemption_amount))
 
         return flow_str
 
     ###########################################################################
 
     def print_coupon_dates(self,
@@ -709,16 +853,16 @@
         prevDf = 1.0
 
         defaultingPrincipalPVPayStart = 0.0
         defaultingPrincipalPVPayEnd = 0.0
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on a settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 q = survival_curve.survival_prob(dt)
 
                 # Add PV of coupon conditional on surviving to payment date
                 # Any default results in all subsequent coupons being lost
                 # with zero recovery
```

### Comparing `financepy-0.270/financepy/products/bonds/bond_annuity.py` & `financepy-0.290/financepy/products/bonds/bond_annuity.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_callable.py` & `financepy-0.290/financepy/products/bonds/bond_callable.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_convertible.py` & `financepy-0.290/financepy/products/bonds/bond_convertible.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_frn.py` & `financepy-0.290/financepy/products/bonds/bond_frn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_future.py` & `financepy-0.290/financepy/products/bonds/bond_future.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_market.py` & `financepy-0.290/financepy/products/bonds/bond_market.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_mortgage.py` & `financepy-0.290/financepy/products/bonds/bond_mortgage.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_option.py` & `financepy-0.290/financepy/products/bonds/bond_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_portfolio.py` & `financepy-0.290/financepy/products/bonds/bond_portfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/bond_zero.py` & `financepy-0.290/financepy/products/bonds/bond_zero.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,16 +254,16 @@
 
         px = 0.0
         df = 1.0
         dfSettle = discount_curve.df(settlement_date, )
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on the settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on the settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 flow = 0
                 pv = flow * df
                 px += pv
 
         px += df * self._redemption
         px = px / dfSettle
@@ -344,16 +344,16 @@
 
         num_flows = len(self._coupon_dates)
 
         if num_flows == 0:
             raise FinError("Accrued interest - not enough flow dates.")
 
         for iFlow in range(1, num_flows):
-            # coupons paid on a settlement date are paid
-            if self._coupon_dates[iFlow] >= settlement_date:
+            # coupons paid on the settlement date are paid to the seller
+            if self._coupon_dates[iFlow] > settlement_date:
                 self._pcd = self._coupon_dates[iFlow - 1]
                 self._ncd = self._coupon_dates[iFlow]
                 break
 
         dc = DayCount(self._accrual_type)
         cal = Calendar(calendar_type)
         exDividend_date = cal.add_business_days(
@@ -397,16 +397,16 @@
         bondPrice = clean_price + accrued_amount
         # Calculate the price of the bond discounted on the Ibor curve
         pvIbor = 0.0
         prev_date = self._pcd
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on the settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 # pvIbor += df * self._coupon / self._frequency
 
         pvIbor += df * self._redemption
 
         # Calculate the PV01 of the floating leg of the asset swap
         # I assume here that the coupon starts accruing on the settlement date
@@ -441,16 +441,16 @@
         settlement date, a discount curve and the oas as a number. """
 
         self.calc_accrued_interest(settlement_date)
 
         pv = 0.0
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on the settlement date are paid to the seller
+            if dt > settlement_date:
                 t = (dt - settlement_date) / gDaysInYear
 
                 t = np.maximum(t, gSmall)
 
                 df = discount_curve.df(dt)
                 # determine the Ibor implied zero rate
                 r = np.power(df, -1.0 / t) - 1.0
@@ -544,16 +544,16 @@
         prevDf = 1.0
 
         defaultingPrincipalPVPayStart = 0.0
         defaultingPrincipalPVPayEnd = 0.0
 
         for dt in self._coupon_dates[1:]:
 
-            # coupons paid on a settlement date are included
-            if dt >= settlement_date:
+            # coupons paid on the settlement date are paid to the seller
+            if dt > settlement_date:
                 df = discount_curve.df(dt)
                 q = survival_curve.survival_prob(dt)
 
                 # Add PV of coupon conditional on surviving to payment date
                 # Any default results in all subsequent coupons being lost
                 # with zero recovery
```

### Comparing `financepy-0.270/financepy/products/bonds/yield_curve.py` & `financepy-0.290/financepy/products/bonds/yield_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/yield_curve_model.py` & `financepy-0.290/financepy/products/bonds/yield_curve_model.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/bonds/zero_curve.py` & `financepy-0.290/financepy/products/bonds/zero_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds.py` & `financepy-0.290/financepy/products/credit/cds.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_basket.py` & `financepy-0.290/financepy/products/credit/cds_basket.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_curve.py` & `financepy-0.290/financepy/products/credit/cds_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_index_option.py` & `financepy-0.290/financepy/products/credit/cds_index_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_index_portfolio.py` & `financepy-0.290/financepy/products/credit/cds_index_portfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_option.py` & `financepy-0.290/financepy/products/credit/cds_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/credit/cds_tranche.py` & `financepy-0.290/financepy/products/credit/cds_tranche.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/__init__.py` & `financepy-0.290/financepy/products/equity/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,9 +12,11 @@
 from .equity_model_types import *
 from .equity_option import *
 from .equity_rainbow_option import *
 from .equity_vanilla_option import *
 from .equity_variance_swap import *
 from .equity_one_touch_option import *
 from .equity_forward import *
+from .equity_swap_leg import *
+from .equity_swap import *
 
 # dividend_curve = FinDiscountCurveFlat(valuation_date, dividend_yield)
```

### Comparing `financepy-0.270/financepy/products/equity/equity_american_option.py` & `financepy-0.290/financepy/products/equity/equity_american_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_asian_option.py` & `financepy-0.290/financepy/products/equity/equity_asian_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_barrier_option.py` & `financepy-0.290/financepy/products/fx/fx_barrier_option.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,447 +1,402 @@
-###############################################################################
+##############################################################################
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
-###############################################################################
+##############################################################################
 
+from math import exp, log, sqrt
 import numpy as np
 from enum import Enum
 
 from ...utils.error import FinError
+from ...utils.math import N
 from ...utils.global_vars import gDaysInYear
-from ...products.equity.equity_option import EquityOption
+from ...products.fx.fx_option import FXOption
 from ...models.process_simulator import FinProcessSimulator
-from ...market.curves.discount_curve import DiscountCurve
 from ...utils.helpers import label_to_string, check_argument_types
 from ...utils.date import Date
 
 
-from ...utils.math import N
-
-# TODO: SOME REDESIGN ON THE MONTE CARLO PROCESS IS PROBABLY NEEDED
-
 ###############################################################################
 
 
-class EquityBarrierTypes(Enum):
+class FinFXBarrierTypes(Enum):
     DOWN_AND_OUT_CALL = 1
     DOWN_AND_IN_CALL = 2
     UP_AND_OUT_CALL = 3
     UP_AND_IN_CALL = 4
     UP_AND_OUT_PUT = 5
     UP_AND_IN_PUT = 6
     DOWN_AND_OUT_PUT = 7
     DOWN_AND_IN_PUT = 8
 
+
 ###############################################################################
 
 
-class EquityBarrierOption(EquityOption):
-    """ Class to hold details of an Equity Barrier Option. It also
-    calculates the option price using Black Scholes for 8 different
-    variants on the Barrier structure in enum EquityBarrierTypes. """
+class FXBarrierOption(FXOption):
 
     def __init__(self,
                  expiry_date: Date,
-                 strike_price: float,
-                 option_type: EquityBarrierTypes,
+                 strike_fx_rate: float,  # 1 unit of foreign in domestic
+                 currency_pair: str,  # FORDOM
+                 option_type: FinFXBarrierTypes,
                  barrier_level: float,
-                 num_observations_per_year: (int, float) = 252,
-                 notional: float = 1.0):
-        """ Create the EquityBarrierOption by specifying the expiry date,
-        strike price, option type, barrier level, the number of observations
-        per year and the notional. """
+                 num_observations_per_year: int,
+                 notional: float,
+                 notional_currency: str):
+        """ Create FX Barrier option product. This is an option that cancels if
+        the FX rate crosses a barrier during the life of the option. """
 
         check_argument_types(self.__init__, locals())
 
         self._expiry_date = expiry_date
-        self._strike_price = float(strike_price)
+        self._strike_fx_rate = float(strike_fx_rate)
+        self._currency_pair = currency_pair
         self._barrier_level = float(barrier_level)
         self._num_observations_per_year = int(num_observations_per_year)
-
-        if option_type not in EquityBarrierTypes:
-            raise FinError("Option Type " + str(option_type) + " unknown.")
-
         self._option_type = option_type
         self._notional = notional
+        self._notional_currency = notional_currency
 
-###############################################################################
+    ##########################################################################
 
     def value(self,
-              valuation_date: Date,
-              stock_price: (float, np.ndarray),
-              discount_curve: DiscountCurve,
-              dividend_curve: DiscountCurve,
+              valuation_date,
+              spot_fx_rate,
+              dom_discount_curve,
+              for_discount_curve,
               model):
-        """ This prices an Equity Barrier option using the formulae given in
-        the paper by Clewlow, Llanos and Strickland December 1994 which can be
-        found at
+        """ Value FX Barrier Option using Black-Scholes model with closed-form
+        analytical models. """
 
-        https://warwick.ac.uk/fac/soc/wbs/subjects/finance/research/wpaperseries/1994/94-54.pdf
-        """
+        # This prices the option using the formulae given in the paper
+        # by Clewlow, Llanos and Strickland December 1994 which can be found at
+        # https://warwick.ac.uk/fac/soc/wbs/subjects/finance/research/wpaperseries/1994/94-54.pdf
 
         if isinstance(valuation_date, Date) == False:
             raise FinError("Valuation date is not a Date")
 
         if valuation_date > self._expiry_date:
             raise FinError("Valuation date after expiry date.")
 
-        if discount_curve._valuation_date != valuation_date:
+        if dom_discount_curve._valuation_date != valuation_date:
             raise FinError(
-                "Discount Curve valuation date not same as option valuation date")
+                "Domestic Curve valuation date not same as option valuation date")
 
-        if dividend_curve._valuation_date != valuation_date:
+        if for_discount_curve._valuation_date != valuation_date:
             raise FinError(
-                "Dividend Curve valuation date not same as option valuation date")
-
-        if isinstance(stock_price, int):
-            stock_price = float(stock_price)
-
-        if isinstance(stock_price, float):
-            stock_prices = [stock_price]
-        else:
-            stock_prices = stock_price
-
-        values = []
-        for s in stock_prices:
-            v = self._value_one(valuation_date, s, discount_curve,
-                                dividend_curve, model)
-            values.append(v)
-
-        if isinstance(stock_price, float):
-            return values[0]
-        else:
-            return np.array(values)
-
-###############################################################################
-
-    def _value_one(self,
-                   valuation_date: Date,
-                   stock_price: (float, np.ndarray),
-                   discount_curve: DiscountCurve,
-                   dividend_curve: DiscountCurve,
-                   model):
-        """ This values a single option. Because of its structure it cannot
-        easily be vectorised which is why it has been wrapped. """
-
-        texp = (self._expiry_date - valuation_date) / gDaysInYear
-
-        if texp < 0:
-            raise FinError("Option expires before value date.")
-
-        texp = max(texp, 1e-6)
+                "Foreign Curve valuation date not same as option valuation date")
 
-        lnS0k = np.log(stock_price / self._strike_price)
-        sqrtT = np.sqrt(texp)
-
-        r = discount_curve.cc_rate(self._expiry_date)
-        q = dividend_curve.cc_rate(self._expiry_date)
-
-        k = self._strike_price
-        s = stock_price
+        K = self._strike_fx_rate
+        S0 = spot_fx_rate
         h = self._barrier_level
 
+        t = (self._expiry_date - valuation_date) / gDaysInYear
+        lnS0k = log(float(S0) / K)
+        sqrtT = sqrt(t)
+
+        dq = for_discount_curve._df(t)
+        df = dom_discount_curve._df(t)
+        rd = -log(df) / t
+        rf = -log(dq) / t
+
         volatility = model._volatility
         sigmaRootT = volatility * sqrtT
         v2 = volatility * volatility
-        mu = r - q
-        d1 = (lnS0k + (mu + v2 / 2.0) * texp) / sigmaRootT
-        d2 = (lnS0k + (mu - v2 / 2.0) * texp) / sigmaRootT
-        df = np.exp(-r * texp)
-        dq = np.exp(-q * texp)
-
-        c = s * dq * N(d1) - k * df * N(d2)
-        p = k * df * N(-d2) - s * dq * N(-d1)
-#        print("CALL:",c,"PUT:",p)
+        mu = rd - rf
+        d1 = (lnS0k + (mu + v2 / 2.0) * t) / sigmaRootT
+        d2 = (lnS0k + (mu - v2 / 2.0) * t) / sigmaRootT
+
+        c = S0 * dq * N(d1) - K * df * N(d2)
+        p = K * df * N(-d2) - S0 * dq * N(-d1)
+        #        print("CALL:",c,"PUT:",p)
 
-        if self._option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL and s <= h:
+        if self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL and S0 <= h:
             return 0.0
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_CALL and s >= h:
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_CALL and S0 >= h:
             return 0.0
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_PUT and s >= h:
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_PUT and S0 >= h:
             return 0.0
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT and s <= h:
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT and S0 <= h:
             return 0.0
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_CALL and s <= h:
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL and S0 <= h:
             return c
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_CALL and s >= h:
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_CALL and S0 >= h:
             return c
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_PUT and s >= h:
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_PUT and S0 >= h:
             return p
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_PUT and s <= h:
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT and S0 <= h:
             return p
 
-        num_observations = 1 + texp * self._num_observations_per_year
+        num_observations = t * self._num_observations_per_year
 
         # Correction by Broadie, Glasserman and Kou, Mathematical Finance, 1997
         # Adjusts the barrier for discrete and not continuous observations
         h_adj = h
-        t = texp / num_observations
-
-        if self._option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL:
-            h_adj = h * np.exp(-0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_CALL:
-            h_adj = h * np.exp(-0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_CALL:
-            h_adj = h * np.exp(0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_CALL:
-            h_adj = h * np.exp(0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_PUT:
-            h_adj = h * np.exp(0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_PUT:
-            h_adj = h * np.exp(0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT:
-            h_adj = h * np.exp(-0.5826 * volatility * np.sqrt(t))
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_PUT:
-            h_adj = h * np.exp(-0.5826 * volatility * np.sqrt(t))
+        if self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL:
+            h_adj = h * exp(-0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL:
+            h_adj = h * exp(-0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_CALL:
+            h_adj = h * exp(0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_CALL:
+            h_adj = h * exp(0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_PUT:
+            h_adj = h * exp(0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_PUT:
+            h_adj = h * exp(0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT:
+            h_adj = h * exp(-0.5826 * volatility * sqrt(t / num_observations))
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT:
+            h_adj = h * exp(-0.5826 * volatility * sqrt(t / num_observations))
         else:
             raise FinError("Unknown barrier option type." +
                            str(self._option_type))
 
         h = h_adj
 
         if abs(volatility) < 1e-5:
             volatility = 1e-5
 
-        l = (mu + v2 / 2.0) / v2
-        y = np.log(h * h / (s * k)) / sigmaRootT + l * sigmaRootT
-        x1 = np.log(s / h) / sigmaRootT + l * sigmaRootT
-        y1 = np.log(h / s) / sigmaRootT + l * sigmaRootT
-        hOverS = h / s
-
-        if self._option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL:
-            if h >= k:
-                c_do = s * dq * N(x1) - k * df * N(x1 - sigmaRootT) \
-                    - s * dq * pow(hOverS, 2.0 * l) * N(y1) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * N(y1 - sigmaRootT)
+        ll = (mu + v2 / 2.0) / v2
+        y = log(h * h / (S0 * K)) / sigmaRootT + ll * sigmaRootT
+        x1 = log(S0 / h) / sigmaRootT + ll * sigmaRootT
+        y1 = log(h / S0) / sigmaRootT + ll * sigmaRootT
+        hOverS = h / S0
+
+        if self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL:
+            if h >= K:
+                c_do = S0 * dq * N(x1) - K * df * N(x1 - sigmaRootT) \
+                    - S0 * dq * pow(hOverS, 2.0 * ll) * N(y1) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * N(y1 - sigmaRootT)
                 price = c_do
             else:
-                c_di = s * dq * pow(hOverS, 2.0 * l) * N(y) \
-                    - k * df * pow(hOverS, 2.0 * l - 2.0) * N(y - sigmaRootT)
+                c_di = S0 * dq * pow(hOverS, 2.0 * ll) * N(y) \
+                    - K * df * pow(hOverS, 2.0 * ll - 2.0) * N(y - sigmaRootT)
                 price = c - c_di
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_CALL:
-            if h <= k:
-                c_di = s * dq * pow(hOverS, 2.0 * l) * N(y) \
-                    - k * df * pow(hOverS, 2.0 * l - 2.0) * N(y - sigmaRootT)
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL:
+            if h <= K:
+                c_di = S0 * dq * pow(hOverS, 2.0 * ll) * N(y) \
+                    - K * df * pow(hOverS, 2.0 * ll - 2.0) * N(y - sigmaRootT)
                 price = c_di
             else:
-                c_do = s * dq * N(x1) \
-                    - k * df * N(x1 - sigmaRootT) \
-                    - s * dq * pow(hOverS, 2.0 * l) * N(y1) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * N(y1 - sigmaRootT)
+                c_do = S0 * dq * N(x1) \
+                    - K * df * N(x1 - sigmaRootT) \
+                    - S0 * dq * pow(hOverS, 2.0 * ll) * N(y1) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * N(y1 - sigmaRootT)
                 price = c - c_do
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_CALL:
-            if h >= k:
-                c_ui = s * dq * N(x1) - k * df * N(x1 - sigmaRootT) \
-                    - s * dq * pow(hOverS, 2.0 * l) * (N(-y) - N(-y1)) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * \
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_CALL:
+            if h >= K:
+                c_ui = S0 * dq * N(x1) - K * df * N(x1 - sigmaRootT) \
+                    - S0 * dq * pow(hOverS, 2.0 * ll) * (N(-y) - N(-y1)) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     (N(-y + sigmaRootT) - N(-y1 + sigmaRootT))
                 price = c_ui
             else:
                 price = c
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_CALL:
-            if h > k:
-                c_ui = s * dq * N(x1) - k * df * N(x1 - sigmaRootT) \
-                    - s * dq * pow(hOverS, 2.0 * l) * (N(-y) - N(-y1)) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * \
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_CALL:
+            if h > K:
+                c_ui = S0 * dq * N(x1) - K * df * N(x1 - sigmaRootT) \
+                    - S0 * dq * pow(hOverS, 2.0 * ll) * (N(-y) - N(-y1)) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     (N(-y + sigmaRootT) - N(-y1 + sigmaRootT))
                 price = c - c_ui
             else:
                 price = 0.0
-        elif self._option_type == EquityBarrierTypes.UP_AND_IN_PUT:
-            if h > k:
-                p_ui = -s * dq * pow(hOverS, 2.0 * l) * N(-y) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * N(-y + sigmaRootT)
+        elif self._option_type == FinFXBarrierTypes.UP_AND_IN_PUT:
+            if h > K:
+                p_ui = -S0 * dq * pow(hOverS, 2.0 * ll) * N(-y) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * N(-y + sigmaRootT)
                 price = p_ui
             else:
-                p_uo = -s * dq * N(-x1) \
-                    + k * df * N(-x1 + sigmaRootT) \
-                    + s * dq * pow(hOverS, 2.0 * l) * N(-y1) \
-                       - k * df * pow(hOverS, 2.0 * l - 2.0) * \
+                p_uo = -S0 * dq * N(-x1) \
+                    + K * df * N(-x1 + sigmaRootT) \
+                    + S0 * dq * pow(hOverS, 2.0 * ll) * N(-y1) \
+                       - K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     N(-y1 + sigmaRootT)
                 price = p - p_uo
-        elif self._option_type == EquityBarrierTypes.UP_AND_OUT_PUT:
-            if h >= k:
-                p_ui = -s * dq * pow(hOverS, 2.0 * l) * N(-y) \
-                    + k * df * pow(hOverS, 2.0 * l - 2.0) * N(-y + sigmaRootT)
+        elif self._option_type == FinFXBarrierTypes.UP_AND_OUT_PUT:
+            if h >= K:
+                p_ui = -S0 * dq * pow(hOverS, 2.0 * ll) * N(-y) \
+                    + K * df * pow(hOverS, 2.0 * ll - 2.0) * N(-y + sigmaRootT)
                 price = p - p_ui
             else:
-                p_uo = -s * dq * N(-x1) \
-                    + k * df * N(-x1 + sigmaRootT) \
-                    + s * dq * pow(hOverS, 2.0 * l) * N(-y1) \
-                       - k * df * pow(hOverS, 2.0 * l - 2.0) * \
+                p_uo = -S0 * dq * N(-x1) \
+                    + K * df * N(-x1 + sigmaRootT) \
+                    + S0 * dq * pow(hOverS, 2.0 * ll) * N(-y1) \
+                       - K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     N(-y1 + sigmaRootT)
                 price = p_uo
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT:
-            if h >= k:
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT:
+            if h >= K:
                 price = 0.0
             else:
-                p_di = -s * dq * N(-x1) \
-                    + k * df * N(-x1 + sigmaRootT) \
-                    + s * dq * pow(hOverS, 2.0 * l) * (N(y) - N(y1)) \
-                       - k * df * pow(hOverS, 2.0 * l - 2.0) * \
+                p_di = -S0 * dq * N(-x1) \
+                    + K * df * N(-x1 + sigmaRootT) \
+                    + S0 * dq * pow(hOverS, 2.0 * ll) * (N(y) - N(y1)) \
+                       - K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     (N(y - sigmaRootT) - N(y1 - sigmaRootT))
                 price = p - p_di
-        elif self._option_type == EquityBarrierTypes.DOWN_AND_IN_PUT:
-            if h >= k:
+        elif self._option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT:
+            if h >= K:
                 price = p
             else:
-                p_di = -s * dq * N(-x1) \
-                    + k * df * N(-x1 + sigmaRootT) \
-                    + s * dq * pow(hOverS, 2.0 * l) * (N(y) - N(y1)) \
-                       - k * df * pow(hOverS, 2.0 * l - 2.0) * \
+                p_di = -S0 * dq * N(-x1) \
+                    + K * df * N(-x1 + sigmaRootT) \
+                    + S0 * dq * pow(hOverS, 2.0 * ll) * (N(y) - N(y1)) \
+                       - K * df * pow(hOverS, 2.0 * ll - 2.0) * \
                     (N(y - sigmaRootT) - N(y1 - sigmaRootT))
                 price = p_di
         else:
             raise FinError("Unknown barrier option type." +
                            str(self._option_type))
 
-        v = price * self._notional
-        return v
+        return price
 
-###############################################################################
+    ###############################################################################
 
     def value_mc(self,
-                 valuation_date: Date,
-                 stock_price: float,
-                 discount_curve: DiscountCurve,
-                 dividend_curve: DiscountCurve,
+                 valuation_date,
+                 spot_fx_rate,
+                 dom_interest_rate,
                  process_type,
                  model_params,
-                 numAnnObs: int = 252,
-                 num_paths: int = 10000,
-                 seed: int = 4242):
-        """ A Monte-Carlo based valuation of the barrier option which simulates
-        the evolution of the stock price of at a specified number of annual
-        observation times until expiry to examine if the barrier has been
-        crossed and the corresponding value of the final payoff, if any. It
-        assumes a GBM model for the stock price. """
-
-        texp = (self._expiry_date - valuation_date) / gDaysInYear
-        num_time_steps = int(texp * numAnnObs)
-        K = self._strike_price
+                 num_ann_steps=552,
+                 num_paths=5000,
+                 seed=4242):
+        """ Value the FX Barrier Option using Monte Carlo. """
+
+        t = (self._expiry_date - valuation_date) / gDaysInYear
+        num_time_steps = int(t * num_ann_steps)
+        K = self._strike_fx_rate
         B = self._barrier_level
+        S0 = spot_fx_rate
         option_type = self._option_type
 
         process = FinProcessSimulator()
 
-        r = discount_curve.zero_rate(self._expiry_date)
-
-        # TODO - NEED TO DECIDE IF THIS IS PART OF MODEL PARAMS OR NOT ??????????????
-
-        r = discount_curve.cc_rate(self._expiry_date)
-        q = dividend_curve.cc_rate(self._expiry_date)
+        rd = dom_interest_rate
 
         #######################################################################
 
-        if option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL and stock_price <= B:
+        if option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL and S0 <= B:
             return 0.0
-        elif option_type == EquityBarrierTypes.UP_AND_OUT_CALL and stock_price >= B:
+        elif option_type == FinFXBarrierTypes.UP_AND_OUT_CALL and S0 >= B:
             return 0.0
-        elif option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT and stock_price <= B:
+        elif option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT and S0 <= B:
             return 0.0
-        elif option_type == EquityBarrierTypes.UP_AND_OUT_PUT and stock_price >= B:
+        elif option_type == FinFXBarrierTypes.UP_AND_OUT_PUT and S0 >= B:
             return 0.0
 
         #######################################################################
 
         simple_call = False
         simple_put = False
 
-        if option_type == EquityBarrierTypes.DOWN_AND_IN_CALL and stock_price <= B:
+        if option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL and S0 <= B:
             simple_call = True
-        elif option_type == EquityBarrierTypes.UP_AND_IN_CALL and stock_price >= B:
+        elif option_type == FinFXBarrierTypes.UP_AND_IN_CALL and S0 >= B:
             simple_call = True
-        elif option_type == EquityBarrierTypes.UP_AND_IN_PUT and stock_price >= B:
+        elif option_type == FinFXBarrierTypes.UP_AND_IN_PUT and S0 >= B:
             simple_put = True
-        elif option_type == EquityBarrierTypes.DOWN_AND_IN_PUT and stock_price <= B:
+        elif option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT and S0 <= B:
             simple_put = True
 
         if simple_put or simple_call:
             Sall = process.get_process(
-                process_type, texp, model_params, 1, num_paths, seed)
+                process_type, t, model_params, 1, num_paths, seed)
 
         if simple_call:
-            c = (np.maximum(Sall[:, -1] - K, 0.0)).mean()
-            c = c * np.exp(-r * texp)
+            sT = Sall[:, -1]
+            c = (np.maximum(sT - K, 0.0)).mean()
+            c = c * exp(-rd * t)
             return c
 
         if simple_put:
-            p = (np.maximum(K - Sall[:, -1], 0.0)).mean()
-            p = p * np.exp(-r * texp)
+            sT = Sall[:, -1]
+            p = (np.maximum(K - sT, 0.0)).mean()
+            p = p * exp(-rd * t)
             return p
 
         # Get full set of paths
-        Sall = process.get_process(process_type, texp, model_params, num_time_steps,
-                                   num_paths, seed)
+        Sall = process.get_process(process_type,
+                                   t,
+                                   model_params,
+                                   num_time_steps,
+                                   num_paths,
+                                   seed)
 
         (num_paths, num_time_steps) = Sall.shape
 
-        if option_type == EquityBarrierTypes.DOWN_AND_IN_CALL or \
-           option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL or \
-           option_type == EquityBarrierTypes.DOWN_AND_IN_PUT or \
-           option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT:
+        if option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL or \
+                option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL or \
+                option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT or \
+                option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT:
 
             barrierCrossedFromAbove = [False] * num_paths
 
             for p in range(0, num_paths):
                 barrierCrossedFromAbove[p] = np.any(Sall[p] <= B)
 
-        if option_type == EquityBarrierTypes.UP_AND_IN_CALL or \
-           option_type == EquityBarrierTypes.UP_AND_OUT_CALL or \
-           option_type == EquityBarrierTypes.UP_AND_IN_PUT or \
-           option_type == EquityBarrierTypes.UP_AND_OUT_PUT:
+        if option_type == FinFXBarrierTypes.UP_AND_IN_CALL or \
+                option_type == FinFXBarrierTypes.UP_AND_OUT_CALL or \
+                option_type == FinFXBarrierTypes.UP_AND_IN_PUT or \
+                option_type == FinFXBarrierTypes.UP_AND_OUT_PUT:
 
             barrierCrossedFromBelow = [False] * num_paths
             for p in range(0, num_paths):
                 barrierCrossedFromBelow[p] = np.any(Sall[p] >= B)
 
         payoff = np.zeros(num_paths)
         ones = np.ones(num_paths)
 
-        if option_type == EquityBarrierTypes.DOWN_AND_OUT_CALL:
+        if option_type == FinFXBarrierTypes.DOWN_AND_OUT_CALL:
             payoff = np.maximum(Sall[:, -1] - K, 0.0) * \
                 (ones - barrierCrossedFromAbove)
-        elif option_type == EquityBarrierTypes.DOWN_AND_IN_CALL:
+        elif option_type == FinFXBarrierTypes.DOWN_AND_IN_CALL:
             payoff = np.maximum(Sall[:, -1] - K, 0.0) * barrierCrossedFromAbove
-        elif option_type == EquityBarrierTypes.UP_AND_IN_CALL:
+        elif option_type == FinFXBarrierTypes.UP_AND_IN_CALL:
             payoff = np.maximum(Sall[:, -1] - K, 0.0) * barrierCrossedFromBelow
-        elif option_type == EquityBarrierTypes.UP_AND_OUT_CALL:
+        elif option_type == FinFXBarrierTypes.UP_AND_OUT_CALL:
             payoff = np.maximum(Sall[:, -1] - K, 0.0) * \
                 (ones - barrierCrossedFromBelow)
-        elif option_type == EquityBarrierTypes.UP_AND_IN_PUT:
+        elif option_type == FinFXBarrierTypes.UP_AND_IN_PUT:
             payoff = np.maximum(K - Sall[:, -1], 0.0) * barrierCrossedFromBelow
-        elif option_type == EquityBarrierTypes.UP_AND_OUT_PUT:
+        elif option_type == FinFXBarrierTypes.UP_AND_OUT_PUT:
             payoff = np.maximum(K - Sall[:, -1], 0.0) * \
                 (ones - barrierCrossedFromBelow)
-        elif option_type == EquityBarrierTypes.DOWN_AND_OUT_PUT:
+        elif option_type == FinFXBarrierTypes.DOWN_AND_OUT_PUT:
             payoff = np.maximum(K - Sall[:, -1], 0.0) * \
                 (ones - barrierCrossedFromAbove)
-        elif option_type == EquityBarrierTypes.DOWN_AND_IN_PUT:
+        elif option_type == FinFXBarrierTypes.DOWN_AND_IN_PUT:
             payoff = np.maximum(K - Sall[:, -1], 0.0) * barrierCrossedFromAbove
         else:
             raise FinError("Unknown barrier option type." +
                            str(self._option_type))
 
-        v = payoff.mean() * np.exp(- r * texp)
+        v = payoff.mean() * exp(-rd * t)
 
-        return v * self._notional
+        return v
 
-###############################################################################
+    ###############################################################################
 
     def __repr__(self):
         s = label_to_string("OBJECT TYPE", type(self).__name__)
         s += label_to_string("EXPIRY DATE", self._expiry_date)
-        s += label_to_string("STRIKE PRICE", self._strike_price)
+        s += label_to_string("STRIKE FX RATE", self._strike_fx_rate)
+        s += label_to_string("CURRENCY PAIR", self._currency_pair)
         s += label_to_string("OPTION TYPE", self._option_type)
         s += label_to_string("BARRIER LEVEL", self._barrier_level)
         s += label_to_string("NUM OBSERVATIONS",
                              self._num_observations_per_year)
-        s += label_to_string("NOTIONAL", self._notional, "")
+        s += label_to_string("NOTIONAL", self._notional)
+        s += label_to_string("NOTIONAL CURRENCY", self._notional_currency, "")
         return s
 
-###############################################################################
+    ###############################################################################
 
     def _print(self):
-        """ Simple print function for backward compatibility. """
+        """ Print a list of the unadjusted coupon payment dates used in
+        analytic calculations for the bond. """
         print(self)
 
 ###############################################################################
```

### Comparing `financepy-0.270/financepy/products/equity/equity_basket_option.py` & `financepy-0.290/financepy/products/equity/equity_basket_option.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,16 +103,14 @@
               volatilities: np.ndarray,
               correlations: np.ndarray):
         """ Basket valuation using a moment matching method to approximate the
         effective variance of the underlying basket value. This approach is
         able to handle a full rank correlation structure between the individual
         assets. """
 
-    # https://pdfs.semanticscholar.org/16ed/c0e804379e22ff36dcbab7e9bb06519faa43.pdf
-
         texp = (self._expiry_date - valuation_date) / gDaysInYear
 
         if valuation_date > self._expiry_date:
             raise FinError("Value date after expiry date.")
 
         qs = []
         for curve in dividend_curves:
```

### Comparing `financepy-0.270/financepy/products/equity/equity_binomial_tree.py` & `financepy-0.290/financepy/products/equity/equity_binomial_tree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_chooser_option.py` & `financepy-0.290/financepy/products/equity/equity_chooser_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_cliquet_option.py` & `financepy-0.290/financepy/products/equity/equity_cliquet_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_compound_option.py` & `financepy-0.290/financepy/products/equity/equity_compound_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_digital_option.py` & `financepy-0.290/financepy/products/equity/equity_digital_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_fixed_lookback_option.py` & `financepy-0.290/financepy/products/equity/equity_fixed_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_float_lookback_option.py` & `financepy-0.290/financepy/products/equity/equity_float_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_forward.py` & `financepy-0.290/financepy/products/equity/equity_forward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_model_types.py` & `financepy-0.290/financepy/products/equity/equity_model_types.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_one_touch_option.py` & `financepy-0.290/financepy/products/equity/equity_one_touch_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_option.py` & `financepy-0.290/financepy/products/equity/equity_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_rainbow_option.py` & `financepy-0.290/financepy/products/equity/equity_rainbow_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_vanilla_option.py` & `financepy-0.290/financepy/products/equity/equity_vanilla_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/equity/equity_variance_swap.py` & `financepy-0.290/financepy/products/equity/equity_variance_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_digital_option.py` & `financepy-0.290/financepy/products/fx/fx_digital_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_fixed_lookback_option.py` & `financepy-0.290/financepy/products/fx/fx_fixed_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_float_lookback_option.py` & `financepy-0.290/financepy/products/fx/fx_float_lookback_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_forward.py` & `financepy-0.290/financepy/products/fx/fx_forward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_mkt_conventions.py` & `financepy-0.290/financepy/products/fx/fx_mkt_conventions.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_one_touch_option.py` & `financepy-0.290/financepy/products/fx/fx_one_touch_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_option.py` & `financepy-0.290/financepy/products/fx/fx_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_rainbow_option.py` & `financepy-0.290/financepy/products/fx/fx_rainbow_option.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/fx/fx_vanilla_option.py` & `financepy-0.290/financepy/products/fx/fx_vanilla_option.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,19 +294,18 @@
 
         if type(model) == BlackScholes or \
            type(model) == SABR:
 
             if type(model) == BlackScholes:
                 volatility = model._volatility
             elif type(model) == SABR:
-                volatility = vol_function_sabr(model.alpha,
-                                               model.beta,
-                                               model.rho,
-                                               model.nu,
-                                               F0T, K, tdel)
+
+                params_list = np.array([model._alpha, model._beta, model._rho, model._nu])
+                
+                volatility = vol_function_sabr(params_list, F0T, K, tdel)
 
             if np.any(volatility < 0.0):
                 raise FinError("Volatility should not be negative.")
 
             v = np.maximum(volatility, 1e-10)
 
             if self._option_type == OptionTypes.EUROPEAN_CALL:
```

### Comparing `financepy-0.270/financepy/products/fx/fx_variance_swap.py` & `financepy-0.290/financepy/products/fx/fx_variance_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/inflation/FinInflationBond.py` & `financepy-0.290/financepy/products/inflation/FinInflationBond.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,16 +35,18 @@
                  num_ex_dividend_days: int = 0, 
                  calendar_type: CalendarTypes = CalendarTypes.NONE):  # Value of CPI index at bond issue date
         """ Create FinInflationBond object by providing Maturity, Frequency,
         coupon, frequency and the accrual convention type. You must also supply
         the base CPI used for all coupon and principal related calculations. 
         The class inherits from Bond so has many similar functions. The YTM"""
 
+        Bond.__init__(self,issue_date, maturity_date, coupon, freq_type, accrual_type, face_amount, calendar_type)
         check_argument_types(self.__init__, locals())
 
+        
         if issue_date >= maturity_date:
             raise FinError("Issue Date must preceded maturity date.")
 
         # If the maturity date falls on the last day of the month we assume
         # that earlier flows also fall on month ends
         self._end_of_month = False
         if maturity_date.is_eom():
```

### Comparing `financepy-0.270/financepy/products/inflation/FinInflationIndexCurve.py` & `financepy-0.290/financepy/products/inflation/FinInflationIndexCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/inflation/FinInflationSwap.py` & `financepy-0.290/financepy/products/inflation/FinInflationSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/inflation/FinInflationSwapCurve.py` & `financepy-0.290/financepy/products/inflation/FinInflationSwapCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/bermudan_swaption.py` & `financepy-0.290/financepy/products/rates/bermudan_swaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/callable_swap.py` & `financepy-0.290/financepy/products/rates/callable_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/dual_curve.py` & `financepy-0.290/financepy/products/rates/dual_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_basis_swap.py` & `financepy-0.290/financepy/products/rates/ibor_basis_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_cap_floor.py` & `financepy-0.290/financepy/products/rates/ibor_cap_floor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_conventions.py` & `financepy-0.290/financepy/products/rates/ibor_conventions.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_deposit.py` & `financepy-0.290/financepy/products/rates/ibor_deposit.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_fra.py` & `financepy-0.290/financepy/products/rates/ibor_fra.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_future.py` & `financepy-0.290/financepy/products/rates/ibor_future.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_lmm_products.py` & `financepy-0.290/financepy/products/rates/ibor_lmm_products.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_single_curve.py` & `financepy-0.290/financepy/products/rates/ibor_single_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_swap.py` & `financepy-0.290/financepy/products/rates/ibor_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ibor_swaption.py` & `financepy-0.290/financepy/products/rates/ibor_swaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ois.py` & `financepy-0.290/financepy/products/rates/ois.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ois_basis_swap.py` & `financepy-0.290/financepy/products/rates/ois_basis_swap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/ois_curve.py` & `financepy-0.290/financepy/products/rates/ois_curve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/products/rates/swap_fixed_leg.py` & `financepy-0.290/financepy/products/rates/swap_float_leg.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from ...utils.date import Date
 from ...utils.math import ONE_MILLION
 from ...utils.day_count import DayCount, DayCountTypes
 from ...utils.frequency import FrequencyTypes
 from ...utils.calendar import CalendarTypes,  DateGenRuleTypes
 from ...utils.calendar import Calendar, BusDayAdjustTypes
 from ...utils.schedule import Schedule
-from ...utils.helpers import label_to_string, check_argument_types
+from ...utils.helpers import format_table, label_to_string, check_argument_types
 from ...utils.global_types import SwapTypes
 from ...market.curves.discount_curve import DiscountCurve
 
 ##########################################################################
 
 
-class SwapFixedLeg:
-    """ Class for managing the fixed leg of a swap. A fixed leg is a leg with
+class SwapFloatLeg:
+    """ Class for managing the floating leg of a swap. A float leg consists of
     a sequence of flows calculated according to an ISDA schedule and with a 
-    coupon that is fixed over the life of the swap. """
+    coupon determined by an index curve which changes over life of the swap."""
 
     def __init__(self,
                  effective_date: Date,  # Date interest starts to accrue
                  end_date: (Date, str),  # Date contract ends
                  leg_type: SwapTypes,
-                 coupon: (float),
+                 spread: (float),
                  freq_type: FrequencyTypes,
                  day_count_type: DayCountTypes,
                  notional: float = ONE_MILLION,
                  principal: float = 0.0,
                  payment_lag: int = 0,
                  calendar_type: CalendarTypes = CalendarTypes.WEEKEND,
                  bus_day_adjust_type: BusDayAdjustTypes = BusDayAdjustTypes.FOLLOWING,
@@ -44,55 +44,50 @@
 
         if type(end_date) == Date:
             self._termination_date = end_date
         else:
             self._termination_date = effective_date.add_tenor(end_date)
 
         calendar = Calendar(calendar_type)
-
         self._maturity_date = calendar.adjust(self._termination_date,
                                               bus_day_adjust_type)
 
         if effective_date > self._maturity_date:
-            raise FinError("Effective date after maturity date")
+            raise FinError("Start date after maturity date")
 
         self._effective_date = effective_date
         self._end_date = end_date
         self._leg_type = leg_type
         self._freq_type = freq_type
         self._payment_lag = payment_lag
+        self._principal = 0.0
         self._notional = notional
-        self._principal = principal
-        self._coupon = coupon
+        self._notional_array = []
+        self._spread = spread
 
         self._day_count_type = day_count_type
         self._calendar_type = calendar_type
         self._bus_day_adjust_type = bus_day_adjust_type
         self._date_gen_rule_type = date_gen_rule_type
         self._end_of_month = end_of_month
 
         self._startAccruedDates = []
         self._endAccruedDates = []
         self._payment_dates = []
         self._payments = []
         self._year_fracs = []
         self._accrued_days = []
-        self._rates = []
 
-        self.generate_payments()
+        self.generate_payment_dates()
 
 ###############################################################################
 
-    def generate_payments(self):
-        ''' These are generated immediately as they are for the entire
-        life of the swap. Given a valuation date we can determine
-        which cash flows are in the future and value the swap
-        The schedule allows for a specified lag in the payment date
-        Nothing is paid on the swap effective date and so the first payment
-        date is the first actual payment date. '''
+    def generate_payment_dates(self):
+        """ Generate the floating leg payment dates and accrual factors. The
+        coupons cannot be generated yet as we do not have the index curve. """
 
         schedule = Schedule(self._effective_date,
                             self._termination_date,
                             self._freq_type,
                             self._calendar_type,
                             self._bus_day_adjust_type,
                             self._date_gen_rule_type,
@@ -102,90 +97,125 @@
 
         if len(scheduleDates) < 2:
             raise FinError("Schedule has none or only one date")
 
         self._startAccruedDates = []
         self._endAccruedDates = []
         self._payment_dates = []
-        self._payments = []
         self._year_fracs = []
         self._accrued_days = []
-        self._rates = []
 
         prev_dt = scheduleDates[0]
 
         day_counter = DayCount(self._day_count_type)
         calendar = Calendar(self._calendar_type)
 
+        # All of the lists end up with the same length
         for next_dt in scheduleDates[1:]:
 
             self._startAccruedDates.append(prev_dt)
             self._endAccruedDates.append(next_dt)
 
             if self._payment_lag == 0:
                 payment_date = next_dt
             else:
                 payment_date = calendar.add_business_days(next_dt,
                                                           self._payment_lag)
 
             self._payment_dates.append(payment_date)
 
-            (year_frac, num, den) = day_counter.year_frac(prev_dt,
-                                                          next_dt)
+            (year_frac, num, _) = day_counter.year_frac(prev_dt,
+                                                        next_dt)
 
-            self._rates.append(self._coupon)
-
-            payment = year_frac * self._notional * self._coupon
-
-            self._payments.append(payment)
             self._year_fracs.append(year_frac)
             self._accrued_days.append(num)
 
             prev_dt = next_dt
 
 ###############################################################################
 
     def value(self,
-              valuation_date: Date,
-              discount_curve: DiscountCurve):
+              valuation_date: Date,  # This should be the settlement date
+              discount_curve: DiscountCurve,
+              index_curve: DiscountCurve,
+              firstFixingRate: float = None):
+        """ Value the floating leg with payments from an index curve and
+        discounting based on a supplied discount curve as of the valuation date
+        supplied. For an existing swap, the user must enter the next fixing
+        coupon. """
+
+        if discount_curve is None:
+            raise FinError("Discount curve is None")
 
+        if index_curve is None:
+            index_curve = discount_curve
+
+        self._rates = []
+        self._payments = []
         self._paymentDfs = []
         self._paymentPVs = []
         self._cumulativePVs = []
 
-        notional = self._notional
         dfValue = discount_curve.df(valuation_date)
         legPV = 0.0
         numPayments = len(self._payment_dates)
+        firstPayment = False
 
-        dfPmnt = 0.0
+        if not len(self._notional_array):
+            self._notional_array = [self._notional] * numPayments
+
+        index_basis = index_curve._day_count_type
+        index_day_counter = DayCount(index_basis)
 
         for iPmnt in range(0, numPayments):
 
             pmntDate = self._payment_dates[iPmnt]
-            pmntAmount = self._payments[iPmnt]
 
             if pmntDate > valuation_date:
 
+                startAccruedDt = self._startAccruedDates[iPmnt]
+                endAccruedDt = self._endAccruedDates[iPmnt]
+                pay_alpha = self._year_fracs[iPmnt]
+
+                (index_alpha, num, _) = index_day_counter.year_frac(startAccruedDt,
+                                                                    endAccruedDt)
+
+                if firstPayment is False and firstFixingRate is not None:
+
+                    fwd_rate = firstFixingRate
+                    firstPayment = True
+
+                else:
+
+                    dfStart = index_curve.df(startAccruedDt)
+                    dfEnd = index_curve.df(endAccruedDt)
+                    fwd_rate = (dfStart / dfEnd - 1.0) / index_alpha
+
+                pmntAmount = (fwd_rate + self._spread) * pay_alpha * self._notional_array[iPmnt]
+
                 dfPmnt = discount_curve.df(pmntDate) / dfValue
                 pmntPV = pmntAmount * dfPmnt
                 legPV += pmntPV
 
+                self._rates.append(fwd_rate)
+                self._payments.append(pmntAmount)
                 self._paymentDfs.append(dfPmnt)
-                self._paymentPVs.append(pmntAmount*dfPmnt)
+                self._paymentPVs.append(pmntPV)
                 self._cumulativePVs.append(legPV)
 
             else:
 
+                self._rates.append(0.0)
+                self._payments.append(0.0)
                 self._paymentDfs.append(0.0)
                 self._paymentPVs.append(0.0)
-                self._cumulativePVs.append(0.0)
+                self._cumulativePVs.append(legPV)
 
         if pmntDate > valuation_date:
-            paymentPV = self._principal * dfPmnt * notional
+            paymentPV = self._principal * dfPmnt * self._notional_array[-1]
             self._paymentPVs[-1] += paymentPV
             legPV += paymentPV
             self._cumulativePVs[-1] = legPV
 
         if self._leg_type == SwapTypes.PAY:
             legPV = legPV * (-1.0)
 
@@ -196,85 +226,90 @@
     def print_payments(self):
         """ Prints the fixed leg dates, accrual factors, discount factors,
         cash amounts, their present value and their cumulative PV using the
         last valuation performed. """
 
         print("START DATE:", self._effective_date)
         print("MATURITY DATE:", self._maturity_date)
-        print("COUPON (%):", self._coupon * 100)
+        print("SPREAD (bp):", self._spread * 10000)
         print("FREQUENCY:", str(self._freq_type))
         print("DAY COUNT:", str(self._day_count_type))
 
-        if len(self._payments) == 0:
-            print("Payments not calculated.")
+        if len(self._payment_dates) == 0:
+            print("Payments Dates not calculated.")
             return
 
-        header = "PAY_DATE     ACCR_START   ACCR_END      DAYS  YEARFRAC"
-        header += "    RATE      PAYMENT "
-        print(header)
+        header = [ "PAY_NUM", "PAY_DATE", "ACCR_START", "ACCR_END", "DAYS", "YEARFRAC"]
 
+        rows = []
         num_flows = len(self._payment_dates)
-
         for iFlow in range(0, num_flows):
-            print("%11s  %11s  %11s  %4d  %8.6f  %8.6f  %11.2f" %
-                  (self._payment_dates[iFlow],
-                   self._startAccruedDates[iFlow],
-                   self._endAccruedDates[iFlow],
-                   self._accrued_days[iFlow],
-                   self._year_fracs[iFlow],
-                   self._rates[iFlow] * 100.0,
-                   self._payments[iFlow]))
+            rows.append([
+                iFlow + 1,
+                self._payment_dates[iFlow],
+                self._startAccruedDates[iFlow],
+                self._endAccruedDates[iFlow],
+                self._accrued_days[iFlow],
+                round(self._year_fracs[iFlow],4),
+            ])
+            
+        table = format_table(header, rows)
+        print("\nPAYMENTS SCHEDULE:")
+        print(table)
 
 ###############################################################################
 
     def print_valuation(self):
         """ Prints the fixed leg dates, accrual factors, discount factors,
         cash amounts, their present value and their cumulative PV using the
         last valuation performed. """
 
         print("START DATE:", self._effective_date)
         print("MATURITY DATE:", self._maturity_date)
-        print("COUPON (%):", self._coupon * 100)
+        print("SPREAD (BPS):", self._spread * 10000)
         print("FREQUENCY:", str(self._freq_type))
         print("DAY COUNT:", str(self._day_count_type))
 
+        self.print_payments()
+
         if len(self._payments) == 0:
             print("Payments not calculated.")
             return
 
-        header = "PAY_DATE     ACCR_START   ACCR_END     DAYS  YEARFRAC"
-        header += "    RATE      PAYMENT       DF          PV        CUM PV"
-        print(header)
+        header = [ "PAY_NUM", "PAY_DATE",  "NOTIONAL", 
+                  "IBOR", "PMNT", "DF", "PV", "CUM_PV"]
 
+        rows = []          
         num_flows = len(self._payment_dates)
-
         for iFlow in range(0, num_flows):
-            print("%11s  %11s  %11s  %4d  %8.6f  %8.5f  % 11.2f  %10.8f  % 11.2f  % 11.2f" %
-                  (self._payment_dates[iFlow],
-                   self._startAccruedDates[iFlow],
-                   self._endAccruedDates[iFlow],
-                   self._accrued_days[iFlow],
-                   self._year_fracs[iFlow],
-                   self._rates[iFlow] * 100.0,
-                   self._payments[iFlow],
-                   self._paymentDfs[iFlow],
-                   self._paymentPVs[iFlow],
-                   self._cumulativePVs[iFlow]))
+            rows.append([
+                iFlow + 1,
+                self._payment_dates[iFlow],
+                round(self._notional_array[iFlow], 0),
+                round(self._rates[iFlow] * 100.0, 4),
+                round(self._payments[iFlow], 2),
+                round(self._paymentDfs[iFlow], 4),
+                round(self._paymentPVs[iFlow], 2),
+                round(self._cumulativePVs[iFlow], 2),
+            ])
+
+        table = format_table(header, rows)
+        print("\nPAYMENTS VALUATION:")
+        print(table)
 
-##########################################################################
+###############################################################################
 
     def __repr__(self):
         s = label_to_string("OBJECT TYPE", type(self).__name__)
         s += label_to_string("START DATE", self._effective_date)
         s += label_to_string("TERMINATION DATE", self._termination_date)
         s += label_to_string("MATURITY DATE", self._maturity_date)
         s += label_to_string("NOTIONAL", self._notional)
-        s += label_to_string("PRINCIPAL", self._principal)
-        s += label_to_string("LEG TYPE", self._leg_type)
-        s += label_to_string("COUPON", self._coupon)
+        s += label_to_string("SWAP TYPE", self._leg_type)
+        s += label_to_string("SPREAD (BPS)", self._spread*10000)
         s += label_to_string("FREQUENCY", self._freq_type)
         s += label_to_string("DAY COUNT", self._day_count_type)
         s += label_to_string("CALENDAR", self._calendar_type)
         s += label_to_string("BUS DAY ADJUST", self._bus_day_adjust_type)
         s += label_to_string("DATE GEN TYPE", self._date_gen_rule_type)
         return s
```

### Comparing `financepy-0.270/financepy/products/rates/swap_float_leg.py` & `financepy-0.290/financepy/products/rates/swap_fixed_leg.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from ...utils.date import Date
 from ...utils.math import ONE_MILLION
 from ...utils.day_count import DayCount, DayCountTypes
 from ...utils.frequency import FrequencyTypes
 from ...utils.calendar import CalendarTypes,  DateGenRuleTypes
 from ...utils.calendar import Calendar, BusDayAdjustTypes
 from ...utils.schedule import Schedule
-from ...utils.helpers import label_to_string, check_argument_types
+from ...utils.helpers import format_table, label_to_string, check_argument_types
 from ...utils.global_types import SwapTypes
 from ...market.curves.discount_curve import DiscountCurve
 
 ##########################################################################
 
 
-class SwapFloatLeg:
-    """ Class for managing the floating leg of a swap. A float leg consists of
+class SwapFixedLeg:
+    """ Class for managing the fixed leg of a swap. A fixed leg is a leg with
     a sequence of flows calculated according to an ISDA schedule and with a 
-    coupon determined by an index curve which changes over life of the swap."""
+    coupon that is fixed over the life of the swap. """
 
     def __init__(self,
                  effective_date: Date,  # Date interest starts to accrue
                  end_date: (Date, str),  # Date contract ends
                  leg_type: SwapTypes,
-                 spread: (float),
+                 coupon: (float),
                  freq_type: FrequencyTypes,
                  day_count_type: DayCountTypes,
                  notional: float = ONE_MILLION,
                  principal: float = 0.0,
                  payment_lag: int = 0,
                  calendar_type: CalendarTypes = CalendarTypes.WEEKEND,
                  bus_day_adjust_type: BusDayAdjustTypes = BusDayAdjustTypes.FOLLOWING,
@@ -44,49 +44,55 @@
 
         if type(end_date) == Date:
             self._termination_date = end_date
         else:
             self._termination_date = effective_date.add_tenor(end_date)
 
         calendar = Calendar(calendar_type)
+
         self._maturity_date = calendar.adjust(self._termination_date,
                                               bus_day_adjust_type)
 
         if effective_date > self._maturity_date:
-            raise FinError("Start date after maturity date")
+            raise FinError("Effective date after maturity date")
 
         self._effective_date = effective_date
         self._end_date = end_date
         self._leg_type = leg_type
         self._freq_type = freq_type
         self._payment_lag = payment_lag
         self._notional = notional
-        self._principal = 0.0
-        self._spread = spread
+        self._principal = principal
+        self._coupon = coupon
 
         self._day_count_type = day_count_type
         self._calendar_type = calendar_type
         self._bus_day_adjust_type = bus_day_adjust_type
         self._date_gen_rule_type = date_gen_rule_type
         self._end_of_month = end_of_month
 
         self._startAccruedDates = []
         self._endAccruedDates = []
         self._payment_dates = []
         self._payments = []
         self._year_fracs = []
         self._accrued_days = []
+        self._rates = []
 
-        self.generate_payment_dates()
+        self.generate_payments()
 
 ###############################################################################
 
-    def generate_payment_dates(self):
-        """ Generate the floating leg payment dates and accrual factors. The
-        coupons cannot be generated yet as we do not have the index curve. """
+    def generate_payments(self):
+        ''' These are generated immediately as they are for the entire
+        life of the swap. Given a valuation date we can determine
+        which cash flows are in the future and value the swap
+        The schedule allows for a specified lag in the payment date
+        Nothing is paid on the swap effective date and so the first payment
+        date is the first actual payment date. '''
 
         schedule = Schedule(self._effective_date,
                             self._termination_date,
                             self._freq_type,
                             self._calendar_type,
                             self._bus_day_adjust_type,
                             self._date_gen_rule_type,
@@ -96,120 +102,87 @@
 
         if len(scheduleDates) < 2:
             raise FinError("Schedule has none or only one date")
 
         self._startAccruedDates = []
         self._endAccruedDates = []
         self._payment_dates = []
+        self._payments = []
         self._year_fracs = []
         self._accrued_days = []
+        self._rates = []
 
         prev_dt = scheduleDates[0]
 
         day_counter = DayCount(self._day_count_type)
         calendar = Calendar(self._calendar_type)
 
-        # All of the lists end up with the same length
         for next_dt in scheduleDates[1:]:
 
             self._startAccruedDates.append(prev_dt)
             self._endAccruedDates.append(next_dt)
 
             if self._payment_lag == 0:
                 payment_date = next_dt
             else:
                 payment_date = calendar.add_business_days(next_dt,
                                                           self._payment_lag)
 
             self._payment_dates.append(payment_date)
 
-            (year_frac, num, _) = day_counter.year_frac(prev_dt,
-                                                        next_dt)
+            (year_frac, num, den) = day_counter.year_frac(prev_dt,
+                                                          next_dt)
+
+            self._rates.append(self._coupon)
+
+            payment = year_frac * self._notional * self._coupon
 
+            self._payments.append(payment)
             self._year_fracs.append(year_frac)
             self._accrued_days.append(num)
 
             prev_dt = next_dt
 
 ###############################################################################
 
     def value(self,
-              valuation_date: Date,  # This should be the settlement date
-              discount_curve: DiscountCurve,
-              index_curve: DiscountCurve,
-              firstFixingRate: float = None):
-        """ Value the floating leg with payments from an index curve and
-        discounting based on a supplied discount curve as of the valuation date
-        supplied. For an existing swap, the user must enter the next fixing
-        coupon. """
+              valuation_date: Date,
+              discount_curve: DiscountCurve):
 
-        if discount_curve is None:
-            raise FinError("Discount curve is None")
-
-        if index_curve is None:
-            index_curve = discount_curve
-
-        self._rates = []
-        self._payments = []
         self._paymentDfs = []
         self._paymentPVs = []
         self._cumulativePVs = []
 
         notional = self._notional
         dfValue = discount_curve.df(valuation_date)
         legPV = 0.0
         numPayments = len(self._payment_dates)
-        firstPayment = False
 
-        index_basis = index_curve._day_count_type
-        index_day_counter = DayCount(index_basis)
+        dfPmnt = 0.0
 
         for iPmnt in range(0, numPayments):
 
             pmntDate = self._payment_dates[iPmnt]
+            pmntAmount = self._payments[iPmnt]
 
             if pmntDate > valuation_date:
 
-                startAccruedDt = self._startAccruedDates[iPmnt]
-                endAccruedDt = self._endAccruedDates[iPmnt]
-                pay_alpha = self._year_fracs[iPmnt]
-
-                (index_alpha, num, _) = index_day_counter.year_frac(startAccruedDt,
-                                                                    endAccruedDt)
-
-                if firstPayment is False and firstFixingRate is not None:
-
-                    fwd_rate = firstFixingRate
-                    firstPayment = True
-
-                else:
-
-                    dfStart = index_curve.df(startAccruedDt)
-                    dfEnd = index_curve.df(endAccruedDt)
-                    fwd_rate = (dfStart / dfEnd - 1.0) / index_alpha
-
-                pmntAmount = (fwd_rate + self._spread) * pay_alpha * notional
-
                 dfPmnt = discount_curve.df(pmntDate) / dfValue
                 pmntPV = pmntAmount * dfPmnt
                 legPV += pmntPV
 
-                self._rates.append(fwd_rate)
-                self._payments.append(pmntAmount)
                 self._paymentDfs.append(dfPmnt)
-                self._paymentPVs.append(pmntPV)
+                self._paymentPVs.append(pmntAmount*dfPmnt)
                 self._cumulativePVs.append(legPV)
 
             else:
 
-                self._rates.append(0.0)
-                self._payments.append(0.0)
                 self._paymentDfs.append(0.0)
                 self._paymentPVs.append(0.0)
-                self._cumulativePVs.append(legPV)
+                self._cumulativePVs.append(0.0)
 
         if pmntDate > valuation_date:
             paymentPV = self._principal * dfPmnt * notional
             self._paymentPVs[-1] += paymentPV
             legPV += paymentPV
             self._cumulativePVs[-1] = legPV
 
@@ -223,81 +196,92 @@
     def print_payments(self):
         """ Prints the fixed leg dates, accrual factors, discount factors,
         cash amounts, their present value and their cumulative PV using the
         last valuation performed. """
 
         print("START DATE:", self._effective_date)
         print("MATURITY DATE:", self._maturity_date)
-        print("SPREAD (bp):", self._spread * 10000)
+        print("COUPON (%):", self._coupon * 100)
         print("FREQUENCY:", str(self._freq_type))
         print("DAY COUNT:", str(self._day_count_type))
 
-        if len(self._payment_dates) == 0:
-            print("Payments Dates not calculated.")
+        if len(self._payments) == 0:
+            print("Payments not calculated.")
             return
 
-        header = "PAY_DATE     ACCR_START   ACCR_END      DAYS  YEARFRAC"
-        print(header)
+        header = [ "PAY_NUM", "PAY_DATE", "ACCR_START", "ACCR_END", 
+                    "DAYS", "YEARFRAC", "RATE", "PMNT"]
 
+        rows = []
         num_flows = len(self._payment_dates)
-
         for iFlow in range(0, num_flows):
-            print("%11s  %11s  %11s  %4d  %8.6f  " %
-                  (self._payment_dates[iFlow],
-                   self._startAccruedDates[iFlow],
-                   self._endAccruedDates[iFlow],
-                   self._accrued_days[iFlow],
-                   self._year_fracs[iFlow]))
+            rows.append([
+                iFlow + 1,
+                self._payment_dates[iFlow],
+                self._startAccruedDates[iFlow],
+                self._endAccruedDates[iFlow],
+                self._accrued_days[iFlow],
+                round(self._year_fracs[iFlow],4),
+                round(self._rates[iFlow] * 100.0, 4),
+                round(self._payments[iFlow], 2),
+            ])
+
+        table = format_table(header, rows)
+        print("\nPAYMENTS SCHEDULE:")
+        print(table)
 
 ###############################################################################
 
     def print_valuation(self):
         """ Prints the fixed leg dates, accrual factors, discount factors,
         cash amounts, their present value and their cumulative PV using the
         last valuation performed. """
 
         print("START DATE:", self._effective_date)
         print("MATURITY DATE:", self._maturity_date)
-        print("SPREAD (BPS):", self._spread * 10000)
+        print("COUPON (%):", self._coupon * 100)
         print("FREQUENCY:", str(self._freq_type))
         print("DAY COUNT:", str(self._day_count_type))
 
         if len(self._payments) == 0:
             print("Payments not calculated.")
             return
 
-        header = "PAY_DATE     ACCR_START   ACCR_END     DAYS  YEARFRAC"
-        header += "    IBOR      PAYMENT       DF          PV        CUM PV"
-        print(header)
+        header = [ "PAY_NUM", "PAY_DATE", "NOTIONAL", 
+                  "RATE", "PMNT", "DF", "PV", "CUM_PV"]
 
+        rows = []
         num_flows = len(self._payment_dates)
-
         for iFlow in range(0, num_flows):
-            print("%11s  %11s  %11s  %4d  %8.6f  %9.5f  % 11.2f  %10.8f  % 11.2f  % 11.2f" %
-                  (self._payment_dates[iFlow],
-                   self._startAccruedDates[iFlow],
-                   self._endAccruedDates[iFlow],
-                   self._accrued_days[iFlow],
-                   self._year_fracs[iFlow],
-                   self._rates[iFlow] * 100.0,
-                   self._payments[iFlow],
-                   self._paymentDfs[iFlow],
-                   self._paymentPVs[iFlow],
-                   self._cumulativePVs[iFlow]))
+            rows.append([
+                iFlow + 1,
+                self._payment_dates[iFlow],
+                round(self._notional, 0),
+                round(self._rates[iFlow] * 100.0, 4),
+                round(self._payments[iFlow], 2),
+                round(self._paymentDfs[iFlow], 4),
+                round(self._paymentPVs[iFlow], 2),
+                round(self._cumulativePVs[iFlow], 2),
+            ])
+
+        table = format_table(header, rows)
+        print("\nPAYMENTS VALUATION:")
+        print(table)
 
-###############################################################################
+##########################################################################
 
     def __repr__(self):
         s = label_to_string("OBJECT TYPE", type(self).__name__)
         s += label_to_string("START DATE", self._effective_date)
         s += label_to_string("TERMINATION DATE", self._termination_date)
         s += label_to_string("MATURITY DATE", self._maturity_date)
         s += label_to_string("NOTIONAL", self._notional)
-        s += label_to_string("SWAP TYPE", self._leg_type)
-        s += label_to_string("SPREAD (BPS)", self._spread*10000)
+        s += label_to_string("PRINCIPAL", self._principal)
+        s += label_to_string("LEG TYPE", self._leg_type)
+        s += label_to_string("COUPON", self._coupon)
         s += label_to_string("FREQUENCY", self._freq_type)
         s += label_to_string("DAY COUNT", self._day_count_type)
         s += label_to_string("CALENDAR", self._calendar_type)
         s += label_to_string("BUS DAY ADJUST", self._bus_day_adjust_type)
         s += label_to_string("DATE GEN TYPE", self._date_gen_rule_type)
         return s
```

### Comparing `financepy-0.270/financepy/utils/amount.py` & `financepy-0.290/financepy/utils/amount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/calendar.py` & `financepy-0.290/financepy/utils/calendar.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/currency.py` & `financepy-0.290/financepy/utils/currency.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/date.py` & `financepy-0.290/financepy/utils/date.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/day_count.py` & `financepy-0.290/financepy/utils/day_count.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/distribution.py` & `financepy-0.290/financepy/utils/distribution.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/error.py` & `financepy-0.290/financepy/utils/error.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/frequency.py` & `financepy-0.290/financepy/utils/frequency.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/global_types.py` & `financepy-0.290/financepy/utils/global_types.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,27 +27,46 @@
     ASIAN_PUT = 8
     COMPOUND_CALL = 9
     COMPOUND_PUT = 10
 
 ###############################################################################
 
 
+class EquityBarrierTypes(Enum):
+    DOWN_AND_OUT_CALL = 1
+    DOWN_AND_IN_CALL = 2
+    UP_AND_OUT_CALL = 3
+    UP_AND_IN_CALL = 4
+    UP_AND_OUT_PUT = 5
+    UP_AND_IN_PUT = 6
+    DOWN_AND_OUT_PUT = 7
+    DOWN_AND_IN_PUT = 8
+
+###############################################################################
+
+
 class FinCapFloorTypes(Enum):
     CAP = 1
     FLOOR = 2
 
 ###############################################################################
 
 
 class SwapTypes(Enum):
     PAY = 1
     RECEIVE = 2
 
+
 ###############################################################################
 
+class ReturnTypes(Enum):
+    TOTAL_RETURN = 1
+    PRICE_RETURN = 2
+
+###############################################################################
 
 class FinExerciseTypes(Enum):
     EUROPEAN = 1
     BERMUDAN = 2
     AMERICAN = 3
 
 ###############################################################################
```

### Comparing `financepy-0.270/financepy/utils/helpers.py` & `financepy-0.290/financepy/utils/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
 ##############################################################################
 
 import sys
 import numpy as np
 from numba import njit, float64
 from typing import Union
+from prettytable import PrettyTable
+
 from .date import Date
 from .global_vars import gDaysInYear, gSmall
 from .error import FinError
 from .day_count import DayCountTypes, DayCount
 
 
 ###############################################################################
@@ -353,14 +355,37 @@
                 s += format(vList[i], floatPrecision) + ", "
             else:
                 s += str(vList[i]) + ", "
         s = s[:-2] + "\n"
 
     return s[:-1]
 
+###############################################################################
+
+
+def format_table(header: (list, tuple),
+                 rows: (list, tuple)):
+    """ Format a 2D array into a table-like string. 
+    Similar to "table_to_string", but using a wrapper
+    around PrettyTable to get a nice formatting. """
+    
+    t = PrettyTable(header)
+    numRows = len(header)
+
+    if len(rows) == 0:
+        print(len(rows))
+        return ""
+
+    for row in rows:
+        if len(row) != numRows:
+            raise ValueError("Header and Row Size must match!")
+
+        t.add_row(row)
+
+    return t
 
 ###############################################################################
 
 
 def to_usable_type(t):
     """ Convert a type such that it can be used with `isinstance` """
     if hasattr(t, '__origin__'):
@@ -471,16 +496,17 @@
 
 def check_argument_types(func, values):
     """ Check that all values passed into a function are of the same type
     as the function annotations. If a value has not been annotated, it
     will not be checked. """
     for valueName, annotationType in func.__annotations__.items():
 
-        value = values[valueName]
-        usableType = to_usable_type(annotationType)
+        if valueName in values:
+            value = values[valueName]
+            usableType = to_usable_type(annotationType)
         
         if (not isinstance(value, usableType)):
 
             print("ERROR with function arguments for", func.__name__)
             print("This is in module", func.__module__)
             print("Please check inputs for argument >>", valueName, "<<")
             print("You have input an argument", value, "of type", type(value))
```

### Comparing `financepy-0.270/financepy/utils/latex.py` & `financepy-0.290/financepy/utils/latex.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/math.py` & `financepy-0.290/financepy/utils/math.py`

 * *Files 3% similar despite different names*

```diff
@@ -660,7 +660,73 @@
     Function to calculate the npv given irr and cashflow. It can be used to do root search in IRR.
     times_cfs is a list of tuples. The tuple is in the form of (years from first date, cashflow)
     """
     _npv = 0
     for t, c in times_cfs:
         _npv += c / ((1 + irr) ** t)
     return _npv
+
+
+@njit(fastmath=True, cache=True)
+def band_matrix_multiplication(A, m1, m2, b):
+    n = A.shape[0]
+    x = np.zeros(n)
+
+    jl = np.arange(n) - m1
+    jl[jl < 0] = 0
+
+    ju = np.arange(n) + m2
+    ju[ju > n - 1] = n - 1
+
+    for i in range(n):
+        for j in range(jl[i], ju[i] + 1):
+            k = j - i + m1
+            x[i] += A[i, k] * b[j]
+
+    return x
+
+
+@njit(fastmath=True, cache=True)
+def solve_tridiagonal_matrix(A, r):
+    """
+    Solve A u = r for vector u when A is tridiagonal
+
+    The matrix A is split into vectors a, b, and c contain the three
+    non-zero elements of each row of A, in order.
+    i.e. the vector b is the main diagonal of A, with a and c the elements
+    either side of the main diagonal.
+
+    Note that a[0] and c[-1] are not used, and so can be any value.
+    """
+    a, b, c = A.T
+
+    if b[0] == 0:
+        raise ValueError("First entry is zero, rewrite as set of N-1 equations")
+
+    n = len(a)  # Length of output vector
+    u = np.zeros(n)  # Output vector
+    gam = np.zeros(n)  # Workspace
+
+    bet = b[0]
+    u[0] = r[0] / bet
+
+    for j in range(1, n):
+        gam[j] = c[j - 1] / bet
+        bet = b[j] - a[j] * gam[j]
+        if bet == 0:
+            raise ValueError(
+                "Variable bet should be non-zero. "
+                "Perhaps this algorithm is not suited to the problem"
+            )
+        u[j] = (r[j] - a[j] * u[j - 1]) / bet
+
+    for j in range(n - 2, -1, -1):
+        u[j] -= gam[j + 1] * u[j + 1]
+
+    return u
+
+
+@njit(fastmath=True, cache=True)
+def transpose_tridiagonal_matrix(A):
+    out = np.zeros_like(A)
+    out[:, 0], out[:, 1], out[:, 2] = A[:, 2], A[:, 1], A[:, 0]
+    return out
```

### Comparing `financepy-0.270/financepy/utils/polyfit.py` & `financepy-0.290/financepy/utils/polyfit.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/schedule.py` & `financepy-0.290/financepy/utils/schedule.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,32 +199,35 @@
         if self._adjusted_dates[0] < self._effective_date:
             self._adjusted_dates[0] = self._effective_date
 
         # The market standard for swaps is not to adjust the termination date
         # unless it is specified in the contract. It is standard for CDS.
         # We change it if the adjust_termination_date flag is True.
         if self._adjust_termination_date is True:
+
             self._termination_date = calendar.adjust(self._termination_date,
                                                      self._bus_day_adjust_type)
 
             self._adjusted_dates[-1] = self._termination_date
 
         #######################################################################
         # Check the resulting schedule to ensure that no two dates are the
-        # same and that they are monotonic - this should never happen but ...
+        # same in which case we remove the duplicate and that they are  
+        # monotonic - this should never happen but ...
         #######################################################################
 
         if len(self._adjusted_dates) < 2:
             raise FinError("Schedule has two dates only.")
 
         prev_dt = self._adjusted_dates[0]
         for dt in self._adjusted_dates[1:]:
 
+            # if the first date lands on the effective date then remove it
             if dt == prev_dt:
-                raise FinError("Two matching dates in schedule")
+                self._adjusted_dates.pop(0)
 
             if dt < prev_dt:  # Dates must be ordered
                 raise FinError("Dates are not monotonic")
 
             prev_dt = dt
 
         #######################################################################
```

### Comparing `financepy-0.270/financepy/utils/solver_1d.py` & `financepy-0.290/financepy/utils/solver_1d.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy/utils/solver_cg.py` & `financepy-0.290/financepy/utils/solver_cg.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
        quadratic function of the variables,
     3. `f` is continuous and has a continuous gradient,
     4. `fprime` is not too large, e.g., has a norm less than 1000,
     5. The initial guess, `x0`, is reasonably close to `f` 's global
        minimizing point, `xopt`.
     References
     ----------
-    .. [1] Wright & Nocedal, "Numerical Optimization", 1999, pp. 120-122.
+    .. [1] Wright and Nocedal, "Numerical Optimization", 1999, pp. 120-122.
     Examples
     --------
     Example 1: seek the minimum value of the expression
     ``a*u**2 + b*u*v + c*v**2 + d*u + e*v + f`` for given values
     of the parameters and an initial guess ``(u, v) = (0, 0)``.
     >>> args = (2, 3, 7, 8, 9, 10)  # parameter values
     >>> def f(x, *args):
```

### Comparing `financepy-0.270/financepy/utils/solver_nm.py` & `financepy-0.290/financepy/utils/solver_nm.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ###############################################################################
 
 from collections import namedtuple
 import numpy as np
 from numba import njit
 
 ###############################################################################
-## from https://quanteconpy.readthedocs.io/en/latest/_modules/quantecon/optimize/root_finding.html #####################
+# from https://quanteconpy.readthedocs.io/en/latest/_modules/quantecon/optimize/root_finding.html #####################
 
 _ECONVERGED = 0
 _ECONVERR = -1
 
 _iter = 100
 _xtol = 2e-12
 _rtol = 4*np.finfo(float).eps
@@ -202,15 +202,15 @@
             if f_e < f_r:  # Greedy minimization
                 vertices[worst_val_idx] = x_e
                 LV_ratio *= rohchi
             else:
                 vertices[worst_val_idx] = x_r
                 LV_ratio *= roh
 
-        # Step 4 & 5: Contraction and Shrink
+        # Step 4 and 5: Contraction and Shrink
         else:
             # Step 4: Contraction
             # https://github.com/QuantEcon/QuantEcon.py/issues/530
             temp = v * (x_r - x_bar)
             if f_r < f_val[worst_val_idx]:  # Step 4.a: Outside Contraction
                 x_c = x_bar + temp
                 LV_ratio_update = rohv
```

### Comparing `financepy-0.270/financepy/utils/stats.py` & `financepy-0.290/financepy/utils/stats.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/financepy.egg-info/PKG-INFO` & `financepy-0.290/financepy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: financepy
-Version: 0.270
+Version: 0.290
 Summary: A Finance Securities Valuation Library
 Home-page: https://github.com/domokane/FinancePy
 Author: Dominic O'Kane
 Author-email: dominic.okane@edhec.edu
-License: UNKNOWN
 Keywords: FINANCE,OPTIONS,BONDS,VALUATION,DERIVATIVES
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![unit test action](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml/badge.svg)](https://github.com/ru-corporate/FinancePy/actions/workflows/run-unit-tests.yml)
-
-![alt text](./images/logo.jpg?raw=true)
-
 # Latest News and Versions
 
 22 Nov 22
 Version 0.260 has been released and pushed to PyPI
 - Create Date from python datetime
 - Zero coupon bond class
 - Fixed bug in bond payment date
@@ -31,15 +25,15 @@
 31-Aug-2022
 Version 0.240 has just been released and pushed to PyPI with changes
 - Negative terms in date class
 - Recovery rates do not default to standard value for CDS curves 
 
 # DISCLAIMER
 
-This software is distributed FREE & WITHOUT ANY WARRANTY. 
+This software is distributed FREE AND WITHOUT ANY WARRANTY. 
 
 Report any bugs or suggestions here as an issue. 
 
 # CONTRIBUTORS WANTED !
 
 If you have a knowledge of Quantitative Finance and a reasonable knowledge of Python, then please consider contributing to this project. There are small tasks and big tasks to be done. Just look in the list of Issues and you may find something you can do. Before you begin, please comment in the issue thread in case someone else may be working on that issue. Or you can contact me directly at dominic.okane at edhec.edu. 
 
@@ -139,9 +133,7 @@
 * Comments are required for every class and function and they should be a clear description.
 * At least one broad test case and a set of unit tests must be provided for every function.
 * Avoid very pythonic constructions. For example a loop is as good as a list comprehension. And with numba it can be faster. Readability is the priority.
 
 ## License
 
  GPL-3.0 License - See the license file in this folder for details.
-
-
```

### Comparing `financepy-0.270/financepy.egg-info/SOURCES.txt` & `financepy-0.290/financepy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,19 @@
 financepy/models/black_scholes.py
 financepy/models/black_scholes_analytic.py
 financepy/models/black_scholes_mc.py
 financepy/models/black_scholes_mc_tests.py
 financepy/models/black_shifted.py
 financepy/models/bond_analytics.py
 financepy/models/cir_mc.py
+financepy/models/equity_barrier_models.py
 financepy/models/equity_crr_tree.py
 financepy/models/equity_lsmc.py
+financepy/models/finite_difference.py
+financepy/models/finite_difference_PSOR.py
 financepy/models/gauss_copula.py
 financepy/models/gauss_copula_lhp.py
 financepy/models/gauss_copula_lhplus.py
 financepy/models/gauss_copula_onefactor.py
 financepy/models/gbm_process_simulator.py
 financepy/models/heston.py
 financepy/models/hw_tree.py
@@ -96,18 +99,21 @@
 financepy/products/equity/equity_chooser_option.py
 financepy/products/equity/equity_cliquet_option.py
 financepy/products/equity/equity_compound_option.py
 financepy/products/equity/equity_digital_option.py
 financepy/products/equity/equity_fixed_lookback_option.py
 financepy/products/equity/equity_float_lookback_option.py
 financepy/products/equity/equity_forward.py
+financepy/products/equity/equity_index_option.py
 financepy/products/equity/equity_model_types.py
 financepy/products/equity/equity_one_touch_option.py
 financepy/products/equity/equity_option.py
 financepy/products/equity/equity_rainbow_option.py
+financepy/products/equity/equity_swap.py
+financepy/products/equity/equity_swap_leg.py
 financepy/products/equity/equity_vanilla_option.py
 financepy/products/equity/equity_variance_swap.py
 financepy/products/fx/__init__.py
 financepy/products/fx/fx_barrier_option.py
 financepy/products/fx/fx_digital_option.py
 financepy/products/fx/fx_fixed_lookback_option.py
 financepy/products/fx/fx_float_lookback_option.py
@@ -211,14 +217,15 @@
 tests_golden/TestFinEquityCliquetOption.py
 tests_golden/TestFinEquityCompoundOption.py
 tests_golden/TestFinEquityDigitalOption.py
 tests_golden/TestFinEquityForward.py
 tests_golden/TestFinEquityLookbackOption.py
 tests_golden/TestFinEquityOneTouchOption.py
 tests_golden/TestFinEquityRainbowOption.py
+tests_golden/TestFinEquitySwap.py
 tests_golden/TestFinEquityVanillaOption.py
 tests_golden/TestFinEquityVarianceSwap.py
 tests_golden/TestFinEquityVolSurface.py
 tests_golden/TestFinFXAmericanOption.py
 tests_golden/TestFinFXBarrierOption.py
 tests_golden/TestFinFXDigitalOption.py
 tests_golden/TestFinFXForward.py
```

### Comparing `financepy-0.270/setup.py` & `financepy-0.290/setup.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/FinTestCases.py` & `financepy-0.290/tests_golden/FinTestCases.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinAmount.py` & `financepy-0.290/tests_golden/TestFinAmount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBond.py` & `financepy-0.290/tests_golden/TestFinBond.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 from financepy.utils.frequency import FrequencyTypes
 from financepy.utils.day_count import DayCountTypes
 from financepy.utils.date import Date, from_datetime
 from financepy.utils.math import ONE_MILLION
 from financepy.products.rates.ibor_swap import IborSwap
 from financepy.products.rates.ibor_deposit import IborDeposit
 from financepy.products.rates.ibor_single_curve import IborSingleCurve
+from financepy.products.bonds.bond_market import *
 from financepy.products.bonds.bond import YTMCalcType, Bond
 from financepy.utils.global_types import SwapTypes
+
 import os
 import datetime as dt
 import pandas as pd
-
+import numpy as np
 
 
 testCases = FinTestCases(__file__, globalTestCaseMode)
 
 
 ##########################################################################
 
@@ -572,23 +574,86 @@
     coupon = 0.045
     freq_type = FrequencyTypes.SEMI_ANNUAL
     accrual_type = DayCountTypes.ACT_ACT_ICMA
     face = ONE_MILLION
 
     bond = Bond(issue_date, maturity_date, coupon, freq_type, accrual_type, face)
 
-#    print(bond.coupon_dates(settle_date))
-
-    ai = bond.calc_accrued_interest(settle_date)
-    print(ai)
-    # should be 8406.59
+    ai = bond.calc_accrued_interest(settle_date) # should be 8406.593406
     
 ###############################################################################
+
+def test_key_rate_durations():
+
+#    print("Complete test case logging")
+
+    issue_date = Date(31, 7, 2022)
+    maturity_date = Date(31, 7, 2027)
+    coupon = 0.0275
+    face = 100.0
+
+    accrual_type, freq_type, settlementDays, exDiv, calendar = get_bond_market_conventions(
+    BondMarkets.UNITED_STATES)
+
+    bond = Bond(issue_date, maturity_date, coupon,
+                freq_type, accrual_type, face)
+
+    settlement_date = Date(24, 4, 2023)
+
+    ytm = 3.725060/100
+
+    key_rate_tenors, key_rate_durations = bond.key_rate_durations(
+        settlement_date, ytm)
+
+#    print(key_rate_tenors)
+#    print(key_rate_durations)
+
+################################################################################
+
+def test_key_rate_durations_Bloomberg_example():
+
+    accrual_type, frequencyType, settlementDays, exDiv, calendar = \
+    get_bond_market_conventions(BondMarkets.UNITED_STATES)
+
+    # interest accrues on this date. Issue date is 01/08/2022
+    issue_date = Date(31, 7, 2022)
+    maturity_date = Date(31, 7, 2027)
+    coupon = 2.75/100.0
+    face = 100.0
+
+    accrual_type, freq_type, settlementDays, exDiv, calendar = get_bond_market_conventions(
+    BondMarkets.UNITED_STATES)
+
+    bond = Bond(issue_date, maturity_date, coupon,
+                freq_type, accrual_type, face)
+
+    settlement_date = Date(24, 4, 2023)
+
+    # US Street yield on Bloomberg as of 20 April 2023
+    # with settle date 24 April 2023
+    ytm = 3.725060/100
     
+    # Details of yields of market bonds at KRD maturity points
+    my_tenors = np.array([0.5,  1,  2,  3,  5,  7,  10])
+    my_rates = np.array([5.0367, 4.7327, 4.1445, 3.8575, 3.6272,  3.5825,  3.5347])/100
+
+    key_rate_tenors, key_rate_durations = bond.key_rate_durations(settlement_date, 
+                                                                  ytm, 
+                                                                  key_rate_tenors = my_tenors, 
+                                                                  rates = my_rates)
+
+#    print(key_rate_tenors)
+#    print(key_rate_durations)
+
+    # Differences due to bonds not sitting exactly on these maturity points ? Did BBG interpolate ?
+
+###############################################################################
+
 test_Bond()
 test_BondExDividend()
 test_BondPaymentDates()
 test_Bond_ror()
 test_Bond_eom()
-
+test_key_rate_durations()
+test_key_rate_durations_Bloomberg_example()
 
 testCases.compareTestCases()
```

### Comparing `financepy-0.270/tests_golden/TestFinBondAnnuity.py` & `financepy-0.290/tests_golden/TestFinBondAnnuity.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondConvertible.py` & `financepy-0.290/tests_golden/TestFinBondConvertible.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondEmbeddedOptionBK.py` & `financepy-0.290/tests_golden/TestFinBondEmbeddedOptionBK.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondEmbeddedOptionHW.py` & `financepy-0.290/tests_golden/TestFinBondEmbeddedOptionHW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondFRN.py` & `financepy-0.290/tests_golden/TestFinBondFRN.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondFutures.py` & `financepy-0.290/tests_golden/TestFinBondFutures.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondMortgage.py` & `financepy-0.290/tests_golden/TestFinBondMortgage.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondOptionBDTModel.py` & `financepy-0.290/tests_golden/TestFinBondOptionBDTModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondOptionBKModel.py` & `financepy-0.290/tests_golden/TestFinBondOptionBKModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondOptionHWModel.py` & `financepy-0.290/tests_golden/TestFinBondOptionHWModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondPortfolio.py` & `financepy-0.290/tests_golden/TestFinBondPortfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondYieldCurve.py` & `financepy-0.290/tests_golden/TestFinBondYieldCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondZeroCoupon.py` & `financepy-0.290/tests_golden/TestFinBondZeroCoupon.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinBondZeroCurve.py` & `financepy-0.290/tests_golden/TestFinBondZeroCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDS.py` & `financepy-0.290/tests_golden/TestFinCDS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSBasket.py` & `financepy-0.290/tests_golden/TestFinCDSBasket.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSCurve.py` & `financepy-0.290/tests_golden/TestFinCDSCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSIndex.py` & `financepy-0.290/tests_golden/TestFinCDSIndex.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSIndexAdjustHazards.py` & `financepy-0.290/tests_golden/TestFinCDSIndexAdjustHazards.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSIndexAdjustSpreads.py` & `financepy-0.290/tests_golden/TestFinCDSIndexAdjustSpreads.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSIndexOption.py` & `financepy-0.290/tests_golden/TestFinCDSIndexOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSIndexPortfolio.py` & `financepy-0.290/tests_golden/TestFinCDSIndexPortfolio.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSOption.py` & `financepy-0.290/tests_golden/TestFinCDSOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCDSTranche.py` & `financepy-0.290/tests_golden/TestFinCDSTranche.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinCalendar.py` & `financepy-0.290/tests_golden/TestFinCalendar.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDate.py` & `financepy-0.290/tests_golden/TestFinDate.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDateAdjust.py` & `financepy-0.290/tests_golden/TestFinDateAdjust.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDayCount.py` & `financepy-0.290/tests_golden/TestFinDayCount.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurve.py` & `financepy-0.290/tests_golden/TestFinDiscountCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurveFlat.py` & `financepy-0.290/tests_golden/TestFinDiscountCurveFlat.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurveNS.py` & `financepy-0.290/tests_golden/TestFinDiscountCurveNS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurveNSS.py` & `financepy-0.290/tests_golden/TestFinDiscountCurveNSS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurvePolynomial.py` & `financepy-0.290/tests_golden/TestFinDiscountCurvePolynomial.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurveZeros.py` & `financepy-0.290/tests_golden/TestFinDiscountCurveZeros.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinDiscountCurves.py` & `financepy-0.290/tests_golden/TestFinDiscountCurves.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityAmericanMC.py` & `financepy-0.290/tests_golden/TestFinEquityAmericanMC.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityAmericanOption.py` & `financepy-0.290/tests_golden/TestFinEquityAmericanOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityAsianOption.py` & `financepy-0.290/tests_golden/TestFinEquityAsianOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityBarrierOption.py` & `financepy-0.290/tests_golden/TestFinEquityBarrierOption.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 ###############################################################################
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
 ###############################################################################
 
 import sys
 sys.path.append("..")
 
+from FinTestCases import FinTestCases, globalTestCaseMode
+
+from financepy.utils.date import Date
+
+from financepy.models.black_scholes import BlackScholes
 from financepy.models.process_simulator import ProcessTypes
 from financepy.models.process_simulator import FinGBMNumericalScheme
+
 from financepy.products.equity.equity_barrier_option import EquityBarrierTypes
 from financepy.products.equity.equity_barrier_option import EquityBarrierOption
-from financepy.models.black_scholes import BlackScholes
 from financepy.market.curves.discount_curve_flat import DiscountCurveFlat
-from financepy.utils.date import Date
-from FinTestCases import FinTestCases, globalTestCaseMode
-
 
 testCases = FinTestCases(__file__, globalTestCaseMode)
 
 ###############################################################################
 
 
 def test_EquityBarrierOption():
@@ -25,14 +27,15 @@
     valuation_date = Date(1, 1, 2015)
     expiry_date = Date(1, 1, 2016)
     stock_price = 100.0
     volatility = 0.20
     interest_rate = 0.05
     dividend_yield = 0.02
     option_type = EquityBarrierTypes.DOWN_AND_OUT_CALL
+    notional = 1.0
 
     drift = interest_rate - dividend_yield
     scheme = FinGBMNumericalScheme.NORMAL
     process_type = ProcessTypes.GBM
 
     discount_curve = DiscountCurveFlat(valuation_date, interest_rate)
     dividend_curve = DiscountCurveFlat(valuation_date, dividend_yield)
@@ -57,42 +60,51 @@
 
     for option_type in EquityBarrierTypes:
         for stock_price in [80, 100, 120]:
 
             B = 110.0
             K = 100.0
 
-            option = EquityBarrierOption(
-                expiry_date, K, option_type, B, num_observations_per_year)
-            value = option.value(
-                valuation_date,
-                stock_price,
-                discount_curve,
-                dividend_curve,
-                model)
+            option = EquityBarrierOption(expiry_date, 
+                                         K, 
+                                         option_type, 
+                                         B, 
+                                         num_observations_per_year)
+
+            value = option.value(valuation_date,
+                                 stock_price,
+                                 discount_curve,
+                                 dividend_curve,
+                                 model)
+            
             start = time.time()
             model_params = (stock_price, drift, volatility, scheme)
-            value_mc = option.value_mc(valuation_date,
-                                       stock_price,
-                                       discount_curve,
-                                       dividend_curve,
-                                       process_type,
-                                       model_params)
+
+            test_value_mc = option.value_mc(expiry_date, 
+                                     K, 
+                                     option_type.value, 
+                                     B, 
+                                     notional, 
+                                     valuation_date, 
+                                     stock_price,
+                                     discount_curve.cc_rate(expiry_date), 
+                                     process_type, 
+                                     model_params)
 
             end = time.time()
             time_elapsed = round(end - start, 3)
-            diff = value_mc - value
+            diff = test_value_mc - value
 
             testCases.print(
                 option_type,
                 K,
                 B,
                 stock_price,
                 value,
-                value_mc,
+                test_value_mc,
                 diff,
                 time_elapsed)
 
         for stock_price in [80, 100, 120]:
 
             B = 100.0
             K = 110.0
@@ -103,32 +115,37 @@
                 valuation_date,
                 stock_price,
                 discount_curve,
                 dividend_curve,
                 model)
             start = time.time()
             model_params = (stock_price, drift, volatility, scheme)
-            value_mc = option.value_mc(
-                valuation_date,
-                stock_price,
-                discount_curve,
-                dividend_curve,
-                process_type,
-                model_params)
+
+            test_value_mc = option.value_mc(expiry_date, 
+                                     K, 
+                                     option_type.value, 
+                                     B, 
+                                     notional, 
+                                     valuation_date, 
+                                     stock_price,
+                                     discount_curve.cc_rate(expiry_date), 
+                                     process_type, 
+                                     model_params)
+
             end = time.time()
             time_elapsed = round(end - start, 3)
-            diff = value_mc - value
+            diff = test_value_mc - value
 
             testCases.print(
                 option_type,
                 K,
                 B,
                 stock_price,
                 value,
-                value_mc,
+                test_value_mc,
                 diff,
                 time_elapsed)
 
         end = time.time()
 
 ##########################################################################
```

### Comparing `financepy-0.270/tests_golden/TestFinEquityBasketOption.py` & `financepy-0.290/tests_golden/TestFinEquityBasketOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityBinomialTree.py` & `financepy-0.290/tests_golden/TestFinEquityBinomialTree.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityChooserOption.py` & `financepy-0.290/tests_golden/TestFinEquityChooserOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityCliquetOption.py` & `financepy-0.290/tests_golden/TestFinEquityCliquetOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityCompoundOption.py` & `financepy-0.290/tests_golden/TestFinEquityCompoundOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityDigitalOption.py` & `financepy-0.290/tests_golden/TestFinEquityDigitalOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityForward.py` & `financepy-0.290/tests_golden/TestFinEquityForward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityLookbackOption.py` & `financepy-0.290/tests_golden/TestFinEquityLookbackOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityOneTouchOption.py` & `financepy-0.290/tests_golden/TestFinEquityOneTouchOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityRainbowOption.py` & `financepy-0.290/tests_golden/TestFinEquityRainbowOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityVanillaOption.py` & `financepy-0.290/tests_golden/TestFinEquityVanillaOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityVarianceSwap.py` & `financepy-0.290/tests_golden/TestFinEquityVarianceSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinEquityVolSurface.py` & `financepy-0.290/tests_golden/TestFinEquityVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXAmericanOption.py` & `financepy-0.290/tests_golden/TestFinFXAmericanOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXBarrierOption.py` & `financepy-0.290/tests_golden/TestFinFXBarrierOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXDigitalOption.py` & `financepy-0.290/tests_golden/TestFinFXDigitalOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXForward.py` & `financepy-0.290/tests_golden/TestFinFXForward.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXLookbackOption.py` & `financepy-0.290/tests_golden/TestFinFXLookbackOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXOneTouchOption.py` & `financepy-0.290/tests_golden/TestFinFXOneTouchOption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXOptionSABR.py` & `financepy-0.290/tests_golden/TestFinFXOptionSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXVanillaOption.py` & `financepy-0.290/tests_golden/TestFinFXVanillaOption.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from financepy.utils.date import Date
 from financepy.products.rates.ibor_deposit import IborDeposit
 from financepy.products.rates.ibor_single_curve import IborSingleCurve
 from financepy.utils.calendar import CalendarTypes
 from financepy.utils.day_count import DayCountTypes
 from financepy.market.curves.discount_curve_flat import DiscountCurveFlat
 from financepy.models.black_scholes import BlackScholes
+from financepy.models.sabr import SABR
 from financepy.products.fx.fx_vanilla_option import FXVanillaOption
 from financepy.utils.global_types import OptionTypes
 import time
 import numpy as np
 import sys
 sys.path.append("..")
 
@@ -462,13 +463,54 @@
                                                     for_discount_curve,
                                                     value)
 
         testCases.print(spot_fx_rate, value, volatility, impliedVol)
 
 ###############################################################################
 
+def test_FinFXVanillaOptionSABRExample():
+    """
+    Test case for FXVanilla option pricing with SABR model
+    """
+    # define option
+    valuation_date = Date(5, 4, 2023)
+    forName = "USD"
+    domName = "JPY"
+    forCCRate = 0.0381  # USD
+    domCCRate = 0.000396 # JPY
+    dom_discount_curve = DiscountCurveFlat(valuation_date, domCCRate)
+    for_discount_curve = DiscountCurveFlat(valuation_date, forCCRate)
+    currency_pair = forName + domName
+    spot_fx_rate = 131.32
+    strike_price = 130
+    expiry_date = valuation_date.add_tenor("10M")
+    notional = 70000000
+    
+    call_option = FXVanillaOption(expiry_date, 
+                                  strike_price, 
+                                  currency_pair, 
+                                  OptionTypes.EUROPEAN_CALL, 
+                                  notional, "USD")
+    
+    volatility = 0.1043
+    # set the params of SABR
+    alpha = 0.174; beta = 0.5; rho = -0.50; nu = 0.5
+    model = SABR(alpha,beta,rho,nu)
+    blackVol = volatility
+    texp = 0.8444 #10M
+    model.set_alpha_from_black_vol(blackVol,spot_fx_rate,strike_price, texp)
+    
+    spot_fx_rate = np.linspace(80,300,1000)
+    callValue = [call_option.value(valuation_date,f,dom_discount_curve,for_discount_curve,model)['cash_dom'] for f in spot_fx_rate]
+
+    testCases.header("spot fx rate", "value")
+    testCases.print(spot_fx_rate,callValue)
+    
+###############################################################################
+
 
 test_FinFXVanillaOptionWystupExample1()
 test_FinFXVanillaOptionWystupExample2()
 test_FinFXVanillaOptionBloombergExample()
 test_FinFXVanillaOptionHullExample()
+test_FinFXVanillaOptionSABRExample()
 testCases.compareTestCases()
```

### Comparing `financepy-0.270/tests_golden/TestFinFXVolSurface.py` & `financepy-0.290/tests_golden/TestFinFXVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinFXVolSurfacePlus.py` & `financepy-0.290/tests_golden/TestFinFXVolSurfacePlus.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborBermudanSwaption.py` & `financepy-0.290/tests_golden/TestFinIborBermudanSwaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborCapFloor.py` & `financepy-0.290/tests_golden/TestFinIborCapFloor.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborCapVolCurve.py` & `financepy-0.290/tests_golden/TestFinIborCapVolCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborDualCurve.py` & `financepy-0.290/tests_golden/TestFinIborDualCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborFuture.py` & `financepy-0.290/tests_golden/TestFinIborFuture.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborLMMProducts.py` & `financepy-0.290/tests_golden/TestFinIborLMMProducts.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborSingleCurve.py` & `financepy-0.290/tests_golden/TestFinIborSingleCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborSwap.py` & `financepy-0.290/tests_golden/TestFinIborSwap.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinIborSwaption.py` & `financepy-0.290/tests_golden/TestFinIborSwaption.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinInflationBond.py` & `financepy-0.290/tests_golden/TestFinInflationBond.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinInflationIndexCurve.py` & `financepy-0.290/tests_golden/TestFinInflationIndexCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinInterpolate.py` & `financepy-0.290/tests_golden/TestFinInterpolate.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinInterpolatedForwards.py` & `financepy-0.290/tests_golden/TestFinInterpolatedForwards.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinLossDbnBuilder.py` & `financepy-0.290/tests_golden/TestFinLossDbnBuilder.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinMath.py` & `financepy-0.290/tests_golden/TestFinMath.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinMathAccruedInterp.py` & `financepy-0.290/tests_golden/TestFinMathAccruedInterp.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelBlack.py` & `financepy-0.290/tests_golden/TestFinModelBlack.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelBlackScholes.py` & `financepy-0.290/tests_golden/TestFinModelBlackScholes.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelBlack_SABR_HW.py` & `financepy-0.290/tests_golden/TestFinModelBlack_SABR_HW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelCIR.py` & `financepy-0.290/tests_golden/TestFinModelCIR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelHeston.py` & `financepy-0.290/tests_golden/TestFinModelHeston.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelMerton.py` & `financepy-0.290/tests_golden/TestFinModelMerton.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelRatesBDT.py` & `financepy-0.290/tests_golden/TestFinModelRatesBDT.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelRatesBK.py` & `financepy-0.290/tests_golden/TestFinModelRatesBK.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelRatesHW.py` & `financepy-0.290/tests_golden/TestFinModelRatesHW.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelRatesLMM.py` & `financepy-0.290/tests_golden/TestFinModelRatesLMM.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelSABR.py` & `financepy-0.290/tests_golden/TestFinModelSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinModelShiftedSABR.py` & `financepy-0.290/tests_golden/TestFinModelShiftedSABR.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinNumbaNumpySpeed.py` & `financepy-0.290/tests_golden/TestFinNumbaNumpySpeed.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinOIS.py` & `financepy-0.290/tests_golden/TestFinOIS.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinOISCurve.py` & `financepy-0.290/tests_golden/TestFinOISCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinOptionImpliedDbn.py` & `financepy-0.290/tests_golden/TestFinOptionImpliedDbn.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinPieceCurve.py` & `financepy-0.290/tests_golden/TestFinPieceCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinProcessSimulator.py` & `financepy-0.290/tests_golden/TestFinProcessSimulator.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinSchedule.py` & `financepy-0.290/tests_golden/TestFinSchedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ###############################################################################
 # Copyright (C) 2018, 2019, 2020 Dominic O'Kane
 ###############################################################################
 
+import sys
+sys.path.append("..")
+
+from FinTestCases import FinTestCases, globalTestCaseMode
 from financepy.utils.calendar import BusDayAdjustTypes
 from financepy.utils.calendar import DateGenRuleTypes
 from financepy.utils.schedule import Schedule
 from financepy.utils.frequency import FrequencyTypes
 from financepy.utils.calendar import CalendarTypes, Calendar
 from financepy.utils.date import Date, set_date_format, DateFormatTypes
-from FinTestCases import FinTestCases, globalTestCaseMode
-import sys
-sys.path.append("..")
-
 
 testCases = FinTestCases(__file__, globalTestCaseMode)
 
 ###############################################################################
 
 set_date_format(DateFormatTypes.UK_LONGEST)
 
@@ -107,14 +107,15 @@
                         calendar_type,
                         bus_day_adjust_type,
                         date_gen_rule_type,
                         termination_dateAdjust)
 
     dumpSchedule("BACKWARD MONTHLY FREQUENCY", schedule)
 
+
     ###########################################################################
     # FORWARD SCHEDULES TESTING DIFFERENT FREQUENCIES
     ###########################################################################
 
     d1 = Date(20, 6, 2018)
     d2 = Date(20, 6, 2020)
     freq_type = FrequencyTypes.ANNUAL
@@ -297,14 +298,25 @@
                         bus_day_adjust_type,
                         date_gen_rule_type,
                         termination_dateAdjust,
                         eomFlag)
 
     dumpSchedule("END OF MONTH - EOM TERM DATE - USING MOD FOLL", schedule)
 
+    # PROBLEM WITH THIS ONE AS DATES COLLIDE BUT REMOVE FIRST ONE
+    schedule = Schedule(Date(28, 4, 2023),
+                        Date(30, 4, 2024),
+                        FrequencyTypes.ANNUAL,
+                        CalendarTypes.UNITED_STATES,
+                        BusDayAdjustTypes.MODIFIED_FOLLOWING,
+                        DateGenRuleTypes.BACKWARD)
+    
+#    print(schedule)
+#    print(schedule._adjusted_dates)
+    
 ###############################################################################
 
 
 def test_FinScheduleAlignment(eomFlag):
 
     valuation_date = Date(29, 3, 2005)
     effDate = valuation_date.add_tenor("2d")
```

### Comparing `financepy-0.270/tests_golden/TestFinSobol.py` & `financepy-0.290/tests_golden/TestFinSobol.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinStatistics.py` & `financepy-0.290/tests_golden/TestFinStatistics.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinSwapLegs.py` & `financepy-0.290/tests_golden/TestFinSwapLegs.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinSwaptionVolSurface.py` & `financepy-0.290/tests_golden/TestFinSwaptionVolSurface.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinVasicekRateModel.py` & `financepy-0.290/tests_golden/TestFinVasicekRateModel.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/TestFinVolatilityCurve.py` & `financepy-0.290/tests_golden/TestFinVolatilityCurve.py`

 * *Files identical despite different names*

### Comparing `financepy-0.270/tests_golden/runAllTests.py` & `financepy-0.290/tests_golden/runAllTests.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 sys.path.append("./..")
 
 from os.path import dirname, basename, join
 import glob
 from financepy.utils.error import FinError
 from financepy.utils.date import set_date_format, DateFormatTypes
 
-
 # This only works if I have an init.py in the parent folder
 
-
 set_date_format(DateFormatTypes.UK_LONG)
 
 # I put this here to get the library loaded and header printed before loop
 
 print("Looking in folder:", dirname(__file__))
 modules = sorted(glob.glob(join(dirname(__file__), "Test*.py")))
 numModules = len(modules)
```

