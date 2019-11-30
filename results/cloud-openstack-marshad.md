#Openstack (Chameleon Cloud) Benchmarks (2_security)

##cloud-openstack-marshad.md

###test_00_sys.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_00_sys.py`

Results:

`+-------------------+-----------------------------------------------------------------------------------+
| Machine Attribute | Value                                                                             |
+-------------------+-----------------------------------------------------------------------------------+
| cpu_count         | 4                                                                                 |
| mac_version       |                                                                                   |
| machine           | ('AMD64',)                                                                        |
| mem_available     | 602.5 MiB                                                                         |
| mem_free          | 602.5 MiB                                                                         |
| mem_percent       | 92.6%                                                                             |
| mem_total         | 7.9 GiB                                                                           |
| mem_used          | 7.3 GiB                                                                           |
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
+---------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                     | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+---------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_00_sys/test_cms_help | 3.818 | 2019-11-30 05:15:05 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop      | 0.0   | 2019-11-30 05:15:09 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+---------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ 2 passed in 5.63s =========================================================`


###test_01_clean_local_remote.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_01_clean_local_remote.py`

Results:

`cloudmesh-cloud\tests\cloud\test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_benchmark
+-----------------------------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                                           | time   | start               | tag       | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_01_clean_local_remote/test_cms_init                        | 31.787 | 2019-11-30 05:19:41 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_keys_from_cloud      | 0.287  | 2019-11-30 05:20:15 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_01_clean_local_remote/test_delete_all_secgroups_from_cloud | 0.016  | 2019-11-30 05:20:16 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                            | 0.0    | 2019-11-30 05:20:16 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_keys_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_keys_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_keys_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
tests/cloud/test_01_clean_local_remote.py::Test_Clean_Local_Remote::test_delete_all_secgroups_from_cloud
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
===================================================================== 4 passed, 16 warnings in 38.21s =====================================================================`


###test_02_key.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_02_key.py`

Results:

`cloudmesh-cloud\tests\cloud\test_02_key.py::Test_Key::test_benchmark
+-----------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                   | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_02_key/test_upload_key_to_database | 0.682 | 2019-11-30 05:25:59 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_upload_key_to_cloud    | 0.369 | 2019-11-30 05:26:03 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_list_key_from_cloud    | 0.903 | 2019-11-30 05:26:03 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_02_key/test_delete_key_from_cloud  | 0.483 | 2019-11-30 05:26:04 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                    | 0.0   | 2019-11-30 05:26:04 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_02_key.py::Test_Key::test_list_key_from_cloud
tests/cloud/test_02_key.py::Test_Key::test_list_key_from_cloud
tests/cloud/test_02_key.py::Test_Key::test_list_key_from_cloud
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
====================================================================== 7 passed, 3 warnings in 9.86s ======================================================================`



###test_03_key_upload.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_03_key_upload.py`

Results:

`cloudmesh-cloud\tests\cloud\test_03_key_upload.py::Test_Key::test_benchmark
+------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                          | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_03_key_upload/test_upload_key_to_database | 0.657 | 2019-11-30 05:26:58 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_03_key_upload/test_upload_key_to_cloud    | 0.339 | 2019-11-30 05:27:02 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_03_key_upload/test_list_key_from_cloud    | 0.928 | 2019-11-30 05:27:02 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                           | 0.0   | 2019-11-30 05:27:03 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_03_key_upload.py::Test_Key::test_list_key_from_cloud
tests/cloud/test_03_key_upload.py::Test_Key::test_list_key_from_cloud
tests/cloud/test_03_key_upload.py::Test_Key::test_list_key_from_cloud
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
====================================================================== 5 passed, 3 warnings in 9.15s ======================================================================`

###test_04_flavor.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_04_flavor.py`

Results:

`cloudmesh-cloud\tests\cloud\test_04_flavor.py::Test_Flavor::test_benchmark
+--------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                      | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+--------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_04_flavor/test_empty_database         | 1.4   | 2019-11-30 05:28:35 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_provider_flavor        | 2.899 | 2019-11-30 05:28:36 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_provider_flavor_update | 2.13  | 2019-11-30 05:28:39 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_cms_flavor_refresh     | 8.774 | 2019-11-30 05:28:42 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_04_flavor/test_cms_flavor             | 5.779 | 2019-11-30 05:28:51 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                       | 0.0   | 2019-11-30 05:28:57 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+--------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
tests/cloud/test_04_flavor.py::Test_Flavor::test_provider_flavor_update
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
===================================================================== 6 passed, 14 warnings in 23.96s =====================================================================`



###test_05_image.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_05_image.py`

Results:

`cloudmesh-cloud\tests\cloud\test_05_image.py::Test_Image::test_benchmark
+------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                    | time   | start               | tag       | node        | user | system  | mac_version | win_version                     |
+------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_05_image/test_empty_database        | 1.674  | 2019-11-30 05:30:45 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_provider_image        | 5.854  | 2019-11-30 05:30:47 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_provider_image_update | 3.425  | 2019-11-30 05:30:52 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_cms_image_refresh     | 12.842 | 2019-11-30 05:30:57 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_05_image/test_cms_image             | 7.824  | 2019-11-30 05:31:09 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                     | 0.0    | 2019-11-30 05:31:17 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------+--------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
  c:\users\m\env3\lib\site-packages\openstack\compute\v2\_proxy.py:289: DeprecationWarning: This API is deprecated and may disappear shortly
    DeprecationWarning)

tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
tests/cloud/test_05_image.py::Test_Image::test_provider_image_update
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
===================================================================== 6 passed, 20 warnings in 35.27s =====================================================================`

###test_06_sec_command.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_06_sec_command.py`

Results:

`cloudmesh-cloud\tests\cloud\test_06_sec_command.py::TestSecCLI::test_benchmark
+-----------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                         | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_06_sec_command/test_group_add            | 6.162 | 2019-11-30 05:32:40 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_group_delete         | 5.068 | 2019-11-30 05:32:46 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_list             | 5.204 | 2019-11-30 05:33:14 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_local | 5.693 | 2019-11-30 05:33:20 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_06_sec_command/test_sec_group_list_cloud | 5.754 | 2019-11-30 05:33:26 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                          | 0.0   | 2019-11-30 05:33:33 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

=========================================================================== 9 passed in 57.60s ============================================================================`


###test_07_secgroup_provider.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_07_secgroup_provider.py`

Results:

`cloudmesh-cloud\tests\cloud\test_07_secgroup_provider.py::Test_secgroup_provider::test_benchmark
+-------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                                 | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+-------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_07_secgroup_provider/test_load                   | 0.692 | 2019-11-30 05:34:38 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_variables         | 0.014 | 2019-11-30 05:34:40 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups         | 1.112 | 2019-11-30 05:34:40 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_list_secgroups_rules   | 0.429 | 2019-11-30 05:34:41 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_add          | 0.44  | 2019-11-30 05:34:41 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_upload_secgroup        | 6.913 | 2019-11-30 05:34:42 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete       | 0.916 | 2019-11-30 05:34:50 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_07_secgroup_provider/test_secgroups_delete_again | 0.613 | 2019-11-30 05:34:51 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                  | 0.0   | 2019-11-30 05:34:52 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

============================================================================ warnings summary =============================================================================
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_list_secgroups_rules
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_add
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_upload_secgroup
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
tests/cloud/test_07_secgroup_provider.py::Test_secgroup_provider::test_secgroups_delete_again
  c:\users\m\env3\lib\site-packages\openstack\resource.py:351: DeprecationWarning: inspect.getargspec() is deprecated since Python 3.0, use inspect.signature() or inspect.getfullargspec()
    len(inspect.getargspec(type_).args) > 1)

-- Docs: https://docs.pytest.org/en/latest/warnings.html
==================================================================== 9 passed, 208 warnings in 18.60s =====================================================================`

###test_08_vm_provider.py
*FAILED*
*Note: Failed due to timeout.*

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_08_vm_provider.py`

Results:

`cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_benchmark
+------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                                | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_08_vm_provider/test_provider_vm_create          |       | 2019-11-30 05:38:30 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| create vm test-marshad-vm-3                          |       | 2019-11-30 05:38:31 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vmprovider_vm_list | 2.586 | 2019-11-30 05:41:43 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_wait            |       | 2019-11-30 05:41:46 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_ssh             |       | 2019-11-30 05:48:53 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_info            | 1.438 | 2019-11-30 05:48:54 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_vm_status                   | 1.699 | 2019-11-30 05:48:56 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_stop            |       | 2019-11-30 05:48:58 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_start           |       | 2019-11-30 05:49:00 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_08_vm_provider/test_provider_vm_terminate       | 5.237 | 2019-11-30 05:49:02 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                 | 0.0   | 2019-11-30 05:49:09 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_wait
[35m
# ######################################################################
# test_provider_vm_wait \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 75
# ######################################################################
[0m
[34mINFO: waiting for instance test-marshad-vm-3 to be reachable: Interval: 10, Timeout: 360[0m
FAILED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_ssh
[35m
# ######################################################################
# test_provider_vm_ssh \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 84
# ######################################################################
[0m
FAILED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_info
[35m
# ######################################################################
# test_provider_vm_info \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 97
# ######################################################################
[0m
dry run info():
[]
PASSED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_vm_status
[35m
# ######################################################################
# test_vm_status \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 105
# ######################################################################
[0m
{'name': 'test-marshad-vm-3', 'status:': 'BUILD', 'cm.status': 'BUILD'}
FAILED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_stop
[35m
# ######################################################################
# test_provider_vm_stop \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 116
# ######################################################################
[0m
FAILED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_start
[35m
# ######################################################################
# test_provider_vm_start \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 134
# ######################################################################
[0m
FAILED
cloudmesh-cloud\tests\cloud\test_08_vm_provider.py::Test_provider_vm::test_provider_vm_terminate
[35m
# ######################################################################
# test_provider_vm_terminate \cloudmesh-cloud\tests\cloud\test_08_vm_provider.py 154
# ######################################################################
[0m
[KCloudmesh Database Update |################################| 1/1
FAILED


========================================================= 7 failed, 3 passed, 4113 warnings in 644.11s (0:10:44) ==========================================================

`



###test_09_cm_names_find.py

Executed:
`pytest -v --capture=no cloudmesh-cloud\tests\cloud\test_09_cm_names_find.py`

Results:

`cloudmesh-cloud\tests\cloud\test_09_cm_names_find.py::Test_cm_find::test_benchmark
+-----------------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| timer                                                           | time  | start               | tag       | node        | user | system  | mac_version | win_version                     |
+-----------------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+
| test_09_cm_names_find/test_cm_find_collection                   | 1.377 | 2019-11-30 05:55:22 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_loop                         | 1.839 | 2019-11-30 05:55:23 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_cloud                  | 0.616 | 2019-11-30 05:55:27 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_image_name_collection             | 0.616 | 2019-11-30 05:55:28 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_names_regexp                         | 1.284 | 2019-11-30 05:55:28 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vms                          | 0.618 | 2019-11-30 05:55:30 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_ubuntu_in_images             | 0.645 | 2019-11-30 05:55:30 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_cloud_name_attributes        | 0.626 | 2019-11-30 05:55:31 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections               | 0.768 | 2019-11-30 05:55:32 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collections_vm            | 0.926 | 2019-11-30 05:55:32 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| test_09_cm_names_find/test_cm_find_vm_collection_form_parameter | 0.718 | 2019-11-30 05:55:33 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
| benchmark_start_stop                                            | 0.0   | 2019-11-30 05:55:34 | chameleon | ('ONYX64',) |      | Windows |             | ('10', '10.0.18362', 'SP0', '') |
+-----------------------------------------------------------------+-------+---------------------+-----------+-------------+------+---------+-------------+---------------------------------+

PASSED

=========================================================================== 13 passed in 13.61s ===========================================================================`
