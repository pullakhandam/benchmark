# AWS Benchmarks (2_security)

## cloud-aws-marshad.md

### test_00_sys.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_00_sys.py`

Results:

`cloudmesh-cloud\tests\cloud\test_00_sys.py::Test_Sys::test_benchmark
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 1.7 GiB                                                                           |
| mem_free          | 1.7 GiB                                                                           |
| mem_percent       | 78.6%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 6.2 GiB                                                                           |
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
+---------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                     | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+---------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help | 4.799 | 2019-12-02 04:03:14 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop      | 0.0   | 2019-12-02 04:03:19 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 2 passed in 6.60s =====================`

### test_01_clean_local_remote.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_01_clean_local_remote.py`

Results:

`cloudmesh-cloud\tests\cloud\test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_benchmark
+-----------------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_01_clean_local_remote/test_cms_init                        | 27.085 | 2019-12-02 04:03:58 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.203  | 2019-12-02 04:04:25 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.215  | 2019-12-02 04:04:26 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 04:04:26 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 4 passed in 30.31s ========================================================`

### test_02_key.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_02_key.py`

Results:

`cloudmesh-cloud\tests\cloud\test_02_key.py::Test_Key::test_benchmark
+-----------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                   | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_02_key/test_upload_key_to_database | 0.061 | 2019-12-02 04:05:39 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud    | 0.083 | 2019-12-02 04:05:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_list_key_from_cloud    | 0.094 | 2019-12-02 04:05:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud  | 0.101 | 2019-12-02 04:05:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                    | 0.0   | 2019-12-02 04:05:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 7 passed in 3.69s ====================================`

### test_03_key_upload.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_03_key_upload.py`

Results:

`cloudmesh-cloud\tests\cloud\test_03_key_upload.py::Test_Key::test_benchmark
+------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                          | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_03_key_upload/test_upload_key_to_database | 0.06  | 2019-12-02 04:06:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_03_key_upload/test_upload_key_to_cloud    | 0.092 | 2019-12-02 04:06:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_03_key_upload/test_list_key_from_cloud    | 0.087 | 2019-12-02 04:06:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                           | 0.0   | 2019-12-02 04:06:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 5 passed in 3.04s =======================================`

### test_04_flavor.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_04_flavor.py`

Results:

`cloudmesh-cloud\tests\cloud\test_04_flavor.py::Test_Flavor::test_benchmark
+--------------------------------------------+---------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                      | time    | start               | tag | node        | user | system  | mac_version | win_version                     |
+--------------------------------------------+---------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_04_flavor/test_empty_database         | 0.067   | 2019-12-02 04:07:18 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_provider_flavor        | 327.527 | 2019-12-02 04:07:18 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update | 602.284 | 2019-12-02 04:12:46 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh     | 655.688 | 2019-12-02 04:22:48 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_cms_flavor             | 13.472  | 2019-12-02 04:33:44 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                       | 0.0     | 2019-12-02 04:33:58 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+--------------------------------------------+---------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

=========================================== 6 passed in 1603.44s (0:26:43) ============================================`

### test_05_image.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_05_image.py`

Results:

`cloudmesh-cloud\tests\cloud\test_05_image.py::Test_Image::test_benchmark
+------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                    | time   | start               | tag | node        | user | system  | mac_version | win_version                     |
+------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_05_image/test_empty_database        | 0.062  | 2019-12-02 04:35:05 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_provider_image        | 51.741 | 2019-12-02 04:35:05 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_provider_image_update | 47.974 | 2019-12-02 04:35:57 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_cms_image_refresh     | 54.69  | 2019-12-02 04:36:45 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_cms_image             | 26.169 | 2019-12-02 04:37:39 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                     | 0.0    | 2019-12-02 04:38:06 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

====================================================================================================== 6 passed in 183.01s (0:03:03) ===============================`

### test_06_sec_command.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_06_sec_command.py`

Results:

`cloudmesh-cloud\tests\cloud\test_06_sec_command.py::TestSecCLI::test_benchmark
+-----------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                         | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_06_sec_command/test_group_add            | 4.788 | 2019-12-02 04:38:37 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_group_delete         | 4.487 | 2019-12-02 04:38:42 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_list             | 4.484 | 2019-12-02 04:39:01 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local | 4.315 | 2019-12-02 04:39:06 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud | 4.908 | 2019-12-02 04:39:10 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                          | 0.0   | 2019-12-02 04:39:15 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 9 passed in 39.86s ======================================`

### test_07_secgroup_provider.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_07_secgroup_provider.py`

Results:

`cloudmesh-cloud\tests\cloud\test_07_secgroup_provider.py::Test_secgroup_provider::test_benchmark
+-------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                                 | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+-------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_07_secgroup_provider/test_load                   | 0.072 | 2019-12-02 04:39:45 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables         | 0.014 | 2019-12-02 04:39:45 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups         | 0.194 | 2019-12-02 04:39:45 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules   | 0.078 | 2019-12-02 04:39:46 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add          | 0.172 | 2019-12-02 04:39:46 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup        | 0.078 | 2019-12-02 04:39:46 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete       | 0.073 | 2019-12-02 04:39:46 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again | 0.072 | 2019-12-02 04:39:47 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                  | 0.0   | 2019-12-02 04:39:47 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 9 passed in 4.58s ==================================================`

### test_08_vm_provider.py

*FAILED*
*Note: Failed for 2 tests - vm wait, and vm ssh. VM wait failed with a timeout error, which looks to be referencing a keyname outside of the normal configurationn (i.e. keyname=username vs keyname=username-key). vm ssh is likely failing for AWS for the same reason as why cms vm ssh is failing; which currently requires further investigation for root-cause analysis. Note that error with vm ssh may be related to the keyname observation in vm wait.*

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_08_vm_provider.py`

Results:

`cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_benchmark
+------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                                | time   | start               | tag | node        | user | system  | mac_version | win_version                     |
+------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_08_vm_provider/test_provider_vm_create          | 3.359  | 2019-12-02 04:40:16 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| create vm test-marshad-vm-3                          | 1.814  | 2019-12-02 04:40:16 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list | 0.189  | 2019-12-02 04:40:19 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait            |        | 2019-12-02 04:40:20 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh             |        | 2019-12-02 04:46:24 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info            | 0.207  | 2019-12-02 04:46:24 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_vm_status                   | 0.33   | 2019-12-02 04:46:25 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop            | 31.127 | 2019-12-02 04:46:25 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start           | 31.265 | 2019-12-02 04:47:01 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate       | 30.886 | 2019-12-02 04:47:38 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                 | 0.0    | 2019-12-02 04:48:15 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------------------+--------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

================================================================================================================= FAILURES =================================================================================================================
__________________________________________________________________________________________________ Test_provider_vm.test_provider_vm_wait __________________________________________________________________________________________________

self = <test_08_vm_provider.Test_provider_vm object at 0x05AA66B0>

    def test_provider_vm_wait(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        cm = CmDatabase()
        vm = cm.find_name(name, kind="vm")[0]
>       assert provider.wait(vm=vm), "cms wait timed out ..."
E       AssertionError: cms wait timed out ...
E       assert False
E        +  where False = <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x05316B90>>(vm={'KeyName': 'marshad-key', '_id': ObjectId('5de495b069582d4969b43300'), 'cm': {'cloud': 'aws', 'collection': 'aws-vm', 'created': '2019-12-02 04:40:19.993087', 'creation_time': '2.00', ...}, 'created': '12/02/2019, 04:40:17', ...})
E        +    where <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x05316B90>> = <cloudmesh.compute.vm.Provider.Provider object at 0x05316B90>.wait

cloudmesh-cloud\tests\cloud\test_08_vm_provider.py:81: AssertionError
__________________________________________________________________________________________________ Test_provider_vm.test_provider_vm_ssh ___________________________________________________________________________________________________

self = <test_08_vm_provider.Test_provider_vm object at 0x05BF7190>

    def test_provider_vm_ssh(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        cm = CmDatabase()
        vm = cm.find_name(name, kind="vm")[0]
>       data = provider.ssh(vm=vm, command='echo IAmAlive')

cloudmesh-cloud\tests\cloud\test_08_vm_provider.py:90:
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh-cloud\cloudmesh\compute\vm\Provider.py:445: in ssh
    return self.p.ssh(vm=vm, command=command)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.aws.Provider.Provider object at 0x0531A890>
vm = {'KeyName': 'marshad-key', '_id': ObjectId('5de495b069582d4969b43300'), 'cm': {'cloud': 'aws', 'collection': 'aws-vm', 'created': '2019-12-02 04:40:19.993087', 'creation_time': '2.00', ...}, 'created': '12/02/2019, 04:40:17', ...}
command = 'echo IAmAlive'

    def ssh(self, vm=None, command=None):

        def key_selector(keys):
            '''
           This is a helper method for ssh key selection
           THIS IS JUST A SAFETY MEASURE, PLEASE DON'T MIND IT
            :param keys:
            :return:
            '''
            tmp_keys = keys[:]
            # indices = range(1,len(tmp_keys)+1)
            for key_idx, key in enumerate(keys):
                key['idx'] = key_idx + 1;
            print(Printer.flatwrite(tmp_keys,
                                    sort_keys=["idx"],
                                    order=['idx', 'KeyName', 'KeyFingerprint'],
                                    header=['Index', 'Key Name', "Key Fingerprint"],
                                    output="table",
                                    humanize=None)
                  )
            # Console.msg("Please select one of the AWS key indices from the table above: ")
            picked = 0
            while picked < 1 or picked > len(keys):
                try:
                    picked = int(input("Please select one of the AWS key indices from the table above: "))
                except ValueError:
                    pass
            return keys[picked - 1]

        cm = CmDatabase()
        ip = vm['public_ips']

        try:
            key_name = vm['KeyName']
            keys = cm.find_all_by_name(name=key_name, kind="key")
            for k in keys:
                if 'location' in k.keys():
                    if 'private' in k['location'].keys():
                        key = k['location']['private']
                        break

        except (KeyError, IndexError):
            aws_keys = cm.find(kind='key', cloud='aws')
            if len(aws_keys) == 0 :
                Console.error(f"Could not find a key for the AWS instance '{vm['name']}'")
                Console.error(f"Use `cms help key` to learn how to add and upload a key for AWS")
                return
            aws_key = key_selector(aws_keys)
            for sshkey in cm.find_all_by_name(name=aws_key['KeyName'], kind="key"):
                if "location" in sshkey.keys():
                    key = sshkey['location']['private']
                    break
        user = "ubuntu"  # needs to be set on creation.

        if command is None:
            command = ""

        if user is None:
            location = ip
        else:
>           location = user + '@' + ip
E           TypeError: can only concatenate str (not "NoneType") to str

cloudmesh-cloud\cloudmesh\compute\aws\Provider.py:651: TypeError
================================================================================================= 2 failed, 8 passed in 481.53s (0:08:01) ============================================`

### test_09_cm_names_find.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_09_cm_names_find.py`

Results:

`cloudmesh-cloud\tests\cloud\test_09_cm_names_find.py::Test_cm_find::test_benchmark
+-----------------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| timer                                                           | time  | start               | tag | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+
| test_09_cm_names_find/test_cm_find_collection                   | 0.064 | 2019-12-02 05:09:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_loop                         | 2.515 | 2019-12-02 05:09:36 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_cloud                  | 0.306 | 2019-12-02 05:09:39 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_collection             | 0.317 | 2019-12-02 05:09:39 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_names_regexp                         | 0.22  | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vms                          | 0.018 | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_ubuntu_in_images             | 0.163 | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_cloud_name_attributes        | 0.021 | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections               | 0.017 | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections_vm            | 0.02  | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collection_form_parameter | 0.015 | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                            | 0.0   | 2019-12-02 05:09:40 | aws | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------------------------+-------+---------------------+-----+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================================================ 13 passed in 6.29s ============================================================`
