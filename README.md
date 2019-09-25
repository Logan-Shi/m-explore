# map_merger
ROS packages for cell map merge

```
<launch>
<group ns="map_merge">
  <node pkg="multirobot_map_merge" type="map_merge" respawn="false" name="map_merge" output="screen">
    <param name="robot_map_topic" value="map"/>
    <param name="robot_namespace" value=""/>
    <param name="merged_map_topic" value="map"/>
    <param name="world_frame" value="/robot_1/map"/>
    <param name="known_init_poses" value="true"/>
    <param name="merging_rate" value="4.0"/>
    <param name="discovery_rate" value="0.05"/>
    <param name="estimation_rate" value="0.5"/>
    <param name="estimation_confidence" value="1.0"/>
  </node>
</group>
</launch>
```
