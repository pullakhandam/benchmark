# Cloud-AWS Benchmark
## Summary
* test_05_image failed during saving data to mongodb, encountered the same error in custom test script. Data was successfully retrieved
* test_08_vm_provider failed likely due to the same error as openstack, wrong key name lookup, the key name wang542-key doesn't exist on aws, that interrupted the creation of vm and the vm functions afterwards all failed
* test_09_cm_names_find ubuntu image look up failed due to the same error test_05_image, the aws-image collection failed to populate
## test_00_sys
PASSED
tests/cloud/test_00_sys.py::Test_Sys::test_benchmark 
+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 12                                                                                |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 6.5 GiB                                                                           |
| mem_free          | 6.5 GiB                                                                           |
| mem_percent       | 59.4%                                                                             |
| mem_total         | 15.9 GiB                                                                          |
| mem_used          | 9.5 GiB                                                                           |
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
+---------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                     | time  | start               | tag | node                 | user | system  | mac_version | win_version                     |
+---------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help | 2.604 | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop      | 0.0   | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+---------------------------+-------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_01_cleanlocal_remote
PASSED
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604  | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585 | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003  | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003  | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_02_key
PASSED
tests/cloud/test_02_key.py::Test_Key::test_benchmark 
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604  | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585 | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003  | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003  | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316  | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119  | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397  | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127  | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_03_key_upload
tests/cloud/test_03_key_upload.py::Test_Key::test_cleanup SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_upload_key_to_database SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_upload_key_to_cloud SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_list_key_from_cloud SKIPPED
tests/cloud/test_03_key_upload.py::Test_Key::test_benchmark SKIPPED
## test_04_flavor
PASSED
tests/cloud/test_04_flavor.py::Test_Flavor::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_05_image
[0m
Getting the list of images for aws cloud, this might take a few minutes ...
[32mImages list for aws cloud retrieved successfully[0m
Saving the data to file 
Importing the saved data to database
FAILED

PASSED
tests/cloud/test_05_image.py::Test_Image::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 23:02:39 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.338   | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               |         | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        |         | 2019-12-02 22:58:09 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 138.662 | 2019-12-02 23:00:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.861   | 2019-12-02 23:02:35 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_06_sec_command
PASSED
tests/cloud/test_06_sec_command.py::TestSecCLI::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 23:03:12 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.338   | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               |         | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        |         | 2019-12-02 22:58:09 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 138.662 | 2019-12-02 23:00:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.861   | 2019-12-02 23:02:35 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 4.153   | 2019-12-02 23:02:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.563   | 2019-12-02 23:02:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.49    | 2019-12-02 23:03:00 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.58    | 2019-12-02 23:03:04 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.504   | 2019-12-02 23:03:08 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_07_secgroup_provider
PASSED
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 23:03:18 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.338   | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               |         | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        |         | 2019-12-02 22:58:09 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 138.662 | 2019-12-02 23:00:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.861   | 2019-12-02 23:02:35 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 4.153   | 2019-12-02 23:02:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.563   | 2019-12-02 23:02:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.49    | 2019-12-02 23:03:00 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.58    | 2019-12-02 23:03:04 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.504   | 2019-12-02 23:03:08 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.348   | 2019-12-02 23:03:12 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.004   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 0.318   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.131   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.237   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  | 2.598   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 0.211   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.101   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_08_vm_provider
* Failed likely due to same reason in openstack, wrong key name look up, keyname was wang542-key and isn't reachable.
* Wrong key name interrupted creation of vm, and the functions afterwards failed as well
[0m
[34m
----------------------------------------------------------------------
Create Server
----------------------------------------------------------------------
[0m
    Name:    test-wang542-vm-4
    IP:      None
    Image:   ami-00dc79254d0461090
    Size:    t2.micro
    Public:  None
    Key:     wang542-key
    location:None
    timeout: 360
    secgroup:None
    group:   cloudmesh
FAILED

tests/cloud/test_08_vm_provider.py::Test_provider_vm::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 23:09:39 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.338   | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               |         | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        |         | 2019-12-02 22:58:09 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 138.662 | 2019-12-02 23:00:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.861   | 2019-12-02 23:02:35 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 4.153   | 2019-12-02 23:02:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.563   | 2019-12-02 23:02:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.49    | 2019-12-02 23:03:00 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.58    | 2019-12-02 23:03:04 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.504   | 2019-12-02 23:03:08 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.348   | 2019-12-02 23:03:12 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.004   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 0.318   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.131   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.237   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  | 2.598   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 0.211   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.101   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_create                     |         | 2019-12-02 23:03:18 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| create vm test-wang542-vm-4                                     |         | 2019-12-02 23:03:18 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list            |         | 2019-12-02 23:03:19 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait                       |         | 2019-12-02 23:03:20 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh                        |         | 2019-12-02 23:09:21 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info                       | 0.358   | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_vm_status                              |         | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop                       | 0.549   | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start                      | 0.484   | 2019-12-02 23:09:28 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate                  | 0.097   | 2019-12-02 23:09:33 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## test_09_cm_names_find
* image look up failed because the aws-image collection doesn't exist, provider couldn't write data to mongodb

test_09_cm_names_find.py::Test_cm_find::test_cm_find_ubuntu_in_images 
[35m
######################################################################
est_cm_find_ubuntu_in_images \tests\cloud\test_09_cm_names_find.py 131
######################################################################
[0m

{'name': {'$regex': '.*Ubuntu.*'}}
Number of entries [image 0
FAILED

tests/cloud/test_09_cm_names_find.py::Test_cm_find::test_benchmark 
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| timer                                                           | time    | start               | tag | node                 | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help                                       | 2.604   | 2019-12-02 22:40:32 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| benchmark_start_stop                                            | 0.0     | 2019-12-02 23:09:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_cms_init                        | 19.585  | 2019-12-02 22:40:34 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.003   | 2019-12-02 22:40:55 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_database                         | 0.316   | 2019-12-02 22:40:56 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud                            | 0.119   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_list_key_from_cloud                            | 0.397   | 2019-12-02 22:40:57 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud                          | 0.127   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_empty_database                              | 0.317   | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor                             | 182.772 | 2019-12-02 22:40:58 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update                      | 343.193 | 2019-12-02 22:44:01 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh                          | 355.56  | 2019-12-02 22:49:45 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_04_flavor/test_cms_flavor                                  | 6.964   | 2019-12-02 22:55:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_empty_database                               | 0.338   | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image                               |         | 2019-12-02 22:55:47 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_provider_image_update                        |         | 2019-12-02 22:58:09 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image_refresh                            | 138.662 | 2019-12-02 23:00:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_05_image/test_cms_image                                    | 3.861   | 2019-12-02 23:02:35 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_add                              | 4.153   | 2019-12-02 23:02:40 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_group_delete                           | 3.563   | 2019-12-02 23:02:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_list                               | 3.49    | 2019-12-02 23:03:00 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local                   | 3.58    | 2019-12-02 23:03:04 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud                   | 3.504   | 2019-12-02 23:03:08 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_load                             | 0.348   | 2019-12-02 23:03:12 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables                   | 0.004   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups                   | 0.318   | 2019-12-02 23:03:13 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules             | 0.131   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add                    | 0.237   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup                  | 2.598   | 2019-12-02 23:03:14 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete                 | 0.211   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again           | 0.101   | 2019-12-02 23:03:17 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_create                     |         | 2019-12-02 23:03:18 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| create vm test-wang542-vm-4                                     |         | 2019-12-02 23:03:18 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list            |         | 2019-12-02 23:03:19 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait                       |         | 2019-12-02 23:03:20 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh                        |         | 2019-12-02 23:09:21 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info                       | 0.358   | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_vm_status                              |         | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop                       | 0.549   | 2019-12-02 23:09:22 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start                      | 0.484   | 2019-12-02 23:09:28 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate                  | 0.097   | 2019-12-02 23:09:33 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_collection                   | 0.353   | 2019-12-02 23:09:39 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_loop                         | 1.212   | 2019-12-02 23:09:39 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_cloud                  | 0.313   | 2019-12-02 23:09:41 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_collection             | 0.324   | 2019-12-02 23:09:41 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_names_regexp                         | 0.621   | 2019-12-02 23:09:42 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vms                          | 0.324   | 2019-12-02 23:09:42 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_ubuntu_in_images             | 0.314   | 2019-12-02 23:09:43 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_cloud_name_attributes        | 0.309   | 2019-12-02 23:09:43 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections               | 0.312   | 2019-12-02 23:09:43 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections_vm            | 0.305   | 2019-12-02 23:09:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collection_form_parameter | 0.304   | 2019-12-02 23:09:44 | aws | ('LAPTOP-0UEFF4CG',) |      | Windows |             | ('10', '10.0.17763', 'SP0', '') |
+-----------------------------------------------------------------+---------+---------------------+-----+----------------------+------+---------+-------------+---------------------------------+
## Failures
================================== FAILURES ===================================
_______________________ Test_Image.test_provider_image ________________________

self = <test_05_image.Test_Image object at 0x000001ACAEEA9D08>

    def test_provider_image(self):
        HEADING()
        local = Key()
        Benchmark.Start()
>       r = provider.images()

tests\cloud\test_05_image.py:47: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\mongo\DataBaseDecorator.py:86: in wrapper
    current = f(*args, **kwargs)
cloudmesh\compute\vm\Provider.py:151: in images
    return self.p.images(*args, **kwargs)
cloudmesh\compute\aws\Provider.py:1274: in images
    self.get_images_and_import(data)
cloudmesh\mongo\DataBaseDecorator.py:127: in wrapper
    result = self.database.importAsFile(data,collection,db)
cloudmesh\mongo\CmDatabase.py:591: in importAsFile
    MongoDBController().importAsFile(data, collection, db)
cloudmesh\mongo\MongoDBController.py:995: in importAsFile
    result = Shell.run2(cmd)
cloudmesh\common3\Shell.py:60: in run2
    shell=True)
C:\Python37\lib\subprocess.py:395: in check_output
    **kwargs).stdout
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

input = None, capture_output = False, timeout = None, check = True
popenargs = ('mongoimport --db cloudmesh --collection aws-image  --authenticationDatabase admin  --username admin --password admin123  --drop --file C:\\Users\\wangc\\.cloudmesh\\tmp\\tmp_import_file.json',)
kwargs = {'shell': True, 'stderr': -2, 'stdout': -1}
process = <subprocess.Popen object at 0x000001AD0E53CB08>
stdout = b"'mongoimport' is not recognized as an internal or external command,\r\noperable program or batch file.\r\n"
stderr = None, retcode = 1

    def run(*popenargs,
            input=None, capture_output=False, timeout=None, check=False, **kwargs):
        """Run command with arguments and return a CompletedProcess instance.
    
        The returned instance will have attributes args, returncode, stdout and
        stderr. By default, stdout and stderr are not captured, and those attributes
        will be None. Pass stdout=PIPE and/or stderr=PIPE in order to capture them.
    
        If check is True and the exit code was non-zero, it raises a
        CalledProcessError. The CalledProcessError object will have the return code
        in the returncode attribute, and output & stderr attributes if those streams
        were captured.
    
        If timeout is given, and the process takes too long, a TimeoutExpired
        exception will be raised.
    
        There is an optional argument "input", allowing you to
        pass bytes or a string to the subprocess's stdin.  If you use this argument
        you may not also use the Popen constructor's "stdin" argument, as
        it will be used internally.
    
        By default, all communication is in bytes, and therefore any "input" should
        be bytes, and the stdout and stderr will be bytes. If in text mode, any
        "input" should be a string, and stdout and stderr will be strings decoded
        according to locale encoding, or by "encoding" if set. Text mode is
        triggered by setting any of text, encoding, errors or universal_newlines.
    
        The other arguments are the same as for the Popen constructor.
        """
        if input is not None:
            if kwargs.get('stdin') is not None:
                raise ValueError('stdin and input arguments may not both be used.')
            kwargs['stdin'] = PIPE
    
        if capture_output:
            if kwargs.get('stdout') is not None or kwargs.get('stderr') is not None:
                raise ValueError('stdout and stderr arguments may not be used '
                                 'with capture_output.')
            kwargs['stdout'] = PIPE
            kwargs['stderr'] = PIPE
    
        with Popen(*popenargs, **kwargs) as process:
            try:
                stdout, stderr = process.communicate(input, timeout=timeout)
            except TimeoutExpired:
                process.kill()
                stdout, stderr = process.communicate()
                raise TimeoutExpired(process.args, timeout, output=stdout,
                                     stderr=stderr)
            except:  # Including KeyboardInterrupt, communicate handled that.
                process.kill()
                # We don't call process.wait() as .__exit__ does that for us.
                raise
            retcode = process.poll()
            if check and retcode:
                raise CalledProcessError(retcode, process.args,
>                                        output=stdout, stderr=stderr)
E               subprocess.CalledProcessError: Command 'mongoimport --db cloudmesh --collection aws-image  --authenticationDatabase admin  --username admin --password admin123  --drop --file C:\Users\wangc\.cloudmesh\tmp\tmp_import_file.json' returned non-zero exit status 1.

C:\Python37\lib\subprocess.py:487: CalledProcessError
____________________ Test_Image.test_provider_image_update ____________________

self = <test_05_image.Test_Image object at 0x000001AD0E2A8888>

    def test_provider_image_update(self):
        HEADING()
        local = Key()
        Benchmark.Start()
>       r = provider.images()

tests\cloud\test_05_image.py:54: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _
cloudmesh\mongo\DataBaseDecorator.py:86: in wrapper
    current = f(*args, **kwargs)
cloudmesh\compute\vm\Provider.py:151: in images
    return self.p.images(*args, **kwargs)
cloudmesh\compute\aws\Provider.py:1274: in images
    self.get_images_and_import(data)
cloudmesh\mongo\DataBaseDecorator.py:127: in wrapper
    result = self.database.importAsFile(data,collection,db)
cloudmesh\mongo\CmDatabase.py:591: in importAsFile
    MongoDBController().importAsFile(data, collection, db)
cloudmesh\mongo\MongoDBController.py:995: in importAsFile
    result = Shell.run2(cmd)
cloudmesh\common3\Shell.py:60: in run2
    shell=True)
C:\Python37\lib\subprocess.py:395: in check_output
    **kwargs).stdout
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

input = None, capture_output = False, timeout = None, check = True
popenargs = ('mongoimport --db cloudmesh --collection aws-image  --authenticationDatabase admin  --username admin --password admin123  --drop --file C:\\Users\\wangc\\.cloudmesh\\tmp\\tmp_import_file.json',)
kwargs = {'shell': True, 'stderr': -2, 'stdout': -1}
process = <subprocess.Popen object at 0x000001ACE4337E48>
stdout = b"'mongoimport' is not recognized as an internal or external command,\r\noperable program or batch file.\r\n"
stderr = None, retcode = 1

    def run(*popenargs,
            input=None, capture_output=False, timeout=None, check=False, **kwargs):
        """Run command with arguments and return a CompletedProcess instance.
    
        The returned instance will have attributes args, returncode, stdout and
        stderr. By default, stdout and stderr are not captured, and those attributes
        will be None. Pass stdout=PIPE and/or stderr=PIPE in order to capture them.
    
        If check is True and the exit code was non-zero, it raises a
        CalledProcessError. The CalledProcessError object will have the return code
        in the returncode attribute, and output & stderr attributes if those streams
        were captured.
    
        If timeout is given, and the process takes too long, a TimeoutExpired
        exception will be raised.
    
        There is an optional argument "input", allowing you to
        pass bytes or a string to the subprocess's stdin.  If you use this argument
        you may not also use the Popen constructor's "stdin" argument, as
        it will be used internally.
    
        By default, all communication is in bytes, and therefore any "input" should
        be bytes, and the stdout and stderr will be bytes. If in text mode, any
        "input" should be a string, and stdout and stderr will be strings decoded
        according to locale encoding, or by "encoding" if set. Text mode is
        triggered by setting any of text, encoding, errors or universal_newlines.
    
        The other arguments are the same as for the Popen constructor.
        """
        if input is not None:
            if kwargs.get('stdin') is not None:
                raise ValueError('stdin and input arguments may not both be used.')
            kwargs['stdin'] = PIPE
    
        if capture_output:
            if kwargs.get('stdout') is not None or kwargs.get('stderr') is not None:
                raise ValueError('stdout and stderr arguments may not be used '
                                 'with capture_output.')
            kwargs['stdout'] = PIPE
            kwargs['stderr'] = PIPE
    
        with Popen(*popenargs, **kwargs) as process:
            try:
                stdout, stderr = process.communicate(input, timeout=timeout)
            except TimeoutExpired:
                process.kill()
                stdout, stderr = process.communicate()
                raise TimeoutExpired(process.args, timeout, output=stdout,
                                     stderr=stderr)
            except:  # Including KeyboardInterrupt, communicate handled that.
                process.kill()
                # We don't call process.wait() as .__exit__ does that for us.
                raise
            retcode = process.poll()
            if check and retcode:
                raise CalledProcessError(retcode, process.args,
>                                        output=stdout, stderr=stderr)
E               subprocess.CalledProcessError: Command 'mongoimport --db cloudmesh --collection aws-image  --authenticationDatabase admin  --username admin --password admin123  --drop --file C:\Users\wangc\.cloudmesh\tmp\tmp_import_file.json' returned non-zero exit status 1.

C:\Python37\lib\subprocess.py:487: CalledProcessError
__________________ Test_provider_vm.test_provider_vm_create ___________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE40581C8>

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
cloudmesh\compute\aws\Provider.py:1076: in create
    'Tags': metadata }]
..\..\lib\site-packages\boto3\resources\factory.py:520: in do_action
    response = action(self, *args, **kwargs)
..\..\lib\site-packages\boto3\resources\action.py:83: in __call__
    response = getattr(parent.meta.client, operation_name)(**params)
..\..\lib\site-packages\botocore\client.py:357: in _api_call
    return self._make_api_call(operation_name, kwargs)
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <botocore.client.EC2 object at 0x000001ACB37B2C48>
operation_name = 'RunInstances'
api_params = {'ImageId': 'ami-00dc79254d0461090', 'InstanceType': 't2.micro', 'KeyName': 'wang542-key', 'MaxCount': 1, ...}

    def _make_api_call(self, operation_name, api_params):
        operation_model = self._service_model.operation_model(operation_name)
        service_name = self._service_model.service_name
        history_recorder.record('API_CALL', {
            'service': service_name,
            'operation': operation_name,
            'params': api_params,
        })
        if operation_model.deprecated:
            logger.debug('Warning: %s.%s() is deprecated',
                         service_name, operation_name)
        request_context = {
            'client_region': self.meta.region_name,
            'client_config': self.meta.config,
            'has_streaming_input': operation_model.has_streaming_input,
            'auth_type': operation_model.auth_type,
        }
        request_dict = self._convert_to_request_dict(
            api_params, operation_model, context=request_context)
    
        service_id = self._service_model.service_id.hyphenize()
        handler, event_response = self.meta.events.emit_until_response(
            'before-call.{service_id}.{operation_name}'.format(
                service_id=service_id,
                operation_name=operation_name),
            model=operation_model, params=request_dict,
            request_signer=self._request_signer, context=request_context)
    
        if event_response is not None:
            http, parsed_response = event_response
        else:
            http, parsed_response = self._make_request(
                operation_model, request_dict, request_context)
    
        self.meta.events.emit(
            'after-call.{service_id}.{operation_name}'.format(
                service_id=service_id,
                operation_name=operation_name),
            http_response=http, parsed=parsed_response,
            model=operation_model, context=request_context
        )
    
        if http.status_code >= 300:
            error_code = parsed_response.get("Error", {}).get("Code")
            error_class = self.exceptions.from_code(error_code)
>           raise error_class(parsed_response, operation_name)
E           botocore.exceptions.ClientError: An error occurred (InvalidKeyPair.NotFound) when calling the RunInstances operation: The key pair 'wang542-key' does not exist

..\..\lib\site-packages\botocore\client.py:661: ClientError
______________ Test_provider_vm.test_provider_vmprovider_vm_list ______________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE4185CC8>

    def test_provider_vmprovider_vm_list(self):
        # list should be after create() since it would return empty and
        # len(data) would be 0
        HEADING()
        Benchmark.Start()
        data = provider.list()
>       assert len(data) > 0
E       assert 0 > 0
E        +  where 0 = len([])

tests\cloud\test_08_vm_provider.py:75: AssertionError
___________________ Test_provider_vm.test_provider_vm_wait ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE42D3F88>

    def test_provider_vm_wait(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        cm = CmDatabase()
        vm = cm.find_name(name, kind="vm")[0]
>       assert provider.wait(vm=vm), "cms wait timed out ..."
E       AssertionError: cms wait timed out ...
E       assert False
E        +  where False = <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>>(vm={'_id': ObjectId('5de598376b6c66dc67fcf815'), 'cm': {'cloud': 'aws', 'collection': 'aws-vm', 'created': '2019-12-02 23:03:19.096409', 'group': 'cloudmesh', ...}, 'name': 'test-wang542-vm-4'})
E        +    where <bound method Provider.wait of <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>> = <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>.wait

tests\cloud\test_08_vm_provider.py:85: AssertionError
____________________ Test_provider_vm.test_provider_vm_ssh ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE4167988>

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

self = <cloudmesh.compute.aws.Provider.Provider object at 0x000001ACB21D6908>
vm = {'_id': ObjectId('5de598376b6c66dc67fcf815'), 'cm': {'cloud': 'aws', 'collection': 'aws-vm', 'created': '2019-12-02 23:03:19.096409', 'group': 'cloudmesh', ...}, 'name': 'test-wang542-vm-4'}
command = '"echo IAmAlive"'

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
>       ip = vm['public_ips']
E       KeyError: 'public_ips'

cloudmesh\compute\aws\Provider.py:621: KeyError
_______________________ Test_provider_vm.test_vm_status _______________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE40BA9C8>

    def test_vm_status(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
>       data = provider.status(name=name)

tests\cloud\test_08_vm_provider.py:115: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>
name = 'test-wang542-vm-4'

    def status(self, name=None):
        r = self.info(name=name)
    
        status = []
        for entry in r:
>           state = {'name': entry['name'],
                     'status:': entry['status'],
                     'cm.status': entry['cm']['status']}
E           KeyError: 'name'

cloudmesh\compute\vm\Provider.py:315: KeyError
___________________ Test_provider_vm.test_provider_vm_stop ____________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE3FF2348>

    def test_provider_vm_stop(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        data = provider.stop(name=name)
        Benchmark.Stop()
        stop_timeout = 360
        time = 0
        while time <= stop_timeout:
            sleep(5)
            time += 5
>           status = provider.status(name=name)[0]

tests\cloud\test_08_vm_provider.py:134: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>
name = 'test-wang542-vm-4'

    def status(self, name=None):
        r = self.info(name=name)
    
        status = []
        for entry in r:
>           state = {'name': entry['name'],
                     'status:': entry['status'],
                     'cm.status': entry['cm']['status']}
E           KeyError: 'name'

cloudmesh\compute\vm\Provider.py:315: KeyError
___________________ Test_provider_vm.test_provider_vm_start ___________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE4156108>

    def test_provider_vm_start(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        data = provider.start(name=name)
        Benchmark.Stop()
        start_timeout = 360
        time = 0
        while time <= start_timeout:
            sleep(5)
            time += 5
>           status = provider.status(name=name)[0]

tests\cloud\test_08_vm_provider.py:152: 
_ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _

self = <cloudmesh.compute.vm.Provider.Provider object at 0x000001ACB0854688>
name = 'test-wang542-vm-4'

    def status(self, name=None):
        r = self.info(name=name)
    
        status = []
        for entry in r:
>           state = {'name': entry['name'],
                     'status:': entry['status'],
                     'cm.status': entry['cm']['status']}
E           KeyError: 'name'

cloudmesh\compute\vm\Provider.py:315: KeyError
_________________ Test_provider_vm.test_provider_vm_terminate _________________

self = <test_08_vm_provider.Test_provider_vm object at 0x000001ACE4006548>

    def test_provider_vm_terminate(self):
        HEADING()
        name = str(Name())
        Benchmark.Start()
        data = provider.destroy(name=name)
        Benchmark.Stop()
    
        pprint(data)
    
        termination_timeout = 360
        time = 0
        while time <= termination_timeout:
            sleep(5)
            time += 5
            if cloud == 'chameleon' and len(provider.info(name=name)) == 0:
                break
            elif cloud == 'aws' and (len(provider.info(name=name)) == 0 or
>                                    provider.info(name=name)[0]["cm"][
                                         "status"] in ['TERMINATED']):
E                                        KeyError: 'cm'

tests\cloud\test_08_vm_provider.py:180: KeyError
____________________ Test_cm_find.test_cm_image_name_cloud ____________________

self = <test_09_cm_names_find.Test_cm_find object at 0x000001ACE422BFC8>

    def test_cm_image_name_cloud(self):
        HEADING()
        Benchmark.Start()
        names = cm.names(cloud=cloud, kind="image")
        Benchmark.Stop()
        kind = "image"
        if benchmark_print:
            pprint(names)
        else:
            print(f"Number of entries [{kind}", len(names))
>       assert len(names) > 0
E       assert 0 > 0
E        +  where 0 = len([])

tests\cloud\test_09_cm_names_find.py:84: AssertionError
_________________ Test_cm_find.test_cm_find_ubuntu_in_images __________________

self = <test_09_cm_names_find.Test_cm_find object at 0x000001ACE4235388>

    def test_cm_find_ubuntu_in_images(self):
        HEADING()
        print()
        query = {"name": {'$regex': ".*Ubuntu.*"}}
        print(query)
    
        Benchmark.Start()
        entries = cm.find(collection=f"{cloud}-image", query=query)
        Benchmark.Stop()
    
        kind = "image"
        if benchmark_print:
            print(entries)
            for entry in entries:
                print(entry['name'])
        else:
            print(f"Number of entries [{kind}", len(entries))
    
>       assert len(entries) > 0
E       assert 0 > 0
E        +  where 0 = len([])

tests\cloud\test_09_cm_names_find.py:149: AssertionError
