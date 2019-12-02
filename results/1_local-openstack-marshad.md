# Openstack (Chameleon Cloud) Benchmarks (1_local)

## 1_local-openstack-marshad.md

### test_cms

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_cms.py`

Results:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attrbute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.1 GiB                                                                           |
| mem_free          | 1.1 GiB                                                                           |
| mem_percent       | 86.2%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.8 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+--------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                    | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+--------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_cms/test_help       | 3.938 | 2019-11-29 17:12:00 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_cms/test_vm         | 5.203 | 2019-11-29 17:12:04 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_cms/test_help_again | 4.923 | 2019-11-29 17:12:09 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop     | 0.0   | 2019-11-29 17:12:14 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+--------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

=========================================================================== 4 passed in 15.35s ============================================================================`

### test_config

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_config.py`

Result:

`+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                 | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_config_load n=1                  | 0.0   | 2019-11-29 17:36:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=2                  | 0.128 | 2019-11-29 17:36:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=3                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=4                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=5                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=6                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=7                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=8                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=9                  | 0.0   | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_search               | 0.011 | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_dict                 | 0.009 | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_config_subscriptable | 0.009 | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_dictreplace          | 0.014 | 2019-11-29 17:36:26 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_set                  | 0.076 | 2019-11-29 17:36:27 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                  | 0.0   | 2019-11-29 17:36:27 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ 9 passed in 2.37s ============================================================================
`

### test_data

*FAILED*
*Failure is likely due to unsupported python modules on windows, `grp` and `pwd`. These modules are used in: test_DatabaseUpdate*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_data.py`

Result:
`=========================================================================== test session starts ===========================================================================
platform win32 -- Python 3.7.4, pytest-5.2.4, py-1.8.0, pluggy-0.13.0 -- c:\users\m\env3\scripts\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\M\cm\cloudmesh-cloud, inifile: pytest.ini
collected 0 items / 1 errors

================================================================================= ERRORS ==================================================================================
_______________________________________________________________ ERROR collecting tests/1_local/test_data.py _______________________________________________________________
ImportError while importing test module 'C:\Users\M\cm\cloudmesh-cloud\tests\1_local\test_data.py'.
Hint: make sure your test modules/packages have valid Python names.
Traceback:
cloudmesh-cloud\tests\1_local\test_data.py:5: in <module>
    import grp
E   ModuleNotFoundError: No module named 'grp'
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! Interrupted: 1 errors during collection !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
============================================================================ 1 error in 0.16s =============================================================================
`

### test_group

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_group.py`

Result:
`cloudmesh-cloud\tests\1_local\test_group.py::TestName::test_benchmark
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_group/test_list | 1.999 | 2019-11-29 18:01:36 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_group/test_add  | 0.91  | 2019-11-29 18:01:38 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-11-29 18:01:40 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

====================================================== 4 passed in 6.49s =======================================================`

### test_key

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_key.py`

Result:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.2 GiB                                                                           |
| mem_free          | 1.2 GiB                                                                           |
| mem_percent       | 85.3%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.7 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_key/test_key    | 0.141 | 2019-11-29 18:10:06 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_key/test_git    | 0.838 | 2019-11-29 18:10:07 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-11-29 18:10:07 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ 3 passed in 2.46s ================================================`

### test_name

*FAILED*
*Errors are likely due to the mismatches when assert is called. There are hardcoded values (e.g. ‘gregor’, ‘/Users/gray/.cloudmesh/name.yaml’) that are being compared against and failing.*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_name.py`

Result:

`=========================================================================== test session starts ===========================================================================
platform win32 -- Python 3.7.4, pytest-5.2.4, py-1.8.0, pluggy-0.13.0 -- c:\users\m\env3\scripts\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\M\cm\cloudmesh-cloud, inifile: pytest.ini
collected 8 items

cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_define FAILED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_define_new {'counter': 1,
 'kind': 'vm',
 'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml',
 'schema': '{user}-{kind}-{counter}',
 'user': 'marshad'}
FAILED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_name_reset PASSED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_name_print marshad-vm-1
FAILED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_name_dict {'counter': 1,
 'kind': 'vm',
 'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml',
 'schema': '{user}-{kind}-{counter}',
 'user': 'marshad'}
FAILED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_name_incr marshad-vm-2
FAILED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_name_counter 2
{'counter': 2,
 'kind': 'vm',
 'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml',
 'schema': '{user}-{kind}-{counter}',
 'user': 'marshad'}
{'counter': 2,
 'kind': 'vm',
 'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml',
 'schema': '{user}-{kind}-{counter}',
 'user': 'marshad'}
marshad-vm-2
PASSED
cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.3 GiB                                                                           |
| mem_free          | 1.3 GiB                                                                           |
| mem_percent       | 83.4%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.6 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+-----------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                       | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+-----------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_name/test_define       | 0.152 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_define_new   | 0.014 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_reset   | 0.012 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_print   |       | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_dict    | 0.011 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_incr    | 0.015 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_counter | 0.007 | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop        | 0.0   | 2019-11-29 18:46:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

================================================================================ FAILURES =================================================================================
__________________________________________________________________________ TestName.test_define ___________________________________________________________________________

self = <test_name.TestName object at 0x049B4A50>

    def test_define(self):
        Benchmark.Start()
        n = Name()
        Benchmark.Stop()
>       assert dict(data) == n.dict()
E       AssertionError: assert {'counter': 1...d': 'vm', ...} == {'counter': 1...r': 'marshad'}
E         Omitting 2 identical items, use -vv to show
E         Differing items:
E         {'schema': '{experiment}-{group}-{user}-{kind}-{counter}'} != {'schema': '{user}-vm-{counter}'}
E         {'user': 'user'} != {'user': 'marshad'}
E         Left contains 3 more items:
E         {'experiment': 'exp', 'group': 'group', 'kind': 'vm'}
E         Full diff:...
E
E         ...Full output truncated (10 lines hidden), use '-vv' to show

cloudmesh-cloud\tests\1_local\test_name.py:42: AssertionError
________________________________________________________________________ TestName.test_define_new _________________________________________________________________________

self = <test_name.TestName object at 0x04A59210>

    def test_define_new(self):
        os.remove(path)

        Benchmark.Start()
        n = Name(schema="{user}-{kind}-{counter}",
                 counter="3",
                 user="gregor",
                 kind="vm")
        Benchmark.Stop()
        data = n.dict()
        pprint(data)
>       assert data == dict({'counter': 3,
                             'kind': 'vm',
                             'path': '/Users/grey/.cloudmesh/name.yaml',
                             'schema': '{user}-{kind}-{counter}',
                             'user': 'gregor'})
E       AssertionError: assert {'counter': 1...ounter}', ...} == {'counter': 3...ounter}', ...}
E         Omitting 2 identical items, use -vv to show
E         Differing items:
E         {'counter': 1} != {'counter': 3}
E         {'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml'} != {'path': '/Users/grey/.cloudmesh/name.yaml'}
E         {'user': 'marshad'} != {'user': 'gregor'}
E         Full diff:
E         - {'counter': 1,...
E
E         ...Full output truncated (12 lines hidden), use '-vv' to show

cloudmesh-cloud\tests\1_local\test_name.py:55: AssertionError
________________________________________________________________________ TestName.test_name_print _________________________________________________________________________

self = <test_name.TestName object at 0x04A5CAD0>

    def test_name_print(self):
        n = Name()
        Benchmark.Start()
        print(n)
        Benchmark.Start()
>       assert str(n) == "gregor-vm-1"
E       AssertionError: assert 'marshad-vm-1' == 'gregor-vm-1'
E         - marshad-vm-1
E         + gregor-vm-1

cloudmesh-cloud\tests\1_local\test_name.py:73: AssertionError
_________________________________________________________________________ TestName.test_name_dict _________________________________________________________________________

self = <test_name.TestName object at 0x04A55550>

    def test_name_dict(self):
        n = Name()
        pprint(n.dict())
        Benchmark.Start()
        data = n.dict()
        Benchmark.Stop()
>       assert data == dict({'counter': 1,
                             'kind': 'vm',
                             'path': '/Users/grey/.cloudmesh/name.yaml',
                             'schema': '{user}-{kind}-{counter}',
                             'user': 'gregor'})
E       AssertionError: assert {'counter': 1...ounter}', ...} == {'counter': 1...ounter}', ...}
E         Omitting 3 identical items, use -vv to show
E         Differing items:
E         {'path': 'C:\\Users\\M\\.cloudmesh\\name.yaml'} != {'path': '/Users/grey/.cloudmesh/name.yaml'}
E         {'user': 'marshad'} != {'user': 'gregor'}
E         Full diff:
E         {'counter': 1,
E         'kind': 'vm',...
E
E         ...Full output truncated (8 lines hidden), use '-vv' to show

cloudmesh-cloud\tests\1_local\test_name.py:81: AssertionError
_________________________________________________________________________ TestName.test_name_incr _________________________________________________________________________

self = <test_name.TestName object at 0x04A59F30>

    def test_name_incr(self):
        n = Name()
        Benchmark.Start()
        n.incr()
        Benchmark.Stop()
        print(n)
>       assert str(n) == "gregor-vm-2"
E       AssertionError: assert 'marshad-vm-2' == 'gregor-vm-2'
E         - marshad-vm-2
E         + gregor-vm-2

cloudmesh-cloud\tests\1_local\test_name.py:93: AssertionError
======================================================================= 5 failed, 3 passed in 1.83s =======================================================================

`

### test_ping

*Note: This test requires the command line interface be run in administrative mode*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_ping.py`

Result:

`+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                      | time   | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| total _ping                | 33.477 | 2019-11-29 21:50:42 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping 127.0.0.1             | 3.033  | 2019-11-29 21:50:42 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping localhost             | 3.048  | 2019-11-29 21:50:45 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.indiana.edu       | 3.083  | 2019-11-29 21:50:48 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.pbs.org           | 3.197  | 2019-11-29 21:50:51 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.github.com        | 3.239  | 2019-11-29 21:50:54 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.redhat.com        | 4.254  | 2019-11-29 21:50:57 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.openstack.org     | 3.089  | 2019-11-29 21:51:01 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.bbc.com           | 3.192  | 2019-11-29 21:51:05 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.ec2instances.info | 3.148  | 2019-11-29 21:51:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping aws.amazon.com        | 4.194  | 2019-11-29 21:51:11 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=1 c=1              | 33.312 | 2019-11-29 21:51:15 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=2 c=1              | 19.715 | 2019-11-29 21:51:48 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=3 c=1              | 14.021 | 2019-11-29 21:52:08 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=4 c=1              | 11.063 | 2019-11-29 21:52:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=5 c=1              | 8.557  | 2019-11-29 21:52:33 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=6 c=1              | 8.747  | 2019-11-29 21:52:42 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=7 c=1              | 9.048  | 2019-11-29 21:52:51 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=8 c=1              | 9.312  | 2019-11-29 21:53:00 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=9 c=1              | 9.664  | 2019-11-29 21:53:09 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
PASSED

============================================ 3 passed in 157.83s (0:02:37) ============================================

`

### test_sec_command

*FAILED*
*NOTE: This test fails on Windows due to:
`from cloudmesh.common3.Shell import Shell`
This is not supported on Windows yet, but works fine on Linux/OSX*

TODO: Fix cloudmesh.common3.Shell to work with Windows.

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_sec_command.py`

Result:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.3 GiB                                                                           |
| mem_free          | 1.3 GiB                                                                           |
| mem_percent       | 84.2%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.7 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                              | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_sec_command/test_clear        |       | 2019-11-29 22:13:55 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_load         | 3.766 | 2019-11-29 22:13:55 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local load                         | 3.752 | 2019-11-29 22:13:55 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_add     | 4.305 | 2019-11-29 22:14:01 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule add                     | 4.285 | 2019-11-29 22:14:01 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_delete  | 3.783 | 2019-11-29 22:14:06 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule delete                  | 3.765 | 2019-11-29 22:14:06 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_add    | 3.802 | 2019-11-29 22:14:10 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local group add                    | 3.783 | 2019-11-29 22:14:10 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_delete | 3.811 | 2019-11-29 22:14:15 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local group delete                 | 3.796 | 2019-11-29 22:14:15 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_list    | 4.311 | 2019-11-29 22:14:19 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule list                    | 4.287 | 2019-11-29 22:14:19 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_list         | 3.778 | 2019-11-29 22:14:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local list                         | 3.842 | 2019-11-29 22:14:29 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_list   | 3.859 | 2019-11-29 22:14:29 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop               | 0.0   | 2019-11-29 22:14:34 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

================================================================================ FAILURES =================================================================================
__________________________________________________________________________ TestSecCLI.test_clear __________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F761F0>

    def test_clear(self):
        HEADING(color="HEADER")

        Benchmark.Start()
        #run("clear", "cms sec clear")
>       run("cms sec clear")
E       TypeError: run() missing 1 required positional argument: 'command'

cloudmesh-cloud\tests\1_local\test_sec_command.py:50: TypeError
________________________________________________________________________ TestSecCLI.test_rule_add _________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F72230>

    def test_rule_add(self):
        HEADING()

        Benchmark.Start()
        result = run("rule add",
                     f"cms sec rule add deleteme FROMPORT TOPORT PROTOCOL CIDR")
        Benchmark.Stop()

        entry = rules.list(name="deleteme")

>       assert len(entry) > 0
E       assert 0 > 0
E        +  where 0 = len([])

cloudmesh-cloud\tests\1_local\test_sec_command.py:89: AssertionError
________________________________________________________________________ TestSecCLI.test_group_add ________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F76D10>

    def test_group_add(self):
        HEADING()

        Benchmark.Start()
        result = run("group add", f"cms sec group add deleteme empty empty")
        Benchmark.Stop()

        entry = groups.list(name="deleteme")

>       assert len(entry) > 0
E       assert 0 > 0
E        +  where 0 = len([])

cloudmesh-cloud\tests\1_local\test_sec_command.py:112: AssertionError
________________________________________________________________________ TestSecCLI.test_rule_list ________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F853D0>

    def test_rule_list(self):
        HEADING()

        Benchmark.Start()
        result = run("rule list", "cms sec rule list")
        Benchmark.Stop()

        r = rules.list()
        g = groups.list()

        for entry in r:
            name = entry['name']
>           assert name in result
E           AssertionError: assert 'ssh' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO...execute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\nTimer: 0.0000s (sec rule list; exit 0)\r\n'

cloudmesh-cloud\tests\1_local\test_sec_command.py:138: AssertionError
__________________________________________________________________________ TestSecCLI.test_list ___________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F8E330>

    def test_list(self):
        HEADING()

        Benchmark.Start()
        result = run("list", "cms sec list")
        Benchmark.Stop()

        g = groups.list()

        for entry in g:
            name = entry['name']
>           assert name in result
E           AssertionError: assert 'default' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO... not execute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\nTimer: 0.0000s (sec list; exit 0)\r\n'

cloudmesh-cloud\tests\1_local\test_sec_command.py:154: AssertionError
_______________________________________________________________________ TestSecCLI.test_group_list ________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04F916D0>

    def test_group_list(self):
        HEADING()

        Benchmark.Start()
        result = run("list", "cms sec group list")
        Benchmark.Stop()

        g = groups.list()

        for entry in g:
            name = entry['name']
>           assert name in result
E           AssertionError: assert 'default' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO...xecute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\nTimer: 0.0000s (sec group list; exit 0)\r\n'

cloudmesh-cloud\tests\1_local\test_sec_command.py:167: AssertionError
====================================================================== 6 failed, 4 passed in 40.79s =======================================================================`

### test_secgroup_database

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_secgroup_database.py`

Result:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.4 GiB                                                                           |
| mem_free          | 1.4 GiB                                                                           |
| mem_percent       | 82.7%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.5 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+----------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                              | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_secgroup_database/test_clear                  | 1.515 | 2019-11-29 22:50:57 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_upload_groups          | 3.165 | 2019-11-29 22:51:00 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_upload_rules           | 3.752 | 2019-11-29 22:51:04 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_add_rule_to_group      | 1.446 | 2019-11-29 22:51:09 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_delete_rule_from_group | 1.433 | 2019-11-29 22:51:13 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_remove_group           | 0.728 | 2019-11-29 22:51:16 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_remove_rule            | 0.956 | 2019-11-29 22:51:19 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_load_defaults          | 0.801 | 2019-11-29 22:51:21 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                               | 0.0   | 2019-11-29 22:51:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

=========================================================================== 9 passed in 29.25s ============================================================================`

### test_shell

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_shell.py`

Result:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.2 GiB                                                                           |
| mem_free          | 1.2 GiB                                                                           |
| mem_percent       | 84.9%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.7 GiB                                                                           |
| node              | ('ONYX64',)                                                                       |
| platform          | Windows-10-10.0.18362-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 61 Stepping 4, GenuineIntel',)                           |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 19:29:22) [MSC v.1916 32 bit (Intel)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.18362                                                                        |
| win_version       | ('10', '10.0.18362', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+---------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                       | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_shell/test_shell                       | 0.019 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_pwd                         | 0.018 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_list                  | 0.017 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_string                | 0.018 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_wrapper               | 0.018 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_wrapper_multi_options | 0.019 | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                        | 0.0   | 2019-11-29 22:52:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ 7 passed in 1.02s ======================================================================`
