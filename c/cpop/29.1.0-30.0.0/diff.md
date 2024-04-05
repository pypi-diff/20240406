# Comparing `tmp/cpop-29.1.0.tar.gz` & `tmp/cpop-30.0.0.tar.gz`

## Comparing `cpop-29.1.0.tar` & `cpop-30.0.0.tar`

### file list

```diff
@@ -1,176 +1,179 @@
--rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-29.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-29.1.0/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-29.1.0/src/cpop/data.pyx
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/src/hub/__init__.py
--rwxr-xr-x   0        0        0     4790 2020-02-02 00:00:00.000000 cpop-29.1.0/src/hub/__main__.py
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/config.yaml
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/exc.py
--rw-r--r--   0        0        0    22326 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/hub.py
--rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/loader.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/ref.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/log/async.py
--rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/config.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/contract.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/sub.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-29.1.0/src/pop/mods/test.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/test.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/contracts/testing.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/coro/contracts/test.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/csigs/sigs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/csigs/contracts/sigs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/external_module/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/__init__.py
--rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_bench.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_coro.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_fail.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_func.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/falias_wrap.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/proc.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/vtrue.py
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/alias_bad/init.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/alias_clash/init.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/README.rst
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/ca/config.yaml
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/ca/contract_alias/init.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/init.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/clash.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/dup1.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/dup2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/float.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/init.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/invalid.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/neg.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/neg_last.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos_first.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/contracts/zero.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/nest/init.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/config/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/__init__.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-29.1.0/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-29.1.0/.gitignore
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 cpop-29.1.0/README.rst
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 cpop-29.1.0/pyproject.toml
--rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 cpop-29.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3038 2020-02-02 00:00:00.000000 cpop-30.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8478 2020-02-02 00:00:00.000000 cpop-30.0.0/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-30.0.0/src/cpop/data.pyx
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-30.0.0/src/hub/__init__.py
+-rwxr-xr-x   0        0        0     4682 2020-02-02 00:00:00.000000 cpop-30.0.0/src/hub/__main__.py
+-rw-r--r--   0        0        0     2499 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/config.yaml
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/exc.py
+-rw-r--r--   0        0        0    24382 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/hub.py
+-rw-r--r--   0        0        0    11481 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/loader.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/verify.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/log/async.py
+-rw-r--r--   0        0        0     7547 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/config.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-30.0.0/src/pop/mods/test.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/test.py
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/contracts/testing.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/csigs/sigs.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/csigs/contracts/sigs.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/external_module/api.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/__init__.py
+-rw-r--r--   0        0        0     7495 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_cli.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_coro.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_fail.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/falias_func.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/falias_wrap.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/vtrue.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/alias_bad/init.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/alias_clash/init.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/README.rst
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/ca/config.yaml
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/ca/contract_alias/init.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/config.yaml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/init.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/clash.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/dup1.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/dup2.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/float.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/init.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/invalid.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/neg.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/neg_last.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/pos.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/contracts/zero.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/nest/init.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/config/config.yaml
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-30.0.0/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-30.0.0/.gitignore
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 cpop-30.0.0/README.rst
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 cpop-30.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5612 2020-02-02 00:00:00.000000 cpop-30.0.0/PKG-INFO
```

### Comparing `cpop-29.1.0/.pre-commit-config.yaml` & `cpop-30.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/cpop/contract.pyx` & `cpop-30.0.0/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/cpop/data.pyx` & `cpop-30.0.0/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/hub/__main__.py` & `cpop-30.0.0/src/hub/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,45 @@
 import asyncio
-import pathlib
-import pickle
 from collections.abc import Callable
 from collections.abc import Iterable
-from pprint import pprint
 
-import cpop.contract
-import cpop.data
 import pop.hub
 
 try:
     import uvloop
 
     HAS_UVLOOP = True
 except ImportError:
     HAS_UVLOOP = False
 
 
-def save_hub_state(hub, state_file: pathlib.Path):
+def save_hub_state(hub, state_file):
     # Manually retrieve the state using __getstate__
     state = hub.__getstate__()
     state_file.parent.mkdir(parents=True, exist_ok=True)
     with state_file.open("wb") as f:
-        pickle.dump(state, f)
+        hub.lib.pickle.dump(state, f)
 
 
-async def load_hub_state(hub, state_file: pathlib.Path, cli: str):
+async def load_hub_state(hub, state_file, cli: str):
     if state_file.exists():
         try:
             async with hub.lib.aiofiles.open(state_file, "rb") as f:
-                state = pickle.loads(await f.read())
+                state = hub.lib.pickle.loads(await f.read())
         except:
             return
 
         if not state:
             return
 
         if hub._init_kwargs != state["init_kwargs"]:
             cli = state["init_kwargs"].pop("cli", cli)
             state["init_kwargs"].pop("load_config", None)
             await hub.__ainit__(cli=cli, **state["init_kwargs"], load_config=False)
 
-        # Now that the hub has started, run all those waiting init tasks
-        await asyncio.gather(*hub._tasks)
-
 
 def main():
     # Initialize the event loop
     if HAS_UVLOOP:
         asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
     loop = asyncio.new_event_loop()
     asyncio.set_event_loop(loop)
@@ -64,18 +56,18 @@
 
     # Try to get a saved hub
     if original_opt.pop_cli.hub_state:
         hub_state = original_opt.pop_cli.hub_state
 
         # Evaluate a reference the hub as the hub_state
         if hub_state.startswith('f"'):
-            safe_env = {"hub": cpop.data.NamespaceDict(lib=hub.lib)}
+            safe_env = {"hub": hub.lib.cpop.data.NamespaceDict(lib=hub.lib)}
             hub_state = eval(hub_state, safe_env)
 
-        hub_state_file = pathlib.Path(hub_state).expanduser()
+        hub_state_file = hub.lib.pathlib.Path(hub_state).expanduser()
         await load_hub_state(hub, hub_state_file, cli)
     else:
         hub_state_file = None
 
     args = []
     kwargs = {}
 
@@ -126,27 +118,29 @@
                     raise
 
     # Call the named reference on the hub
     # This allows you to do
     # $ pop idem.init.cli
     # This way you can have multiple entrypoints, or even alias the above command to "idem"
     if asyncio.iscoroutinefunction(finder) or isinstance(
-        finder, (Callable, cpop.contract.Contracted)
+        finder, (Callable, hub.lib.cpop.contract.Contracted)
     ):
-        ret = await finder(*args, **kwargs)
+        ret = finder(*args, **kwargs)
+        if asyncio.iscoroutine(ret):
+            ret = await ret
     else:
         ret = finder
 
     # TODO handle generator ret
 
     try:
-        pprint(ret.__dict__)
+        hub.lib.pprint.pprint(ret.__dict__)
     except:
         if ret is not None:
-            pprint(ret)
+            hub.lib.pprint.pprint(ret)
 
     # TODO add a hub.OPT.pop_cli.dest to save the result to somewhere on the hub
 
     if hub_state_file:
         save_hub_state(hub, hub_state_file)
```

### Comparing `cpop-29.1.0/src/pop/config.yaml` & `cpop-30.0.0/src/pop/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -97,13 +97,16 @@
   - argparse
   - asyncio
   - collections
   - importlib
   - importlib.resources
   - os
   - pathlib
+  - pickle
+  - pprint
   - pop.exc
   - cpop.contract
   - cpop.data
   - pop.hub
+  - signal
   - sys
   - yaml
```

### Comparing `cpop-29.1.0/src/pop/dirs.py` & `cpop-30.0.0/src/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/exc.py` & `cpop-30.0.0/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/hub.py` & `cpop-30.0.0/src/pop/hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import asyncio
 import importlib.machinery
 import os
 import secrets
+import signal
 import sys
 from collections.abc import Iterable
 from types import ModuleType
 from typing import Any
 
 import cpop.contract
 import cpop.data
@@ -56,36 +58,38 @@
     """
 
     def __init__(self, *args, **kwargs):
         subs = {}
         sub_alias = {}
         imports = {}
         PopMeta.__init__(self, [subs, sub_alias, imports])
-        self._tasks = []
         self._subs = subs
         self._sub_alias = sub_alias
         self._imports = imports
         self._dynamic = None
         self._dscan = False
         # Set up the conf OPT structure so it is always available
         self._opt = None
+        self._task_count = 0
+        self._aio_alive = {}
 
     async def __ainit__(
         self,
         load_all_dynes: bool = True,
         load_all_subdirs: bool = True,
         recurse_subdirs: bool = True,
         pop_mods: list[str] = None,
         cli: str = None,
         logs: bool = True,
         load_config: bool = True,
     ):
         self._init_kwargs = {
             k: v for k, v in locals().items() if k != "self" and not k.startswith("_")
         }
+        self._tasks = asyncio.Queue()
 
         # Add the dyne for python imports to live in to the hub
         if "lib" not in self._subs:
             self._subs["lib"] = await AsyncSub(
                 self, subname="lib", dyne_name="lib", pypath=pop_mods
             )
             # Load all existing libraries onto hub.lib
@@ -137,33 +141,91 @@
             await self.pop.sub.add(dyne_name=dyne)
             if not self._load_all_subdirs:
                 continue
             await self.pop.sub.load_subdirs(
                 self._subs[dyne], recurse=self._recurse_subdirs
             )
 
+    def _loop_start(self, *coros, holder=True, sigint=None, sigterm=None):
+        """
+        Start a loop with a holder coroutine to run a long running application with background task tracking
+        """
+        loop = asyncio.get_running_loop()
+        if sigint:
+            s = signal.SIGINT
+            loop.add_signal_handler(s, lambda s=s: loop.create_task(sigint(s)))
+        if sigterm:
+            s = signal.SIGTERM
+            loop.add_signal_handler(s, lambda s=s: loop.create_task(sigterm(s)))
+        if holder:
+            coros = list(coros)
+            coros.append(self._holder())
+
+        try:
+            # DO NOT CHANGE THIS CALL TO run_forever! If we do that then the tracebacks
+            # do not get resolved.
+            return loop.run_until_complete(asyncio.gather(*coros))
+        except KeyboardInterrupt:
+            print("Caught keyboard interrupt. Canceling...")
+        finally:
+            loop.run_until_complete(loop.shutdown_asyncgens())
+            loop.close()
+
+    async def _holder(self):
+        """
+        Just a sleeping while loop to hold the loop open while it runs until
+        complete
+        """
+        while True:
+            complete = await self._tasks.get()
+            await complete["task"]
+            if complete["cb"]:
+                await self._auto(complete["cb"])
+            self._task_count -= 1
+            if self.task_count == 0:
+                break
+
+    def _auto(hub, coro, cb_coro=None):
+        """
+        Start a task that will be automatically awaited
+
+        coro: An unscheduled coroutine object to run
+        cb_coro: An unscheduled coroutine to run when the main coroutine completes
+        """
+        if hub._task_count:
+            hub._task_count += 1
+
+        task = hub.lib.asyncio.create_task(coro)
+
+        def _callback(task):
+            hub._tasks.put_nowait({"task": task, "cb": cb_coro})
+
+        task.add_done_callback(_callback)
+        return task
+
     def __getstate__(self) -> dict:
         attrs = {}
         for k, v in self._attrs.items():
             if isinstance(v, pop.loader.BASE_TYPES):
                 attrs[k] = v
             elif isinstance(v, dict):
                 if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v.values()):
                     attrs[k] = v
             elif isinstance(v, Iterable):
                 if all(isinstance(v2, pop.loader.BASE_TYPES) for v2 in v):
                     attrs[k] = v
-        return dict(
+        state = dict(
             init_kwargs=self._init_kwargs,
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             OPT=cpop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
+        return state
 
     def __setstate__(self, state: dict):
         subs = state["subs"]
         opt = state["OPT"]
         aliases = state["aliases"]
 
         for subname, modname in state["imports"].items():
@@ -172,15 +234,15 @@
             except ModuleNotFoundError:
                 ...
         self._attrs.update(state["attrs"])
         self._sub_alias.update(aliases)
         self._opt = cpop.data.freeze(opt)
 
         # Schedule the hub's async init function to run later
-        self._tasks.append(self.__ainit__())
+        self._auto(self.__ainit__())
         for name, data in subs.items():
             if name in self._subs:
                 sub = self._subs[name]
             else:
                 sub = Sub(hub=self, root=self, **data["init_kwargs"])
                 self._subs[name] = sub
 
@@ -435,16 +497,16 @@
 
         for name, data in subs.items():
             sub = Sub(hub=self._hub, root=self, **data["init_kwargs"])
             sub.__setstate__(data)
             self._subs[name] = sub
 
         # Initialize the Sub, put these functions on the hub to be gathered
-        self._hub._tasks.append(self.__ainit__())
-        self._hub._tasks.append(self._load_all())
+        self._hub._auto(self.__ainit__())
+        self._hub._auto(self._load_all())
 
         # Make sure all unique items make it back onto the loaded mod
         for item, data in loaded.items():
             try:
                 self._loaded[item].__setstate__(data["state"])
             except KeyError:
                 ...
```

### Comparing `cpop-29.1.0/src/pop/loader.py` & `cpop-30.0.0/src/pop/loader.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/ref.py` & `cpop-30.0.0/src/pop/ref.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/scanner.py` & `cpop-30.0.0/src/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/verify.py` & `cpop-30.0.0/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/log/async.py` & `cpop-30.0.0/src/pop/log/async.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/mods/config.py` & `cpop-30.0.0/src/pop/mods/config.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/mods/contract.py` & `cpop-30.0.0/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/mods/sub.py` & `cpop-30.0.0/src/pop/mods/sub.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/src/pop/mods/test.py` & `cpop-30.0.0/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/conftest.py` & `cpop-30.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/contracts/ctx.py` & `cpop-30.0.0/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/contracts/many.py` & `cpop-30.0.0/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/contracts/test.py` & `cpop-30.0.0/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/func/test_basic.py` & `cpop-30.0.0/tests/func/test_basic.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/func/test_contract_ctx.py` & `cpop-30.0.0/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/func/test_fail.py` & `cpop-30.0.0/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/func/test_no_raise_on_pre_failure.py` & `cpop-30.0.0/tests/func/test_no_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/func/test_raise_on_pre_failure.py` & `cpop-30.0.0/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-30.0.0/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-30.0.0/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/mods/falias_wrap.py` & `cpop-30.0.0/tests/mods/falias_wrap.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/mods/proc.py` & `cpop-30.0.0/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/mods/test.py` & `cpop-30.0.0/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/regression/contract_masking/test_contract_masking.py` & `cpop-30.0.0/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-30.0.0/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/tpath/cn/contract/test.py` & `cpop-30.0.0/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/tpath/co1/contract_ordering/init.py` & `cpop-30.0.0/tests/tpath/co1/contract_ordering/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/tpath/co1/contract_ordering/nest/init.py` & `cpop-30.0.0/tests/tpath/co1/contract_ordering/nest/init.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/tests/unit/test_contract.py` & `cpop-30.0.0/tests/unit/test_contract.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import inspect
 
+import cpop.data
 from cpop.contract import Contracted
 
 
 async def test_contracted_shortcut():
     async def f(hub):
         pass
 
-    c = Contracted(hub="a hub", contracts=[], func=f, ref="", name="")
+    mock_hub = cpop.data.NamespaceDict(_tasks=[])
+    c = Contracted(hub=mock_hub, contracts=[], func=f, ref="", name="")
     c.contract_functions["pre"] = [
         None
     ]  # add some garbage so we raise if we try to evaluate contracts
 
     await c()
```

### Comparing `cpop-29.1.0/tests/unit/test_sigs.py` & `cpop-30.0.0/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/.gitignore` & `cpop-30.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/README.rst` & `cpop-30.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-29.1.0/pyproject.toml` & `cpop-30.0.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "29.1.0"
+version = "30.0.0"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch@saltstack.com"},
 ]
 classifiers = [
```

### Comparing `cpop-29.1.0/PKG-INFO` & `cpop-30.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 29.1.0
+Version: 30.0.0
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch@saltstack.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

