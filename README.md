### 📝 Final project Introduction to robotics - Line Follower 🏎️

### Task:
The objective of the project was to build a line following robot that calibrates the QTR reflectance snesor automatically at the beginging and completes a given track in under `20` seconds. Our team was able to complete the track in `22.889` seconds. The chassis used for the robot must be custom made by the team.


Project made by:
- Panait Ana-Maria
- Balan Sorana
- Radu Antonio Alexandru

<br>

<details>
 <summary><b>See all requirements</b></summary>
 <br>

### ⚙️ Components:
- Arduino Nano
- QTR-8RC reflectance sensor array
- 2 DC motors
- L293D motor driver
- 7.4V LiPo battery
- 2 wheels
- ball caster
- chassis (custom made)
- wires
- zip-ties
- 2 small breadboards


### Implementation:

For the sensor calibration the robot turns left until 
the last sensor on the right sees the black tape, and then change direction of until the last sensor on the left sees the black tape. It keeps repeting this process
for a few seconds then starts following the line.

The robot uses a PID control algorithm to adjust the speed of the motors based on the position of the robot over the line. The constants that we found to give the best results are `Kp = 25` and `Kd = 8` and the error ignore interval was `[-18, 18]` (from a total of [-50, 50]).

<details>
 <summary><b>Components diagram</b></summary>

 <div align="center"> 
  <img width="480px" src="https://github.com/Radu-Antonio/LineFollower/blob/master/ComponentsDiagram.jpeg" alt="Photo">
 </div>
</details>

</details>

</details>

<br>

[💻 <b>Code</b>](https://github.com/Radu-Antonio/LineFollower/blob/master/lineFollower/lineFollower.ino)

<details>
 <summary><b>Photo</b></summary>

 <div align="center"> 
  <img width="480px" src="https://github.com/Radu-Antonio/LineFollower/blob/master/LineFollower-Photo.jpeg" alt="Photo">
 </div>
</details>

<details>
 <summary><b>Video</b></summary>

 <div align="center"> 
   <a href="https://youtu.be/iSsHr05rzcE"><img src="https://img.youtube.com/vi/iSsHr05rzcE/0.jpg" alt="Video"></a>
 </div>
</details>
