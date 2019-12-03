# Cloud-Openstack Benchmark (Chameleon Cloud)
* Complete output can be accessed [here](https://github.com/cloudmesh-community/fa19-516-157/tree/master/Benchmark_Output)
## Summary
* test_08_vm_provider failed due to wrong key name, the keyname wang542-key was set by test, not by user

## test_00_sys
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 6.8 GiB                                                                           |
| mem_free          | 6.8 GiB                                                                           |
| mem_percent       | 57.4%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 9.1 GiB                                                                           |
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
+---------------------------+-------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                     | time  | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+---------------------------+-------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help | 2.584 | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop      | 0.0   | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+---------------------------+-------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_01_clean_local_remote
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:31:15 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test__02_key.py
tests/cloud/test_02_key.py::Test_Key::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_03_key_upload
tests/cloud/test_03_key_upload.py::Test_Key::test_cleanup SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_upload_key_to_database SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_upload_key_to_cloud SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_list_key_from_cloud SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_benchmark SKIPPED
## test_04_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_05_image
PASSED
tests/cloud/test_05_image.py::Test_Image::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:31:55 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.311  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               | 4.562  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        | 4.062  | 2019-12-02 22:31:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 7.631  | 2019-12-02 22:31:43 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.687  | 2019-12-02 22:31:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_06_sec_command
tests/cloud/test_06_sec_command.py::TestSecCLI::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:32:29 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.311  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               | 4.562  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        | 4.062  | 2019-12-02 22:31:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 7.631  | 2019-12-02 22:31:43 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.687  | 2019-12-02 22:31:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 3.895  | 2019-12-02 22:31:55 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.436  | 2019-12-02 22:31:59 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.405  | 2019-12-02 22:32:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.345  | 2019-12-02 22:32:21 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.982  | 2019-12-02 22:32:25 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_07_secgroup_provider
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:32:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.311  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               | 4.562  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        | 4.062  | 2019-12-02 22:31:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 7.631  | 2019-12-02 22:31:43 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.687  | 2019-12-02 22:31:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 3.895  | 2019-12-02 22:31:55 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.436  | 2019-12-02 22:31:59 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.405  | 2019-12-02 22:32:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.345  | 2019-12-02 22:32:21 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.982  | 2019-12-02 22:32:25 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.341  | 2019-12-02 22:32:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.003  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 1.156  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.461  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.477  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  |        | 2019-12-02 22:32:33 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 1.355  | 2019-12-02 22:32:36 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.778  | 2019-12-02 22:32:37 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## test_08_vm_provider
######################################################################
test_provider_vm_create \tests\cloud\test_08_vm_provider.py 55
######################################################################
[31mERROR: Problem starting vm[0m
`
Trace:
Traceback (most recent call last):
      File "d:\school\b649_engineeringcloudcomputing\env4\cm\cloudmesh-cloud\cloudmesh\compute\openstack\Provider.py", line 952, in create
        timeout=timeout
      File "<d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\decorator.py:decorator-gen-4>", line 2, in create_server
      File "d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\cloud\_utils.py", line 378, in func_wrapper
        return func(*args, **kwargs)
      File "d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\cloud\_compute.py", line 936, in create_server
        self.compute.post(endpoint, json=server_json))
      File "d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\proxy.py", line 443, in _json_response
        exceptions.raise_from_response(response, error_message=error_message)
      File "d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\exceptions.py", line 229, in raise_from_response
        http_status=http_status, request_id=request_id
    openstack.exceptions.BadRequestException: BadRequestException: 400: Client Error for url: https://openstack.tacc.chameleoncloud.org:8774/v2/CH-819337/servers, Invalid key_name provided.

BadRequestException: 400: Client Error for url: https://openstack.tacc.chameleoncloud.org:8774/v2/CH-819337/servers, Invalid key_name provided.`


tests/cloud/test_08_vm_provider.py::Test_provider_vm::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:39:45 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.311  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               | 4.562  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        | 4.062  | 2019-12-02 22:31:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 7.631  | 2019-12-02 22:31:43 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.687  | 2019-12-02 22:31:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 3.895  | 2019-12-02 22:31:55 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.436  | 2019-12-02 22:31:59 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.405  | 2019-12-02 22:32:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.345  | 2019-12-02 22:32:21 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.982  | 2019-12-02 22:32:25 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.341  | 2019-12-02 22:32:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.003  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 1.156  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.461  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.477  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  |        | 2019-12-02 22:32:33 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 1.355  | 2019-12-02 22:32:36 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.778  | 2019-12-02 22:32:37 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_create                     |        | 2019-12-02 22:32:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| create vm test-wang542-vm-3                                     |        | 2019-12-02 22:32:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list            | 1.736  | 2019-12-02 22:32:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait                       |        | 2019-12-02 22:32:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh                        |        | 2019-12-02 22:39:38 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info                       | 1.074  | 2019-12-02 22:39:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_vm_status                              |        | 2019-12-02 22:39:40 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop                       |        | 2019-12-02 22:39:41 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start                      |        | 2019-12-02 22:39:42 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate                  |        | 2019-12-02 22:39:44 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
## test_09_cm_names_find
tests/cloud/test_09_cm_names_find.py::Test_cm_find::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.584  | 2019-12-02 22:30:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:39:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.132 | 2019-12-02 22:30:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.68   | 2019-12-02 22:31:11 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 2.655  | 2019-12-02 22:31:13 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.343  | 2019-12-02 22:31:17 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.379  | 2019-12-02 22:31:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.693  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.658  | 2019-12-02 22:31:19 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.338  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 2.023  | 2019-12-02 22:31:20 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 1.305  | 2019-12-02 22:31:22 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 5.718  | 2019-12-02 22:31:24 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 3.778  | 2019-12-02 22:31:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.311  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               | 4.562  | 2019-12-02 22:31:34 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        | 4.062  | 2019-12-02 22:31:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 7.631  | 2019-12-02 22:31:43 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.687  | 2019-12-02 22:31:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 3.895  | 2019-12-02 22:31:55 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.436  | 2019-12-02 22:31:59 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.405  | 2019-12-02 22:32:18 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.345  | 2019-12-02 22:32:21 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.982  | 2019-12-02 22:32:25 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.341  | 2019-12-02 22:32:30 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.003  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 1.156  | 2019-12-02 22:32:31 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.461  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.477  | 2019-12-02 22:32:32 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  |        | 2019-12-02 22:32:33 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 1.355  | 2019-12-02 22:32:36 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.778  | 2019-12-02 22:32:37 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_create                     |        | 2019-12-02 22:32:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| create vm test-wang542-vm-3                                     |        | 2019-12-02 22:32:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list            | 1.736  | 2019-12-02 22:32:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait                       |        | 2019-12-02 22:32:51 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh                        |        | 2019-12-02 22:39:38 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info                       | 1.074  | 2019-12-02 22:39:39 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_vm_status                              |        | 2019-12-02 22:39:40 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop                       |        | 2019-12-02 22:39:41 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start                      |        | 2019-12-02 22:39:42 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate                  |        | 2019-12-02 22:39:44 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_collection                   | 0.317  | 2019-12-02 22:39:45 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_loop                         | 0.948  | 2019-12-02 22:39:45 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_cloud                  | 0.31   | 2019-12-02 22:39:47 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_collection             | 0.326  | 2019-12-02 22:39:47 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_names_regexp                         | 0.717  | 2019-12-02 22:39:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vms                          | 0.331  | 2019-12-02 22:39:48 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_ubuntu_in_images             | 0.311  | 2019-12-02 22:39:49 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_cloud_name_attributes        | 0.296  | 2019-12-02 22:39:49 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections               | 0.312  | 2019-12-02 22:39:49 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections_vm            | 0.299  | 2019-12-02 22:39:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collection_form_parameter | 0.296  | 2019-12-02 22:39:50 | chameleon | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+----------------------+------+---------+-------------+---------------------------------+
PASSED
## Failures
================================== FAILURES ===================================
_________________ Test_secgroup_provider.test_upload_secgroup _________________

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6515D88>
name = 'Test_Sec_Group', rules = ['ssh']

    def add_rules_to_secgroup(self, name=None, rules=None):
        if name is None and rules is None:
            raise ValueError("name or rules are None")
    
        cgroups = self.list_secgroups(name)
        if len(cgroups) == 0:
            raise ValueError("group does not exist")
    
        groups = DictList(Secgroup().list())
        rules_details = DictList(SecgroupRule().list())
    
        try:
>           group = groups[name]
E           KeyError: 'Test_Sec_Group'

cloudmesh\compute\openstack\Provider.py:540: KeyError

During handling of the above exception, another exception occurred:

self = <test_07_secgroup_provider.Test_secgroup_provider object at 0x0000018DD7FBED08>

    def test_upload_secgroup(self):
        HEADING()
        name = "Test_Sec_Group"
        Benchmark.Start()
>       provider.upload_secgroup(name=name)

tests\cloud\test_07_secgroup_provider.py:107: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\compute\vm\Provider.py:422: in upload_secgroup
    return self.p.upload_secgroup(name=name)
cloudmesh\compute\openstack\Provider.py:525: in upload_secgroup
    rules=[found['name']])
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6515D88>
name = 'Test_Sec_Group', rules = ['ssh']

    def add_rules_to_secgroup(self, name=None, rules=None):
        if name is None and rules is None:
            raise ValueError("name or rules are None")
    
        cgroups = self.list_secgroups(name)
        if len(cgroups) == 0:
            raise ValueError("group does not exist")
    
        groups = DictList(Secgroup().list())
        rules_details = DictList(SecgroupRule().list())
    
        try:
            group = groups[name]
        except:
>           raise ValueError("group does not exist")
E           ValueError: group does not exist

cloudmesh\compute\openstack\Provider.py:542: ValueError
__________________ Test_provider_vm.test_provider_vm_create ___________________

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
name = 'test-wang542-vm-3', image = 'CC-Ubuntu18.04', size = 'm1.medium'
location = None, timeout = 360, key = 'wang542-key', secgroup = None
ip = '129.114.33.186', user = 'cc', public = True, group = 'cloudmesh'
metadata = None, cloud = 'chameleon', kwargs = {}, image_use = None
flavor_use = None, groups = ['cloudmesh']

    def create(self,
               name=None,
               image=None,
               size=None,
               location=None,
               timeout=360,
               key=None,
               secgroup=None,
               ip=None,
               user=None,
               public=True,
               group=None,
               metadata=None,
               cloud=None,
               **kwargs):
        """
        creates a named node
    
    
        :param group: the list of groups the vm belongs to
        :param name: the name of the node
        :param image: the image used
        :param size: the size of the image
        :param timeout: a timeout in seconds that is invoked in case the image
                        does not boot. The default is set to 3 minutes.
        :param kwargs: additional arguments HEADING(c=".")ed along at time of
                       boot
        :return:
        """
        image_use = None
        flavor_use = None
    
        # keyname = Config()["cloudmesh"]["profile"]["user"]
        # ex_keyname has to be the registered keypair name in cloud
    
        """
        https://docs.openstack.org/openstacksdk/latest/user/connection.html#openstack.connection.Connection.create_server
    
        """
    
        if 'flavor' in kwargs and size is None:
            size = kwargs['flavor']
    
        # Guess user name
    
        if user is None:
            user = Image.guess_username(image)
            # image_name = image.lower()
            # if image_name.startswith("cc-"):
            #    user = "cc"
            # if "centos" in image_name:
            #    user = "centos"
            # elif "ubuntu" in image_name:
            #    user = "ubuntu"
    
        # get IP
    
        if not ip and public:
            ip = self.find_available_public_ip()
            # pprint(entry)
    
        elif ip is not None:
            entry = self.list_public_ips(ip=ip, available=True)
            if len(entry) == 0:
                print("ip not available")
                raise ValueError(f"The ip can not be assigned {ip}")
    
        if type(group) == str:
            groups = Parameter.expand(group)
    
        banner("Create Server")
        print("    Name:    ", name)
        print("    User:    ", user)
        print("    IP:      ", ip)
        print("    Image:   ", image)
        print("    Size:    ", size)
        print("    Public:  ", public)
        print("    Key:     ", key)
        print("    location:", location)
        print("    timeout: ", timeout)
        print("    secgroup:", secgroup)
        print("    group:   ", group)
        print("    groups:  ", groups)
        print()
    
        try:
            server = self.cloudman.create_server(name,
                                                 flavor=size,
                                                 image=image,
                                                 key_name=key,
                                                 security_groups=[secgroup],
>                                                timeout=timeout
                                                 # tags=groups,
                                                 # wait=True
                                                 )

cloudmesh\compute\openstack\Provider.py:952: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <openstack.connection.Connection object at 0x0000018DD6E20408>
name = 'test-wang542-vm-3', image = 'CC-Ubuntu18.04', flavor = 'm1.medium'
auto_ip = True, ips = None, ip_pool = None, root_volume = None
terminate_volume = False, wait = False, timeout = 360, reuse_ips = True
network = None, boot_from_volume = False, volume_size = '50', boot_volume = None
volumes = None, nat_destination = None, group = None
kwargs = {'key_name': 'wang542-key', 'security_groups': [None]}

>   ???

<d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\decorator.py:decorator-gen-4>:2: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

func = <function ComputeCloudMixin.create_server at 0x0000018DD67EA798>
args = (<openstack.connection.Connection object at 0x0000018DD6E20408>, 'test-wang542-vm-3', 'CC-Ubuntu18.04', 'm1.medium', True, None, ...)
kwargs = {'key_name': 'wang542-key', 'security_groups': [None]}
argspec = ArgSpec(args=['self', 'name', 'image', 'flavor', 'auto_ip', 'ips', 'ip_pool', 'root_volume', 'terminate_volume', 'wait...gs', defaults=(None, None, True, None, None, None, False, False, 180, True, None, False, '50', None, None, None, None))
k = 'security_groups'

    @decorator
    def func_wrapper(func, *args, **kwargs):
        argspec = inspect.getargspec(func)
        for k in kwargs:
            if k not in argspec.args[1:] and k not in valid_args:
                raise TypeError(
                    "{f}() got an unexpected keyword argument "
                    "'{arg}'".format(f=inspect.stack()[1][3], arg=k))
>       return func(*args, **kwargs)

..\..\lib\site-packages\openstack\cloud\_utils.py:378: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <openstack.connection.Connection object at 0x0000018DD6E20408>
name = 'test-wang542-vm-3', image = 'CC-Ubuntu18.04', flavor = 'm1.medium'
auto_ip = True, ips = None, ip_pool = None, root_volume = None
terminate_volume = False, wait = False, timeout = 360, reuse_ips = True
network = None, boot_from_volume = False, volume_size = '50', boot_volume = None
volumes = [], nat_destination = None, group = None
kwargs = {'flavorRef': '3', 'imageRef': '8ab218cb-ad18-4771-aa6a-776704b4af12', 'key_name': 'wang542-key', 'max_count': 1, ...}
server_json = {'server': {'flavorRef': '3', 'imageRef': '8ab218cb-ad18-4771-aa6a-776704b4af12', 'key_name': 'wang542-key', 'max_count': 1, ...}}
security_groups = [None], sec_group = None, desired = 'adminPass'
given = 'admin_pass', value = None

    @_utils.valid_kwargs(
        'meta', 'files', 'userdata',
        'reservation_id', 'return_raw', 'min_count',
        'max_count', 'security_groups', 'key_name',
        'availability_zone', 'block_device_mapping',
        'block_device_mapping_v2', 'nics', 'scheduler_hints',
        'config_drive', 'admin_pass', 'disk_config')
    def create_server(
            self, name, image=None, flavor=None,
            auto_ip=True, ips=None, ip_pool=None,
            root_volume=None, terminate_volume=False,
            wait=False, timeout=180, reuse_ips=True,
            network=None, boot_from_volume=False, volume_size='50',
            boot_volume=None, volumes=None, nat_destination=None,
            group=None,
            **kwargs):
        """Create a virtual server instance.
    
        :param name: Something to name the server.
        :param image: Image dict, name or ID to boot with. image is required
                      unless boot_volume is given.
        :param flavor: Flavor dict, name or ID to boot onto.
        :param auto_ip: Whether to take actions to find a routable IP for
                        the server. (defaults to True)
        :param ips: List of IPs to attach to the server (defaults to None)
        :param ip_pool: Name of the network or floating IP pool to get an
                        address from. (defaults to None)
        :param root_volume: Name or ID of a volume to boot from
                            (defaults to None - deprecated, use boot_volume)
        :param boot_volume: Name or ID of a volume to boot from
                            (defaults to None)
        :param terminate_volume: If booting from a volume, whether it should
                                 be deleted when the server is destroyed.
                                 (defaults to False)
        :param volumes: (optional) A list of volumes to attach to the server
        :param meta: (optional) A dict of arbitrary key/value metadata to
                     store for this server. Both keys and values must be
                     <=255 characters.
        :param files: (optional, deprecated) A dict of files to overwrite
                      on the server upon boot. Keys are file names (i.e.
                      ``/etc/passwd``) and values
                      are the file contents (either as a string or as a
                      file-like object). A maximum of five entries is allowed,
                      and each file must be 10k or less.
        :param reservation_id: a UUID for the set of servers being requested.
        :param min_count: (optional extension) The minimum number of
                          servers to launch.
        :param max_count: (optional extension) The maximum number of
                          servers to launch.
        :param security_groups: A list of security group names
        :param userdata: user data to pass to be exposed by the metadata
                      server this can be a file type object as well or a
                      string.
        :param key_name: (optional extension) name of previously created
                      keypair to inject into the instance.
        :param availability_zone: Name of the availability zone for instance
                                  placement.
        :param block_device_mapping: (optional) A dict of block
                      device mappings for this server.
        :param block_device_mapping_v2: (optional) A dict of block
                      device mappings for this server.
        :param nics:  (optional extension) an ordered list of nics to be
                      added to this server, with information about
                      connected networks, fixed IPs, port etc.
        :param scheduler_hints: (optional extension) arbitrary key-value pairs
                            specified by the client to help boot an instance
        :param config_drive: (optional extension) value for config drive
                            either boolean, or volume-id
        :param disk_config: (optional extension) control how the disk is
                            partitioned when the server is created.  possible
                            values are 'AUTO' or 'MANUAL'.
        :param admin_pass: (optional extension) add a user supplied admin
                           password.
        :param wait: (optional) Wait for the address to appear as assigned
                     to the server. Defaults to False.
        :param timeout: (optional) Seconds to wait, defaults to 60.
                        See the ``wait`` parameter.
        :param reuse_ips: (optional) Whether to attempt to reuse pre-existing
                                     floating ips should a floating IP be
                                     needed (defaults to True)
        :param network: (optional) Network dict or name or ID to attach the
                        server to.  Mutually exclusive with the nics parameter.
                        Can also be be a list of network names or IDs or
                        network dicts.
        :param boot_from_volume: Whether to boot from volume. 'boot_volume'
                                 implies True, but boot_from_volume=True with
                                 no boot_volume is valid and will create a
                                 volume from the image and use that.
        :param volume_size: When booting an image from volume, how big should
                            the created volume be? Defaults to 50.
        :param nat_destination: Which network should a created floating IP
                                be attached to, if it's not possible to
                                infer from the cloud's configuration.
                                (Optional, defaults to None)
        :param group: ServerGroup dict, name or id to boot the server in.
                      If a group is provided in both scheduler_hints and in
                      the group param, the group param will win.
                      (Optional, defaults to None)
        :returns: A ``munch.Munch`` representing the created server.
        :raises: OpenStackCloudException on operation error.
        """
        # TODO(shade) Image is optional but flavor is not - yet flavor comes
        # after image in the argument list. Doh.
        if not flavor:
            raise TypeError(
                "create_server() missing 1 required argument: 'flavor'")
        if not image and not boot_volume:
            raise TypeError(
                "create_server() requires either 'image' or 'boot_volume'")
    
        server_json = {'server': kwargs}
    
        # TODO(mordred) Add support for description starting in 2.19
        security_groups = kwargs.get('security_groups', [])
        if security_groups and not isinstance(kwargs['security_groups'], list):
            security_groups = [security_groups]
        if security_groups:
            kwargs['security_groups'] = []
            for sec_group in security_groups:
                kwargs['security_groups'].append(dict(name=sec_group))
        if 'userdata' in kwargs:
            user_data = kwargs.pop('userdata')
            if user_data:
                kwargs['user_data'] = self._encode_server_userdata(user_data)
        for (desired, given) in (
                ('OS-DCF:diskConfig', 'disk_config'),
                ('config_drive', 'config_drive'),
                ('key_name', 'key_name'),
                ('metadata', 'meta'),
                ('adminPass', 'admin_pass')):
            value = kwargs.pop(given, None)
            if value:
                kwargs[desired] = value
    
        hints = kwargs.pop('scheduler_hints', {})
        if group:
            group_obj = self.get_server_group(group)
            if not group_obj:
                raise exc.OpenStackCloudException(
                    "Server Group {group} was requested but was not found"
                    " on the cloud".format(group=group))
            hints['group'] = group_obj['id']
        if hints:
            server_json['os:scheduler_hints'] = hints
        kwargs.setdefault('max_count', kwargs.get('max_count', 1))
        kwargs.setdefault('min_count', kwargs.get('min_count', 1))
    
        if 'nics' in kwargs and not isinstance(kwargs['nics'], list):
            if isinstance(kwargs['nics'], dict):
                # Be nice and help the user out
                kwargs['nics'] = [kwargs['nics']]
            else:
                raise exc.OpenStackCloudException(
                    'nics parameter to create_server takes a list of dicts.'
                    ' Got: {nics}'.format(nics=kwargs['nics']))
    
        if network and ('nics' not in kwargs or not kwargs['nics']):
            nics = []
            if not isinstance(network, list):
                network = [network]
            for net_name in network:
                if isinstance(net_name, dict) and 'id' in net_name:
                    network_obj = net_name
                else:
                    network_obj = self.get_network(name_or_id=net_name)
                if not network_obj:
                    raise exc.OpenStackCloudException(
                        'Network {network} is not a valid network in'
                        ' {cloud}:{region}'.format(
                            network=network,
                            cloud=self.name, region=self._compute_region))
                nics.append({'net-id': network_obj['id']})
    
            kwargs['nics'] = nics
        if not network and ('nics' not in kwargs or not kwargs['nics']):
            default_network = self.get_default_network()
            if default_network:
                kwargs['nics'] = [{'net-id': default_network['id']}]
    
        networks = []
        for nic in kwargs.pop('nics', []):
            net = {}
            if 'net-id' in nic:
                # TODO(mordred) Make sure this is in uuid format
                net['uuid'] = nic.pop('net-id')
                # If there's a net-id, ignore net-name
                nic.pop('net-name', None)
            elif 'net-name' in nic:
                net_name = nic.pop('net-name')
                nic_net = self.get_network(net_name)
                if not nic_net:
                    raise exc.OpenStackCloudException(
                        "Requested network {net} could not be found.".format(
                            net=net_name))
                net['uuid'] = nic_net['id']
            for ip_key in ('v4-fixed-ip', 'v6-fixed-ip', 'fixed_ip'):
                fixed_ip = nic.pop(ip_key, None)
                if fixed_ip and net.get('fixed_ip'):
                    raise exc.OpenStackCloudException(
                        "Only one of v4-fixed-ip, v6-fixed-ip or fixed_ip"
                        " may be given")
                if fixed_ip:
                    net['fixed_ip'] = fixed_ip
            # TODO(mordred) Add support for tag if server supports microversion
            # 2.32-2.36 or >= 2.42
            for key in ('port', 'port-id'):
                if key in nic:
                    net['port'] = nic.pop(key)
            if nic:
                raise exc.OpenStackCloudException(
                    "Additional unsupported keys given for server network"
                    " creation: {keys}".format(keys=nic.keys()))
            networks.append(net)
        if networks:
            kwargs['networks'] = networks
    
        if image:
            if isinstance(image, dict):
                kwargs['imageRef'] = image['id']
            else:
                kwargs['imageRef'] = self.get_image(image).id
        if isinstance(flavor, dict):
            kwargs['flavorRef'] = flavor['id']
        else:
            kwargs['flavorRef'] = self.get_flavor(flavor, get_extra=False).id
    
        if volumes is None:
            volumes = []
    
        # nova cli calls this boot_volume. Let's be the same
        if root_volume and not boot_volume:
            boot_volume = root_volume
    
        kwargs = self._get_boot_from_volume_kwargs(
            image=image, boot_from_volume=boot_from_volume,
            boot_volume=boot_volume, volume_size=str(volume_size),
            terminate_volume=terminate_volume,
            volumes=volumes, kwargs=kwargs)
    
        kwargs['name'] = name
        endpoint = '/servers'
        # TODO(mordred) We're only testing this in functional tests. We need
        # to add unit tests for this too.
        if 'block_device_mapping_v2' in kwargs:
            endpoint = '/os-volumes_boot'
        with _utils.shade_exceptions("Error in creating instance"):
            data = proxy._json_response(
>               self.compute.post(endpoint, json=server_json))

..\..\lib\site-packages\openstack\cloud\_compute.py:936: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

response = <Response [400]>, result_key = None, error_message = None

    def _json_response(response, result_key=None, error_message=None):
        """Temporary method to use to bridge from ShadeAdapter to SDK calls."""
>       exceptions.raise_from_response(response, error_message=error_message)

..\..\lib\site-packages\openstack\proxy.py:443: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

response = <Response [400]>, error_message = None

    def raise_from_response(response, error_message=None):
        """Raise an instance of an HTTPException based on keystoneauth response."""
        if response.status_code < 400:
            return
    
        if response.status_code == 409:
            cls = ConflictException
        elif response.status_code == 404:
            cls = NotFoundException
        elif response.status_code == 400:
            cls = BadRequestException
        else:
            cls = HttpException
    
        details = None
        content_type = response.headers.get('content-type', '')
        if response.content and 'application/json' in content_type:
            # Iterate over the nested objects to retrieve "message" attribute.
            # TODO(shade) Add exception handling for times when the content type
            # is lying.
    
            try:
                content = response.json()
                messages = [_extract_message(obj) for obj in content.values()]
                # Join all of the messages together nicely and filter out any
                # objects that don't have a "message" attr.
                details = '\n'.join(msg for msg in messages if msg)
            except Exception:
                details = response.text
        elif response.content and 'text/html' in content_type:
            # Split the lines, strip whitespace and inline HTML from the response.
            details = [re.sub(r'<.+?>', '', i.strip())
                       for i in response.text.splitlines()]
            details = list(set([msg for msg in details if msg]))
            # Return joined string separated by colons.
            details = ': '.join(details)
    
        if not details:
            details = response.reason if response.reason else response.text
    
        http_status = response.status_code
        request_id = response.headers.get('x-openstack-request-id')
    
        raise cls(
            message=error_message, response=response, details=details,
>           http_status=http_status, request_id=request_id
        )
E       openstack.exceptions.BadRequestException: BadRequestException: 400: Client Error for url: https://openstack.tacc.chameleoncloud.org:8774/v2/CH-819337/servers, Invalid key_name provided.

..\..\lib\site-packages\openstack\exceptions.py:229: BadRequestException

During handling of the above exception, another exception occurred:

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD7FE1208>

    def test_provider_vm_create(self):
        HEADING()
        name_generator.incr()
        Benchmark.Start()
>       data = provider.create(key=key)

tests\cloud\test_08_vm_provider.py:59: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\mongo\DataBaseDecorator.py:86: in wrapper
    current = f(*args, **kwargs)
cloudmesh\compute\vm\Provider.py:217: in create
    created = self.loop(self._create, **arguments)
cloudmesh\compute\vm\Provider.py:114: in loop
    vm = func(**parameters)
cloudmesh\compute\vm\Provider.py:252: in _create
    data = self.p.create(**arguments)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
name = 'test-wang542-vm-3', image = 'CC-Ubuntu18.04', size = 'm1.medium'
location = None, timeout = 360, key = 'wang542-key', secgroup = None
ip = '129.114.33.186', user = 'cc', public = True, group = 'cloudmesh'
metadata = None, cloud = 'chameleon', kwargs = {}, image_use = None
flavor_use = None, groups = ['cloudmesh']

    def create(self,
               name=None,
               image=None,
               size=None,
               location=None,
               timeout=360,
               key=None,
               secgroup=None,
               ip=None,
               user=None,
               public=True,
               group=None,
               metadata=None,
               cloud=None,
               **kwargs):
        """
        creates a named node
    
    
        :param group: the list of groups the vm belongs to
        :param name: the name of the node
        :param image: the image used
        :param size: the size of the image
        :param timeout: a timeout in seconds that is invoked in case the image
                        does not boot. The default is set to 3 minutes.
        :param kwargs: additional arguments HEADING(c=".")ed along at time of
                       boot
        :return:
        """
        image_use = None
        flavor_use = None
    
        # keyname = Config()["cloudmesh"]["profile"]["user"]
        # ex_keyname has to be the registered keypair name in cloud
    
        """
        https://docs.openstack.org/openstacksdk/latest/user/connection.html#openstack.connection.Connection.create_server
    
        """
    
        if 'flavor' in kwargs and size is None:
            size = kwargs['flavor']
    
        # Guess user name
    
        if user is None:
            user = Image.guess_username(image)
            # image_name = image.lower()
            # if image_name.startswith("cc-"):
            #    user = "cc"
            # if "centos" in image_name:
            #    user = "centos"
            # elif "ubuntu" in image_name:
            #    user = "ubuntu"
    
        # get IP
    
        if not ip and public:
            ip = self.find_available_public_ip()
            # pprint(entry)
    
        elif ip is not None:
            entry = self.list_public_ips(ip=ip, available=True)
            if len(entry) == 0:
                print("ip not available")
                raise ValueError(f"The ip can not be assigned {ip}")
    
        if type(group) == str:
            groups = Parameter.expand(group)
    
        banner("Create Server")
        print("    Name:    ", name)
        print("    User:    ", user)
        print("    IP:      ", ip)
        print("    Image:   ", image)
        print("    Size:    ", size)
        print("    Public:  ", public)
        print("    Key:     ", key)
        print("    location:", location)
        print("    timeout: ", timeout)
        print("    secgroup:", secgroup)
        print("    group:   ", group)
        print("    groups:  ", groups)
        print()
    
        try:
            server = self.cloudman.create_server(name,
                                                 flavor=size,
                                                 image=image,
                                                 key_name=key,
                                                 security_groups=[secgroup],
                                                 timeout=timeout
                                                 # tags=groups,
                                                 # wait=True
                                                 )
            server['user'] = user
            r = self.cloudman.wait_for_server(server)
            s = self.cloudman.add_ips_to_server(server, ips=ip)
            variables = Variables()
            variables['vm'] = name
            if metadata is None:
                metadata = {}
    
            metadata['image'] = image
            metadata['flavor'] = size
    
            self.cloudman.set_server_metadata(server, metadata)
    
            self.add_secgroup(name=secgroup)
    
            # server = self.cloudman.compute.wait_for_server(server)
    
            # print("ssh -i {key} root@{ip}".format(
            #    key=PRIVATE_KEYPAIR_FILE,
            #    ip=server.access_ipv4))
    
        except Exception as e:
            Console.error("Problem starting vm", traceflag=True)
            print(e)
>           raise RuntimeError
E           RuntimeError

cloudmesh\compute\openstack\Provider.py:980: RuntimeError
___________________ Test_provider_vm.test_provider_vm_wait ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD80CAE88>

    def test_provider_vm_wait(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        cm = CmDatabase()
        vm = cm.find_name(name, kind="vm")[0]
>       assert provider.wait(vm=vm), "cms wait timed out ..."
E       AssertionError: cms wait timed out ...
E       assert False
E        +  where False = <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x0000018DD6E1C8C8>>(vm={'_id': ObjectId('5de5910766e2a13223b31e61'), 'cm': {'cloud': 'chameleon', 'collection': 'chameleon-vm', 'created': '2019-12-02 22:32:39.735463', 'group': 'cloudmesh', ...}, 'name': 'test-wang542-vm-3'})
E        +    where <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x0000018DD6E1C8C8>> = <cloudmesh.compute.vm.Provider.Provider object at 0x0000018DD6E1C8C8>.wait

tests\cloud\test_08_vm_provider.py:85: AssertionError
____________________ Test_provider_vm.test_provider_vm_ssh ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD804E508>

    def test_provider_vm_ssh(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        cm = CmDatabase()
        vm = cm.find_name(name, kind="vm")[0]
>       data = provider.ssh(vm=vm, command='\"echo IAmAlive\"')

tests\cloud\test_08_vm_provider.py:94: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\compute\vm\Provider.py:447: in ssh
    return self.p.ssh(vm=vm, command=command)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
vm = {'_id': ObjectId('5de5910766e2a13223b31e61'), 'cm': {'cloud': 'chameleon', 'collection': 'chameleon-vm', 'created': '2019-12-02 22:32:39.735463', 'group': 'cloudmesh', ...}, 'name': 'test-wang542-vm-3'}
command = '"echo IAmAlive"'

    def ssh(self, vm=None, command=None):
        #
        # TODO: fix user name issue, should be stored in db
        #
    
        # VERBOSE(vm)
    
>       ip = vm['ip_public']
E       KeyError: 'ip_public'

cloudmesh\compute\openstack\Provider.py:1101: KeyError
_______________________ Test_provider_vm.test_vm_status _______________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD7F34288>

    def test_vm_status(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        data = provider.status(name=name)
        if type(data) == list:
>           data = data[0]
E           IndexError: list index out of range

tests\cloud\test_08_vm_provider.py:117: IndexError
___________________ Test_provider_vm.test_provider_vm_stop ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD7FC3348>

    def test_provider_vm_stop(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
>       data = provider.stop(name=name)

tests\cloud\test_08_vm_provider.py:127: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\mongo\DataBaseDecorator.py:86: in wrapper
    current = f(*args, **kwargs)
cloudmesh\compute\vm\Provider.py:293: in stop
    return self.loop_name(name, self.p.stop)
cloudmesh\compute\vm\Provider.py:96: in loop_name
    vm = func(name=name)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
name = 'test-wang542-vm-3'

    def stop(self, name=None):
        """
        Stop a list of nodes with the given name
    
        :param name: A list of node name
        :return:  A list of dict representing the nodes
        """
>       server = self.cloudman.get_server(name)['id']
E       TypeError: 'NoneType' object is not subscriptable

cloudmesh\compute\openstack\Provider.py:673: TypeError
___________________ Test_provider_vm.test_provider_vm_start ___________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD815A588>

    def test_provider_vm_start(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
>       data = provider.start(name=name)

tests\cloud\test_08_vm_provider.py:145: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\mongo\DataBaseDecorator.py:86: in wrapper
    current = f(*args, **kwargs)
cloudmesh\compute\vm\Provider.py:298: in start
    return self.loop_name(name, self.p.start)
cloudmesh\compute\vm\Provider.py:96: in loop_name
    vm = func(name=name)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
name = 'test-wang542-vm-3'

    def start(self, name=None):
        """
        Start a server with the given name
    
        :param name: A list of node name
        :return:  A list of dict representing the nodes
        """
>       server = self.cloudman.get_server(name)['id']
E       TypeError: 'NoneType' object is not subscriptable

cloudmesh\compute\openstack\Provider.py:662: TypeError
_________________ Test_provider_vm.test_provider_vm_terminate _________________

self = <test_08_vm_provider.Test_provider_vm object at 0x0000018DD7EF3588>

    def test_provider_vm_terminate(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
>       data = provider.destroy(name=name)

tests\cloud\test_08_vm_provider.py:167: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\compute\vm\Provider.py:470: in destroy
    return self.p.destroy(name=name)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.openstack.Provider.Provider object at 0x0000018DD6511148>
name = 'test-wang542-vm-3'

    def destroy(self, name=None):
        """
        Destroys the node
        :param name: the name of the node
        :return: the dict of the node
        """
>       server = self.info(name=name)[0]
E       IndexError: list index out of range

cloudmesh\compute\openstack\Provider.py:817: IndexError
============================== warnings summary ===============================
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
  d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\compute\v2\_proxy.py:289: DeprecationWarning: This API is deprecated and may disappear shortly
    DeprecationWarning)

tests/cloud/test_08_vm_provider.py::Test_provider_vm::test_provider_vm_create
  d:\school\b649_engineeringcloudcomputing\env4\lib\site-packages\openstack\cloud\_utils.py:372: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    argspec = inspect.getargspec(func)

-- Docs: https://docs.pytest.org/en/latest/warnings.html