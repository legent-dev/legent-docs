| Index | Descriptions | Details                                                   | Num Actions |
| ----- | ------------ | --------------------------------------------------------- | ----------- |
| 0     | move right   | 0:noop, 1:go right, -1:go left                            | 3           |
| 1     | move forward | 0:noop, 1:go forward, 2:sprint forward, -1: go backward   | 4           |
| 2     | look yaw     | horizontal camera rotation, [-180, 180)                   | continuous  |
| 3     | look pitch   | vertical camera rotation, [-90, 90)                       | continuous  |
| 4     | jump         | 0:noop, 1:jump                                            | 2           |
| 5     | grab         | 0:noop, 1:grab the object in the center of the FPV        | 2           |
| 6-520 | speak        | what the agent wants to say to the player. "" means noop, | any string  |