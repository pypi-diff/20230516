# Comparing `tmp/paloma-sdk-3.0.7.tar.gz` & `tmp/paloma-sdk-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paloma-sdk-3.0.7.tar", max compression
+gzip compressed data, was "paloma-sdk-3.0.8.tar", max compression
```

## Comparing `paloma-sdk-3.0.7.tar` & `paloma-sdk-3.0.8.tar`

### file list

```diff
@@ -1,124 +1,124 @@
--rw-r--r--   0        0        0     1083 2022-09-23 22:38:50.559573 paloma-sdk-3.0.7/LICENSE
--rw-r--r--   0        0        0    11543 2022-10-11 22:28:59.273983 paloma-sdk-3.0.7/README.md
--rw-r--r--   0        0        0      162 2022-09-23 22:38:50.627605 paloma-sdk-3.0.7/paloma_sdk/__init__.py
--rw-r--r--   0        0        0        0 2022-08-11 19:03:51.791345 paloma-sdk-3.0.7/paloma_sdk/client/__init__.py
--rw-r--r--   0        0        0      216 2022-08-11 19:03:51.791427 paloma-sdk-3.0.7/paloma_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0        0 2022-08-11 19:03:51.791473 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/__init__.py
--rw-r--r--   0        0        0      812 2022-08-11 19:03:51.791532 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/_base.py
--rw-r--r--   0        0        0     1453 2022-09-23 22:16:21.162401 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/auth.py
--rw-r--r--   0        0        0     3434 2022-09-23 22:16:20.846020 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/authz.py
--rw-r--r--   0        0        0     2470 2022-09-23 22:16:21.012777 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/bank.py
--rw-r--r--   0        0        0     4393 2022-09-23 22:16:21.367362 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/distribution.py
--rw-r--r--   0        0        0     3630 2022-09-23 22:16:21.000959 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/feegrant.py
--rw-r--r--   0        0        0    10270 2022-09-23 22:16:20.785985 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/gov.py
--rw-r--r--   0        0        0      587 2022-08-11 19:03:51.791957 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/ibc.py
--rw-r--r--   0        0        0      762 2022-08-11 19:03:51.792014 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/ibc_transfer.py
--rw-r--r--   0        0        0     2329 2022-09-23 22:16:20.874930 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/mint.py
--rw-r--r--   0        0        0     3767 2022-09-23 22:16:20.789003 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/slashing.py
--rw-r--r--   0        0        0    13194 2022-09-23 22:16:21.200377 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/staking.py
--rw-r--r--   0        0        0     2923 2022-10-12 02:12:20.754393 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/tendermint.py
--rw-r--r--   0        0        0    14754 2022-09-23 22:16:21.215131 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/tx.py
--rw-r--r--   0        0        0     5009 2022-09-23 22:16:21.362831 paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/wasm.py
--rw-r--r--   0        0        0    11121 2022-10-12 02:17:45.365616 paloma-sdk-3.0.7/paloma_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0     1801 2022-09-23 22:16:21.345972 paloma-sdk-3.0.7/paloma_sdk/client/lcd/lcdutils.py
--rw-r--r--   0        0        0     2394 2022-08-11 19:03:51.792631 paloma-sdk-3.0.7/paloma_sdk/client/lcd/params.py
--rw-r--r--   0        0        0     5217 2022-09-23 22:16:20.868073 paloma-sdk-3.0.7/paloma_sdk/client/lcd/wallet.py
--rw-r--r--   0        0        0     3716 2022-09-23 22:40:50.233956 paloma-sdk-3.0.7/paloma_sdk/client/localterra.py
--rw-r--r--   0        0        0      899 2022-08-11 19:03:51.792868 paloma-sdk-3.0.7/paloma_sdk/core/__init__.py
--rw-r--r--   0        0        0      645 2022-08-11 19:03:51.792945 paloma-sdk-3.0.7/paloma_sdk/core/auth/__init__.py
--rw-r--r--   0        0        0      600 2022-09-23 22:16:20.823882 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/__init__.py
--rw-r--r--   0        0        0     1700 2022-09-23 22:16:21.085908 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/account.py
--rw-r--r--   0        0        0     2951 2022-09-30 21:11:59.018082 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/base_account.py
--rw-r--r--   0        0        0     3961 2022-09-30 21:11:59.104316 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/base_vesting_account.py
--rw-r--r--   0        0        0     2727 2022-09-30 21:11:59.055971 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/continuous_vesting_account.py
--rw-r--r--   0        0        0     2494 2022-09-30 21:11:59.029145 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/delayed_vesting_account.py
--rw-r--r--   0        0        0     4435 2022-09-30 21:11:59.118294 paloma-sdk-3.0.7/paloma_sdk/core/auth/data/periodic_vesting_account.py
--rw-r--r--   0        0        0      331 2022-08-11 19:03:51.793455 paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/__init__.py
--rw-r--r--   0        0        0     2916 2022-09-30 21:11:59.080706 paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
--rw-r--r--   0        0        0     2834 2022-09-30 21:11:59.116421 paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_create_vesting_account.py
--rw-r--r--   0        0        0     1616 2022-09-30 21:11:59.097825 paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
--rw-r--r--   0        0        0      446 2022-08-11 19:03:51.793708 paloma-sdk-3.0.7/paloma_sdk/core/authz/__init__.py
--rw-r--r--   0        0        0     9594 2022-09-30 21:11:59.044728 paloma-sdk-3.0.7/paloma_sdk/core/authz/data.py
--rw-r--r--   0        0        0     6101 2022-09-30 21:11:58.997728 paloma-sdk-3.0.7/paloma_sdk/core/authz/msgs.py
--rw-r--r--   0        0        0      149 2022-08-11 19:03:51.793904 paloma-sdk-3.0.7/paloma_sdk/core/bank/__init__.py
--rw-r--r--   0        0        0     7086 2022-09-30 21:11:58.995958 paloma-sdk-3.0.7/paloma_sdk/core/bank/msgs.py
--rw-r--r--   0        0        0     5008 2022-09-23 22:38:50.535721 paloma-sdk-3.0.7/paloma_sdk/core/bech32.py
--rw-r--r--   0        0        0     1616 2022-08-11 19:03:51.794098 paloma-sdk-3.0.7/paloma_sdk/core/block.py
--rw-r--r--   0        0        0     2722 2022-09-23 22:16:21.071287 paloma-sdk-3.0.7/paloma_sdk/core/broadcast.py
--rw-r--r--   0        0        0     7742 2022-09-30 21:11:58.975428 paloma-sdk-3.0.7/paloma_sdk/core/coin.py
--rw-r--r--   0        0        0     8357 2022-09-30 21:11:59.113990 paloma-sdk-3.0.7/paloma_sdk/core/coins.py
--rw-r--r--   0        0        0     2704 2022-09-30 21:11:59.131294 paloma-sdk-3.0.7/paloma_sdk/core/compact_bit_array.py
--rw-r--r--   0        0        0       71 2022-08-11 19:03:51.794436 paloma-sdk-3.0.7/paloma_sdk/core/crisis/__init__.py
--rw-r--r--   0        0        0     2065 2022-09-30 21:11:59.048282 paloma-sdk-3.0.7/paloma_sdk/core/crisis/msgs.py
--rw-r--r--   0        0        0     1081 2022-09-30 21:11:59.111043 paloma-sdk-3.0.7/paloma_sdk/core/deposit.py
--rw-r--r--   0        0        0      371 2022-08-11 19:03:51.794627 paloma-sdk-3.0.7/paloma_sdk/core/distribution/__init__.py
--rw-r--r--   0        0        0     6930 2022-09-30 21:11:59.011894 paloma-sdk-3.0.7/paloma_sdk/core/distribution/msgs.py
--rw-r--r--   0        0        0     2688 2022-09-30 21:11:59.067264 paloma-sdk-3.0.7/paloma_sdk/core/distribution/proposals.py
--rw-r--r--   0        0        0     2003 2022-09-30 21:11:59.060201 paloma-sdk-3.0.7/paloma_sdk/core/fee.py
--rw-r--r--   0        0        0      297 2022-08-11 19:03:51.794956 paloma-sdk-3.0.7/paloma_sdk/core/feegrant/__init__.py
--rw-r--r--   0        0        0     9131 2022-09-30 21:11:59.102317 paloma-sdk-3.0.7/paloma_sdk/core/feegrant/data.py
--rw-r--r--   0        0        0     3172 2022-09-30 21:11:59.050615 paloma-sdk-3.0.7/paloma_sdk/core/feegrant/msgs.py
--rw-r--r--   0        0        0      410 2022-09-30 21:11:59.065152 paloma-sdk-3.0.7/paloma_sdk/core/gov/__init__.py
--rw-r--r--   0        0        0     6138 2022-09-30 21:11:59.003226 paloma-sdk-3.0.7/paloma_sdk/core/gov/data.py
--rw-r--r--   0        0        0     6506 2022-09-30 21:11:59.004953 paloma-sdk-3.0.7/paloma_sdk/core/gov/msgs.py
--rw-r--r--   0        0        0     1692 2022-09-30 21:11:59.013915 paloma-sdk-3.0.7/paloma_sdk/core/gov/proposals.py
--rw-r--r--   0        0        0       47 2022-08-11 19:03:51.795450 paloma-sdk-3.0.7/paloma_sdk/core/ibc/__init__.py
--rw-r--r--   0        0        0      492 2022-08-11 19:03:51.795530 paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/__init__.py
--rw-r--r--   0        0        0     4799 2022-09-30 21:11:59.083111 paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/channel.py
--rw-r--r--   0        0        0     5312 2022-09-30 21:11:59.093973 paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/client.py
--rw-r--r--   0        0        0     1402 2022-09-30 21:11:59.122481 paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/commitment.py
--rw-r--r--   0        0        0     1942 2022-09-30 21:11:59.128858 paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/connection.py
--rw-r--r--   0        0        0      944 2022-08-11 19:03:51.795892 paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/__init__.py
--rw-r--r--   0        0        0    14707 2022-09-30 21:11:59.091606 paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/channel.py
--rw-r--r--   0        0        0     5933 2022-09-30 21:11:59.062690 paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/client.py
--rw-r--r--   0        0        0     9929 2022-09-30 21:11:59.077593 paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/connection.py
--rw-r--r--   0        0        0       80 2022-08-11 19:03:51.796213 paloma-sdk-3.0.7/paloma_sdk/core/ibc/proposals/__init__.py
--rw-r--r--   0        0        0     2202 2022-09-30 21:11:59.058424 paloma-sdk-3.0.7/paloma_sdk/core/ibc/proposals/proposals.py
--rw-r--r--   0        0        0      100 2022-08-11 19:03:51.796362 paloma-sdk-3.0.7/paloma_sdk/core/ibc_transfer/__init__.py
--rw-r--r--   0        0        0      700 2022-09-30 21:11:59.024474 paloma-sdk-3.0.7/paloma_sdk/core/ibc_transfer/data.py
--rw-r--r--   0        0        0     3364 2022-09-30 21:11:59.109375 paloma-sdk-3.0.7/paloma_sdk/core/ibc_transfer/msgs.py
--rw-r--r--   0        0        0     3325 2022-09-30 21:11:59.124977 paloma-sdk-3.0.7/paloma_sdk/core/mode_info.py
--rw-r--r--   0        0        0      803 2022-09-23 22:38:50.588696 paloma-sdk-3.0.7/paloma_sdk/core/msg.py
--rw-r--r--   0        0        0     2388 2022-09-23 22:16:21.238527 paloma-sdk-3.0.7/paloma_sdk/core/multisig.py
--rw-r--r--   0        0        0    11365 2022-09-23 22:16:21.262524 paloma-sdk-3.0.7/paloma_sdk/core/numeric.py
--rw-r--r--   0        0        0      114 2022-08-11 19:03:51.796819 paloma-sdk-3.0.7/paloma_sdk/core/params/__init__.py
--rw-r--r--   0        0        0     3320 2022-09-30 21:11:59.015742 paloma-sdk-3.0.7/paloma_sdk/core/params/proposals.py
--rw-r--r--   0        0        0    10674 2022-09-30 21:11:59.074352 paloma-sdk-3.0.7/paloma_sdk/core/public_key.py
--rw-r--r--   0        0        0     2616 2022-09-30 21:11:59.046546 paloma-sdk-3.0.7/paloma_sdk/core/sign_doc.py
--rw-r--r--   0        0        0     3546 2022-09-30 21:11:59.127032 paloma-sdk-3.0.7/paloma_sdk/core/signature_v2.py
--rw-r--r--   0        0        0       53 2022-08-11 19:03:51.797170 paloma-sdk-3.0.7/paloma_sdk/core/slashing/__init__.py
--rw-r--r--   0        0        0     1099 2022-09-30 21:11:59.053032 paloma-sdk-3.0.7/paloma_sdk/core/slashing/msgs.py
--rw-r--r--   0        0        0      661 2022-08-11 19:03:51.797301 paloma-sdk-3.0.7/paloma_sdk/core/staking/__init__.py
--rw-r--r--   0        0        0      429 2022-08-11 19:03:51.797384 paloma-sdk-3.0.7/paloma_sdk/core/staking/data/__init__.py
--rw-r--r--   0        0        0    11284 2022-09-30 21:11:59.107375 paloma-sdk-3.0.7/paloma_sdk/core/staking/data/delegation.py
--rw-r--r--   0        0        0     9613 2022-09-30 21:11:59.009470 paloma-sdk-3.0.7/paloma_sdk/core/staking/data/validator.py
--rw-r--r--   0        0        0    11079 2022-09-30 21:11:59.026779 paloma-sdk-3.0.7/paloma_sdk/core/staking/msgs.py
--rw-r--r--   0        0        0    15110 2022-09-30 21:11:59.020225 paloma-sdk-3.0.7/paloma_sdk/core/tx.py
--rw-r--r--   0        0        0      176 2022-08-11 19:03:51.798076 paloma-sdk-3.0.7/paloma_sdk/core/upgrade/__init__.py
--rw-r--r--   0        0        0      149 2022-08-11 19:03:51.798166 paloma-sdk-3.0.7/paloma_sdk/core/upgrade/data/__init__.py
--rw-r--r--   0        0        0     3324 2022-09-30 21:11:59.021811 paloma-sdk-3.0.7/paloma_sdk/core/upgrade/data/proposal.py
--rw-r--r--   0        0        0     2187 2022-09-30 21:11:59.000863 paloma-sdk-3.0.7/paloma_sdk/core/upgrade/plan.py
--rw-r--r--   0        0        0      315 2022-08-11 19:03:51.798383 paloma-sdk-3.0.7/paloma_sdk/core/wasm/__init__.py
--rw-r--r--   0        0        0     9303 2022-09-30 21:11:59.031469 paloma-sdk-3.0.7/paloma_sdk/core/wasm/data.py
--rw-r--r--   0        0        0    11287 2022-09-30 21:11:58.989995 paloma-sdk-3.0.7/paloma_sdk/core/wasm/msgs.py
--rw-r--r--   0        0        0    24170 2022-09-30 21:11:59.034118 paloma-sdk-3.0.7/paloma_sdk/core/wasm/proposals.py
--rw-r--r--   0        0        0      428 2022-09-23 22:38:50.587265 paloma-sdk-3.0.7/paloma_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2022-08-11 19:03:51.798889 paloma-sdk-3.0.7/paloma_sdk/key/__init__.py
--rw-r--r--   0        0        0     7961 2022-09-23 22:38:50.537311 paloma-sdk-3.0.7/paloma_sdk/key/key.py
--rw-r--r--   0        0        0     2213 2022-09-23 22:38:50.541688 paloma-sdk-3.0.7/paloma_sdk/key/mnemonic.py
--rw-r--r--   0        0        0     1657 2022-08-11 19:03:51.799182 paloma-sdk-3.0.7/paloma_sdk/key/raw.py
--rw-r--r--   0        0        0        0 2022-08-11 19:03:51.799252 paloma-sdk-3.0.7/paloma_sdk/util/__init__.py
--rw-r--r--   0        0        0     1679 2022-09-23 22:38:50.539112 paloma-sdk-3.0.7/paloma_sdk/util/base.py
--rw-r--r--   0        0        0     3250 2022-09-23 22:16:20.792515 paloma-sdk-3.0.7/paloma_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2022-08-11 19:03:51.799481 paloma-sdk-3.0.7/paloma_sdk/util/converter.py
--rw-r--r--   0        0        0      211 2022-08-11 19:03:51.799550 paloma-sdk-3.0.7/paloma_sdk/util/hash.py
--rw-r--r--   0        0        0     1695 2022-09-23 22:16:21.305185 paloma-sdk-3.0.7/paloma_sdk/util/json.py
--rw-r--r--   0        0        0     1038 2022-09-30 21:11:59.006785 paloma-sdk-3.0.7/paloma_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2533 2022-09-30 21:11:59.100096 paloma-sdk-3.0.7/paloma_sdk/util/parse_content.py
--rw-r--r--   0        0        0     3875 2022-09-23 22:16:20.887515 paloma-sdk-3.0.7/paloma_sdk/util/parse_msg.py
--rw-r--r--   0        0        0      731 2022-09-23 22:16:21.165093 paloma-sdk-3.0.7/paloma_sdk/util/parse_proto.py
--rw-r--r--   0        0        0      294 2022-08-11 19:03:51.799950 paloma-sdk-3.0.7/paloma_sdk/util/remove_none.py
--rw-r--r--   0        0        0      117 2022-10-12 02:37:59.551196 paloma-sdk-3.0.7/paloma_sdk/util/url.py
--rw-r--r--   0        0        0     1818 2022-10-12 02:37:59.511192 paloma-sdk-3.0.7/pyproject.toml
--rw-r--r--   0        0        0    13505 2022-10-12 02:38:26.039868 paloma-sdk-3.0.7/setup.py
--rw-r--r--   0        0        0    12858 2022-10-12 02:38:26.040331 paloma-sdk-3.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1083 2022-09-23 22:38:50.559573 paloma-sdk-3.0.8/LICENSE
+-rw-r--r--   0        0        0    11543 2022-10-11 22:28:59.273983 paloma-sdk-3.0.8/README.md
+-rw-r--r--   0        0        0      162 2022-09-23 22:38:50.627605 paloma-sdk-3.0.8/paloma_sdk/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-11 19:03:51.791345 paloma-sdk-3.0.8/paloma_sdk/client/__init__.py
+-rw-r--r--   0        0        0      216 2022-08-11 19:03:51.791427 paloma-sdk-3.0.8/paloma_sdk/client/lcd/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-11 19:03:51.791473 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/__init__.py
+-rw-r--r--   0        0        0      812 2022-08-11 19:03:51.791532 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/_base.py
+-rw-r--r--   0        0        0     1453 2022-09-23 22:16:21.162401 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/auth.py
+-rw-r--r--   0        0        0     3434 2022-09-23 22:16:20.846020 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/authz.py
+-rw-r--r--   0        0        0     2470 2022-09-23 22:16:21.012777 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/bank.py
+-rw-r--r--   0        0        0     4393 2022-09-23 22:16:21.367362 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/distribution.py
+-rw-r--r--   0        0        0     3630 2022-09-23 22:16:21.000959 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/feegrant.py
+-rw-r--r--   0        0        0    10270 2022-09-23 22:16:20.785985 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/gov.py
+-rw-r--r--   0        0        0      587 2022-08-11 19:03:51.791957 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/ibc.py
+-rw-r--r--   0        0        0      762 2022-08-11 19:03:51.792014 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/ibc_transfer.py
+-rw-r--r--   0        0        0     2329 2022-09-23 22:16:20.874930 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/mint.py
+-rw-r--r--   0        0        0     3767 2022-09-23 22:16:20.789003 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/slashing.py
+-rw-r--r--   0        0        0    13194 2022-09-23 22:16:21.200377 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/staking.py
+-rw-r--r--   0        0        0     2911 2022-10-12 02:43:31.946941 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/tendermint.py
+-rw-r--r--   0        0        0    14754 2022-09-23 22:16:21.215131 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/tx.py
+-rw-r--r--   0        0        0     5009 2022-09-23 22:16:21.362831 paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/wasm.py
+-rw-r--r--   0        0        0    11121 2022-10-12 02:17:45.365616 paloma-sdk-3.0.8/paloma_sdk/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0     1801 2022-09-23 22:16:21.345972 paloma-sdk-3.0.8/paloma_sdk/client/lcd/lcdutils.py
+-rw-r--r--   0        0        0     2394 2022-08-11 19:03:51.792631 paloma-sdk-3.0.8/paloma_sdk/client/lcd/params.py
+-rw-r--r--   0        0        0     5217 2022-09-23 22:16:20.868073 paloma-sdk-3.0.8/paloma_sdk/client/lcd/wallet.py
+-rw-r--r--   0        0        0     3716 2022-09-23 22:40:50.233956 paloma-sdk-3.0.8/paloma_sdk/client/localterra.py
+-rw-r--r--   0        0        0      899 2022-08-11 19:03:51.792868 paloma-sdk-3.0.8/paloma_sdk/core/__init__.py
+-rw-r--r--   0        0        0      645 2022-08-11 19:03:51.792945 paloma-sdk-3.0.8/paloma_sdk/core/auth/__init__.py
+-rw-r--r--   0        0        0      600 2022-09-23 22:16:20.823882 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/__init__.py
+-rw-r--r--   0        0        0     1700 2022-09-23 22:16:21.085908 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/account.py
+-rw-r--r--   0        0        0     2951 2022-09-30 21:11:59.018082 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/base_account.py
+-rw-r--r--   0        0        0     3961 2022-09-30 21:11:59.104316 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/base_vesting_account.py
+-rw-r--r--   0        0        0     2727 2022-09-30 21:11:59.055971 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/continuous_vesting_account.py
+-rw-r--r--   0        0        0     2494 2022-09-30 21:11:59.029145 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/delayed_vesting_account.py
+-rw-r--r--   0        0        0     4435 2022-09-30 21:11:59.118294 paloma-sdk-3.0.8/paloma_sdk/core/auth/data/periodic_vesting_account.py
+-rw-r--r--   0        0        0      331 2022-08-11 19:03:51.793455 paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/__init__.py
+-rw-r--r--   0        0        0     2916 2022-09-30 21:11:59.080706 paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py
+-rw-r--r--   0        0        0     2834 2022-09-30 21:11:59.116421 paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_create_vesting_account.py
+-rw-r--r--   0        0        0     1616 2022-09-30 21:11:59.097825 paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py
+-rw-r--r--   0        0        0      446 2022-08-11 19:03:51.793708 paloma-sdk-3.0.8/paloma_sdk/core/authz/__init__.py
+-rw-r--r--   0        0        0     9594 2022-09-30 21:11:59.044728 paloma-sdk-3.0.8/paloma_sdk/core/authz/data.py
+-rw-r--r--   0        0        0     6101 2022-09-30 21:11:58.997728 paloma-sdk-3.0.8/paloma_sdk/core/authz/msgs.py
+-rw-r--r--   0        0        0      149 2022-08-11 19:03:51.793904 paloma-sdk-3.0.8/paloma_sdk/core/bank/__init__.py
+-rw-r--r--   0        0        0     7086 2022-09-30 21:11:58.995958 paloma-sdk-3.0.8/paloma_sdk/core/bank/msgs.py
+-rw-r--r--   0        0        0     5008 2022-09-23 22:38:50.535721 paloma-sdk-3.0.8/paloma_sdk/core/bech32.py
+-rw-r--r--   0        0        0     1616 2022-08-11 19:03:51.794098 paloma-sdk-3.0.8/paloma_sdk/core/block.py
+-rw-r--r--   0        0        0     2722 2022-09-23 22:16:21.071287 paloma-sdk-3.0.8/paloma_sdk/core/broadcast.py
+-rw-r--r--   0        0        0     7742 2022-09-30 21:11:58.975428 paloma-sdk-3.0.8/paloma_sdk/core/coin.py
+-rw-r--r--   0        0        0     8357 2022-09-30 21:11:59.113990 paloma-sdk-3.0.8/paloma_sdk/core/coins.py
+-rw-r--r--   0        0        0     2704 2022-09-30 21:11:59.131294 paloma-sdk-3.0.8/paloma_sdk/core/compact_bit_array.py
+-rw-r--r--   0        0        0       71 2022-08-11 19:03:51.794436 paloma-sdk-3.0.8/paloma_sdk/core/crisis/__init__.py
+-rw-r--r--   0        0        0     2065 2022-09-30 21:11:59.048282 paloma-sdk-3.0.8/paloma_sdk/core/crisis/msgs.py
+-rw-r--r--   0        0        0     1081 2022-09-30 21:11:59.111043 paloma-sdk-3.0.8/paloma_sdk/core/deposit.py
+-rw-r--r--   0        0        0      371 2022-08-11 19:03:51.794627 paloma-sdk-3.0.8/paloma_sdk/core/distribution/__init__.py
+-rw-r--r--   0        0        0     6930 2022-09-30 21:11:59.011894 paloma-sdk-3.0.8/paloma_sdk/core/distribution/msgs.py
+-rw-r--r--   0        0        0     2688 2022-09-30 21:11:59.067264 paloma-sdk-3.0.8/paloma_sdk/core/distribution/proposals.py
+-rw-r--r--   0        0        0     2003 2022-09-30 21:11:59.060201 paloma-sdk-3.0.8/paloma_sdk/core/fee.py
+-rw-r--r--   0        0        0      297 2022-08-11 19:03:51.794956 paloma-sdk-3.0.8/paloma_sdk/core/feegrant/__init__.py
+-rw-r--r--   0        0        0     9131 2022-09-30 21:11:59.102317 paloma-sdk-3.0.8/paloma_sdk/core/feegrant/data.py
+-rw-r--r--   0        0        0     3172 2022-09-30 21:11:59.050615 paloma-sdk-3.0.8/paloma_sdk/core/feegrant/msgs.py
+-rw-r--r--   0        0        0      410 2022-09-30 21:11:59.065152 paloma-sdk-3.0.8/paloma_sdk/core/gov/__init__.py
+-rw-r--r--   0        0        0     6138 2022-09-30 21:11:59.003226 paloma-sdk-3.0.8/paloma_sdk/core/gov/data.py
+-rw-r--r--   0        0        0     6506 2022-09-30 21:11:59.004953 paloma-sdk-3.0.8/paloma_sdk/core/gov/msgs.py
+-rw-r--r--   0        0        0     1692 2022-09-30 21:11:59.013915 paloma-sdk-3.0.8/paloma_sdk/core/gov/proposals.py
+-rw-r--r--   0        0        0       47 2022-08-11 19:03:51.795450 paloma-sdk-3.0.8/paloma_sdk/core/ibc/__init__.py
+-rw-r--r--   0        0        0      492 2022-08-11 19:03:51.795530 paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/__init__.py
+-rw-r--r--   0        0        0     4799 2022-09-30 21:11:59.083111 paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/channel.py
+-rw-r--r--   0        0        0     5312 2022-09-30 21:11:59.093973 paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/client.py
+-rw-r--r--   0        0        0     1402 2022-09-30 21:11:59.122481 paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/commitment.py
+-rw-r--r--   0        0        0     1942 2022-09-30 21:11:59.128858 paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/connection.py
+-rw-r--r--   0        0        0      944 2022-08-11 19:03:51.795892 paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/__init__.py
+-rw-r--r--   0        0        0    14707 2022-09-30 21:11:59.091606 paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/channel.py
+-rw-r--r--   0        0        0     5933 2022-09-30 21:11:59.062690 paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/client.py
+-rw-r--r--   0        0        0     9929 2022-09-30 21:11:59.077593 paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/connection.py
+-rw-r--r--   0        0        0       80 2022-08-11 19:03:51.796213 paloma-sdk-3.0.8/paloma_sdk/core/ibc/proposals/__init__.py
+-rw-r--r--   0        0        0     2202 2022-09-30 21:11:59.058424 paloma-sdk-3.0.8/paloma_sdk/core/ibc/proposals/proposals.py
+-rw-r--r--   0        0        0      100 2022-08-11 19:03:51.796362 paloma-sdk-3.0.8/paloma_sdk/core/ibc_transfer/__init__.py
+-rw-r--r--   0        0        0      700 2022-09-30 21:11:59.024474 paloma-sdk-3.0.8/paloma_sdk/core/ibc_transfer/data.py
+-rw-r--r--   0        0        0     3364 2022-09-30 21:11:59.109375 paloma-sdk-3.0.8/paloma_sdk/core/ibc_transfer/msgs.py
+-rw-r--r--   0        0        0     3325 2022-09-30 21:11:59.124977 paloma-sdk-3.0.8/paloma_sdk/core/mode_info.py
+-rw-r--r--   0        0        0      803 2022-09-23 22:38:50.588696 paloma-sdk-3.0.8/paloma_sdk/core/msg.py
+-rw-r--r--   0        0        0     2388 2022-09-23 22:16:21.238527 paloma-sdk-3.0.8/paloma_sdk/core/multisig.py
+-rw-r--r--   0        0        0    11365 2022-09-23 22:16:21.262524 paloma-sdk-3.0.8/paloma_sdk/core/numeric.py
+-rw-r--r--   0        0        0      114 2022-08-11 19:03:51.796819 paloma-sdk-3.0.8/paloma_sdk/core/params/__init__.py
+-rw-r--r--   0        0        0     3320 2022-09-30 21:11:59.015742 paloma-sdk-3.0.8/paloma_sdk/core/params/proposals.py
+-rw-r--r--   0        0        0    10674 2022-09-30 21:11:59.074352 paloma-sdk-3.0.8/paloma_sdk/core/public_key.py
+-rw-r--r--   0        0        0     2616 2022-09-30 21:11:59.046546 paloma-sdk-3.0.8/paloma_sdk/core/sign_doc.py
+-rw-r--r--   0        0        0     3546 2022-09-30 21:11:59.127032 paloma-sdk-3.0.8/paloma_sdk/core/signature_v2.py
+-rw-r--r--   0        0        0       53 2022-08-11 19:03:51.797170 paloma-sdk-3.0.8/paloma_sdk/core/slashing/__init__.py
+-rw-r--r--   0        0        0     1099 2022-09-30 21:11:59.053032 paloma-sdk-3.0.8/paloma_sdk/core/slashing/msgs.py
+-rw-r--r--   0        0        0      661 2022-08-11 19:03:51.797301 paloma-sdk-3.0.8/paloma_sdk/core/staking/__init__.py
+-rw-r--r--   0        0        0      429 2022-08-11 19:03:51.797384 paloma-sdk-3.0.8/paloma_sdk/core/staking/data/__init__.py
+-rw-r--r--   0        0        0    11284 2022-09-30 21:11:59.107375 paloma-sdk-3.0.8/paloma_sdk/core/staking/data/delegation.py
+-rw-r--r--   0        0        0     9613 2022-09-30 21:11:59.009470 paloma-sdk-3.0.8/paloma_sdk/core/staking/data/validator.py
+-rw-r--r--   0        0        0    11079 2022-09-30 21:11:59.026779 paloma-sdk-3.0.8/paloma_sdk/core/staking/msgs.py
+-rw-r--r--   0        0        0    15110 2022-09-30 21:11:59.020225 paloma-sdk-3.0.8/paloma_sdk/core/tx.py
+-rw-r--r--   0        0        0      176 2022-08-11 19:03:51.798076 paloma-sdk-3.0.8/paloma_sdk/core/upgrade/__init__.py
+-rw-r--r--   0        0        0      149 2022-08-11 19:03:51.798166 paloma-sdk-3.0.8/paloma_sdk/core/upgrade/data/__init__.py
+-rw-r--r--   0        0        0     3324 2022-09-30 21:11:59.021811 paloma-sdk-3.0.8/paloma_sdk/core/upgrade/data/proposal.py
+-rw-r--r--   0        0        0     2187 2022-09-30 21:11:59.000863 paloma-sdk-3.0.8/paloma_sdk/core/upgrade/plan.py
+-rw-r--r--   0        0        0      315 2022-08-11 19:03:51.798383 paloma-sdk-3.0.8/paloma_sdk/core/wasm/__init__.py
+-rw-r--r--   0        0        0     9303 2022-09-30 21:11:59.031469 paloma-sdk-3.0.8/paloma_sdk/core/wasm/data.py
+-rw-r--r--   0        0        0    11287 2022-09-30 21:11:58.989995 paloma-sdk-3.0.8/paloma_sdk/core/wasm/msgs.py
+-rw-r--r--   0        0        0    24170 2022-09-30 21:11:59.034118 paloma-sdk-3.0.8/paloma_sdk/core/wasm/proposals.py
+-rw-r--r--   0        0        0      428 2022-09-23 22:38:50.587265 paloma-sdk-3.0.8/paloma_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2022-08-11 19:03:51.798889 paloma-sdk-3.0.8/paloma_sdk/key/__init__.py
+-rw-r--r--   0        0        0     7961 2022-09-23 22:38:50.537311 paloma-sdk-3.0.8/paloma_sdk/key/key.py
+-rw-r--r--   0        0        0     2213 2022-09-23 22:38:50.541688 paloma-sdk-3.0.8/paloma_sdk/key/mnemonic.py
+-rw-r--r--   0        0        0     1657 2022-08-11 19:03:51.799182 paloma-sdk-3.0.8/paloma_sdk/key/raw.py
+-rw-r--r--   0        0        0        0 2022-08-11 19:03:51.799252 paloma-sdk-3.0.8/paloma_sdk/util/__init__.py
+-rw-r--r--   0        0        0     1679 2022-09-23 22:38:50.539112 paloma-sdk-3.0.8/paloma_sdk/util/base.py
+-rw-r--r--   0        0        0     3250 2022-09-23 22:16:20.792515 paloma-sdk-3.0.8/paloma_sdk/util/contract.py
+-rw-r--r--   0        0        0      199 2022-08-11 19:03:51.799481 paloma-sdk-3.0.8/paloma_sdk/util/converter.py
+-rw-r--r--   0        0        0      211 2022-08-11 19:03:51.799550 paloma-sdk-3.0.8/paloma_sdk/util/hash.py
+-rw-r--r--   0        0        0     1695 2022-09-23 22:16:21.305185 paloma-sdk-3.0.8/paloma_sdk/util/json.py
+-rw-r--r--   0        0        0     1038 2022-09-30 21:11:59.006785 paloma-sdk-3.0.8/paloma_sdk/util/parse_authorization.py
+-rw-r--r--   0        0        0     2533 2022-09-30 21:11:59.100096 paloma-sdk-3.0.8/paloma_sdk/util/parse_content.py
+-rw-r--r--   0        0        0     3875 2022-09-23 22:16:20.887515 paloma-sdk-3.0.8/paloma_sdk/util/parse_msg.py
+-rw-r--r--   0        0        0      731 2022-09-23 22:16:21.165093 paloma-sdk-3.0.8/paloma_sdk/util/parse_proto.py
+-rw-r--r--   0        0        0      294 2022-08-11 19:03:51.799950 paloma-sdk-3.0.8/paloma_sdk/util/remove_none.py
+-rw-r--r--   0        0        0      117 2022-10-12 02:37:59.551196 paloma-sdk-3.0.8/paloma_sdk/util/url.py
+-rw-r--r--   0        0        0     1818 2022-10-12 02:44:21.096469 paloma-sdk-3.0.8/pyproject.toml
+-rw-r--r--   0        0        0    13505 2022-10-12 02:45:25.344048 paloma-sdk-3.0.8/setup.py
+-rw-r--r--   0        0        0    12858 2022-10-12 02:45:25.344518 paloma-sdk-3.0.8/PKG-INFO
```

### Comparing `paloma-sdk-3.0.7/LICENSE` & `paloma-sdk-3.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/README.md` & `paloma-sdk-3.0.8/README.md`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/_base.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/_base.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/auth.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/auth.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/authz.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/authz.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/bank.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/bank.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/distribution.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/distribution.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/feegrant.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/feegrant.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/gov.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/gov.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/ibc.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/ibc.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/ibc_transfer.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/ibc_transfer.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/mint.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/mint.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/slashing.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/slashing.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/staking.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/staking.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/tendermint.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/tendermint.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,28 +39,28 @@
         Args:
             height (int, optional): block height.
             params (APIParams): optional parameters
 
         Returns:
             dict: validator set
         """
-        x = "latest" if height is None else height
+        x = "" if height is None else height
         return await self._c._get(f"/validators?height={x}", params)
 
     async def block_info(self, height: Optional[int] = None, params: Optional[APIParams] = None) -> dict:
         """Fetches the block information for a given height. If no height is given, defaults to latest block.
 
         Args:
             height (int, optional): block height.
             params (APIParams): optional parameters
 
         Returns:
             dict: block info
         """
-        x = "latest" if height is None else height
+        x = "" if height is None else height
         return await self._c._get(f"/block?height={x}", params)
 
 
 class TendermintAPI(AsyncTendermintAPI):
     @sync_bind(AsyncTendermintAPI.node_info)
     def node_info(self, params: Optional[APIParams] = None) -> dict:
         pass
```

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/tx.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/tx.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/api/wasm.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/api/wasm.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/lcdclient.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/lcdclient.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/lcdutils.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/lcdutils.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/params.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/params.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/lcd/wallet.py` & `paloma-sdk-3.0.8/paloma_sdk/client/lcd/wallet.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/client/localterra.py` & `paloma-sdk-3.0.8/paloma_sdk/client/localterra.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/__init__.py` & `paloma-sdk-3.0.8/paloma_sdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/__init__.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/__init__.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/__init__.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/base_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/base_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/base_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/base_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/continuous_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/continuous_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/delayed_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/delayed_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/data/periodic_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/data/periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_create_periodic_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_create_vesting_account.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_create_vesting_account.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py` & `paloma-sdk-3.0.8/paloma_sdk/core/auth/msgs/msg_donate_all_vesting_tokens.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/authz/data.py` & `paloma-sdk-3.0.8/paloma_sdk/core/authz/data.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/authz/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/authz/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/bank/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/bank/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/bech32.py` & `paloma-sdk-3.0.8/paloma_sdk/core/bech32.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/block.py` & `paloma-sdk-3.0.8/paloma_sdk/core/block.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/broadcast.py` & `paloma-sdk-3.0.8/paloma_sdk/core/broadcast.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/coin.py` & `paloma-sdk-3.0.8/paloma_sdk/core/coin.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/coins.py` & `paloma-sdk-3.0.8/paloma_sdk/core/coins.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/compact_bit_array.py` & `paloma-sdk-3.0.8/paloma_sdk/core/compact_bit_array.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/crisis/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/crisis/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/deposit.py` & `paloma-sdk-3.0.8/paloma_sdk/core/deposit.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/distribution/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/distribution/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/distribution/proposals.py` & `paloma-sdk-3.0.8/paloma_sdk/core/distribution/proposals.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/fee.py` & `paloma-sdk-3.0.8/paloma_sdk/core/fee.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/feegrant/data.py` & `paloma-sdk-3.0.8/paloma_sdk/core/feegrant/data.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/feegrant/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/feegrant/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/gov/data.py` & `paloma-sdk-3.0.8/paloma_sdk/core/gov/data.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/gov/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/gov/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/gov/proposals.py` & `paloma-sdk-3.0.8/paloma_sdk/core/gov/proposals.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/channel.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/channel.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/client.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/client.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/commitment.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/commitment.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/data/connection.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/data/connection.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/__init__.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/__init__.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/channel.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/channel.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/client.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/client.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/msgs/connection.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/msgs/connection.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc/proposals/proposals.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc/proposals/proposals.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc_transfer/data.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc_transfer/data.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/ibc_transfer/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/ibc_transfer/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/mode_info.py` & `paloma-sdk-3.0.8/paloma_sdk/core/mode_info.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/msg.py` & `paloma-sdk-3.0.8/paloma_sdk/core/msg.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/multisig.py` & `paloma-sdk-3.0.8/paloma_sdk/core/multisig.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/numeric.py` & `paloma-sdk-3.0.8/paloma_sdk/core/numeric.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/params/proposals.py` & `paloma-sdk-3.0.8/paloma_sdk/core/params/proposals.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/public_key.py` & `paloma-sdk-3.0.8/paloma_sdk/core/public_key.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/sign_doc.py` & `paloma-sdk-3.0.8/paloma_sdk/core/sign_doc.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/signature_v2.py` & `paloma-sdk-3.0.8/paloma_sdk/core/signature_v2.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/slashing/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/slashing/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/staking/__init__.py` & `paloma-sdk-3.0.8/paloma_sdk/core/staking/__init__.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/staking/data/delegation.py` & `paloma-sdk-3.0.8/paloma_sdk/core/staking/data/delegation.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/staking/data/validator.py` & `paloma-sdk-3.0.8/paloma_sdk/core/staking/data/validator.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/staking/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/staking/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/tx.py` & `paloma-sdk-3.0.8/paloma_sdk/core/tx.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/upgrade/data/proposal.py` & `paloma-sdk-3.0.8/paloma_sdk/core/upgrade/data/proposal.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/upgrade/plan.py` & `paloma-sdk-3.0.8/paloma_sdk/core/upgrade/plan.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/wasm/data.py` & `paloma-sdk-3.0.8/paloma_sdk/core/wasm/data.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/wasm/msgs.py` & `paloma-sdk-3.0.8/paloma_sdk/core/wasm/msgs.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/core/wasm/proposals.py` & `paloma-sdk-3.0.8/paloma_sdk/core/wasm/proposals.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/key/key.py` & `paloma-sdk-3.0.8/paloma_sdk/key/key.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/key/mnemonic.py` & `paloma-sdk-3.0.8/paloma_sdk/key/mnemonic.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/key/raw.py` & `paloma-sdk-3.0.8/paloma_sdk/key/raw.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/base.py` & `paloma-sdk-3.0.8/paloma_sdk/util/base.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/contract.py` & `paloma-sdk-3.0.8/paloma_sdk/util/contract.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/json.py` & `paloma-sdk-3.0.8/paloma_sdk/util/json.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/parse_authorization.py` & `paloma-sdk-3.0.8/paloma_sdk/util/parse_authorization.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/parse_content.py` & `paloma-sdk-3.0.8/paloma_sdk/util/parse_content.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/parse_msg.py` & `paloma-sdk-3.0.8/paloma_sdk/util/parse_msg.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/paloma_sdk/util/parse_proto.py` & `paloma-sdk-3.0.8/paloma_sdk/util/parse_proto.py`

 * *Files identical despite different names*

### Comparing `paloma-sdk-3.0.7/pyproject.toml` & `paloma-sdk-3.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 documentation = "http://docs.palomachain.coml"
 homepage = "https://github.com/palomachain/paloma.py"
 keywords = ["jigu", "blockchain", "paloma", "defi", "crypto"]
 license = "MIT"
 packages = [{ include = "paloma_sdk" }]
 readme = "README.md"
 repository = "https://github.com/palomachain/paloma.py"
-version = "3.0.7"
+version = "3.0.8"
 
 [tool.poetry.dependencies]
 aiohttp = "^3.8.1"
 bech32 = "^1.2.0"
 bip32utils = "^0.3.post4"
 ecdsa = "^0.17.0"
 mnemonic = "^0.19"
```

### Comparing `paloma-sdk-3.0.7/setup.py` & `paloma-sdk-3.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
  'nest-asyncio>=1.5.4,<2.0.0',
  'protobuf>=3.19.1,<4.0.0',
  'terra-proto==2.1.0',
  'wrapt>=1.13.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'paloma-sdk',
-    'version': '3.0.7',
+    'version': '3.0.8',
     'description': 'The Python SDK for Paloma',
     'long_description': '<br/>\n<br/>\n\n<h1>The Python SDK for Paloma</h1>\n<br/>\n\n<p><sub>(Unfamiliar with Paloma?  <a href="https://docs.palomachain.com">Check out the Paloma Docs</a>)</sub></p>\n\n  \n\n<p>\n  <a href="https://docs.palomachain.com"><strong>Explore the Docs »</strong></a>\n  ·\n  <a href="https://github.com/palomachain/paloma.py">GitHub Repository</a>\n</p></div>\n\nThe Paloma Software Development Kit (SDK) in Python is a simple library toolkit for building software that can interact with the Paloma blockchain and provides simple abstractions over core data structures, serialization, key management, and API request generation.\n\n## Features\n\n- Written in Python with extensive support libraries\n- Versatile support for key management solutions\n- Exposes the Paloma API through LCDClient\n\n<br/>\n\n# Table of Contents\n\n- [API Reference](#api-reference)\n- [Getting Started](#getting-started)\n  - [Requirements](#requirements)\n  - [Installation](#installation)\n  - [Dependencies](#dependencies)\n  - [Tests](#tests)\n  - [Code Quality](#code-quality)\n- [Usage Examples](#usage-examples)\n  - [Getting Blockchain Information](#getting-blockchain-information)\n    - [Async Usage](#async-usage)\n  - [Building and Signing Transactions](#building-and-signing-transactions)\n    - [Example Using a Wallet](#example-using-a-wallet-recommended)\n- [Contributing](#contributing)\n  - [Reporting an Issue](#reporting-an-issue)\n  - [Requesting a Feature](#requesting-a-feature)\n  - [Contributing Code](#contributing-code)\n  - [Documentation Contributions](#documentation-contributions)\n- [License](#license)\n\n<br/>\n\n# API Reference\n\nAn intricate reference to the APIs on the Paloma SDK can be found <a href="https://docs.palomachain.com">here</a>.\n\n<br/>\n\n# Getting Started\n\nA walk-through of the steps to get started with the Paloma SDK alongside a few use case examples are provided below. git ad\n\n## Requirements\n\nPaloma SDK requires <a href="https://www.python.org/downloads/">Python v3.7+</a>.\n\n## Installation\n\n<sub>**NOTE:** _All code starting with a `$` is meant to run on your terminal (a bash prompt). All code starting with a `>>>` is meant to run in a python interpreter, like <a href="https://pypi.org/project/ipython/">ipython</a>._</sub>\n\nPaloma SDK can be installed (preferably in a `virtual environment` from PyPI using `pip`) as follows:\n  \n```\n$ pip install -U paloma_sdk\n```\n\n<sub>_You might have `pip3` installed instead of `pip`; proceed according to your own setup._<sub>\n  \n❗ If you want to communicate with Paloma Classic, use paloma-sdk==2.x\n  \n## Dependencies\n\nPaloma SDK uses <a href="https://python-poetry.org/">Poetry</a> to manage dependencies. To get set up with all the required dependencies, run:\n\n```\n$ pip install poetry\n$ poetry install\n```\n\n## Tests\n\nPaloma SDK provides extensive tests for data classes and functions. To run them, after the steps in [Dependencies](#dependencies):\n\n```\n$ make test\n```\n\n## Code Quality\n\nPaloma SDK uses <a href="https://black.readthedocs.io/en/stable/">Black</a>, <a href="https://isort.readthedocs.io/en/latest/">isort</a>, and <a href="https://mypy.readthedocs.io/en/stable/index.html">Mypy</a> for checking code quality and maintaining style. To reformat, after the steps in [Dependencies](#dependencies):\n\n```\n$ make qa && make format\n```\n\n<br/>\n\n# Usage Examples\n\nPaloma SDK can help you read block data, sign and send transactions, deploy and interact with contracts, and many more.\nThe following examples are provided to help you get started. Use cases and functionalities of the Paloma SDK are not limited to the following examples and can be found in full <a href="https://paloma-money.github.io/paloma.py/index.html">here</a>.\n\nIn order to interact with the Paloma blockchain, you\'ll need a connection to a Paloma node. This can be done through setting up an LCDClient (The LCDClient is an object representing an HTTP connection to a Paloma LCD node.):\n\n```\n>>> from paloma_sdk.client.lcd import LCDClient\n>>> paloma = LCDClient(chain_id="<CHECK DOCS FOR LATEST TESTNET>", url="https://testnet.palomaswap.com")\n```\n\n## Getting Blockchain Information\n\nOnce properly configured, the `LCDClient` instance will allow you to interact with the Paloma blockchain. Try getting the latest block height:\n\n```\n>>> paloma.tendermint.block_info()[\'block\'][\'header\'][\'height\']\n```\n\n`\'1687543\'`\n\n### Async Usage\n\nIf you want to make asynchronous, non-blocking LCD requests, you can use AsyncLCDClient. The interface is similar to LCDClient, except the module and wallet API functions must be awaited.\n\n<pre><code>\n>>> import asyncio \n>>> from paloma_sdk.client.lcd import AsyncLCDClient\n\n>>> async def main():\n      <strong>paloma = AsyncLCDClient("https://testnet.palomaswap.com", "<CHECK DOCS FOR LATEST TESTNET>")</strong>\n      total_supply = await paloma.bank.total()\n      print(total_supply)\n      <strong>await paloma.session.close # you must close the session</strong>\n\n>>> asyncio.get_event_loop().run_until_complete(main())\n</code></pre>\n\n## Building and Signing Transactions\n\nIf you wish to perform a state-changing operation on the Paloma blockchain such as sending tokens, swapping assets, withdrawing rewards, or even invoking functions on smart contracts, you must create a **transaction** and broadcast it to the network.\nPaloma SDK provides functions that help create StdTx objects.\n\n### Example Using a Wallet (_recommended_)\n\nA `Wallet` allows you to create and sign a transaction in a single step by automatically fetching the latest information from the blockchain (chain ID, account number, sequence).\n\nUse `LCDClient.wallet()` to create a Wallet from any Key instance. The Key provided should correspond to the account you intend to sign the transaction with.\n  \n<sub>**NOTE:** *If you are using MacOS and got an exception \'bad key length\' from MnemonicKey, please check your python implementation. if `python3 -c "import ssl; print(ssl.OPENSSL_VERSION)"` returns LibreSSL 2.8.3, you need to reinstall python via pyenv or homebrew.*</sub>\n\n```\n>>> from paloma_sdk.client.lcd import LCDClient\n>>> from paloma_sdk.key.mnemonic import MnemonicKey\n\n>>> mk = MnemonicKey(mnemonic=MNEMONIC)\n>>> paloma = LCDClient("https://testnet.palomaswap.com", "<CHECK DOCS FOR LATEST TESTNET>")\n>>> wallet = paloma.wallet(mk)\n```\n\nOnce you have your Wallet, you can simply create a StdTx using `Wallet.create_and_sign_tx`.\n\n```\n>>> from paloma_sdk.core.fee import Fee\n>>> from paloma_sdk.core.bank import MsgSend\n>>> from paloma_sdk.client.lcd.api.tx import CreateTxOptions\n\n>>> tx = wallet.create_and_sign_tx(CreateTxOptions(\n        msgs=[MsgSend(\n            wallet.key.acc_address,\n            RECIPIENT,\n            "1000000uluna"    # send 1 luna\n        )],\n        memo="test transaction!",\n        fee=Fee(200000, "120000uluna")\n    ))\n```\n\nYou should now be able to broadcast your transaction to the network.\n\n```\n>>> result = paloma.tx.broadcast(tx)\n>>> print(result)\n```\n\n<br/>\n\n# Contributing\n\nCommunity contribution, whether it\'s a new feature, correction, bug report, additional documentation, or any other feedback is always welcome. Please read through this section to ensure that your contribution is in the most suitable format for us to effectively process.\n\n<br/>\n\n## Reporting an Issue\n\nFirst things first: **Do NOT report security vulnerabilities in public issues!** Please disclose responsibly by submitting your findings to the [Paloma Bugcrowd submission form](https://www.paloma.money/bugcrowd). The issue will be assessed as soon as possible.\nIf you encounter a different issue with the Python SDK, check first to see if there is an existing issue on the <a href="https://github.com/paloma-money/paloma-sdk-python/issues">Issues</a> page, or if there is a pull request on the <a href="https://github.com/paloma-money/paloma-sdk-python/pulls">Pull requests</a> page. Be sure to check both the Open and Closed tabs addressing the issue.\n\nIf there isn\'t a discussion on the topic there, you can file an issue. The ideal report includes:\n\n- A description of the problem / suggestion.\n- How to recreate the bug.\n- If relevant, including the versions of your:\n  - Python interpreter\n  - Paloma SDK\n  - Optionally of the other dependencies involved\n- If possible, create a pull request with a (failing) test case demonstrating what\'s wrong. This makes the process for fixing bugs quicker & gets issues resolved sooner.\n  </br>\n\n## Requesting a Feature\n\nIf you wish to request the addition of a feature, please first check out the <a href="https://github.com/paloma-money/paloma-sdk-python/issues">Issues</a> page and the <a href="https://github.com/paloma-money/paloma-sdk-python/pulls">Pull requests</a> page (both Open and Closed tabs). If you decide to continue with the request, think of the merits of the feature to convince the project\'s developers, and provide as much detail and context as possible in the form of filing an issue on the <a href="https://github.com/paloma-money/paloma-sdk-python/issues">Issues</a> page.\n\n<br/>\n\n## Contributing Code\n\nIf you wish to contribute to the repository in the form of patches, improvements, new features, etc., first scale the contribution. If it is a major development, like implementing a feature, it is recommended that you consult with the developers of the project before starting the development to avoid duplicating efforts. Once confirmed, you are welcome to submit your pull request.\n</br>\n\n### For new contributors, here is a quick guide:\n\n1. Fork the repository.\n2. Build the project using the [Dependencies](#dependencies) and [Tests](#tests) steps.\n3. Install a <a href="https://virtualenv.pypa.io/en/latest/index.html">virtualenv</a>.\n4. Develop your code and test the changes using the [Tests](#tests) and [Code Quality](#code-quality) steps.\n5. Commit your changes (ideally follow the <a href="https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit">Angular commit message guidelines</a>).\n6. Push your fork and submit a pull request to the repository\'s `main` branch to propose your code.\n\nA good pull request:\n\n- Is clear and concise.\n- Works across all supported versions of Python. (3.7+)\n- Follows the existing style of the code base (<a href="https://pypi.org/project/flake8/">`Flake8`</a>).\n- Has comments included as needed.\n- Includes a test case that demonstrates the previous flaw that now passes with the included patch, or demonstrates the newly added feature.\n- Must include documentation for changing or adding any public APIs.\n- Must be appropriately licensed (MIT License).\n  </br>\n\n## Documentation Contributions\n\nDocumentation improvements are always welcome. The documentation files live in the [docs](./docs) directory of the repository and are written in <a href="https://docutils.sourceforge.io/rst.html">reStructuredText</a> and use <a href="https://www.sphinx-doc.org/en/master/">Sphinx</a> to create the full suite of documentation.\n</br>\nWhen contributing documentation, please do your best to follow the style of the documentation files. This means a soft limit of 88 characters wide in your text files and a semi-formal, yet friendly and approachable, prose style. You can propose your improvements by submitting a pull request as explained above.\n\n### Need more information on how to contribute?\n\nYou can give this <a href="https://opensource.guide/how-to-contribute/#how-to-submit-a-contribution">guide</a> read for more insight.\n\n<br/>\n\n# License\n\nThis software is licensed under the MIT license. See [LICENSE](./LICENSE) for full disclosure.\n\n© 2021 Paloma\n\n<hr/>\n',
     'author': 'Paloma',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/palomachain/paloma.py',
```

#### html2text {}

```diff
@@ -12,15 +12,15 @@
 'paloma_sdk.core.upgrade.data', 'paloma_sdk.core.wasm', 'paloma_sdk.key',
 'paloma_sdk.util'] package_data = \ {'': ['*']} install_requires = \
 ['aiohttp>=3.8.1,<4.0.0', 'attrs>=21.4.0,<22.0.0', 'bech32>=1.2.0,<2.0.0',
 'betterproto==2.0.0b4', 'bip32utils>=0.3.post4,<0.4',
 'boltons>=21.0.0,<22.0.0', 'ecdsa>=0.17.0,<0.18.0', 'furl>=2.1.3,<3.0.0',
 'mnemonic>=0.19,<0.20', 'nest-asyncio>=1.5.4,<2.0.0',
 'protobuf>=3.19.1,<4.0.0', 'terra-proto==2.1.0', 'wrapt>=1.13.3,<2.0.0']
-setup_kwargs = { 'name': 'paloma-sdk', 'version': '3.0.7', 'description': 'The
+setup_kwargs = { 'name': 'paloma-sdk', 'version': '3.0.8', 'description': 'The
 Python SDK for Paloma', 'long_description': '
 \n
 \n\n
 ****** The Python SDK for Paloma ******
 \n
 \n\n
 (Unfamiliar with Paloma? Check_out_the_Paloma_Docs)
```

### Comparing `paloma-sdk-3.0.7/PKG-INFO` & `paloma-sdk-3.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paloma-sdk
-Version: 3.0.7
+Version: 3.0.8
 Summary: The Python SDK for Paloma
 Home-page: https://github.com/palomachain/paloma.py
 License: MIT
 Keywords: jigu,blockchain,paloma,defi,crypto
 Author: Paloma
 Requires-Python: >=3.7,<4.0
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: paloma-sdk Version: 3.0.7 Summary: The Python SDK
+Metadata-Version: 2.1 Name: paloma-sdk Version: 3.0.8 Summary: The Python SDK
 for Paloma Home-page: https://github.com/palomachain/paloma.py License: MIT
 Keywords: jigu,blockchain,paloma,defi,crypto Author: Paloma Requires-Python:
 >=3.7,<4.0 Classifier: Intended Audience :: Developers Classifier: License ::
 OSI Approved :: MIT License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

