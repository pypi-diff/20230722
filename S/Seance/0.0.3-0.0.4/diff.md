# Comparing `tmp/Seance-0.0.3-py3-none-any.whl.zip` & `tmp/Seance-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 15469 bytes, number of entries: 16
+Zip file size: 15513 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat     2360 b- defN 23-Jun-21 13:29 Seance/Explainer.py
--rw-rw-rw-  2.0 fat    11991 b- defN 23-Jul-07 01:46 Seance/Forecaster.py
--rw-rw-rw-  2.0 fat    10054 b- defN 23-Jul-06 14:42 Seance/Optimizer.py
+-rw-rw-rw-  2.0 fat    11987 b- defN 23-Jul-22 12:20 Seance/Forecaster.py
+-rw-rw-rw-  2.0 fat    10533 b- defN 23-Jul-22 03:43 Seance/Optimizer.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:41 Seance/__init__.py
 -rw-rw-rw-  2.0 fat     3358 b- defN 23-May-18 13:18 Seance/Builder/PanelAxis.py
 -rw-rw-rw-  2.0 fat     3916 b- defN 23-Jul-06 20:13 Seance/Builder/PreProcess.py
 -rw-rw-rw-  2.0 fat     6595 b- defN 23-May-31 15:17 Seance/Builder/Transformations.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-May-04 14:40 Seance/Builder/__init__.py
 -rw-rw-rw-  2.0 fat       27 b- defN 23-Jun-03 01:07 Seance/basis_functions/__init__.py
 -rw-rw-rw-  2.0 fat      845 b- defN 23-Jul-06 19:45 Seance/basis_functions/fourier_basis.py
 -rw-rw-rw-  2.0 fat     2834 b- defN 23-May-31 21:10 Seance/basis_functions/linear_basis.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2684 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-07 01:48 Seance-0.0.3.dist-info/RECORD
-16 files, 47207 bytes uncompressed, 13321 bytes compressed:  71.8%
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2725 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1303 b- defN 23-Jul-22 12:22 Seance-0.0.4.dist-info/RECORD
+16 files, 47723 bytes uncompressed, 13365 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: Seance/basis_functions/fourier_basis.py
 Comment: 
 
 Filename: Seance/basis_functions/linear_basis.py
 Comment: 
 
-Filename: Seance-0.0.3.dist-info/LICENSE
+Filename: Seance-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: Seance-0.0.3.dist-info/METADATA
+Filename: Seance-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: Seance-0.0.3.dist-info/WHEEL
+Filename: Seance-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: Seance-0.0.3.dist-info/top_level.txt
+Filename: Seance-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: Seance-0.0.3.dist-info/RECORD
+Filename: Seance-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Seance/Forecaster.py

```diff
@@ -244,9 +244,7 @@
         return predicted
 
     def plot_importance(self, max_num_features=20):
         lgb.plot_importance(self.mlforecast.models_['LGBMRegressor'],
                             max_num_features=max_num_features)
         return
 
-
-
```

## Seance/Optimizer.py

```diff
@@ -29,17 +29,17 @@
                  metric='mse',
                  seasonal_period=0,
                  n_folds=1, #TODO
                  n_trials=100,
                  max_n_estimators=500,
                  ar_lags=None,
                  scale_types=['log','standard','minmax','robust_boxcox','none'],
-                 min_bagging_pct=.1,
+                 min_bagging_pct=.6,
                  max_bagging_pct=1.0,
-                 min_feature_fraction=.1,
+                 min_feature_fraction=.6,
                  max_n_basis=25,
                  timeout=None):
         self.df = df.sort_values([id_column, date_column])
         if isinstance(seasonal_period, list):
             self.max_pulse = max(seasonal_period)
         else:
             self.max_pulse = seasonal_period
@@ -79,42 +79,42 @@
         self.train_df = df[df['test_split'] == False]
         # self.train_df[self.date_column] = pd.to_datetime(self.train_df[self.date_column]).dt.
         self.test_df = df[df['test_split'] == True]
 
     def scorer(self, params, metric):
         scores = []
         # for train_index, test_index in cv_splits:
-        # try:
-        print(params)
-        model_obj = Forecaster()
-        model_obj.fit(self.train_df,
-                      target_column=self.target_column,
-                      date_column=self.date_column,
-                      id_column=self.id_column,
-                      freq=self.freq,
-                      categorical_columns=self.categorical_columns,
-                      **params)
-        predicted = model_obj.predict(self.test_size)
-        self.predicted = predicted
-        if len(predicted) != len(self.test_df):
-            print('Predicted not the same size as test set')
-
-        if any(np.isnan(predicted['LGBMRegressor'])):
-            scores.append(np.inf)
-        else:
-            # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
-            self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
-            self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
-            if metric == 'mse':
-                scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
-            elif metric == 'smape':
-                scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
-        # except Exception as e:
-        #         scores.append(np.inf)
-        #         print(f'ERROR WHILE TUNING: {e}')
+        try:
+            # print(params)
+            model_obj = Forecaster()
+            model_obj.fit(self.train_df,
+                          target_column=self.target_column,
+                          date_column=self.date_column,
+                          id_column=self.id_column,
+                          freq=self.freq,
+                          categorical_columns=self.categorical_columns,
+                          **params)
+            predicted = model_obj.predict(self.test_size)
+            self.predicted = predicted
+            if len(predicted) != len(self.test_df):
+                print('Predicted not the same size as test set')
+    
+            if any(np.isnan(predicted['LGBMRegressor'])):
+                scores.append(np.inf)
+            else:
+                # predicted[self.date_column] = predicted[self.date_column].dt.tz_localize(None)
+                self.test_df[self.date_column] = self.test_df[self.date_column].dt.tz_localize(None)
+                self.cv_df = self.test_df[[self.id_column, self.date_column, self.target_column]].merge(predicted, on=[self.id_column, self.date_column])
+                if metric == 'mse':
+                    scores.append(mean_squared_error(self.cv_df[self.target_column].values, self.cv_df['LGBMRegressor'].values))
+                elif metric == 'smape':
+                    scores.append(self.cv_df.groupby(self.id_column).apply(grouped_smape, self.target_column))
+        except Exception as e:
+                scores.append(np.inf)
+                print(f'ERROR WHILE TUNING: {e}')
         return np.mean(scores)
 
 
     def objective(self, trial):
         params = {
             "n_estimators": trial.suggest_int(name="n_estimators", low=50, high=self.max_n_estimators),
             'lambda_l1': trial.suggest_float('lambda_l1', 1e-8, 10.0),
@@ -164,24 +164,35 @@
         else:
             best_params.update({'lags': list(range(1, best_params['lags']))})
         return best_params, study
 
 #%%
 if __name__ == '__main__':
     import matplotlib.pyplot as plt
+    # opt = Optimize(train_df[['V', 'Datetime', 'ID']],
+    #             target_column='V',
+    #             date_column='Datetime',
+    #             id_column='ID',
+    #             freq='H',
+    #             metric='smape',
+    #             seasonal_period=24,
+    #             test_size=72,
+    #             n_trials=50)
+    # best_params, study = opt.fit(seed=1)
+
     opt = Optimize(train_df[['V', 'Datetime', 'ID']],
                 target_column='V',
                 date_column='Datetime',
                 id_column='ID',
                 freq='W',
-                seasonal_period=52,
+                metric='smape',
+                seasonal_period=[52],
                 test_size=26,
-                ar_lags=[list(range(1, 53))],
-                n_trials=3)
-    study = opt.fit(seed=1)
+                n_trials=50)
+    best_params, study = opt.fit(seed=1)
 
     look = opt.test_df
     look2 = opt.predicted
     merged = opt.test_df.merge(opt.predicted, on=['ID', 'Datetime'])
     optuna.visualization.matplotlib.plot_param_importances(study)
     optuna.visualization.matplotlib.plot_optimization_history(study)
     optuna.visualization.plot_contour(study).show(renderer="browser")
```

## Comparing `Seance-0.0.3.dist-info/LICENSE` & `Seance-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Seance-0.0.3.dist-info/METADATA` & `Seance-0.0.4.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Seance
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Wrapper around MLForecast.
 Home-page: https://github.com/tblume1992/Seance
 Author: Tyler Blume
 Author-email: tblume@mail.USF.edu
 Keywords: forecasting,time series,lightgbm,mlforecast
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -55,14 +55,15 @@
 Here we can see the most important parameter is (unsurprisingly) the number of lags. Followd by decay which controls the 'forgetfulness' of the basis functions.
 ```
 optuna.visualization.matplotlib.plot_optimization_history(study)
 ```
 ![alt text](https://github.com/tblume1992/Seance/blob/main/static/seance_study.png?raw=true "Study")
 ## passing off best params for forecasts
 ```
+from Seance.Forecaster import Forecaster
 seance = Forecaster()
 output = seance.fit(series,
                     target_column='y',
                     date_column='ds',
                     id_column='unique_id',
                     freq='D',
                     **best_params)
```

## Comparing `Seance-0.0.3.dist-info/RECORD` & `Seance-0.0.4.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Seance/Explainer.py,sha256=ViUQvXZhsyrKjAscA88NOmBZEXwBl6pldjKe8IJ_fT0,2360
-Seance/Forecaster.py,sha256=mjbPTFddHdjKe2TKlzO_Ak-0hnvPPrv5gWntMUs3_kQ,11991
-Seance/Optimizer.py,sha256=vRqi42lO7ry4OkWBKnuZ7yqGfgOy_YWc3XiC4S9a82I,10054
+Seance/Forecaster.py,sha256=exTxoAirjiDFNlvKDHlovpHP5RH2LU8oEk3xCEIvyJ8,11987
+Seance/Optimizer.py,sha256=ekfQHFRtK_guUSkuE1l0ZBXVdKbwx6akOEVfv1U9DI4,10533
 Seance/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/Builder/PanelAxis.py,sha256=w5YYnDXgprHWUzCWcqqBEkV1xJ_6qLabzW_PIbQF9ZQ,3358
 Seance/Builder/PreProcess.py,sha256=lXDwzPEYw_01pDEB9533v60uqYJEQE7Jb12vjIxmWhA,3916
 Seance/Builder/Transformations.py,sha256=JY27tWWvxha2JXhVgOALQFJUhV-N2Hcmg2u9hhBSeaA,6595
 Seance/Builder/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/__init__.py,sha256=M9j1NuexsmXRO0O_LLRNrLF7fEfPAHWIxm90hC6gV3I,27
 Seance/basis_functions/fourier_basis.py,sha256=8KePMSK7FGqu9t_mkir101B2OvJGZ-FY9kqepiJSCyw,845
 Seance/basis_functions/linear_basis.py,sha256=1RHj--VkbA4heV8QwzNE7a9O0-aPu3Br3EqLlcuUHWU,2834
-Seance-0.0.3.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
-Seance-0.0.3.dist-info/METADATA,sha256=hrQO8PZ1drDxFK646muHOtoLwU10_4uBi_BNUqoqQjg,2684
-Seance-0.0.3.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-Seance-0.0.3.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
-Seance-0.0.3.dist-info/RECORD,,
+Seance-0.0.4.dist-info/LICENSE,sha256=Dk4ScfuH6m_hggBOkCWWWoKU4wkTVtAInrZB4yhn5HU,1087
+Seance-0.0.4.dist-info/METADATA,sha256=WFmB5Z7q-op0jZHzpjRXWNlNVVrtfVyhoQNjJwmOako,2725
+Seance-0.0.4.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+Seance-0.0.4.dist-info/top_level.txt,sha256=NBiOB1gdtNGUu8k7LuJVpJoaNIhKeZK5izXE8-qbRc0,7
+Seance-0.0.4.dist-info/RECORD,,
```

