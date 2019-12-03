# Openstack (Chameleon Cloud) Benchmarks (2_security)

## 2_security-openstack-marshad.md

### test_encryption.py

*FAILED*
*NOTE1: This test should be run in administrative mode.
NOTE2: First point of failure can be attributed to
`'username': os.environ['USER']`
`os.environ` does not have a key labeled `'USER'`, but rather has one called `'USERNAME'`.*

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\2_security\test_encryption.py`

Results:

`=========================================================================== test session starts ===========================================================================
platform win32 -- Python 3.7.4, pytest-5.2.4, py-1.8.0, pluggy-0.13.0 -- c:\users\m\env3\scripts\python.exe
cachedir: .pytest_cache
rootdir: C:\Users\M\cm\cloudmesh-cloud, inifile: pytest.ini
collected 3 items

cloudmesh-cloud\tests\2_local\test_ssh.py::TestSsh::test_internal_ssh
FAILED
cloudmesh-cloud\tests\2_local\test_ssh.py::TestSsh::test_ssh_processors
Processors: 1
FAILED
cloudmesh-cloud\tests\2_local\test_ssh.py::TestSsh::test_benchmark
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer         | time | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| total _ssh    |      | 2019-11-30 05:07:46 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=1 c=1 |      | 2019-11-30 05:07:46 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

================================================================================ FAILURES =================================================================================
________________________________________________________________________ TestSsh.test_internal_ssh ________________________________________________________________________

self = <test_ssh.TestSsh object at 0x040299B0>

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
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

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
_______________________________________________________________________ TestSsh.test_ssh_processors _______________________________________________________________________

self = <test_ssh.TestSsh object at 0x03D8B850>

    def test_ssh_processors(self):

        print()
        for processors in range(1, len(hosts)):
            print("Processors:", processors)
>           results = self.ssh(processors=processors)

cloudmesh-cloud\tests\2_local\test_ssh.py:89:
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh-cloud\tests\2_local\test_ssh.py:57: in ssh
    processors=processors)
cloudmesh-cloud\cloudmesh\common3\host.py:60: in ssh
    username = os.environ['USER']
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

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
======================================================================= 2 failed, 1 passed in 1.06s =======================================================================
`
