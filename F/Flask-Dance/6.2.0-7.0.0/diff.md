# Comparing `tmp/Flask-Dance-6.2.0.tar.gz` & `tmp/Flask-Dance-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Dance-6.2.0.tar", last modified: Wed Oct 12 15:18:22 2022, max compression
+gzip compressed data, was "Flask-Dance-7.0.0.tar", last modified: Wed May 10 18:28:20 2023, max compression
```

## Comparing `Flask-Dance-6.2.0.tar` & `Flask-Dance-7.0.0.tar`

### file list

```diff
@@ -1,111 +1,111 @@
--rw-r--r--   0        0        0       99 2021-01-22 09:05:51.217815 Flask-Dance-6.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      144 2021-04-30 10:40:50.706231 Flask-Dance-6.2.0/.github/dependabot.yml
--rw-r--r--   0        0        0      867 2022-10-12 15:07:49.501394 Flask-Dance-6.2.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      757 2022-10-12 15:07:49.501870 Flask-Dance-6.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1645 2022-10-12 15:08:29.990916 Flask-Dance-6.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      138 2022-08-05 13:56:01.871288 Flask-Dance-6.2.0/.gitignore
--rw-r--r--   0        0        0      510 2022-10-12 15:12:58.373731 Flask-Dance-6.2.0/.readthedocs.yml
--rw-r--r--   0        0        0    19191 2022-10-12 15:17:41.973765 Flask-Dance-6.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0     1092 2021-02-25 13:21:12.503871 Flask-Dance-6.2.0/LICENSE
--rw-r--r--   0        0        0      165 2021-01-22 09:05:51.218317 Flask-Dance-6.2.0/MANIFEST.in
--rw-r--r--   0        0        0     4747 2021-10-14 14:54:56.666015 Flask-Dance-6.2.0/README.rst
--rw-r--r--   0        0        0     7029 2021-01-22 09:05:51.218505 Flask-Dance-6.2.0/docs/Makefile
--rw-r--r--   0        0        0    44272 2021-01-22 09:05:51.218673 Flask-Dance-6.2.0/docs/_static/flask-dance.pdf
--rw-r--r--   0        0        0    19362 2021-01-22 09:05:51.218816 Flask-Dance-6.2.0/docs/_static/flask-dance.png
--rw-r--r--   0        0        0    96288 2021-01-22 09:05:51.219045 Flask-Dance-6.2.0/docs/_static/flask-dance.svg
--rw-r--r--   0        0        0     4392 2021-05-12 13:01:19.230914 Flask-Dance-6.2.0/docs/api.rst
--rw-r--r--   0        0        0     5248 2022-08-05 13:53:22.337114 Flask-Dance-6.2.0/docs/concepts.rst
--rw-r--r--   0        0        0     9597 2022-04-05 18:06:17.896396 Flask-Dance-6.2.0/docs/conf.py
--rw-r--r--   0        0        0     1950 2021-01-22 09:05:51.219379 Flask-Dance-6.2.0/docs/contributing.rst
--rw-r--r--   0        0        0      590 2021-01-22 09:05:51.219431 Flask-Dance-6.2.0/docs/examples.rst
--rw-r--r--   0        0        0     8855 2021-01-22 09:05:51.219527 Flask-Dance-6.2.0/docs/how-oauth-works.rst
--rw-r--r--   0        0        0     1482 2021-01-22 09:05:51.219585 Flask-Dance-6.2.0/docs/index.rst
--rw-r--r--   0        0        0      346 2021-01-22 09:05:51.219641 Flask-Dance-6.2.0/docs/install.rst
--rw-r--r--   0        0        0     7113 2021-01-22 09:05:51.219718 Flask-Dance-6.2.0/docs/logout.rst
--rw-r--r--   0        0        0     6709 2021-01-22 09:05:51.219782 Flask-Dance-6.2.0/docs/make.bat
--rw-r--r--   0        0        0    10121 2021-01-22 09:05:51.219877 Flask-Dance-6.2.0/docs/multi-user.rst
--rw-r--r--   0        0        0    10984 2022-10-12 14:47:25.709126 Flask-Dance-6.2.0/docs/providers.rst
--rw-r--r--   0        0        0     2223 2022-08-05 13:53:22.337481 Flask-Dance-6.2.0/docs/proxies.rst
--rw-r--r--   0        0        0     2518 2022-04-05 11:39:51.713803 Flask-Dance-6.2.0/docs/quickstart.rst
--rw-r--r--   0        0        0      152 2022-08-05 13:53:22.337633 Flask-Dance-6.2.0/docs/requirements.txt
--rw-r--r--   0        0        0     3521 2021-05-12 13:01:19.231918 Flask-Dance-6.2.0/docs/signals.rst
--rw-r--r--   0        0        0      542 2022-08-05 13:56:01.872263 Flask-Dance-6.2.0/docs/spelling_wordlist.txt
--rw-r--r--   0        0        0     4520 2021-01-22 09:05:51.220389 Flask-Dance-6.2.0/docs/storages.rst
--rw-r--r--   0        0        0     7852 2021-05-12 13:01:19.232219 Flask-Dance-6.2.0/docs/testing.rst
--rw-r--r--   0        0        0     4845 2021-01-22 09:05:51.220589 Flask-Dance-6.2.0/docs/understanding-the-magic.rst
--rw-r--r--   0        0        0      165 2022-10-12 15:16:39.559869 Flask-Dance-6.2.0/flask_dance/__init__.py
--rw-r--r--   0        0        0      207 2022-04-05 18:06:17.896841 Flask-Dance-6.2.0/flask_dance/consumer/__init__.py
--rw-r--r--   0        0        0     6022 2022-04-05 18:06:17.897259 Flask-Dance-6.2.0/flask_dance/consumer/base.py
--rw-r--r--   0        0        0     9815 2022-04-05 18:06:17.897625 Flask-Dance-6.2.0/flask_dance/consumer/oauth1.py
--rw-r--r--   0        0        0    10931 2022-04-05 18:06:17.897975 Flask-Dance-6.2.0/flask_dance/consumer/oauth2.py
--rw-r--r--   0        0        0     7158 2022-04-05 18:06:17.898301 Flask-Dance-6.2.0/flask_dance/consumer/requests.py
--rw-r--r--   0        0        0     1267 2021-03-02 10:26:34.771215 Flask-Dance-6.2.0/flask_dance/consumer/storage/__init__.py
--rw-r--r--   0        0        0     1086 2022-04-05 18:06:17.898702 Flask-Dance-6.2.0/flask_dance/consumer/storage/session.py
--rw-r--r--   0        0        0    11132 2022-08-05 13:32:07.107569 Flask-Dance-6.2.0/flask_dance/consumer/storage/sqla.py
--rw-r--r--   0        0        0     1518 2021-01-22 09:05:51.221475 Flask-Dance-6.2.0/flask_dance/contrib/README.rst
--rw-r--r--   0        0        0        0 2021-01-22 09:05:51.221499 Flask-Dance-6.2.0/flask_dance/contrib/__init__.py
--rw-r--r--   0        0        0     3490 2022-08-05 13:53:22.337967 Flask-Dance-6.2.0/flask_dance/contrib/atlassian.py
--rw-r--r--   0        0        0     3454 2022-08-05 13:53:22.338164 Flask-Dance-6.2.0/flask_dance/contrib/authentiq.py
--rw-r--r--   0        0        0     5228 2022-08-05 13:53:22.338351 Flask-Dance-6.2.0/flask_dance/contrib/azure.py
--rw-r--r--   0        0        0     3420 2022-08-05 13:53:22.338520 Flask-Dance-6.2.0/flask_dance/contrib/digitalocean.py
--rw-r--r--   0        0        0     3668 2022-08-05 13:53:22.338694 Flask-Dance-6.2.0/flask_dance/contrib/discord.py
--rw-r--r--   0        0        0     4563 2022-08-05 13:53:22.338878 Flask-Dance-6.2.0/flask_dance/contrib/dropbox.py
--rw-r--r--   0        0        0     3646 2022-08-05 13:53:22.339042 Flask-Dance-6.2.0/flask_dance/contrib/facebook.py
--rw-r--r--   0        0        0     3261 2022-08-05 13:53:22.339209 Flask-Dance-6.2.0/flask_dance/contrib/fitbit.py
--rw-r--r--   0        0        0     3220 2022-08-05 13:53:22.339372 Flask-Dance-6.2.0/flask_dance/contrib/github.py
--rw-r--r--   0        0        0     4212 2022-08-05 13:53:22.339540 Flask-Dance-6.2.0/flask_dance/contrib/gitlab.py
--rw-r--r--   0        0        0     5368 2022-08-05 13:53:22.339704 Flask-Dance-6.2.0/flask_dance/contrib/google.py
--rw-r--r--   0        0        0     3703 2022-08-05 13:53:22.339868 Flask-Dance-6.2.0/flask_dance/contrib/heroku.py
--rw-r--r--   0        0        0     4012 2022-08-05 13:53:22.340046 Flask-Dance-6.2.0/flask_dance/contrib/jira.py
--rw-r--r--   0        0        0     3330 2022-08-05 13:53:22.340205 Flask-Dance-6.2.0/flask_dance/contrib/linkedin.py
--rw-r--r--   0        0        0     3284 2022-08-05 13:53:22.340360 Flask-Dance-6.2.0/flask_dance/contrib/meetup.py
--rw-r--r--   0        0        0     3296 2022-08-05 13:53:22.340511 Flask-Dance-6.2.0/flask_dance/contrib/nylas.py
--rw-r--r--   0        0        0     3710 2022-10-12 14:47:25.710401 Flask-Dance-6.2.0/flask_dance/contrib/orcid.py
--rw-r--r--   0        0        0     3213 2022-08-05 13:57:36.708027 Flask-Dance-6.2.0/flask_dance/contrib/osm.py
--rw-r--r--   0        0        0     4477 2022-08-05 13:53:22.340675 Flask-Dance-6.2.0/flask_dance/contrib/reddit.py
--rw-r--r--   0        0        0     3989 2022-08-05 13:53:22.340903 Flask-Dance-6.2.0/flask_dance/contrib/salesforce.py
--rw-r--r--   0        0        0     3708 2022-08-05 13:53:22.341095 Flask-Dance-6.2.0/flask_dance/contrib/slack.py
--rw-r--r--   0        0        0     3229 2022-08-05 13:53:22.341276 Flask-Dance-6.2.0/flask_dance/contrib/spotify.py
--rw-r--r--   0        0        0     4040 2022-08-05 13:53:22.341470 Flask-Dance-6.2.0/flask_dance/contrib/strava.py
--rw-r--r--   0        0        0     4191 2022-08-05 13:53:22.341642 Flask-Dance-6.2.0/flask_dance/contrib/twitch.py
--rw-r--r--   0        0        0     3178 2022-08-05 13:53:22.341822 Flask-Dance-6.2.0/flask_dance/contrib/twitter.py
--rw-r--r--   0        0        0     5262 2022-08-05 13:53:22.342057 Flask-Dance-6.2.0/flask_dance/contrib/zoho.py
--rw-r--r--   0        0        0        0 2021-01-22 09:05:51.223263 Flask-Dance-6.2.0/flask_dance/fixtures/__init__.py
--rw-r--r--   0        0        0     2977 2022-08-05 13:53:22.342273 Flask-Dance-6.2.0/flask_dance/fixtures/pytest.py
--rw-r--r--   0        0        0     1051 2022-04-05 17:53:52.846018 Flask-Dance-6.2.0/flask_dance/utils.py
--rw-r--r--   0        0        0     2059 2022-10-12 15:07:56.132448 Flask-Dance-6.2.0/pyproject.toml
--rw-r--r--   0        0        0      336 2021-01-22 09:05:51.223660 Flask-Dance-6.2.0/tests/conftest.py
--rw-r--r--   0        0        0    24640 2022-08-05 13:53:22.342539 Flask-Dance-6.2.0/tests/consumer/storage/test_sqla.py
--rw-r--r--   0        0        0    18653 2022-08-22 12:26:59.152611 Flask-Dance-6.2.0/tests/consumer/test_oauth1.py
--rw-r--r--   0        0        0    23557 2022-08-22 12:27:18.236730 Flask-Dance-6.2.0/tests/consumer/test_oauth2.py
--rw-r--r--   0        0        0     2674 2022-04-05 18:06:17.908143 Flask-Dance-6.2.0/tests/consumer/test_requests.py
--rw-r--r--   0        0        0     3886 2022-04-05 18:06:17.908373 Flask-Dance-6.2.0/tests/contrib/test_atlassian.py
--rw-r--r--   0        0        0     3462 2022-04-05 18:06:17.908605 Flask-Dance-6.2.0/tests/contrib/test_authentiq.py
--rw-r--r--   0        0        0     6313 2022-04-05 18:06:17.908905 Flask-Dance-6.2.0/tests/contrib/test_azure.py
--rw-r--r--   0        0        0     3256 2022-04-05 18:06:17.909190 Flask-Dance-6.2.0/tests/contrib/test_digitalocean.py
--rw-r--r--   0        0        0     3646 2022-04-05 18:06:17.909435 Flask-Dance-6.2.0/tests/contrib/test_discord.py
--rw-r--r--   0        0        0     3900 2022-04-05 18:06:17.909679 Flask-Dance-6.2.0/tests/contrib/test_dropbox.py
--rw-r--r--   0        0        0     3767 2022-04-05 18:06:17.909939 Flask-Dance-6.2.0/tests/contrib/test_facebook.py
--rw-r--r--   0        0        0     2736 2022-04-05 18:06:17.910199 Flask-Dance-6.2.0/tests/contrib/test_fitbit.py
--rw-r--r--   0        0        0     2745 2022-04-05 18:06:17.910456 Flask-Dance-6.2.0/tests/contrib/test_github.py
--rw-r--r--   0        0        0     5430 2022-04-05 18:06:17.910727 Flask-Dance-6.2.0/tests/contrib/test_gitlab.py
--rw-r--r--   0        0        0     6617 2022-04-05 18:06:17.910987 Flask-Dance-6.2.0/tests/contrib/test_google.py
--rw-r--r--   0        0        0     2724 2022-04-05 18:06:17.911218 Flask-Dance-6.2.0/tests/contrib/test_heroku.py
--rw-r--r--   0        0        0     6500 2022-04-05 18:06:17.911447 Flask-Dance-6.2.0/tests/contrib/test_jira.py
--rw-r--r--   0        0        0     2827 2022-04-05 18:06:17.911681 Flask-Dance-6.2.0/tests/contrib/test_linkedin.py
--rw-r--r--   0        0        0     2917 2022-04-05 18:06:17.911892 Flask-Dance-6.2.0/tests/contrib/test_meetup.py
--rw-r--r--   0        0        0     2752 2022-04-05 18:06:17.912097 Flask-Dance-6.2.0/tests/contrib/test_nylas.py
--rw-r--r--   0        0        0     3343 2022-10-12 14:47:25.711259 Flask-Dance-6.2.0/tests/contrib/test_orcid.py
--rw-r--r--   0        0        0     2709 2022-08-05 14:10:59.920253 Flask-Dance-6.2.0/tests/contrib/test_osm.py
--rw-r--r--   0        0        0     3476 2022-04-05 18:06:17.912308 Flask-Dance-6.2.0/tests/contrib/test_reddit.py
--rw-r--r--   0        0        0     5461 2022-04-05 18:06:17.912528 Flask-Dance-6.2.0/tests/contrib/test_salesforce.py
--rw-r--r--   0        0        0     7471 2022-04-05 18:41:56.437662 Flask-Dance-6.2.0/tests/contrib/test_slack.py
--rw-r--r--   0        0        0     2799 2022-04-05 18:06:17.912973 Flask-Dance-6.2.0/tests/contrib/test_spotify.py
--rw-r--r--   0        0        0     2767 2022-04-05 18:06:17.913208 Flask-Dance-6.2.0/tests/contrib/test_strava.py
--rw-r--r--   0        0        0     2986 2022-04-05 18:06:17.913455 Flask-Dance-6.2.0/tests/contrib/test_twitch.py
--rw-r--r--   0        0        0     3800 2022-04-05 18:06:17.913697 Flask-Dance-6.2.0/tests/contrib/test_twitter.py
--rw-r--r--   0        0        0     2584 2022-04-05 18:06:17.913928 Flask-Dance-6.2.0/tests/contrib/test_zoho.py
--rw-r--r--   0        0        0     2606 2021-01-22 09:05:51.225870 Flask-Dance-6.2.0/tests/fixtures/cassettes/test_home_page.json
--rw-r--r--   0        0        0     1510 2022-08-22 17:22:12.799257 Flask-Dance-6.2.0/tests/fixtures/test_pytest.py
--rw-r--r--   0        0        0      686 2022-04-05 18:06:17.914423 Flask-Dance-6.2.0/tests/test_utils.py
--rw-r--r--   0        0        0     6826 1970-01-01 00:00:00.000000 Flask-Dance-6.2.0/PKG-INFO
+-rw-r--r--   0        0        0       99 2021-01-22 09:05:51.217815 Flask-Dance-7.0.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      144 2021-04-30 10:40:50.706231 Flask-Dance-7.0.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      867 2023-01-19 21:47:16.240249 Flask-Dance-7.0.0/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      757 2023-01-19 21:47:16.240648 Flask-Dance-7.0.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1645 2023-01-19 21:47:16.241019 Flask-Dance-7.0.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      138 2023-01-19 21:47:16.241370 Flask-Dance-7.0.0/.gitignore
+-rw-r--r--   0        0        0      510 2023-01-19 21:47:16.243522 Flask-Dance-7.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    19492 2023-05-10 18:25:15.807294 Flask-Dance-7.0.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1092 2021-02-25 13:21:12.503871 Flask-Dance-7.0.0/LICENSE
+-rw-r--r--   0        0        0      165 2021-01-22 09:05:51.218317 Flask-Dance-7.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     4747 2021-10-14 14:54:56.666015 Flask-Dance-7.0.0/README.rst
+-rw-r--r--   0        0        0     7029 2021-01-22 09:05:51.218505 Flask-Dance-7.0.0/docs/Makefile
+-rw-r--r--   0        0        0    44272 2021-01-22 09:05:51.218673 Flask-Dance-7.0.0/docs/_static/flask-dance.pdf
+-rw-r--r--   0        0        0    19362 2021-01-22 09:05:51.218816 Flask-Dance-7.0.0/docs/_static/flask-dance.png
+-rw-r--r--   0        0        0    96288 2021-01-22 09:05:51.219045 Flask-Dance-7.0.0/docs/_static/flask-dance.svg
+-rw-r--r--   0        0        0     4392 2021-05-12 13:01:19.230914 Flask-Dance-7.0.0/docs/api.rst
+-rw-r--r--   0        0        0     5248 2023-01-19 21:47:16.244586 Flask-Dance-7.0.0/docs/concepts.rst
+-rw-r--r--   0        0        0     9597 2023-01-19 21:47:16.245041 Flask-Dance-7.0.0/docs/conf.py
+-rw-r--r--   0        0        0     1950 2021-01-22 09:05:51.219379 Flask-Dance-7.0.0/docs/contributing.rst
+-rw-r--r--   0        0        0      590 2021-01-22 09:05:51.219431 Flask-Dance-7.0.0/docs/examples.rst
+-rw-r--r--   0        0        0     8852 2023-05-10 18:22:19.220405 Flask-Dance-7.0.0/docs/how-oauth-works.rst
+-rw-r--r--   0        0        0     1487 2023-01-23 13:30:34.574634 Flask-Dance-7.0.0/docs/index.rst
+-rw-r--r--   0        0        0      346 2021-01-22 09:05:51.219641 Flask-Dance-7.0.0/docs/install.rst
+-rw-r--r--   0        0        0     7113 2021-01-22 09:05:51.219718 Flask-Dance-7.0.0/docs/logout.rst
+-rw-r--r--   0        0        0     6709 2021-01-22 09:05:51.219782 Flask-Dance-7.0.0/docs/make.bat
+-rw-r--r--   0        0        0    10121 2021-01-22 09:05:51.219877 Flask-Dance-7.0.0/docs/multi-user.rst
+-rw-r--r--   0        0        0    10976 2023-05-10 18:22:19.220715 Flask-Dance-7.0.0/docs/providers.rst
+-rw-r--r--   0        0        0     2223 2023-01-19 21:47:16.245863 Flask-Dance-7.0.0/docs/proxies.rst
+-rw-r--r--   0        0        0     2373 2023-05-10 18:22:19.221564 Flask-Dance-7.0.0/docs/quickstart.rst
+-rw-r--r--   0        0        0      152 2023-01-19 21:47:16.246229 Flask-Dance-7.0.0/docs/requirements.txt
+-rw-r--r--   0        0        0     3521 2021-05-12 13:01:19.231918 Flask-Dance-7.0.0/docs/signals.rst
+-rw-r--r--   0        0        0      549 2023-05-10 18:22:19.221896 Flask-Dance-7.0.0/docs/spelling_wordlist.txt
+-rw-r--r--   0        0        0     4520 2021-01-22 09:05:51.220389 Flask-Dance-7.0.0/docs/storages.rst
+-rw-r--r--   0        0        0     7852 2021-05-12 13:01:19.232219 Flask-Dance-7.0.0/docs/testing.rst
+-rw-r--r--   0        0        0     4845 2021-01-22 09:05:51.220589 Flask-Dance-7.0.0/docs/understanding-the-magic.rst
+-rw-r--r--   0        0        0      165 2023-05-10 18:25:47.877023 Flask-Dance-7.0.0/flask_dance/__init__.py
+-rw-r--r--   0        0        0      207 2023-01-19 21:47:16.247547 Flask-Dance-7.0.0/flask_dance/consumer/__init__.py
+-rw-r--r--   0        0        0     6024 2023-05-10 18:22:19.222293 Flask-Dance-7.0.0/flask_dance/consumer/base.py
+-rw-r--r--   0        0        0     9814 2023-05-10 18:22:19.222526 Flask-Dance-7.0.0/flask_dance/consumer/oauth1.py
+-rw-r--r--   0        0        0    12871 2023-05-10 18:22:19.222773 Flask-Dance-7.0.0/flask_dance/consumer/oauth2.py
+-rw-r--r--   0        0        0     7154 2023-05-10 18:22:19.222996 Flask-Dance-7.0.0/flask_dance/consumer/requests.py
+-rw-r--r--   0        0        0     1267 2021-03-02 10:26:34.771215 Flask-Dance-7.0.0/flask_dance/consumer/storage/__init__.py
+-rw-r--r--   0        0        0     1086 2023-01-19 21:47:16.249485 Flask-Dance-7.0.0/flask_dance/consumer/storage/session.py
+-rw-r--r--   0        0        0    11131 2023-05-10 18:22:19.223283 Flask-Dance-7.0.0/flask_dance/consumer/storage/sqla.py
+-rw-r--r--   0        0        0     1518 2021-01-22 09:05:51.221475 Flask-Dance-7.0.0/flask_dance/contrib/README.rst
+-rw-r--r--   0        0        0        0 2021-01-22 09:05:51.221499 Flask-Dance-7.0.0/flask_dance/contrib/__init__.py
+-rw-r--r--   0        0        0     3490 2023-01-19 21:47:16.250442 Flask-Dance-7.0.0/flask_dance/contrib/atlassian.py
+-rw-r--r--   0        0        0     3454 2023-01-19 21:47:16.250773 Flask-Dance-7.0.0/flask_dance/contrib/authentiq.py
+-rw-r--r--   0        0        0     5228 2023-01-19 21:47:16.251097 Flask-Dance-7.0.0/flask_dance/contrib/azure.py
+-rw-r--r--   0        0        0     3298 2023-05-10 18:22:19.223568 Flask-Dance-7.0.0/flask_dance/contrib/dexcom.py
+-rw-r--r--   0        0        0     3420 2023-01-19 21:47:16.251434 Flask-Dance-7.0.0/flask_dance/contrib/digitalocean.py
+-rw-r--r--   0        0        0     3668 2023-01-19 21:47:16.251738 Flask-Dance-7.0.0/flask_dance/contrib/discord.py
+-rw-r--r--   0        0        0     4563 2023-01-19 21:47:16.251988 Flask-Dance-7.0.0/flask_dance/contrib/dropbox.py
+-rw-r--r--   0        0        0     3646 2023-01-19 21:47:16.252237 Flask-Dance-7.0.0/flask_dance/contrib/facebook.py
+-rw-r--r--   0        0        0     3261 2023-01-19 21:47:16.252565 Flask-Dance-7.0.0/flask_dance/contrib/fitbit.py
+-rw-r--r--   0        0        0     3220 2023-01-19 21:47:16.252936 Flask-Dance-7.0.0/flask_dance/contrib/github.py
+-rw-r--r--   0        0        0     4212 2023-01-19 21:47:16.253200 Flask-Dance-7.0.0/flask_dance/contrib/gitlab.py
+-rw-r--r--   0        0        0     5368 2023-01-19 21:47:16.253513 Flask-Dance-7.0.0/flask_dance/contrib/google.py
+-rw-r--r--   0        0        0     3703 2023-01-19 21:47:16.253775 Flask-Dance-7.0.0/flask_dance/contrib/heroku.py
+-rw-r--r--   0        0        0     4012 2023-01-19 21:47:16.254077 Flask-Dance-7.0.0/flask_dance/contrib/jira.py
+-rw-r--r--   0        0        0     3330 2023-01-19 21:47:16.254321 Flask-Dance-7.0.0/flask_dance/contrib/linkedin.py
+-rw-r--r--   0        0        0     3284 2023-01-19 21:47:16.254552 Flask-Dance-7.0.0/flask_dance/contrib/meetup.py
+-rw-r--r--   0        0        0     3296 2023-01-19 21:47:16.254792 Flask-Dance-7.0.0/flask_dance/contrib/nylas.py
+-rw-r--r--   0        0        0     3710 2023-01-19 21:47:16.255069 Flask-Dance-7.0.0/flask_dance/contrib/orcid.py
+-rw-r--r--   0        0        0     3213 2023-01-19 21:47:16.255345 Flask-Dance-7.0.0/flask_dance/contrib/osm.py
+-rw-r--r--   0        0        0     4477 2023-01-19 21:47:16.255564 Flask-Dance-7.0.0/flask_dance/contrib/reddit.py
+-rw-r--r--   0        0        0     3989 2023-01-19 21:47:16.255791 Flask-Dance-7.0.0/flask_dance/contrib/salesforce.py
+-rw-r--r--   0        0        0     3708 2023-01-19 21:47:16.256087 Flask-Dance-7.0.0/flask_dance/contrib/slack.py
+-rw-r--r--   0        0        0     3229 2023-01-19 21:47:16.256406 Flask-Dance-7.0.0/flask_dance/contrib/spotify.py
+-rw-r--r--   0        0        0     4040 2023-01-19 21:47:16.256686 Flask-Dance-7.0.0/flask_dance/contrib/strava.py
+-rw-r--r--   0        0        0     4191 2023-01-19 21:47:16.256940 Flask-Dance-7.0.0/flask_dance/contrib/twitch.py
+-rw-r--r--   0        0        0     5262 2023-01-19 21:47:16.257400 Flask-Dance-7.0.0/flask_dance/contrib/zoho.py
+-rw-r--r--   0        0        0        0 2021-01-22 09:05:51.223263 Flask-Dance-7.0.0/flask_dance/fixtures/__init__.py
+-rw-r--r--   0        0        0     2977 2023-01-19 21:47:16.257722 Flask-Dance-7.0.0/flask_dance/fixtures/pytest.py
+-rw-r--r--   0        0        0     1051 2023-01-19 21:47:16.258015 Flask-Dance-7.0.0/flask_dance/utils.py
+-rw-r--r--   0        0        0     2106 2023-01-19 21:47:16.258262 Flask-Dance-7.0.0/pyproject.toml
+-rw-r--r--   0        0        0      336 2021-01-22 09:05:51.223660 Flask-Dance-7.0.0/tests/conftest.py
+-rw-r--r--   0        0        0    24645 2023-01-23 13:30:34.575100 Flask-Dance-7.0.0/tests/consumer/storage/test_sqla.py
+-rw-r--r--   0        0        0    18653 2023-01-19 21:47:16.259061 Flask-Dance-7.0.0/tests/consumer/test_oauth1.py
+-rw-r--r--   0        0        0    27910 2023-01-23 13:30:34.575576 Flask-Dance-7.0.0/tests/consumer/test_oauth2.py
+-rw-r--r--   0        0        0     2674 2023-01-19 21:47:16.259634 Flask-Dance-7.0.0/tests/consumer/test_requests.py
+-rw-r--r--   0        0        0     3886 2023-01-19 21:47:16.259853 Flask-Dance-7.0.0/tests/contrib/test_atlassian.py
+-rw-r--r--   0        0        0     3462 2023-01-19 21:47:16.260064 Flask-Dance-7.0.0/tests/contrib/test_authentiq.py
+-rw-r--r--   0        0        0     6313 2023-01-19 21:47:16.260296 Flask-Dance-7.0.0/tests/contrib/test_azure.py
+-rw-r--r--   0        0        0     2738 2023-05-10 18:22:19.223848 Flask-Dance-7.0.0/tests/contrib/test_dexcom.py
+-rw-r--r--   0        0        0     3256 2023-01-19 21:47:16.260510 Flask-Dance-7.0.0/tests/contrib/test_digitalocean.py
+-rw-r--r--   0        0        0     3646 2023-01-19 21:47:16.260817 Flask-Dance-7.0.0/tests/contrib/test_discord.py
+-rw-r--r--   0        0        0     3900 2023-01-19 21:47:16.261422 Flask-Dance-7.0.0/tests/contrib/test_dropbox.py
+-rw-r--r--   0        0        0     3767 2023-01-19 21:47:16.261690 Flask-Dance-7.0.0/tests/contrib/test_facebook.py
+-rw-r--r--   0        0        0     2736 2023-01-19 21:47:16.261913 Flask-Dance-7.0.0/tests/contrib/test_fitbit.py
+-rw-r--r--   0        0        0     2745 2023-01-19 21:47:16.262146 Flask-Dance-7.0.0/tests/contrib/test_github.py
+-rw-r--r--   0        0        0     5430 2023-01-19 21:47:16.262398 Flask-Dance-7.0.0/tests/contrib/test_gitlab.py
+-rw-r--r--   0        0        0     6617 2023-01-19 21:47:16.262635 Flask-Dance-7.0.0/tests/contrib/test_google.py
+-rw-r--r--   0        0        0     2724 2023-01-19 21:47:16.262864 Flask-Dance-7.0.0/tests/contrib/test_heroku.py
+-rw-r--r--   0        0        0     6500 2023-01-19 21:47:16.263121 Flask-Dance-7.0.0/tests/contrib/test_jira.py
+-rw-r--r--   0        0        0     2827 2023-01-19 21:47:16.263357 Flask-Dance-7.0.0/tests/contrib/test_linkedin.py
+-rw-r--r--   0        0        0     2917 2023-01-19 21:47:16.263583 Flask-Dance-7.0.0/tests/contrib/test_meetup.py
+-rw-r--r--   0        0        0     2752 2023-01-19 21:47:16.263796 Flask-Dance-7.0.0/tests/contrib/test_nylas.py
+-rw-r--r--   0        0        0     3343 2023-01-19 21:47:16.264063 Flask-Dance-7.0.0/tests/contrib/test_orcid.py
+-rw-r--r--   0        0        0     2709 2023-01-19 21:47:16.264319 Flask-Dance-7.0.0/tests/contrib/test_osm.py
+-rw-r--r--   0        0        0     3476 2023-01-19 21:47:16.264561 Flask-Dance-7.0.0/tests/contrib/test_reddit.py
+-rw-r--r--   0        0        0     5461 2023-01-19 21:47:16.264802 Flask-Dance-7.0.0/tests/contrib/test_salesforce.py
+-rw-r--r--   0        0        0     7471 2023-01-19 21:47:16.265127 Flask-Dance-7.0.0/tests/contrib/test_slack.py
+-rw-r--r--   0        0        0     2799 2023-01-19 21:47:16.265350 Flask-Dance-7.0.0/tests/contrib/test_spotify.py
+-rw-r--r--   0        0        0     2767 2023-01-19 21:47:16.265590 Flask-Dance-7.0.0/tests/contrib/test_strava.py
+-rw-r--r--   0        0        0     2986 2023-01-19 21:47:16.265796 Flask-Dance-7.0.0/tests/contrib/test_twitch.py
+-rw-r--r--   0        0        0     2584 2023-01-19 21:47:16.266226 Flask-Dance-7.0.0/tests/contrib/test_zoho.py
+-rw-r--r--   0        0        0     2606 2021-01-22 09:05:51.225870 Flask-Dance-7.0.0/tests/fixtures/cassettes/test_home_page.json
+-rw-r--r--   0        0        0     1510 2023-01-19 21:47:16.266618 Flask-Dance-7.0.0/tests/fixtures/test_pytest.py
+-rw-r--r--   0        0        0      686 2023-01-19 21:47:16.266818 Flask-Dance-7.0.0/tests/test_utils.py
+-rw-r--r--   0        0        0     6861 1970-01-01 00:00:00.000000 Flask-Dance-7.0.0/PKG-INFO
```

### Comparing `Flask-Dance-6.2.0/.github/workflows/docs.yml` & `Flask-Dance-7.0.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/.github/workflows/lint.yml` & `Flask-Dance-7.0.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/.github/workflows/test.yml` & `Flask-Dance-7.0.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/CHANGELOG.rst` & `Flask-Dance-7.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 Changelog
 =========
 
 `unreleased`_
 -------------
 nothing yet
 
+`7.0.0`_ (2023-05-10)
+---------------------
+* Removed Twitter pre-set configuration
+* Added Dexcom pre-set configuration
+* Added support for authorization flow with PKCE_
+
 `6.2.0`_ (2022-10-12)
 ---------------------
 * Added ORCID and ORCID sandbox provider
 * Switched from setuptools to flit_ for packaging
 
 `6.1.1`_ (2022-08-22)
 ---------------------
@@ -391,17 +397,18 @@
 .. _issue 53: https://github.com/singingwolfboy/flask-dance/issues/53
 .. _issue 149: https://github.com/singingwolfboy/flask-dance/issues/149
 .. _#143: https://github.com/singingwolfboy/flask-dance/issues/143
 .. _#144: https://github.com/singingwolfboy/flask-dance/issues/144
 .. _#161: https://github.com/singingwolfboy/flask-dance/issues/161
 .. _isort: https://pycqa.github.io/isort/
 .. _flit: https://flit.pypa.io/
+.. _PKCE: https://www.rfc-editor.org/rfc/rfc7636
 
-
-.. _unreleased: https://github.com/singingwolfboy/flask-dance/compare/v6.2.0...HEAD
+.. _unreleased: https://github.com/singingwolfboy/flask-dance/compare/v7.0.0...HEAD
+.. _7.0.0: https://github.com/singingwolfboy/flask-dance/compare/v6.2.0...v7.0.0
 .. _6.2.0: https://github.com/singingwolfboy/flask-dance/compare/v6.1.1...v6.2.0
 .. _6.1.1: https://github.com/singingwolfboy/flask-dance/compare/v6.1.0...v6.1.1
 .. _6.1.0: https://github.com/singingwolfboy/flask-dance/compare/v6.0.0...v6.1.0
 .. _6.0.0: https://github.com/singingwolfboy/flask-dance/compare/v5.1.0...v6.0.0
 .. _5.1.0: https://github.com/singingwolfboy/flask-dance/compare/v5.0.0...v5.1.0
 .. _5.0.0: https://github.com/singingwolfboy/flask-dance/compare/v4.0.0...v5.0.0
 .. _4.0.0: https://github.com/singingwolfboy/flask-dance/compare/v3.3.1...v4.0.0
```

### Comparing `Flask-Dance-6.2.0/LICENSE` & `Flask-Dance-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/README.rst` & `Flask-Dance-7.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/Makefile` & `Flask-Dance-7.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/_static/flask-dance.pdf` & `Flask-Dance-7.0.0/docs/_static/flask-dance.pdf`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/_static/flask-dance.png` & `Flask-Dance-7.0.0/docs/_static/flask-dance.png`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/_static/flask-dance.svg` & `Flask-Dance-7.0.0/docs/_static/flask-dance.svg`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/api.rst` & `Flask-Dance-7.0.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/concepts.rst` & `Flask-Dance-7.0.0/docs/concepts.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/conf.py` & `Flask-Dance-7.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/contributing.rst` & `Flask-Dance-7.0.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/examples.rst` & `Flask-Dance-7.0.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/how-oauth-works.rst` & `Flask-Dance-7.0.0/docs/how-oauth-works.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 OAuth uses a series of specially-crafted HTTP views and redirects to allow
 websites to share information with each other securely, and with the user's
 consent [#oauth-user]_. There are four roles in an OAuth interaction:
 
 provider
     A website that has information about a user. Well-known OAuth providers
-    include Google, Facebook, Twitter, etc.
+    include Google, Facebook, GitHub etc.
 consumer
     A website that wants to obtain some information about a user from the
     provider.
 user
     An actual person who controls information stored with the provider.
 client
     A program (usually a web browser) that interacts with the provider and
@@ -106,15 +106,15 @@
         Consumer --> Provider [label = "send client secret\n& authorization code"];
         Consumer <-- Provider [label = "return access token"];
         Client <-- Consumer [label = "render page or redirect"];
     }
 
 1.  The client visits the consumer at a special URL, indicating that they
     want to connect to the provider with OAuth. Typically, there is a button
-    on the consumer's website labeled "Log In with Twitter" or similar, which
+    on the consumer's website labeled "Log In with Google" or similar, which
     takes the user to this special URL.
 
 2.  The consumer tells the provider that they're about to do the OAuth dance.
     The consumer gives the provider the client secret, to verify that
     everything's cool. The provider checks the OAuth secret, and if it
     looks good, the provider makes up a new secret called a
     "request token", and gives it to the consumer.
```

### Comparing `Flask-Dance-6.2.0/docs/index.rst` & `Flask-Dance-7.0.0/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         resp = github.get("/user")
         assert resp.ok
         return "You are @{login} on GitHub".format(login=resp.json()["login"])
 
 Ready to get started?
 
 .. _Flask: http://flask.pocoo.org/
-.. _requests: http://python-requests.org/
+.. _requests: https://requests.readthedocs.io/
 .. _oauthlib: https://oauthlib.readthedocs.io/
 
 User Guide
 ----------
 
 .. toctree::
    :maxdepth: 1
```

### Comparing `Flask-Dance-6.2.0/docs/logout.rst` & `Flask-Dance-7.0.0/docs/logout.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/make.bat` & `Flask-Dance-7.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/multi-user.rst` & `Flask-Dance-7.0.0/docs/multi-user.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/providers.rst` & `Flask-Dance-7.0.0/docs/providers.rst`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,26 @@
 
 .. data:: azure
 
     A :class:`~werkzeug.local.LocalProxy` to a :class:`requests.Session` that
     already has the Azure AD authentication token loaded (assuming that the user
     has authenticated with Azure AD at some point in the past).
 
+Dexcom
+------
+.. module:: flask_dance.contrib.dexcom
+
+.. autofunction:: make_dexcom_blueprint
+
+.. data:: dexcom
+
+    A :class:`~werkzeug.local.LocalProxy` to a :class:`requests.Session` that
+    already has the Dexcom authentication token loaded (assuming that the user
+    has authenticated with Dexcom at some point in the past).
+
 Digital Ocean
 -------------
 .. module:: flask_dance.contrib.digitalocean
 
 .. autofunction:: make_digitalocean_blueprint
 
 .. data:: digitalocean
@@ -220,15 +232,15 @@
 .. module:: flask_dance.contrib.orcid
 
 .. autofunction:: make_orcid_blueprint
 
 .. data:: orcid
 
     A :class:`~werkzeug.local.LocalProxy` to a :class:`requests.Session` that
-    already has the ORCID (or sandbox ORCID) authentication token loaded (assuming 
+    already has the ORCID (or sandbox ORCID) authentication token loaded (assuming
     that the user has authenticated with ORCID at some point in the past).
 
 Reddit
 ------
 .. module:: flask_dance.contrib.reddit
 
 .. autofunction:: make_reddit_blueprint
@@ -283,26 +295,14 @@
 
 .. data:: twitch
 
     A :class:`~werkzeug.local.LocalProxy` to a :class:`requests.Session` that
     already has the Twitch authentication token loaded (assuming that the user
     has authenticated with Twitch at some point in the past).
 
-Twitter
--------
-.. module:: flask_dance.contrib.twitter
-
-.. autofunction:: make_twitter_blueprint
-
-.. data:: twitter
-
-    A :class:`~werkzeug.local.LocalProxy` to a :class:`requests.Session` that
-    already has the Twitter authentication token loaded (assuming that the user
-    has authenticated with Twitter at some point in the past).
-
 Spotify
 -------
 .. module:: flask_dance.contrib.spotify
 
 .. autofunction:: make_spotify_blueprint
 
 .. data:: spotify
```

### Comparing `Flask-Dance-6.2.0/docs/proxies.rst` & `Flask-Dance-7.0.0/docs/proxies.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/quickstart.rst` & `Flask-Dance-7.0.0/docs/quickstart.rst`

 * *Files 3% similar despite different names*

```diff
@@ -24,25 +24,23 @@
 Flask sessions (easiest)
 ------------------------
 
 * `GitHub <https://github.com/singingwolfboy/flask-dance-github>`__
 * `Google <https://github.com/singingwolfboy/flask-dance-google>`__
 * `Facebook <https://github.com/singingwolfboy/flask-dance-facebook>`__
 * `Slack <https://github.com/singingwolfboy/flask-dance-slack>`__
-* `Twitter <https://github.com/singingwolfboy/flask-dance-twitter>`__
 * `LinkedIn <https://github.com/singingwolfboy/flask-dance-linkedin>`__
 * `Heroku <https://github.com/singingwolfboy/flask-dance-heroku>`__
 * `Fitbit <https://github.com/lila/flask-dance-fitbit>`__
 
 SQLAlchemy
 ----------
 
 * `Google <https://github.com/singingwolfboy/flask-dance-google-sqla>`__
 * `Google with Flask-Security <https://github.com/singingwolfboy/flask-dance-google-security-sqla>`__
-* `Twitter <https://github.com/singingwolfboy/flask-dance-twitter-sqla>`__
 * `Facebook <https://github.com/singingwolfboy/flask-dance-facebook-sqla>`__
 * `Heroku <https://github.com/singingwolfboy/flask-dance-heroku-sqla>`__
 * `Multiple providers simultaneously <https://github.com/singingwolfboy/flask-dance-multi-provider>`__
 
 .. admonition:: Other Providers
 
     Don't see the OAuth provider you want? Flask-Dance provides
```

### Comparing `Flask-Dance-6.2.0/docs/signals.rst` & `Flask-Dance-7.0.0/docs/signals.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/spelling_wordlist.txt` & `Flask-Dance-7.0.0/docs/spelling_wordlist.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 initializer
 
 Authentiq
 authentiq
 Azure
 Discord
 Dropbox
+Dexcom
 DigitalOcean
 Facebook
 GitHub
 GitLab
 Google
 Heroku
 Jira
```

### Comparing `Flask-Dance-6.2.0/docs/storages.rst` & `Flask-Dance-7.0.0/docs/storages.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/testing.rst` & `Flask-Dance-7.0.0/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/docs/understanding-the-magic.rst` & `Flask-Dance-7.0.0/docs/understanding-the-magic.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/base.py` & `Flask-Dance-7.0.0/flask_dance/consumer/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         url_defaults=None,
         root_path=None,
         login_url=None,
         authorized_url=None,
         storage=None,
         rule_kwargs=None,
     ):
-
         bp_kwargs = dict(
             name=name,
             import_name=import_name,
             static_folder=static_folder,
             static_url_path=static_url_path,
             template_folder=template_folder,
             url_prefix=url_prefix,
@@ -142,15 +141,15 @@
 
     @token.setter
     def token(self, value):
         _token = value
         if _token and _token.get("expires_in"):
             # Set the `expires_at` value, overwriting any value
             # that may already be there.
-            delta = timedelta(seconds=_token["expires_in"])
+            delta = timedelta(seconds=int(_token["expires_in"]))
             expires_at = datetime.utcnow() + delta
             _token["expires_at"] = expires_at.replace(tzinfo=timezone.utc).timestamp()
         self.storage.set(self, _token)
         try:
             del self.session.token
         except KeyError:
             pass
@@ -163,24 +162,24 @@
         except KeyError:
             pass
 
     @abstractproperty
     def session(self):
         """
         This is a session between the consumer (your website) and the provider
-        (e.g. Twitter). It is *not* a session between a user of your website
+        (e.g. Google). It is *not* a session between a user of your website
         and your website.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def login(self):
         raise NotImplementedError()
 
     @abstractmethod
     def authorized(self):
         """
         This is the route/function that the user will be redirected to by
-        the provider (e.g. Twitter) after the user has logged into the
+        the provider (e.g. Google) after the user has logged into the
         provider's website and authorized your app to access their account.
         """
         raise NotImplementedError()
```

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/oauth1.py` & `Flask-Dance-7.0.0/flask_dance/consumer/oauth1.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         authorization_url=None,
         access_token_url=None,
         redirect_url=None,
         redirect_to=None,
         session_class=None,
         storage=None,
         rule_kwargs=None,
-        **kwargs
+        **kwargs,
     ):
         """
         Most of the constructor arguments are forwarded either to the
         :class:`flask.Blueprint` constructor or the
         :class:`requests_oauthlib.OAuth1Session` constructor, including
         ``**kwargs`` (which is forwarded to
         :class:`~requests_oauthlib.OAuth1Session`).
@@ -99,15 +99,15 @@
             redirect_to: When the OAuth dance is complete,
                 redirect the user to the URL obtained by calling
                 :func:`~flask.url_for` with this argument. If you do not specify
                 either ``redirect_url`` or ``redirect_to``, the user will be
                 redirected to the root path (``/``).
             session_class: The class to use for creating a Requests session
                 between the consumer (your website) and the provider (e.g.
-                Twitter). Defaults to
+                Google). Defaults to
                 :class:`~flask_dance.consumer.requests.OAuth1Session`.
             storage: A token storage class, or an instance of a token storage
                 class, to use for this blueprint. Defaults to
                 :class:`~flask_dance.consumer.storage.session.SessionStorage`.
             rule_kwargs (dict, optional): Additional arguments that should be passed when adding
                 the login and authorized routes. Defaults to ``None``.
         """
@@ -150,29 +150,29 @@
 
         self.teardown_app_request(self.teardown_session)
 
     @cached_property
     def session(self):
         """
         This is a session between the consumer (your website) and the provider
-        (e.g. Twitter). It is *not* a session between a user of your website
+        (e.g. Google). It is *not* a session between a user of your website
         and your website.
         :return:
         """
         return self.session_class(
             client_key=self.client_key,
             client_secret=self.client_secret,
             signature_method=self.signature_method,
             signature_type=self.signature_type,
             rsa_key=self.rsa_key,
             client_class=self.client_class,
             force_include_body=self.force_include_body,
             blueprint=self,
             base_url=self.base_url,
-            **self.kwargs
+            **self.kwargs,
         )
 
     def teardown_session(self, exception=None):
         try:
             del self.session
         except KeyError:
             pass
@@ -202,15 +202,15 @@
         url = self.session.authorization_url(self.authorization_url)
         oauth_before_login.send(self, url=url)
         return redirect(url)
 
     def authorized(self):
         """
         This is the route/function that the user will be redirected to by
-        the provider (e.g. Twitter) after the user has logged into the
+        the provider (e.g. Google) after the user has logged into the
         provider's website and authorized your app to access their account.
         """
         if self.redirect_url:
             next_url = self.redirect_url
         elif self.redirect_to:
             next_url = url_for(self.redirect_to)
         else:
```

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/oauth2.py` & `Flask-Dance-7.0.0/flask_dance/consumer/oauth2.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 import logging
 
 import flask
 from flask import current_app, redirect, request, url_for
+from oauthlib.common import generate_token
 from oauthlib.oauth2 import MissingCodeError
 from werkzeug.utils import cached_property
 from werkzeug.wrappers import Response
 
 from .base import (
     BaseOAuthConsumerBlueprint,
     oauth_authorized,
@@ -50,14 +51,16 @@
         token_url=None,
         token_url_params=None,
         redirect_url=None,
         redirect_to=None,
         session_class=None,
         storage=None,
         rule_kwargs=None,
+        use_pkce=False,
+        code_challenge_method="S256",
         **kwargs,
     ):
         """
         Most of the constructor arguments are forwarded either to the
         :class:`flask.Blueprint` constructor or the
         :class:`requests_oauthlib.OAuth2Session` constructor, including
         ``**kwargs`` (which is forwarded to
@@ -103,21 +106,26 @@
             redirect_to: When the OAuth dance is complete,
                 redirect the user to the URL obtained by calling
                 :func:`~flask.url_for` with this argument. If you do not specify
                 either ``redirect_url`` or ``redirect_to``, the user will be
                 redirected to the root path (``/``).
             session_class: The class to use for creating a Requests session
                 between the consumer (your website) and the provider (e.g.
-                Twitter). Defaults to
+                Google). Defaults to
                 :class:`~flask_dance.consumer.requests.OAuth2Session`.
             storage: A token storage class, or an instance of a token storage
                 class, to use for this blueprint. Defaults to
                 :class:`~flask_dance.consumer.storage.session.SessionStorage`.
             rule_kwargs (dict, optional): Additional arguments that should be passed when adding
                 the login and authorized routes. Defaults to ``None``.
+            use_pkce: If true then the authorization flow will follow the PKCE (Proof Key for Code Exchange).
+                For more details please refer to `RFC7636 <https://www.rfc-editor.org/rfc/rfc7636#section-4.1>`__
+            code_challenge_method: Code challenge method to be used in authorization code flow with PKCE
+                instead of client secret. It will be used only if ``use_pkce`` is set to True.
+                Defaults to ``S256``.
         """
         BaseOAuthConsumerBlueprint.__init__(
             self,
             name,
             import_name,
             static_folder=static_folder,
             static_url_path=static_url_path,
@@ -148,14 +156,16 @@
         # used by view functions
         self.authorization_url = authorization_url
         self.authorization_url_params = authorization_url_params or {}
         self.token_url = token_url
         self.token_url_params = token_url_params or {}
         self.redirect_url = redirect_url
         self.redirect_to = redirect_to
+        self.code_challenge_method = code_challenge_method
+        self.use_pkce = use_pkce
 
         self.teardown_app_request(self.teardown_session)
 
     @property
     def client_id(self):
         return self.session.client_id
 
@@ -165,15 +175,15 @@
         # due to a bug in requests-oauthlib, we need to set this manually
         self.session._client.client_id = value
 
     @cached_property
     def session(self):
         """
         This is a session between the consumer (your website) and the provider
-        (e.g. Twitter). It is *not* a session between a user of your website
+        (e.g. Google). It is *not* a session between a user of your website
         and your website.
         :return:
         """
         ret = self.session_class(
             client_id=self._client_id,
             client=self.client,
             auto_refresh_url=self.auto_refresh_url,
@@ -199,28 +209,44 @@
             del self.session
         except KeyError:
             pass
 
     def login(self):
         log.debug("client_id = %s", self.client_id)
         self.session.redirect_uri = url_for(".authorized", _external=True)
+        if self.use_pkce:
+            code_verifier = generate_token(length=48)
+            code_challenge = self.session._client.create_code_challenge(
+                code_verifier=code_verifier,
+                code_challenge_method=self.code_challenge_method,
+            )
+            self.authorization_url_params.update(
+                {
+                    "code_challenge_method": self.code_challenge_method,
+                    "code_challenge": code_challenge,
+                }
+            )
+            code_verifier_key = f"{self.name}_oauth_code_verifier"
+            flask.session[code_verifier_key] = code_verifier
+            log.debug("code_verifier = %s", code_verifier)
+
         url, state = self.session.authorization_url(
             self.authorization_url, state=self.state, **self.authorization_url_params
         )
         state_key = f"{self.name}_oauth_state"
         flask.session[state_key] = state
         log.debug("state = %s", state)
         log.debug("redirect URL = %s", url)
         oauth_before_login.send(self, url=url)
         return redirect(url)
 
     def authorized(self):
         """
         This is the route/function that the user will be redirected to by
-        the provider (e.g. Twitter) after the user has logged into the
+        the provider (e.g. Google) after the user has logged into the
         provider's website and authorized your app to access their account.
         """
         if self.redirect_url:
             next_url = self.redirect_url
         elif self.redirect_to:
             next_url = url_for(self.redirect_to)
         else:
@@ -250,14 +276,26 @@
             return redirect(url_for(".login"))
 
         state = flask.session[state_key]
         log.debug("state = %s", state)
         self.session._state = state
         del flask.session[state_key]
 
+        if self.use_pkce:
+            code_verifier_key = f"{self.name}_oauth_code_verifier"
+            if code_verifier_key not in flask.session:
+                # can't find code_verifier, so redirect back to login view
+                log.info("code_verifier not found, redirecting user to login")
+                return redirect(url_for(".login"))
+
+            code_verifier = flask.session[code_verifier_key]
+            log.debug("code_verifier = %s", code_verifier)
+            del flask.session[code_verifier_key]
+            self.token_url_params["code_verifier"] = code_verifier
+
         self.session.redirect_uri = url_for(".authorized", _external=True)
 
         log.debug("client_id = %s", self.client_id)
         log.debug("client_secret = %s", self.client_secret)
         try:
             token = self.session.fetch_token(
                 self.token_url,
```

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/requests.py` & `Flask-Dance-7.0.0/flask_dance/consumer/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
     * lazy-loads OAuth1 tokens from the storage via the blueprint
     * handles OAuth1 authentication
       (from :class:`requests_oauthlib.OAuth1Session` superclass)
     * has a ``base_url`` property used for relative URL resolution
 
     Note that this is a session between the consumer (your website) and the
-    provider (e.g. Twitter), and *not* a session between a user of your website
+    provider (e.g. Google), and *not* a session between a user of your website
     and your website.
     """
 
     def __init__(self, blueprint=None, base_url=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.blueprint = blueprint
         self.base_url = URLObject(base_url)
@@ -43,15 +43,15 @@
             self.auth.client.resource_owner_secret = to_unicode(t["oauth_token_secret"])
             return True
         return False
 
     @property
     def authorized(self):
         """This is the property used when you have a statement in your code
-        that reads "if <provider>.authorized:", e.g. "if twitter.authorized:".
+        that reads "if <provider>.authorized:", e.g. "if google.authorized:".
 
         The way it works is kind of complicated: this function just tries
         to load the token, and then the 'super()' statement basically just
         tests if the token exists (see BaseOAuth1Session.authorized).
 
         To load the token, it calls the load_token() function within this class,
         which in turn checks the 'token' property of this class (another
@@ -107,15 +107,15 @@
 
     * lazy-loads OAuth2 tokens from the storage via the blueprint
     * handles OAuth2 authentication
       (from :class:`requests_oauthlib.OAuth2Session` superclass)
     * has a ``base_url`` property used for relative URL resolution
 
     Note that this is a session between the consumer (your website) and the
-    provider (e.g. Twitter), and *not* a session between a user of your website
+    provider (e.g. Google), and *not* a session between a user of your website
     and your website.
     """
 
     def __init__(self, blueprint=None, base_url=None, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.blueprint = blueprint
         self.base_url = URLObject(base_url)
@@ -141,15 +141,15 @@
         Returns the ``access_token`` from the OAuth token.
         """
         return self.token and self.token.get("access_token")
 
     @property
     def authorized(self):
         """This is the property used when you have a statement in your code
-        that reads "if <provider>.authorized:", e.g. "if twitter.authorized:".
+        that reads "if <provider>.authorized:", e.g. "if google.authorized:".
 
         The way it works is kind of complicated: this function just tries
         to load the token, and then the 'super()' statement basically just
         tests if the token exists (see BaseOAuth1Session.authorized).
 
         To load the token, it calls the load_token() function within this class,
         which in turn checks the 'token' property of this class (another
```

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/storage/__init__.py` & `Flask-Dance-7.0.0/flask_dance/consumer/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/storage/session.py` & `Flask-Dance-7.0.0/flask_dance/consumer/storage/session.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/consumer/storage/sqla.py` & `Flask-Dance-7.0.0/flask_dance/consumer/storage/sqla.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             uid = getattr(u, "id", u)
         return "flask_dance_token|{name}|{user_id}".format(
             name=blueprint.name, user_id=uid
         )
 
     def get(self, blueprint, user=None, user_id=None):
         """When you have a statement in your code that says
-        "if <provider>.authorized:" (for example "if twitter.authorized:"),
+        "if <provider>.authorized:" (for example "if google.authorized:"),
         a long string of function calls result in this function being used to
         check the Flask server's cache and database for any records associated
         with the current_user. The `user` and `user_id` parameters are actually
         not set in that case (see base.py:token(), that's what calls this
         function), so the user information is instead loaded from the
         current_user (if that's what you specified when you created the
         blueprint) with blueprint.config.get('user_id').
```

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/README.rst` & `Flask-Dance-7.0.0/flask_dance/contrib/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/atlassian.py` & `Flask-Dance-7.0.0/flask_dance/contrib/atlassian.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/authentiq.py` & `Flask-Dance-7.0.0/flask_dance/contrib/authentiq.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/azure.py` & `Flask-Dance-7.0.0/flask_dance/contrib/azure.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/digitalocean.py` & `Flask-Dance-7.0.0/flask_dance/contrib/digitalocean.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/discord.py` & `Flask-Dance-7.0.0/flask_dance/contrib/discord.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/dropbox.py` & `Flask-Dance-7.0.0/flask_dance/contrib/dropbox.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/facebook.py` & `Flask-Dance-7.0.0/flask_dance/contrib/facebook.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/fitbit.py` & `Flask-Dance-7.0.0/flask_dance/contrib/fitbit.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/github.py` & `Flask-Dance-7.0.0/flask_dance/contrib/github.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/gitlab.py` & `Flask-Dance-7.0.0/flask_dance/contrib/gitlab.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/google.py` & `Flask-Dance-7.0.0/flask_dance/contrib/google.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/heroku.py` & `Flask-Dance-7.0.0/flask_dance/contrib/heroku.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/jira.py` & `Flask-Dance-7.0.0/flask_dance/contrib/jira.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/linkedin.py` & `Flask-Dance-7.0.0/flask_dance/contrib/linkedin.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/meetup.py` & `Flask-Dance-7.0.0/flask_dance/contrib/meetup.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/nylas.py` & `Flask-Dance-7.0.0/flask_dance/contrib/nylas.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/orcid.py` & `Flask-Dance-7.0.0/flask_dance/contrib/orcid.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/osm.py` & `Flask-Dance-7.0.0/flask_dance/contrib/osm.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/reddit.py` & `Flask-Dance-7.0.0/flask_dance/contrib/reddit.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/salesforce.py` & `Flask-Dance-7.0.0/flask_dance/contrib/salesforce.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/slack.py` & `Flask-Dance-7.0.0/flask_dance/contrib/slack.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/spotify.py` & `Flask-Dance-7.0.0/flask_dance/contrib/spotify.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/strava.py` & `Flask-Dance-7.0.0/flask_dance/contrib/strava.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/twitch.py` & `Flask-Dance-7.0.0/flask_dance/contrib/twitch.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/twitter.py` & `Flask-Dance-7.0.0/flask_dance/contrib/dexcom.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 from flask import g
 from werkzeug.local import LocalProxy
 
-from flask_dance.consumer import OAuth1ConsumerBlueprint
+from flask_dance.consumer import OAuth2ConsumerBlueprint
 
-__maintainer__ = "David Baumgold <david@davidbaumgold.com>"
+__maintainer__ = "Karan Bhatia <karan.bhatia@gmail.com>"
 
 
-def make_twitter_blueprint(
-    api_key=None,
-    api_secret=None,
+def make_dexcom_blueprint(
+    client_id=None,
+    client_secret=None,
     *,
+    base_url="https://api.dexcom.com/",
+    scope="offline_access",
     redirect_url=None,
     redirect_to=None,
     login_url=None,
     authorized_url=None,
     session_class=None,
     storage=None,
     rule_kwargs=None,
 ):
     """
-    Make a blueprint for authenticating with Twitter using OAuth 1. This requires
-    an API key and API secret from Twitter. You should either pass them to
+    Make a blueprint for authenticating with Dexcom using OAuth 2. This requires
+    a client ID and client secret from Dexcom. You should either pass them to
     this constructor, or make sure that your Flask application config defines
-    them, using the variables :envvar:`TWITTER_OAUTH_CLIENT_KEY` and
-    :envvar:`TWITTER_OAUTH_CLIENT_SECRET`.
+    them, using the variables :envvar:`DEXCOM_OAUTH_CLIENT_ID` and
+    :envvar:`DEXCOM_OAUTH_CLIENT_SECRET`.
 
     Args:
-        api_key (str): The API key for your Twitter application
-        api_secret (str): The API secret for your Twitter application
+        client_id (str): The client ID for your application on Dexcom.
+        client_secret (str): The client secret for your application on Dexcom
+        scope (str, optional): comma-separated list of scopes for the OAuth token
         redirect_url (str): the URL to redirect to after the authentication
             dance is complete
         redirect_to (str): if ``redirect_url`` is not defined, the name of the
             view to redirect to after the authentication dance is complete.
             The actual URL will be determined by :func:`flask.url_for`
         login_url (str, optional): the URL path for the ``login`` view.
-            Defaults to ``/twitter``
+            Defaults to ``/dexcom``
         authorized_url (str, optional): the URL path for the ``authorized`` view.
-            Defaults to ``/twitter/authorized``.
+            Defaults to ``/dexcom/authorized``.
         session_class (class, optional): The class to use for creating a
             Requests session. Defaults to
-            :class:`~flask_dance.consumer.requests.OAuth1Session`.
+            :class:`~flask_dance.consumer.requests.OAuth2Session`.
         storage: A token storage class, or an instance of a token storage
                 class, to use for this blueprint. Defaults to
                 :class:`~flask_dance.consumer.storage.session.SessionStorage`.
         rule_kwargs (dict, optional): Additional arguments that should be passed when adding
             the login and authorized routes. Defaults to ``None``.
 
-    :rtype: :class:`~flask_dance.consumer.OAuth1ConsumerBlueprint`
+    :rtype: :class:`~flask_dance.consumer.OAuth2ConsumerBlueprint`
     :returns: A :doc:`blueprint <flask:blueprints>` to attach to your Flask app.
     """
-    twitter_bp = OAuth1ConsumerBlueprint(
-        "twitter",
+    dexcom_bp = OAuth2ConsumerBlueprint(
+        "dexcom",
         __name__,
-        client_key=api_key,
-        client_secret=api_secret,
-        base_url="https://api.twitter.com/1.1/",
-        request_token_url="https://api.twitter.com/oauth/request_token",
-        access_token_url="https://api.twitter.com/oauth/access_token",
-        authorization_url="https://api.twitter.com/oauth/authorize",
+        client_id=client_id,
+        client_secret=client_secret,
+        scope=scope,
+        base_url=base_url,
+        authorization_url="https://api.dexcom.com/v2/oauth2/login",
+        token_url="https://api.dexcom.com/v2/oauth2/token",
         redirect_url=redirect_url,
         redirect_to=redirect_to,
         login_url=login_url,
         authorized_url=authorized_url,
         session_class=session_class,
         storage=storage,
         rule_kwargs=rule_kwargs,
     )
-    twitter_bp.from_config["client_key"] = "TWITTER_OAUTH_CLIENT_KEY"
-    twitter_bp.from_config["client_secret"] = "TWITTER_OAUTH_CLIENT_SECRET"
+    dexcom_bp.from_config["client_id"] = "DEXCOM_OAUTH_CLIENT_ID"
+    dexcom_bp.from_config["client_secret"] = "DEXCOM_OAUTH_CLIENT_SECRET"
+    dexcom_bp.auto_refresh_url = dexcom_bp.token_url
 
-    @twitter_bp.before_app_request
+    @dexcom_bp.before_app_request
     def set_applocal_session():
-        g.flask_dance_twitter = twitter_bp.session
+        g.flask_dance_dexcom = dexcom_bp.session
 
-    return twitter_bp
+    return dexcom_bp
 
 
-twitter = LocalProxy(lambda: g.flask_dance_twitter)
+dexcom = LocalProxy(lambda: g.flask_dance_dexcom)
```

### Comparing `Flask-Dance-6.2.0/flask_dance/contrib/zoho.py` & `Flask-Dance-7.0.0/flask_dance/contrib/zoho.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/fixtures/pytest.py` & `Flask-Dance-7.0.0/flask_dance/fixtures/pytest.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/flask_dance/utils.py` & `Flask-Dance-7.0.0/flask_dance/utils.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/pyproject.toml` & `Flask-Dance-7.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "Flask-Dance"
 authors = [{ name = "David Baumgold", email = "david@davidbaumgold.com" }]
+maintainers = [{ name = "Daniele Sluijters" }]
 readme = "README.rst"
 dynamic = ["description", "version"]
 license = { file = "LICENSE" }
 requires-python = ">=3.6"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Framework :: Flask",
@@ -18,15 +19,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "requests>=2.0",
-    "oauthlib",
+    "oauthlib>=3.2",
     "requests-oauthlib>=1.0.0",
     "Flask>=2.0.3",
     "Werkzeug",
     "urlobject",
 ]
 
 [project.urls]
@@ -56,15 +57,15 @@
     "sphinxcontrib-seqdiag",
     "sphinxcontrib-spelling",
     "Flask-Sphinx-Themes",
 
     # code dependencies, needed for imports
     "sqlalchemy>=1.3.11",
     "pytest",
-    "betamax"
+    "betamax",
 ]
 sqla = ["sqlalchemy>=1.3.11"]
 signals = ["blinker"]
 
 [project.entry-points.pytest11]
 pytest_flask_dance = "flask_dance.fixtures.pytest"
 
@@ -74,13 +75,11 @@
 [tool.distutils.bdist_wheel]
 universal = true
 
 [tool.isort]
 profile = "black"
 
 [tool.pytest.ini_options]
-markers = [
-    "install_required: can only pass if flask_dance is installed"
-]
+markers = ["install_required: can only pass if flask_dance is installed"]
 
 [tool.coverage.run]
 source = ["flask_dance"]
```

### Comparing `Flask-Dance-6.2.0/tests/consumer/storage/test_sqla.py` & `Flask-Dance-7.0.0/tests/consumer/storage/test_sqla.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 @pytest.fixture
 def app(blueprint, db, request):
     "Make a Flask app, attach Flask-SQLAlchemy, and establish an app context"
     app = flask.Flask(__name__)
     app.config["SQLALCHEMY_DATABASE_URI"] = os.environ.get("DATABASE_URI", "sqlite://")
     app.config["SQLALCHEMY_TRACK_MODIFICATIONS"] = False
-    app.config["CACHE_TYPE"] = "simple"
+    app.config["CACHE_TYPE"] = "SimpleCache"
     app.secret_key = "secret"
     app.register_blueprint(blueprint, url_prefix="/login")
     db.init_app(app)
     # establish app context
     ctx = app.app_context()
     ctx.push()
     request.addfinalizer(ctx.pop)
```

### Comparing `Flask-Dance-6.2.0/tests/consumer/test_oauth1.py` & `Flask-Dance-7.0.0/tests/consumer/test_oauth1.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/consumer/test_oauth2.py` & `Flask-Dance-7.0.0/tests/consumer/test_oauth2.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from urllib.parse import parse_qsl
 
 import flask
 import pytest
 import responses
 from freezegun import freeze_time
 from oauthlib.oauth2 import MissingCodeError
+from oauthlib.oauth2.rfc6749.clients import Client as OAuth2Client
 from urlobject import URLObject
 from werkzeug.middleware.proxy_fix import ProxyFix
 
 from flask_dance.consumer import (
     OAuth2ConsumerBlueprint,
     oauth_authorized,
     oauth_before_login,
@@ -23,27 +24,28 @@
 try:
     import blinker
 except ImportError:
     blinker = None
 requires_blinker = pytest.mark.skipif(not blinker, reason="requires blinker")
 
 
-def make_app(login_url=None, debug=False):
+def make_app(login_url=None, debug=False, **kwargs):
     blueprint = OAuth2ConsumerBlueprint(
         "test-service",
         __name__,
         client_id="client_id",
         client_secret="client_secret",
         scope="admin",
         state="random-string",
         base_url="https://example.com",
         authorization_url="https://example.com/oauth/authorize",
         token_url="https://example.com/oauth/access_token",
         redirect_to="index",
         login_url=login_url,
+        **kwargs,
     )
     app = flask.Flask(__name__)
     app.secret_key = "secret"
     app.register_blueprint(blueprint, url_prefix="/login")
     app.debug = debug
 
     @app.route("/")
@@ -87,14 +89,58 @@
         == "https://a.b.c/login/test-service/authorized"
     )
     assert location.query_dict["scope"] == "admin"
     assert location.query_dict["state"] == "random-string"
 
 
 @responses.activate
+def test_login_url_with_pkce():
+    _code_challenge_method = "S256"  # That should be a default value
+    app, _ = make_app(use_pkce=True)
+    with app.test_client() as client:
+        resp = client.get(
+            "/login/test-service", base_url="https://a.b.c", follow_redirects=False
+        )
+        # check that we saved the code verifier in the session
+        with client.session_transaction() as sess:
+            assert "test-service_oauth_code_verifier" in sess
+            _code_verifier = sess["test-service_oauth_code_verifier"]
+            assert 43 <= len(_code_verifier) <= 128  # RFC7636 section 4.1
+            _code_challenge = OAuth2Client("123").create_code_challenge(
+                _code_verifier, _code_challenge_method
+            )
+
+    # check that we redirected the client
+    assert resp.status_code == 302
+    location = URLObject(resp.headers["Location"])
+    assert location.without_query() == "https://example.com/oauth/authorize"
+    # check PKCE specific query parameters
+    assert location.query_dict["code_challenge_method"] == _code_challenge_method
+    assert location.query_dict["code_challenge"] == _code_challenge
+
+
+@responses.activate
+def test_login_url_with_invalid_code_challenge_method():
+    app, _ = make_app(use_pkce=True, code_challenge_method="MD5")
+    with app.test_client() as client:
+        resp = client.get(
+            "/login/test-service", base_url="https://a.b.c", follow_redirects=False
+        )
+        # the code verifier is saved in the session ...
+        with client.session_transaction() as sess:
+            assert "test-service_oauth_code_verifier" in sess
+
+    location = URLObject(resp.headers["Location"])
+    assert location.without_query() == "https://example.com/oauth/authorize"
+    # ... but because the "code challenge method" was invalid it was not added to the query parameters
+    assert "code_challenge_method" not in location.query_dict
+    assert "code_challenge" not in location.query_dict
+
+
+@responses.activate
 def test_login_url_forwarded_proto():
     app, _ = make_app()
     app.wsgi_app = ProxyFix(app.wsgi_app, x_proto=1)
     with app.test_client() as client:
         resp = client.get(
             "/login/test-service",
             base_url="http://a.b.c",
@@ -134,20 +180,19 @@
         assert len(responses.calls) == 1
         request_data = dict(parse_qsl(responses.calls[0].request.body))
         assert (
             request_data["redirect_uri"]
             == "https://a.b.c/login/test-service/authorized"
         )
         # check that we stored the access token in the session
-        with client.session_transaction() as sess:
-            assert sess["test-service_oauth_token"] == {
-                "access_token": "foobar",
-                "scope": ["admin"],
-                "token_type": "bearer",
-            }
+        assert flask.session["test-service_oauth_token"] == {
+            "access_token": "foobar",
+            "scope": ["admin"],
+            "token_type": "bearer",
+        }
 
 
 def test_authorized_url_no_state():
     app, _ = make_app()
     with app.test_client() as client:
         # make the request, without resetting the session beforehand
         resp = client.get(
@@ -157,16 +202,15 @@
         # check that we redirected the client back to login view
         assert resp.status_code == 302
         assert resp.headers["Location"] in (
             "https://a.b.c/login/test-service",
             "/login/test-service",
         )
         # check that there's nothing in the session
-        with client.session_transaction() as sess:
-            assert "test-service_oauth_token" not in sess
+        assert "test-service_oauth_token" not in flask.session
 
 
 @responses.activate
 def test_authorized_url_behind_proxy():
     responses.add(
         responses.POST,
         "https://example.com/oauth/access_token",
@@ -245,16 +289,75 @@
         # check that we stored the access token and expiration date in the session
         expected_stored_token = {
             "access_token": "foobar",
             "token_type": "bearer",
             "expires_in": 300,
             "expires_at": 1451649901,
         }
+        assert flask.session["test-service_oauth_token"] == expected_stored_token
+
+
+@responses.activate
+def test_authorized_url_with_pkce():
+    responses.add(
+        responses.POST,
+        "https://example.com/oauth/access_token",
+        body='{"access_token":"foobar","token_type":"bearer","scope":"admin"}',
+    )
+    app, _ = make_app(use_pkce=True)
+
+    _state = "random-string"
+    _code_verifier = "random-code-very-secure"
+    with app.test_client() as client:
+        # reset the session before the request
         with client.session_transaction() as sess:
-            assert sess["test-service_oauth_token"] == expected_stored_token
+            sess["test-service_oauth_state"] = _state
+            sess[f"test-service_oauth_code_verifier"] = _code_verifier
+        # make the request
+        resp = client.get(
+            f"/login/test-service/authorized?code=secret-code&state={_state}&code_verifier={_code_verifier}",
+            base_url="https://a.b.c",
+        )
+        # check that we redirected the client
+        assert resp.status_code == 302
+        assert resp.headers["Location"] in ("https://a.b.c/", "/")
+        # check that we obtained an access token
+        assert len(responses.calls) == 1
+        request_data = dict(parse_qsl(responses.calls[0].request.body))
+        assert (
+            request_data["redirect_uri"]
+            == "https://a.b.c/login/test-service/authorized"
+        )
+        assert request_data["code_verifier"] == _code_verifier
+        # check that we stored the access token in the session
+        assert flask.session["test-service_oauth_token"] == {
+            "access_token": "foobar",
+            "scope": ["admin"],
+            "token_type": "bearer",
+        }
+
+
+def test_authorized_url_pkce_flow_no_code_verifier():
+    app, _ = make_app(use_pkce=True)
+    with app.test_client() as client:
+        # make the request, without adding the code_verifier to the session
+        with client.session_transaction() as sess:
+            sess["test-service_oauth_state"] = "random-string"
+        resp = client.get(
+            "/login/test-service/authorized?code=secret-code&state=random-string",
+            base_url="https://a.b.c",
+        )
+        # check that we redirected the client back to login view
+        assert resp.status_code == 302
+        assert resp.headers["Location"] in (
+            "https://a.b.c/login/test-service",
+            "/login/test-service",
+        )
+        # check that there's nothing in the session
+        assert "test-service_oauth_token" not in flask.session
 
 
 def test_return_expired_token(request):
     app, bp = make_app()
     time1 = "2016-01-01 12:00:01"
     time2 = "2016-01-01 12:05:00"  # 299 sec in future
     time3 = "2016-01-01 12:10:01"  # 600 sec in future
```

### Comparing `Flask-Dance-6.2.0/tests/consumer/test_requests.py` & `Flask-Dance-7.0.0/tests/consumer/test_requests.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_atlassian.py` & `Flask-Dance-7.0.0/tests/contrib/test_atlassian.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_authentiq.py` & `Flask-Dance-7.0.0/tests/contrib/test_authentiq.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_azure.py` & `Flask-Dance-7.0.0/tests/contrib/test_azure.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_digitalocean.py` & `Flask-Dance-7.0.0/tests/contrib/test_digitalocean.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_discord.py` & `Flask-Dance-7.0.0/tests/contrib/test_discord.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_dropbox.py` & `Flask-Dance-7.0.0/tests/contrib/test_dropbox.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_facebook.py` & `Flask-Dance-7.0.0/tests/contrib/test_facebook.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_fitbit.py` & `Flask-Dance-7.0.0/tests/contrib/test_fitbit.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_github.py` & `Flask-Dance-7.0.0/tests/contrib/test_github.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_gitlab.py` & `Flask-Dance-7.0.0/tests/contrib/test_gitlab.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_google.py` & `Flask-Dance-7.0.0/tests/contrib/test_google.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_heroku.py` & `Flask-Dance-7.0.0/tests/contrib/test_heroku.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_jira.py` & `Flask-Dance-7.0.0/tests/contrib/test_jira.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_linkedin.py` & `Flask-Dance-7.0.0/tests/contrib/test_linkedin.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_meetup.py` & `Flask-Dance-7.0.0/tests/contrib/test_meetup.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_nylas.py` & `Flask-Dance-7.0.0/tests/contrib/test_nylas.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_orcid.py` & `Flask-Dance-7.0.0/tests/contrib/test_orcid.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_osm.py` & `Flask-Dance-7.0.0/tests/contrib/test_osm.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_reddit.py` & `Flask-Dance-7.0.0/tests/contrib/test_reddit.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_salesforce.py` & `Flask-Dance-7.0.0/tests/contrib/test_salesforce.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_slack.py` & `Flask-Dance-7.0.0/tests/contrib/test_slack.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_spotify.py` & `Flask-Dance-7.0.0/tests/contrib/test_spotify.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_strava.py` & `Flask-Dance-7.0.0/tests/contrib/test_strava.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_twitch.py` & `Flask-Dance-7.0.0/tests/contrib/test_twitch.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/contrib/test_zoho.py` & `Flask-Dance-7.0.0/tests/contrib/test_zoho.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/fixtures/cassettes/test_home_page.json` & `Flask-Dance-7.0.0/tests/fixtures/cassettes/test_home_page.json`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/fixtures/test_pytest.py` & `Flask-Dance-7.0.0/tests/fixtures/test_pytest.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/tests/test_utils.py` & `Flask-Dance-7.0.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `Flask-Dance-6.2.0/PKG-INFO` & `Flask-Dance-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: Flask-Dance
-Version: 6.2.0
+Version: 7.0.0
 Summary: Doing the OAuth dance with style using Flask, requests, and oauthlib
 Author-email: David Baumgold <david@davidbaumgold.com>
+Maintainer: Daniele Sluijters
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: requests>=2.0
-Requires-Dist: oauthlib
+Requires-Dist: oauthlib>=3.2
 Requires-Dist: requests-oauthlib>=1.0.0
 Requires-Dist: Flask>=2.0.3
 Requires-Dist: Werkzeug
 Requires-Dist: urlobject
 Requires-Dist: sphinx>=1.3 ; extra == "docs"
 Requires-Dist: sphinxcontrib-seqdiag ; extra == "docs"
 Requires-Dist: sphinxcontrib-spelling ; extra == "docs"
```

