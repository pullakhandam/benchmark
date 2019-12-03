# AWS Benchmarks (1_local)

## 1_local-aws-marshad.md

### test_cms

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_cms.py`

Results:

`cloudmesh-cloud\tests\1_local\test_cms.py::TestConfig::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 518.0 MiB                                                                         |
| mem_free          | 518.0 MiB                                                                         |
| mem_percent       | 93.6%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 7.4 GiB                                                                           |
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
| test_cms/test_help       | 4.649 | 2019-12-02 03:34:35 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_cms/test_vm         | 4.269 | 2019-12-02 03:34:40 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_cms/test_help_again | 4.418 | 2019-12-02 03:34:44 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop     | 0.0   | 2019-12-02 03:34:49 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+--------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 4 passed in 14.61s ===============================================`

### test_config

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_config.py`

Result:

`cloudmesh-cloud\tests\1_local\test_config.py::TestConfig::test_benchmark
+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                 | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_config_load n=1                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=2                  | 0.282 | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=3                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=4                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=5                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=6                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=7                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=8                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config_load n=9                  | 0.0   | 2019-12-02 03:44:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_search               | 0.018 | 2019-12-02 03:44:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_dict                 | 0.017 | 2019-12-02 03:44:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_config_subscriptable | 0.014 | 2019-12-02 03:44:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_dictreplace          | 0.02  | 2019-12-02 03:44:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_config/test_set                  | 0.142 | 2019-12-02 03:44:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                  | 0.0   | 2019-12-02 03:44:25 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 9 passed in 3.81s ===========================================================
`

### test_data

*FAILED*
*Failure is likely due to unsupported python modules on windows, `grp` and `pwd`. These modules are used in: test_DatabaseUpdate*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_data.py`

Result:
`=========================================================================================================== test session starts ============================================================================================================
platform win32 -- Python 3.7.4, pytest-5.2.4, py-1.8.0, pluggy-0.13.0 -- c:\users\m\env3\scripts\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\M\cm\cloudmesh-cloud, inifile: pytest.ini
collected 0 items / 1 errors

================================================================================================================== ERRORS ==================================================================================================================
_______________________________________________________________________________________________ ERROR collecting tests/1_local/test_data.py ________________________________________________________________________________________________
ImportError while importing test module 'C:\Users\M\cm\cloudmesh-cloud\tests\1_local\test_data.py'.
Hint: make sure your test modules/packages have valid Python names.
Traceback:
cloudmesh-cloud\tests\1_local\test_data.py:5: in <module>
    import grp
E   ModuleNotFoundError: No module named 'grp'
!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!! Interrupted: 1 errors during collection !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
============================================================================================================= 1 error in 0.17s =============================================================================================================
`

### test_group

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_group.py`

Result:
`cloudmesh-cloud\tests\1_local\test_group.py::TestName::test_benchmark
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_group/test_list | 0.096 | 2019-12-02 03:49:45 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_group/test_add  | 0.064 | 2019-12-02 03:49:45 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-12-02 03:49:46 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 4 passed in 2.13s =============================================`

### test_key

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_key.py`

Result:

`cloudmesh-cloud\tests\1_local\test_key.py::TestName::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1009.9 MiB                                                                        |
| mem_free          | 1009.9 MiB                                                                        |
| mem_percent       | 87.5%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.9 GiB                                                                           |
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
| test_key/test_key    | 0.174 | 2019-12-02 03:50:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_key/test_git    | 0.163 | 2019-12-02 03:50:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-12-02 03:50:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 3 passed in 1.77s ===========================`

### test_name

*FAILED*
*Errors are likely due to the mismatches when assert is called. There are hardcoded values (e.g. ‘gregor’, ‘/Users/gray/.cloudmesh/name.yaml’) that are being compared against and failing.*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_name.py`

Result:

`cloudmesh-cloud\tests\1_local\test_name.py::TestName::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 993.4 MiB                                                                         |
| mem_free          | 993.4 MiB                                                                         |
| mem_percent       | 87.7%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.9 GiB                                                                           |
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
| test_name/test_define       | 0.157 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_define_new   | 0.015 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_reset   | 0.013 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_print   |       | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_dict    | 0.012 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_incr    | 0.012 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_name/test_name_counter | 0.008 | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop        | 0.0   | 2019-12-02 03:51:03 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

================================================================================================================= FAILURES =================================================================================================================
___________________________________________________________________________________________________________ TestName.test_define ___________________________________________________________________________________________________________

self = <test_name.TestName object at 0x04A2E9D0>

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
_________________________________________________________________________________________________________ TestName.test_define_new _________________________________________________________________________________________________________

self = <test_name.TestName object at 0x04AD8570>

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
_________________________________________________________________________________________________________ TestName.test_name_print _________________________________________________________________________________________________________

self = <test_name.TestName object at 0x04AD3D90>

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
_________________________________________________________________________________________________________ TestName.test_name_dict __________________________________________________________________________________________________________

self = <test_name.TestName object at 0x04AD3950>

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
_________________________________________________________________________________________________________ TestName.test_name_incr __________________________________________________________________________________________________________

self = <test_name.TestName object at 0x04ADB5B0>

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
======================================================================================================= 5 failed, 3 passed in 2.10s ========================================================================================================`

### test_ping

*Note: This test requires the command line interface be run in administrative mode*

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_ping.py`

Result:

`cloudmesh-cloud\tests\1_local\test_ping.py::TestPing::test_benchmark
+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                      | time   | start               | tag | node        | user | system  | mac_version | win_version                     |
+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| total _ping                | 30.769 | 2019-12-02 03:52:09 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping 127.0.0.1             | 3.133  | 2019-12-02 03:52:09 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping localhost             | 3.032  | 2019-12-02 03:52:12 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.indiana.edu       | 3.09   | 2019-12-02 03:52:15 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.pbs.org           | 3.057  | 2019-12-02 03:52:18 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.github.com        | 3.061  | 2019-12-02 03:52:21 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.redhat.com        | 3.104  | 2019-12-02 03:52:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.openstack.org     | 3.11   | 2019-12-02 03:52:27 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.bbc.com           | 3.055  | 2019-12-02 03:52:30 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping www.ec2instances.info | 3.061  | 2019-12-02 03:52:33 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| ping aws.amazon.com        | 3.067  | 2019-12-02 03:52:37 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=1 c=1              | 31.732 | 2019-12-02 03:52:40 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=2 c=1              | 19.578 | 2019-12-02 03:53:11 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=3 c=1              | 13.77  | 2019-12-02 03:53:31 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=4 c=1              | 11.323 | 2019-12-02 03:53:45 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=5 c=1              | 8.772  | 2019-12-02 03:53:56 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=6 c=1              | 9.082  | 2019-12-02 03:54:05 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=7 c=1              | 10.213 | 2019-12-02 03:54:14 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=8 c=1              | 9.901  | 2019-12-02 03:54:24 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=9 c=1              | 10.152 | 2019-12-02 03:54:34 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

====================================================================================================== 3 passed in 156.25s (0:02:36) ======================================`

### test_sec_command

*FAILED*
*NOTE: This test fails on Windows due to:
`from cloudmesh.common3.Shell import Shell`
This is not supported on Windows yet, but works fine on Linux/OSX*

TODO: Fix cloudmesh.common3.Shell to work with Windows.

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_sec_command.py`

Result:

`cloudmesh-cloud\tests\1_local\test_sec_command.py::TestSecCLI::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.3 GiB                                                                           |
| mem_free          | 1.3 GiB                                                                           |
| mem_percent       | 84.1%                                                                             |
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
| test_sec_command/test_clear        | 4.402 | 2019-12-02 03:55:43 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local clear                        | 4.383 | 2019-12-02 03:55:43 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_load         | 4.311 | 2019-12-02 03:55:47 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local load                         | 4.292 | 2019-12-02 03:55:47 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_add     | 4.672 | 2019-12-02 03:55:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule add                     | 4.654 | 2019-12-02 03:55:52 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_delete  | 4.271 | 2019-12-02 03:55:57 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule delete                  | 4.254 | 2019-12-02 03:55:57 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_add    | 4.284 | 2019-12-02 03:56:01 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local group add                    | 4.264 | 2019-12-02 03:56:01 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_delete | 4.751 | 2019-12-02 03:56:05 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local group delete                 | 4.733 | 2019-12-02 03:56:05 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_rule_list    | 4.33  | 2019-12-02 03:56:10 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local rule list                    | 4.314 | 2019-12-02 03:56:10 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_list         | 4.306 | 2019-12-02 03:56:14 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| local list                         | 4.271 | 2019-12-02 03:56:19 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_sec_command/test_group_list   | 4.291 | 2019-12-02 03:56:19 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop               | 0.0   | 2019-12-02 03:56:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

================================================================================================================= FAILURES =================================================================================================================
__________________________________________________________________________________________________________ TestSecCLI.test_clear ___________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04AE80B0>

    def test_clear(self):
        HEADING(color="HEADER")

        Benchmark.Start()
        run("clear", "cms sec clear")
        Benchmark.Stop()

        r = rules.list()
        g = groups.list()

>       assert len(r) == 0
E       assert 5 == 0
E         -5
E         +0

cloudmesh-cloud\tests\1_local\test_sec_command.py:55: AssertionError
_________________________________________________________________________________________________________ TestSecCLI.test_rule_add _________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04AF0CD0>

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

cloudmesh-cloud\tests\1_local\test_sec_command.py:83: AssertionError
________________________________________________________________________________________________________ TestSecCLI.test_group_add _________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04AF0C10>

    def test_group_add(self):
        HEADING()

        Benchmark.Start()
        result = run("group add", f"cms sec group add deleteme empty empty")
        Benchmark.Stop()

        entry = groups.list(name="deleteme")

>       assert len(entry) > 0
E       assert 0 > 0
E        +  where 0 = len([])

cloudmesh-cloud\tests\1_local\test_sec_command.py:106: AssertionError
________________________________________________________________________________________________________ TestSecCLI.test_rule_list _________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04B001D0>

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

cloudmesh-cloud\tests\1_local\test_sec_command.py:132: AssertionError
___________________________________________________________________________________________________________ TestSecCLI.test_list ___________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04AF8370>

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

cloudmesh-cloud\tests\1_local\test_sec_command.py:148: AssertionError
________________________________________________________________________________________________________ TestSecCLI.test_group_list ________________________________________________________________________________________________________

self = <test_sec_command.TestSecCLI object at 0x04B03530>

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

cloudmesh-cloud\tests\1_local\test_sec_command.py:161: AssertionError
======================================================================================================= 6 failed, 4 passed in 42.03s ======================================================`

### test_secgroup_database

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_secgroup_database.py`

Result:

`cloudmesh-cloud\tests\1_local\test_secgroup_database.py::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.6 GiB                                                                           |
| mem_free          | 1.6 GiB                                                                           |
| mem_percent       | 79.6%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.3 GiB                                                                           |
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
| test_secgroup_database/test_clear                  | 0.077 | 2019-12-02 03:57:39 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_upload_groups          | 0.29  | 2019-12-02 03:57:39 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_upload_rules           | 1.987 | 2019-12-02 03:57:40 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_add_rule_to_group      | 0.041 | 2019-12-02 03:57:42 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_delete_rule_from_group | 0.042 | 2019-12-02 03:57:43 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_remove_group           | 0.023 | 2019-12-02 03:57:43 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_remove_rule            | 0.024 | 2019-12-02 03:57:44 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_secgroup_database/test_load_defaults          | 0.458 | 2019-12-02 03:57:44 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                               | 0.0   | 2019-12-02 03:57:44 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+----------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 9 passed in 6.88s ===================================================`

### test_shell

Executed:

`pytest -v --capture=no cloudmesh-cloud\tests\1_local\test_shell.py`

Result:

`cloudmesh-cloud\tests\1_local\test_shell.py::TestName::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.6 GiB                                                                           |
| mem_free          | 1.6 GiB                                                                           |
| mem_percent       | 79.7%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.3 GiB                                                                           |
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
| test_shell/test_shell                       | 0.018 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_pwd                         | 0.054 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_list                  | 0.026 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_string                | 0.028 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_wrapper               | 0.027 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_shell/test_ls_la_wrapper_multi_options | 0.038 | 2019-12-02 03:58:22 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                        | 0.0   | 2019-12-02 03:58:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 7 passed in 1.17s =========================================`
