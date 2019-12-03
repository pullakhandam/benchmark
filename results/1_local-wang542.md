# 1_local Benchmark
## Summary
* test_data fails because grp isn't supported
* test_name fails because of hardcoded name in assertion, name "gregor-vm"
* test_ping fails because windows need admin mode to run the commands
* test_sec_command fails because shell isn't supported in windows
* Overall, similar behavior as Arshad's benchamark run

### test-cms
tests/1_local/test_cms.py::TestConfig::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 5.9 GiB                                                                           |
| mem_free          | 5.9 GiB                                                                           |
| mem_percent       | 62.8%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 10.0 GiB                                                                          |
| node              | ('LAPTOP-0UEFF4CG',)                                                              |
| platform          | Windows-10-10.0.17763-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 158 Stepping 10, GenuineIntel',)                         |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 20:34:20) [MSC v.1916 64 bit (AMD64)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.17763                                                                        |
| win_version       | ('10', '10.0.17763', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+--------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                    | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+--------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_cms/test_help       | 2.624 | 2019-12-02 22:02:40 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_cms/test_vm         | 2.664 | 2019-12-02 22:02:42 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_cms/test_help_again | 2.565 | 2019-12-02 22:02:45 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop     | 0.0   | 2019-12-02 22:02:48 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+--------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================== 4 passed in 8.54s ==============================
### test_config
tests/1_local/test_config.py::TestConfig::test_benchmark 
+---------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                 | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+---------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_config_load n=1                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=2                  | 0.052 | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=3                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=4                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=5                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=6                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=7                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=8                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config_load n=9                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config/test_search               | 0.005 | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config/test_dict                 | 0.003 | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config/test_config_subscriptable | 0.003 | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config/test_dictreplace          | 0.005 | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_config/test_set                  | 0.03  | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                  | 0.0   | 2019-12-02 22:02:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+---------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================== 9 passed in 1.01s ==============================
### test_data
=================================== ERRORS ====================================
_________________ ERROR collecting tests/1_local/test_data.py _________________
ImportError while importing test module 'D:\School\B649_engineeringCloudComputing\ENV4\cm\cloudmesh-cloud\tests\1_local\test_data.py'.
Hint: make sure your test modules/packages have valid Python names.
Traceback:
tests\1_local\test_data.py:5: in <module>
    import grp
E   ModuleNotFoundError: No module named 'grp'
!!!!!!!!!!!!!!!!!!! Interrupted: 1 errors during collection !!!!!!!!!!!!!!!!!!!
============================== 1 error in 0.05s ===============================
### test_group
tests/1_local/test_group.py::TestName::test_benchmark 
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_group/test_list | 0.757 | 2019-12-02 22:03:32 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_group/test_add  | 0.278 | 2019-12-02 22:03:33 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-12-02 22:03:34 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================== 4 passed in 2.58s ==============================
### test_key
tests/1_local/test_key.py::TestName::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 5.9 GiB                                                                           |
| mem_free          | 5.9 GiB                                                                           |
| mem_percent       | 62.9%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 10.0 GiB                                                                          |
| node              | ('LAPTOP-0UEFF4CG',)                                                              |
| platform          | Windows-10-10.0.17763-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 158 Stepping 10, GenuineIntel',)                         |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 20:34:20) [MSC v.1916 64 bit (AMD64)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.17763                                                                        |
| win_version       | ('10', '10.0.17763', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_key/test_key    | 0.064 | 2019-12-02 22:03:51 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_key/test_git    | 0.343 | 2019-12-02 22:03:51 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop | 0.0   | 2019-12-02 22:03:51 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+----------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================== 3 passed in 1.33s ==============================
### test_name
================================== FAILURES ===================================
____________________________ TestName.test_define _____________________________

self = <test_name.TestName object at 0x00000245F8B6C6C8>

    def test_define(self):
        Benchmark.Start()
        n = Name()
        Benchmark.Stop()
>       assert dict(data) == n.dict()
E       AssertionError: assert {'counter': 1...d': 'vm', ...} == {'counter': 1...r': 'wang542'}
E         Omitting 2 identical items, use -vv to show
E         Differing items:
E         {'user': 'user'} != {'user': 'wang542'}
E         {'schema': '{experiment}-{group}-{user}-{kind}-{counter}'} != {'schema': '{user}-vm-{counter}'}
E         Left contains 3 more items:
E         {'experiment': 'exp', 'group': 'group', 'kind': 'vm'}
E         Full diff:...
E         
E         ...Full output truncated (10 lines hidden), use '-vv' to show

tests\1_local\test_name.py:42: AssertionError
__________________________ TestName.test_define_new ___________________________

self = <test_name.TestName object at 0x00000245F8BB01C8>

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
E         {'user': 'wang542'} != {'user': 'gregor'}
E         {'counter': 1} != {'counter': 3}
E         {'path': 'C:\\Users\\wangc\\.cloudmesh\\name.yaml'} != {'path': '/Users/grey/.cloudmesh/name.yaml'}
E         Full diff:
E         - {'counter': 1,...
E         
E         ...Full output truncated (12 lines hidden), use '-vv' to show

tests\1_local\test_name.py:55: AssertionError
__________________________ TestName.test_name_print ___________________________

self = <test_name.TestName object at 0x00000245F8BB83C8>

    def test_name_print(self):
        n = Name()
        Benchmark.Start()
        print(n)
        Benchmark.Start()
>       assert str(n) == "gregor-vm-1"
E       AssertionError: assert 'wang542-vm-1' == 'gregor-vm-1'
E         - wang542-vm-1
E         + gregor-vm-1

tests\1_local\test_name.py:73: AssertionError
___________________________ TestName.test_name_dict ___________________________

self = <test_name.TestName object at 0x00000245F8BBC5C8>

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
E         {'user': 'wang542'} != {'user': 'gregor'}
E         {'path': 'C:\\Users\\wangc\\.cloudmesh\\name.yaml'} != {'path': '/Users/grey/.cloudmesh/name.yaml'}
E         Full diff:
E         {'counter': 1,
E         'kind': 'vm',...
E         
E         ...Full output truncated (8 lines hidden), use '-vv' to show

tests\1_local\test_name.py:81: AssertionError
___________________________ TestName.test_name_incr ___________________________

self = <test_name.TestName object at 0x00000245F8BC0B88>

    def test_name_incr(self):
        n = Name()
        Benchmark.Start()
        n.incr()
        Benchmark.Stop()
        print(n)
>       assert str(n) == "gregor-vm-2"
E       AssertionError: assert 'wang542-vm-2' == 'gregor-vm-2'
E         - wang542-vm-2
E         + gregor-vm-2

tests\1_local\test_name.py:93: AssertionError
========================= 5 failed, 3 passed in 1.03s =========================
### test_ping
tests/1_local/test_ping.py::TestPing::test_ping_processor 
Processors: 1
+-----------------------+---------+-----+-----+--------+
| host                  | success | max | min | stddev |
+-----------------------+---------+-----+-----+--------+
| 127.0.0.1             | False   |     |     |        |
| localhost             | False   |     |     |        |
| www.indiana.edu       | False   |     |     |        |
| www.pbs.org           | False   |     |     |        |
| www.github.com        | False   |     |     |        |
| www.redhat.com        | False   |     |     |        |
| www.openstack.org     | False   |     |     |        |
| www.bbc.com           | False   |     |     |        |
| www.ec2instances.info | False   |     |     |        |
| aws.amazon.com        | False   |     |     |        |
+-----------------------+---------+-----+-----+--------+
FAILED
tests/1_local/test_ping.py::TestPing::test_benchmark 
+----------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer          | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+----------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| total _ping    | 0.019 | 2019-12-02 22:04:53 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| ping 127.0.0.1 | 0.019 | 2019-12-02 22:04:53 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| total p=1 c=1  | 0.432 | 2019-12-02 22:04:53 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+----------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
================================== FAILURES ===================================
_________________________ TestPing.test_internal_ping _________________________

self = <test_ping.TestPing object at 0x0000017E54DD8988>

    def test_internal_ping(self):
        StopWatch.start("total _ping")
    
        for host in hosts:
            location = {
                'ip': host,
                'count': 1,
            }
    
            StopWatch.start(f"ping {host}")
            result = Host._ping(location)
            StopWatch.stop(f"ping {host}")
    
            StopWatch.stop("total _ping")
    
    
>           assert result['success']
E           assert False

tests\1_local\test_ping.py:56: AssertionError
________________________ TestPing.test_ping_processor _________________________

self = <test_ping.TestPing object at 0x0000017E54DDFD08>

    def test_ping_processor(self):
    
        print ()
        for processors in range(1,len(hosts)):
            print ("Processors:", processors)
            results = self.ping(processors=processors)
            print (Printer.write(results,
                                 order=['host',
                                         'success',
                                         'max',
                                         'min',
                                         'stddev']
                                 ))
            for result in results:
>               assert result['success']
E               assert False

tests\1_local\test_ping.py:72: AssertionError
========================= 2 failed, 1 passed in 1.10s =========================
### test_sec_command
================================== FAILURES ===================================
____________________________ TestSecCLI.test_clear ____________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A7363188>

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

tests\1_local\test_sec_command.py:55: AssertionError
__________________________ TestSecCLI.test_rule_add ___________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A73E1188>

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

tests\1_local\test_sec_command.py:83: AssertionError
__________________________ TestSecCLI.test_group_add __________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A735D648>

    def test_group_add(self):
        HEADING()
    
        Benchmark.Start()
        result = run("group add", f"cms sec group add deleteme empty empty")
        Benchmark.Stop()
    
        entry = groups.list(name="deleteme")
    
>       assert len(entry) > 0
E       assert 0 > 0
E        +  where 0 = len([])

tests\1_local\test_sec_command.py:106: AssertionError
__________________________ TestSecCLI.test_rule_list __________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A7353408>

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
E           AssertionError: assert 'ssh' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO...\r\n    sec clear\r\n\r\nERROR: Could not execute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\n'

tests\1_local\test_sec_command.py:132: AssertionError
____________________________ TestSecCLI.test_list _____________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A73BFB08>

    def test_list(self):
        HEADING()
    
        Benchmark.Start()
        result = run("list", "cms sec list")
        Benchmark.Stop()
    
        g = groups.list()
    
        for entry in g:
            name = entry['name']
>           assert name in result
E           AssertionError: assert 'default' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO...\r\n    sec clear\r\n\r\nERROR: Could not execute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\n'

tests\1_local\test_sec_command.py:148: AssertionError
_________________________ TestSecCLI.test_group_list __________________________

self = <test_sec_command.TestSecCLI object at 0x00000146A73DB448>

    def test_group_list(self):
        HEADING()
    
        Benchmark.Start()
        result = run("list", "cms sec group list")
        Benchmark.Stop()
    
        g = groups.list()
    
        for entry in g:
            name = entry['name']
>           assert name in result
E           AssertionError: assert 'default' in '\r\nUsage:\r\n\r\n    sec rule list [--cloud=CLOUDS] [--output=OUTPUT]\r\n    sec rule add RULE FROMPORT TOPORT PROTO...\r\n    sec clear\r\n\r\nERROR: Could not execute the command. Please check usage with\r\n\r\n    cms help sec\r\n\r\n'

tests\1_local\test_sec_command.py:161: AssertionError
======================== 6 failed, 4 passed in 28.46s =========================
tests/1_local/test_sec_command.py::TestSecCLI::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 5.8 GiB                                                                           |
| mem_free          | 5.8 GiB                                                                           |
| mem_percent       | 63.3%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 10.1 GiB                                                                          |
| node              | ('LAPTOP-0UEFF4CG',)                                                              |
| platform          | Windows-10-10.0.17763-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 158 Stepping 10, GenuineIntel',)                         |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 20:34:20) [MSC v.1916 64 bit (AMD64)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.17763                                                                        |
| win_version       | ('10', '10.0.17763', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                              | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_sec_command/test_clear        | 2.616 | 2019-12-02 22:05:10 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local clear                        | 2.613 | 2019-12-02 22:05:10 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_load         | 2.541 | 2019-12-02 22:05:14 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local load                         | 2.538 | 2019-12-02 22:05:14 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_rule_add     | 2.541 | 2019-12-02 22:05:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local rule add                     | 2.537 | 2019-12-02 22:05:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_rule_delete  | 2.641 | 2019-12-02 22:05:20 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local rule delete                  | 2.638 | 2019-12-02 22:05:20 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_group_add    | 2.551 | 2019-12-02 22:05:23 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local group add                    | 2.548 | 2019-12-02 22:05:23 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_group_delete | 2.709 | 2019-12-02 22:05:26 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local group delete                 | 2.706 | 2019-12-02 22:05:26 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_rule_list    | 2.92  | 2019-12-02 22:05:29 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local rule list                    | 2.916 | 2019-12-02 22:05:29 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_list         | 2.584 | 2019-12-02 22:05:32 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| local list                         | 2.721 | 2019-12-02 22:05:35 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_sec_command/test_group_list   | 2.725 | 2019-12-02 22:05:35 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop               | 0.0   | 2019-12-02 22:05:38 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
### test_secgroup
tests/1_local/test_secgroup_database.py::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 6.1 GiB                                                                           |
| mem_free          | 6.1 GiB                                                                           |
| mem_percent       | 61.8%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 9.8 GiB                                                                           |
| node              | ('LAPTOP-0UEFF4CG',)                                                              |
| platform          | Windows-10-10.0.17763-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 158 Stepping 10, GenuineIntel',)                         |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 20:34:20) [MSC v.1916 64 bit (AMD64)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.17763                                                                        |
| win_version       | ('10', '10.0.17763', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+----------------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                              | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+----------------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_secgroup_database/test_clear                  | 0.552 | 2019-12-02 22:06:24 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_upload_groups          | 1.202 | 2019-12-02 22:06:25 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_upload_rules           | 2.07  | 2019-12-02 22:06:27 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_add_rule_to_group      | 0.503 | 2019-12-02 22:06:29 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_delete_rule_from_group | 0.84  | 2019-12-02 22:06:31 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_remove_group           | 0.257 | 2019-12-02 22:06:33 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_remove_rule            | 0.289 | 2019-12-02 22:06:33 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_secgroup_database/test_load_defaults          | 0.309 | 2019-12-02 22:06:34 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                               | 0.0   | 2019-12-02 22:06:35 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+----------------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================= 9 passed in 12.37s ==============================
### test_shell
tests/1_local/test_shell.py::TestName::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 6.1 GiB                                                                           |
| mem_free          | 6.1 GiB                                                                           |
| mem_percent       | 61.7%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 9.8 GiB                                                                           |
| node              | ('LAPTOP-0UEFF4CG',)                                                              |
| platform          | Windows-10-10.0.17763-SP0                                                         |
| processor         | ('Intel64 Family 6 Model 158 Stepping 10, GenuineIntel',)                         |
| processors        | Windows                                                                           |
| python            | 3.7.4 (tags/v3.7.4:e09359112e, Jul  8 2019, 20:34:20) [MSC v.1916 64 bit (AMD64)] |
| release           | ('10',)                                                                           |
| sys               | win32                                                                             |
| system            | Windows                                                                           |
| user              |                                                                                   |
| version           | 10.0.17763                                                                        |
| win_version       | ('10', '10.0.17763', 'SP0', '')                                                   |
+-------------------+-----------------------------------------------------------------------------------+
+---------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                       | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+---------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_shell/test_shell                       | 0.004 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_shell/test_pwd                         | 0.121 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_shell/test_ls_la_list                  | 0.005 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_shell/test_ls_la_string                | 0.005 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_shell/test_ls_la_wrapper               | 0.004 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_shell/test_ls_la_wrapper_multi_options | 0.005 | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                        | 0.0   | 2019-12-02 22:07:17 |     | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+---------------------------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
PASSED
============================== 7 passed in 0.87s ==============================