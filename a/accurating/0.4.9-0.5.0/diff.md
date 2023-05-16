# Comparing `tmp/accurating-0.4.9.tar.gz` & `tmp/accurating-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.9.tar", max compression
+gzip compressed data, was "accurating-0.5.0.tar", max compression
```

## Comparing `accurating-0.4.9.tar` & `accurating-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.9/LICENSE
--rw-r--r--   0        0        0     6369 2023-05-14 19:51:52.513579 accurating-0.4.9/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.9/accurating/__init__.py
--rw-r--r--   0        0        0     9316 2023-05-15 00:36:02.306450 accurating-0.4.9/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.9/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3131 2023-05-15 00:37:22.194706 accurating-0.4.9/accurating/tests/model_test.py
--rw-r--r--   0        0        0      648 2023-05-15 00:37:53.362805 accurating-0.4.9/pyproject.toml
--rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 accurating-0.4.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.5.0/LICENSE
+-rw-r--r--   0        0        0     6438 2023-05-16 03:53:39.354834 accurating-0.5.0/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.5.0/accurating/__init__.py
+-rw-r--r--   0        0        0    11050 2023-05-16 03:41:24.848579 accurating-0.5.0/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.5.0/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3188 2023-05-16 03:43:28.310705 accurating-0.5.0/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      725 2023-05-16 03:54:22.575075 accurating-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7192 1970-01-01 00:00:00.000000 accurating-0.5.0/PKG-INFO
```

### Comparing `accurating-0.4.9/LICENSE` & `accurating-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.9/README.md` & `accurating-0.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,52 +14,54 @@
 If we want to use data efficienty Leon's rating should be adjusted because Caesar clearly demonstrated his power and it was not long ago that poor Leon lucked out a victory against Caesar.
 
 EGD, Chess ELO go over the data once, so they have no way of taking that into account.
 AccuRating shows that we need about 1500 - 2000 passes over the data to converge to accurate ratings.
 
 AccuRating is a variant of [Whole-History-Rating](https://www.remi-coulom.fr/WHR/), which is also used at https://www.goratings.org/.
 
+[Interesting discussion](https://www.mail-archive.com/computer-go@computer-go.org/msg07781.html) on why WHR is good.
+
 ## What AccuRating ratings numbers mean exactly?
 
 Only differences matter, i.e. adding say 100 to all the ratings would yield equally valid points.
 
 - 100 AccuRating point difference is 1:2 win odds (33% vs 66%)
 - 200 AccuRating point difference is 1:5 win odds (20% vs 80%)
-- 300 AccuRating point difference is 1:10 win odds (10% vs 90%)
+- 300 AccuRating point difference is 1:9 win odds (11% vs 89%)
 
 The exact formula is $P(win) = 1 / (1 + 2^{d / 100})$.
 Optimization algorithm find ratings that maximize probability of the data.
 
 ### Compared to Chess ELO
 
 Chess ELO is similar, but the points are rescaled by 1.20412:
 
 - 120.412 chess ELO difference for 1:2 win odds (33% vs 66%)
 - 240.824 chess ELO difference for 1:5 win odds (20% vs 80%)
-- 361.236 chess ELO difference for 1:10 win odds (10% vs 90%)
+- 361.236 chess ELO difference for 1:9 win odds (11% vs 89%)
 
 The Chess ELO formula is $P(win) = 1 / (1 + 10^{d / 400})$
 
 ### Compared to EGD
 
 [In EGD, winning odds for 100 points of rating is not fixed.](http://goratings.eu/Home/About)
 This is beacuse: 1 dan/kyu difference = 100 EGD = 1 handicap.
 The nature of Go is that 1 handicap (i.e. 100 EGD) means more on a dan level than on a kyu level.
 
 On the dan level:
 
 - 90 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 180 EGD point difference is approximately 1:5 win odds (20% vs 80%)
-- 270 EGD point difference is approximately 1:10 win odds (10% vs 90%)
+- 270 EGD point difference is approximately 1:9 win odds (11% vs 89%)
 
 On the kyu level:
 
 - 300 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 600 EGD point difference is approximately 1:5 win odds (20% vs 80%)
-- 900 EGD point difference is approximately 1:10 win odds (10% vs 90%)
+- 900 EGD point difference is approximately 1:9 win odds (11% vs 89%)
 
 [Based on these tables.](https://www.europeangodatabase.eu/EGD/winning_stats.php)
 
 ## If AccuRating is so accurate why other systems are not using it?
 
 Typical ELO systems (like EGD) use every game result only once and update rating based on it.
 This model can do 1500 passes over the data until it converged (the first pass returns numbers more or less like standard ELO system, equations are almost the same).
@@ -121,17 +123,20 @@
 - EGD conversion
 - Fit player variance (high variance player can more easily win against stonger players and more easily lose against weaker players)
 - Follow this: https://www.marwandebbiche.com/posts/python-package-tooling/
 
 ## Development
 
 ```shell
+git config --global core.hooksPath .githooks/
+```
+
+```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
-# TODO(lew): Should automate it somehow.
-poetry run mypy accurating/model.py
-poetry run mypy accurating/tests/model_test.py
+poetry run mypy .
+
 # edit stuff; increase version
 poetry build
 poetry publish
 ```
```

### Comparing `accurating-0.4.9/accurating/model.py` & `accurating-0.5.0/accurating/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import dataclasses
 
 import jax
 import jax.numpy as jnp
 from jax.tree_util import tree_map
 from jax.config import config
+from tabulate import tabulate
 
 config.update("jax_numpy_rank_promotion", "raise")  # bug prevention
 config.update("jax_enable_x64", True)  # better model accuracy
 
 
 def win_prob(rating, opp_rating):
     """Probability of win for given ratings."""
@@ -27,15 +28,15 @@
 
 
 def log_data_prob(p1_ratings, p2_ratings, p1_win_probs, p2_win_probs):
     log_data_prov_values = (
         p1_win_probs * log_win_prob(p1_ratings, p2_ratings) +
         p2_win_probs * log_win_prob(p2_ratings, p1_ratings)
     )
-    return jnp.mean(log_data_prov_values)
+    return log_data_prov_values
 
 
 @dataclasses.dataclass
 class MatchResultArrays:
     """Match data for AccuRating in numpy arrays.
     All attributes have a shape (match_count,).
     """
@@ -76,28 +77,39 @@
     Setting smoothing to 1.0 ignorse match result would rely on player pairing only.
 
     Typically, in the absence of data ratings assume a prior that the skill of a player some fixed value like 1000.
     This allows the rating to not escape to infinity when only losses or only wins are available.
     Smoothing essentially allows to specify that the looser (in every match) had a small chance of winning.
     This is also known as 'label smoothing'."""
 
-    winner_prior_rating: float = 1000.0
-    loser_prior_rating: float = 1000.0
+    winner_prior_rating: float = 4000.0
     winner_prior_match_count: float = 0.0
+    loser_prior_rating: float = 1000.0
     loser_prior_match_count: float = 0.0
+    """Adds two virtual players with a fixed ratings of winner_prior_rating and loser_prior_rating that will always win and always lose.
+    Adds to the data set, for every player and *every season*, winner_prior_match_count (loser_prior_match_count) games with them.
+    The match_counts should be much smaller than the actual number of matches that players played.
+    If match_counts are set to 0.0 the prior is disabled and so the resulting ratings float (can be shifted as a whole by a constant).
+    """
 
     max_steps: int = 1_000_000
     """Limits the number of passes over the dataset."""
 
     do_log: bool = False
     """Enables additional logging."""
 
     initial_lr: float = 10000.0
     """It is automatically adjusted, but sometimes it is too large and blows up."""
 
+    rating_difference_for_2_to_1_odds: float = 100.0
+    """That many points difference creates 2:1 win odds.
+    Twice the difference predicts 5:1 odds.
+    You can change it to 120.412 to match chess ELO scale.
+    Apart from rescaling the final result, it also rescales prior_ratings in this config above."""
+
 
 @dataclasses.dataclass
 class Model:
     """Trained model."""
 
     rating: dict[str, dict[int, float]]
     """Player rating, indexed by name and season"""
@@ -126,60 +138,65 @@
 
     (data_size,) = p1s.shape
     assert seasons.shape == (data_size,)
     assert p1s.shape == (data_size,)
     assert p2s.shape == (data_size,)
     assert p1_win_probs.shape == (data_size,)
 
+    winner_prior = config.winner_prior_rating / config.rating_difference_for_2_to_1_odds
+    loser_prior = config.loser_prior_rating / config.rating_difference_for_2_to_1_odds
+
     def model(params):
         log_likelihood = 0.0
         ratings = params['rating']
         assert ratings.shape == (player_count, season_count)
         p1_ratings = ratings[p1s, seasons]
         p2_ratings = ratings[p2s, seasons]
 
         assert p1_ratings.shape == (data_size,)
         assert p2_ratings.shape == (data_size,)
 
-        mean_log_data_prob = log_data_prob(p1_ratings, p2_ratings, p1_win_probs, p2_win_probs)
+        # We need to sum instead of averaging, because the more data we have, the more should it outweigh the priors
+        # and even the season_rating_stability.
+        mean_log_data_prob = jnp.sum(log_data_prob(p1_ratings, p2_ratings, p1_win_probs, p2_win_probs))
         log_likelihood += mean_log_data_prob
 
         if config.season_rating_stability > 0.0:
-            log_likelihood -= config.season_rating_stability * jnp.mean((ratings[:, 1:] - ratings[:, :-1])**2)
+            log_likelihood -= config.season_rating_stability * jnp.sum((ratings[:, 1:] - ratings[:, :-1])**2)
 
         if config.winner_prior_match_count > 0.0:
-            log_likelihood += log_data_prob(ratings, config.winner_prior_rating, 0.0, config.winner_prior_match_count)
+            log_likelihood += jnp.sum(log_data_prob(ratings, jnp.ones_like(ratings) * winner_prior, 0.0, config.winner_prior_match_count))
 
         if config.loser_prior_match_count > 0.0:
-            log_likelihood += log_data_prob(ratings, config.loser_prior_rating, config.loser_prior_match_count, 0.0)
+            log_likelihood += jnp.sum(log_data_prob(ratings, jnp.ones_like(ratings) * loser_prior, config.loser_prior_match_count, 0.0))
 
-        geomean_data_prob = jnp.exp2(mean_log_data_prob)
-        return log_likelihood, geomean_data_prob
+        geomean_data_prob = jnp.exp2(mean_log_data_prob / data_size)
+        return log_likelihood / data_size, geomean_data_prob
 
         # TODO: This is an experiment trying to evaluate ELO playing consistency. Try again and delete if does not work.
         # cons = params['consistency']
         # p1_cons = jnp.take(cons, p1s)
         # p2_cons = jnp.take(cons, p2s)
         # winner_win_prob_log = 0.0
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p2_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p2_cons))
         # winner_win_prob_log /= 2
-        # return jnp.mean(winner_win_prob_log) - 0.005*jnp.mean(cons ** 2)
+        # return jnp.sum(winner_win_prob_log) - 0.005*jnp.sum(cons ** 2) # or mean?
 
     # Optimize for these params:
-    rating = jnp.zeros([player_count, season_count], dtype=jnp.float64)
+    rating = jnp.zeros([player_count, season_count], dtype=jnp.float64) + (loser_prior + winner_prior) / 2.0
     params = { 'rating': rating }
     # 'consistency': jnp.zeros([player_count, season_count]),
 
     # Momentum gradient descent with restarts
     m_lr = 1.0
     lr = float(config.initial_lr)
     momentum = tree_map(jnp.zeros_like, params)
     last_params = params
-    last_eval = -2  # eval of initial data is -1
+    last_eval = -1e8  # eval of initial data is -1, but regularizations might push it lower.
     last_grad = tree_map(jnp.zeros_like, params)
     last_reset_step = 0
 
     for i in range(config.max_steps):
         (eval, model_fit), grad = jax.value_and_grad(model, has_aux=True)(params)
 
         if False:
@@ -203,37 +220,44 @@
 
         max_d_rating = jnp.max(
             jnp.abs(params['rating'] - last_params['rating']))
 
         if config.do_log:
             g = jnp.linalg.norm(grad['rating'])
             print(
-                f'Step {i:4}: eval: {jnp.exp2(eval):0.12f} lr={lr: 4.4f} grad={g:2.4f} delta={max_d_rating}')
+                f'Step {i:4}: eval={jnp.exp2(eval):0.12f} pred_power={model_fit:0.6f} lr={lr: 4.4f} grad={g:2.4f} delta={max_d_rating}')
 
         if max_d_rating < 1e-15:
             break
 
         lr *= 1.5 ** (1.0 / 12)
 
     def postprocess():
         rating = {}
         last_rating = []
         for id, name in enumerate(data.player_name):
             rating[name] = {}
             for season in range(season_count):
-                rating[name][season] = float(params['rating'][id, season]) * 100.0
+                rating[name][season] = float(params['rating'][id, season]) * config.rating_difference_for_2_to_1_odds
             last_rating.append((rating[name][season_count - 1], name))
         if config.do_log:
+            headers = ['Nick']
+            for season in range(season_count-1, -1, -1):
+                headers.append(f'S{season}')
             last_rating.sort(reverse=True)
-            print("Top 10 last season:")
-            for i in range(min(len(last_rating), 10)):
-                print(f'{last_rating[i][1]:30}: {last_rating[i][0]: 8.1f}')
+            table = []
+            for _, name in last_rating:
+                # if len(table) > 10: break # max rows
+                row = [name]
+                for season in range(season_count-1, 0, -1):
+                    row.append(rating[name][season])
+                table.append(row)
+            print(tabulate(table, headers=headers, floatfmt=".1f", numalign="decimal"))
 
-        ret = Model(rating=rating)
-        return ret
+        return Model(rating=rating)
 
     return postprocess()
 
 
 def data_from_dicts(matches) -> MatchResultArrays:
     player_set = set()
```

### Comparing `accurating-0.4.9/accurating/tests/model_test.py` & `accurating-0.5.0/accurating/tests/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,23 @@
 
     cfg = accurating.Config(
         season_rating_stability=0.5,
         smoothing=0.1,
         max_steps=100,
         do_log=True,
         initial_lr=1.0,
+        winner_prior_rating=0.,
+        loser_prior_rating=0.,
+
     )
     model = accurating.fit(data, cfg)
+
     # ratings = np.array([[model.rating[pl][s] for s in range(len(season))] for pl in player_name])
     assert_almost_equal(model.rating['Alusia'][0], 0.0)
     assert_almost_equal(model.rating['Alusia'][1], 0.0)
-    assert_almost_equal(model.rating['Caesar'][0], -13.45060654581596)
-    assert_almost_equal(model.rating['Caesar'][1], 26.90122721761437)
-    assert_almost_equal(model.rating['Leon'][0], 13.45060654581597)
-    assert_almost_equal(model.rating['Leon'][1], -26.901227217614354)
+
+    v = 13.45060623432789
+    v2 = 26.901228584915188
+    assert_almost_equal(model.rating['Caesar'][0], -v)
+    assert_almost_equal(model.rating['Caesar'][1], v2)
+    assert_almost_equal(model.rating['Leon'][0], v)
+    assert_almost_equal(model.rating['Leon'][1], -v2)
```

### Comparing `accurating-0.4.9/PKG-INFO` & `accurating-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.9
+Version: 0.5.0
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: jax (>=0.4.8,<0.5.0)
 Requires-Dist: jaxlib (>=0.4.7,<0.5.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: types-requests (>=2.30.0.0,<3.0.0.0)
+Requires-Dist: types-tabulate (>=0.9.0.2,<0.10.0.0)
 Project-URL: Documentation, https://lukaszlew.github.io/accurating/
 Description-Content-Type: text/markdown
 
 # AccuRating
 
 Library computing accurate ratings based on match results.
 
@@ -30,52 +33,54 @@
 If we want to use data efficienty Leon's rating should be adjusted because Caesar clearly demonstrated his power and it was not long ago that poor Leon lucked out a victory against Caesar.
 
 EGD, Chess ELO go over the data once, so they have no way of taking that into account.
 AccuRating shows that we need about 1500 - 2000 passes over the data to converge to accurate ratings.
 
 AccuRating is a variant of [Whole-History-Rating](https://www.remi-coulom.fr/WHR/), which is also used at https://www.goratings.org/.
 
+[Interesting discussion](https://www.mail-archive.com/computer-go@computer-go.org/msg07781.html) on why WHR is good.
+
 ## What AccuRating ratings numbers mean exactly?
 
 Only differences matter, i.e. adding say 100 to all the ratings would yield equally valid points.
 
 - 100 AccuRating point difference is 1:2 win odds (33% vs 66%)
 - 200 AccuRating point difference is 1:5 win odds (20% vs 80%)
-- 300 AccuRating point difference is 1:10 win odds (10% vs 90%)
+- 300 AccuRating point difference is 1:9 win odds (11% vs 89%)
 
 The exact formula is $P(win) = 1 / (1 + 2^{d / 100})$.
 Optimization algorithm find ratings that maximize probability of the data.
 
 ### Compared to Chess ELO
 
 Chess ELO is similar, but the points are rescaled by 1.20412:
 
 - 120.412 chess ELO difference for 1:2 win odds (33% vs 66%)
 - 240.824 chess ELO difference for 1:5 win odds (20% vs 80%)
-- 361.236 chess ELO difference for 1:10 win odds (10% vs 90%)
+- 361.236 chess ELO difference for 1:9 win odds (11% vs 89%)
 
 The Chess ELO formula is $P(win) = 1 / (1 + 10^{d / 400})$
 
 ### Compared to EGD
 
 [In EGD, winning odds for 100 points of rating is not fixed.](http://goratings.eu/Home/About)
 This is beacuse: 1 dan/kyu difference = 100 EGD = 1 handicap.
 The nature of Go is that 1 handicap (i.e. 100 EGD) means more on a dan level than on a kyu level.
 
 On the dan level:
 
 - 90 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 180 EGD point difference is approximately 1:5 win odds (20% vs 80%)
-- 270 EGD point difference is approximately 1:10 win odds (10% vs 90%)
+- 270 EGD point difference is approximately 1:9 win odds (11% vs 89%)
 
 On the kyu level:
 
 - 300 EGD point difference is approximately 1:2 win odds (33% vs 66%)
 - 600 EGD point difference is approximately 1:5 win odds (20% vs 80%)
-- 900 EGD point difference is approximately 1:10 win odds (10% vs 90%)
+- 900 EGD point difference is approximately 1:9 win odds (11% vs 89%)
 
 [Based on these tables.](https://www.europeangodatabase.eu/EGD/winning_stats.php)
 
 ## If AccuRating is so accurate why other systems are not using it?
 
 Typical ELO systems (like EGD) use every game result only once and update rating based on it.
 This model can do 1500 passes over the data until it converged (the first pass returns numbers more or less like standard ELO system, equations are almost the same).
@@ -137,18 +142,21 @@
 - EGD conversion
 - Fit player variance (high variance player can more easily win against stonger players and more easily lose against weaker players)
 - Follow this: https://www.marwandebbiche.com/posts/python-package-tooling/
 
 ## Development
 
 ```shell
+git config --global core.hooksPath .githooks/
+```
+
+```shell
 git clone https://github.com/lukaszlew/accurating
 poetry install
 poetry run pytest
-# TODO(lew): Should automate it somehow.
-poetry run mypy accurating/model.py
-poetry run mypy accurating/tests/model_test.py
+poetry run mypy .
+
 # edit stuff; increase version
 poetry build
 poetry publish
 ```
```

