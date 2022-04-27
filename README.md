# tf_to_pose_publisher
This repository contains code for publishing pose from tf tree. 

## Launch
```
roslaunch tf_to_pose_publisher tf_to_pose_publisher.launch
```
## Parameters
- from frame: `odom`

- to frame: `base_link`
- Publications: 
```
 /robot_pose [geometry_msgs/PoseWithCovarianceStamped]
 /rosout [rosgraph_msgs/Log]
```
- Subscriptions: 
```
 /tf [unknown type]
 /tf_static [unknown type]
```
## Enquire from rosnode
```
$rosnode info /publish_pose_from_tf
--------------------------------------------------------------------------------
Node [/publish_pose_from_tf]
Publications: 
 * /robot_pose [geometry_msgs/PoseWithCovarianceStamped]
 * /rosout [rosgraph_msgs/Log]

Subscriptions: 
 * /tf [unknown type]
 * /tf_static [unknown type]

Services: 
 * /publish_pose_from_tf/get_loggers
 * /publish_pose_from_tf/set_logger_level


contacting node http://arghya-Erazer-X7849-MD60379:34147/ ...
Pid: 7665
Connections:
 * topic: /rosout
    * to: /rosout
    * direction: outbound (38353 - 127.0.0.1:41186) [8]
    * transport: TCPROS
```




