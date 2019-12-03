# AWS Benchmarks (2_local)

## 2_local-aws-marshad.md

### test_ssh

*FAILED*
*NOTE: first point of failure can be attributed to
`'username': os.environ['USER']`
`os.environ` does not have a key labeled `'USER'`, but rather has one called `'USERNAME'`.*

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\2_local\test_ssh.py`

Results:

`cloudmesh-cloud\tests\2_local\test_ssh.py::TestSsh::test_benchmark
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer         | time | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| total _ssh    |      | 2019-12-02 03:59:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=1 c=1 |      | 2019-12-02 03:59:23 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

================================================================================================================= FAILURES =================================================================================================================
________________________________________________________________________________________________________ TestSsh.test_internal_ssh _________________________________________________________________________________________________________

self = <test_ssh.TestSsh object at 0x036BC930>

    def test_internal_ssh(self):
        print()
        StopWatch.start("total _ssh")

        for host in hosts:
            location = {
                'host': host,
>               'username': os.environ['USER'],
                'key': '~/.ssh/id_rsa.pub',
                'command': 'uname -a'

            }

cloudmesh-cloud\tests\2_local\test_ssh.py:69:
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = environ({'ALLUSERSPROFILE': 'C:\\ProgramData', 'APPDATA': 'C:\\Users\\M\\AppData\\Roaming', 'COMMONPROGRAMFILES': 'C:\... '_OLD_VIRTUAL_PROMPT': '$P$G', 'PYTEST_CURRENT_TEST': 'tests/2_local/test_ssh.py::TestSsh::test_internal_ssh (call)'})
key = 'USER'

    def __getitem__(self, key):
        try:
            value = self._data[self.encodekey(key)]
        except KeyError:
            # raise KeyError with the original key value
>           raise KeyError(key) from None
E           KeyError: 'USER'

..\AppData\Local\Programs\Python\Python37-32\lib\os.py:678: KeyError
_______________________________________________________________________________________________________ TestSsh.test_ssh_processors ________________________________________________________________________________________________________

self = <test_ssh.TestSsh object at 0x038DF510>

    def test_ssh_processors(self):

        print()
        for processors in range(1, len(hosts)):
            print("Processors:", processors)
>           results = self.ssh(processors=processors)

cloudmesh-cloud\tests\2_local\test_ssh.py:89:
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh-cloud\tests\2_local\test_ssh.py:57: in ssh
    processors=processors)
cloudmesh-cloud\cloudmesh\common3\host.py:60: in ssh
    username = os.environ['USER']
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = environ({'ALLUSERSPROFILE': 'C:\\ProgramData', 'APPDATA': 'C:\\Users\\M\\AppData\\Roaming', 'COMMONPROGRAMFILES': 'C:\..._OLD_VIRTUAL_PROMPT': '$P$G', 'PYTEST_CURRENT_TEST': 'tests/2_local/test_ssh.py::TestSsh::test_ssh_processors (call)'})
key = 'USER'

    def __getitem__(self, key):
        try:
            value = self._data[self.encodekey(key)]
        except KeyError:
            # raise KeyError with the original key value
>           raise KeyError(key) from None
E           KeyError: 'USER'

..\AppData\Local\Programs\Python\Python37-32\lib\os.py:678: KeyError
======================================================================================================= 2 failed, 1 passed in 1.17s ========================================================`
