#Openstack (Chameleon Cloud) Benchmarks (2_local)

##2_local-openstack-marshad.md

###test_ssh

*FAILED*
*NOTE: first point of failure can be attributed to
`'username': os.environ['USER']`
`os.environ` does not have a key labeled `'USER'`, but rather has one called `'USERNAME'`.*

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\2_local\test_ssh.py`

Results:

`+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer         | time | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| total _ssh    |      | 2019-11-29 23:20:06 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| total p=1 c=1 |      | 2019-11-29 23:20:06 |     | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------+------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

================================================================================ FAILURES =================================================================================
________________________________________________________________________ TestSsh.test_internal_ssh ________________________________________________________________________

self = <test_ssh.TestSsh object at 0x04630350>

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

self = <test_ssh.TestSsh object at 0x046E95F0>

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
======================================================================= 2 failed, 1 passed in 0.96s =======================================================================

`


##2_security-aws-USERNAME.md

##cloud-aws-USERNAME.md

##others

###aws-USERNAME.md

###azure-USERNAME.md

###google-USERNAME.md

##storage tests
###storage-USERNAME.md

other storage tests are in cloudmesh-storage\tests
