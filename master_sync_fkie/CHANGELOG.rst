^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Changelog for package master_sync_fkie
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

0.3.10 (2014-03-31)
-------------------
* master_sync_fkie: fixed a bug which sometimes does not synchronized some topics
* multimaster_fkie: fixed problems detected by catkin_lint

0.3.9 (2013-12-12)
------------------
* multimaster_fkie: moved .gitignore to top level

0.3.8 (2013-12-10)
------------------
* master_sync_fkie: added sync for subscriber with AnyMsg, e.g relay (topic_tools), if local a publisher with known type is available
* multimaster_fkie: catkin_lint inspired fixes, thanks @roehling

0.3.7 (2013-10-17)
------------------
* multimaster_fkie: fixed problems with resolving service types while sync
  while synchronization not all topics and services can be synchronized
  because of filter or errors. A detection for this case was added.

0.3.6 (2013-09-17)
------------------
* multimaster_fkie: added SyncServiceInfo message to detect changes on services
* master_sync_fkie: kill the own ros node on error while load interface to inform the user in node_manager about errors

0.3.5 (2013-09-06)
------------------
* master_sync_fkie: fixed a brocken connection after desync

0.3.4 (2013-09-05)
------------------

0.3.3 (2013-09-04)
------------------
* node_manager_fkie: fixed a problem while launching a default cfg nodes
* multimaster_fkie: (*) added additional filtered interface to master_discovery rpc-server to get a filtered MasterInfo and reduce the load on network.
  (*) added the possibility to sync remote nodes using ~sync_remote_nodes parameter
* master_sync_fkie: added support to ignore nodes/topic/services of selected hosts
* master_sync_fkie: fixed ignore hosts, some topics sync ignores
