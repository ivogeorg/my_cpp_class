### my_cpp_class

#### [`bb8_move_circle_class`](src/bb8_move_circle_class.cpp)

`roslaunch my_cpp_class bb8_move_circle_class.launch`

1. Uses the custom message from [`my_custom_srv_msg_pkg`](https://github.com/ivogeorg/my_custom_srv_msg_pkg.git).
2. Advertises service `/move_bb8_in_circle_with_timeout`.
3. Takes a duration (in secs) for the motion in request.
3. Sends `Twist` messages to topic `/cmd_vel` to start the robot moving in a circle.
4. Sleeps for `req.duration` and stops the robot.
5. Sends `success=true` when done.
