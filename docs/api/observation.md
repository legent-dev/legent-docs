Below is the observations of an agent.

| Observation  | Descriptions                                                 | Details                                                      |
| ------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| vision_obs   | the first person view of the playmate                        | 224*224 numpy array (customizable soon)<br />the same as many pretrained image encoders such as CLIP. |
| language_obs | the text received by the playmate (i.e. what the player  just said) | string.<br /> "" means noop.                                       |

Besides, you can use all the game inner states from `info['game_states']` showed in `demo.py` for customized reward calculation.
The game states include:

* All the position and rotations of a game object in the scene.
* The player and the playmate's camera position and direction.
* The player and the playmate's position and rotation.
* Grabbed objects by the player and the playmate.
