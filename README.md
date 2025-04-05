
![EPITECH](https://studyadv.s3.amazonaws.com/production/schools/covers/000/005/919/original/Enseigne_Epitech_2.png)

- [Server Documentation](server/README.md)
- [AI Documentation](ai/README.md)
- [GUI Documentation](gui/README.md)

# Zappy

## Prerequisites

To use this project, you'll need a compiler that supports C++ 20.

The graphical client was made in [C++20](https://gcc.gnu.org/) using the [SFML](https://www.sfml-dev.org)for the graphical interface. \
The artificial intelligence was made with [Python](https://www.python.org/downloads) (3.10+). \
The server client was made in C using the GNU compiler [GCC](https://gcc.gnu.org/).

## Principle

The game is about managing a universe and its inhabitants. This world, named Trantor, is geographically made up of plains and does not include any other relief.

The game board represents the entire surface of this world, like a planisphere. Food and mining resources are randomly generated on the field.

The Trantorian is peaceful. He is neither violent nor aggressive. It strolls happily in search of stones and feeds on the way. He crosses without difficulty his fellows on the same unit of ground and sees as far as his visual capacities allow him.

It is an immaterial being, vague, which occupies all the box in which it is. It is impossible to distinguish its orientation when crossing it. The food it collects allows it to live for a certain period of time.

The objective of the players is to rise in the Trantorian hierarchy. This "increase", which increases one's physical and mental capacities, must be carried out according to a particular rite. It is indeed necessary to bring together on the same unit of land:

● A combination of stones\
● A certain number of players of the same level.

A player begins the incantation and thus initiates the elevation process. Participants do not need to be from the same team. Only their level matters. All players in the group performing the incantation reach the next level.

To complicate the task of the AI, the players' field of vision is limited. With each elevation, the vision increases by one measurement unit forward and one on each side of the new row.

A Trantorian also has a means of detecting the presence of his congeners by emitting a radar wave indicating the direction to take to join them.

The game is played by team. The winning team is the one whose six players have reached the maximum elevation.

## Usage

### Building program

Zappy is a B-YEP-400 EPITECH module project.
It is build with [Makefile](https://www.gnu.org/software/make/).

You can build the binaries as it follows:
```make``` or ```make re``` to recompile all the files.

Once the project is build, you will found 3 binaries:

- A server, that generates the inhabitants’ world.
- A graphical client, that can be used to watch what happens in the world.
- A client, that drives an inhabitant through orders sent to the server.

### Configuration file format

The trantorians can adopt multiple strategies to evolve through the game. These strategies can be found in the ```ai.conf``` file in the ```ai``` folder. \

| Strategy | Description |
|----------|----------------|
| Default | The default strategy. It is the strategy used if no strategy is set.|
| Eject | The player will try to eject the other players when a broadcast is sent.|
| Materialist | By default, the player will stop at the number of stones needed to finish the game. The materialist, on the other hand, will constantly collect these stones. |
| Thrifty | The player will save his stones and use them only to reach levels 2, 7 and 8. Attention: This one will never fork. |
| Opportunist | The player will collect stones only to rise to level 2. He will take advantage of the others to level up afterward. Attention: This one will never fork. |
| Fool | Sometimes, the player will spin on himself... |
| Greedy | The player will focus the food. The stones are not really important for him. |

** Beware for the ```Materialist```: his love for his stones means that he will never initiate an elevation to the next level (except to level 2). This one will never fork either.

### Launch program

After building project, here is the help output for the 3 binaries:

```bash
USAGE: ./zappy_gui -p port -h machine

DESCRIPTION:
        port is the port number
        machine is the name of the machine; localhost by default
```

```bash
usage: zappy_ai -p port -n name [-h machine] [-c file]

options:
  -p port     is the port number
  -n name     is the name of the team
  -h machine  is the name of the machine; localhost by default
  -c file     is the configuration file
```

```bash
USAGE: ./zappy_server -p port -x width -y height -n name1 name2 ... -c clientsNb -f freq
    port        is the port number
    width       is the width of the world
    height      is the height of the world
    nameX       is the name of the team X
    clientsNb   is the number of authorized clients per team
    freq        is the reciprocal of time unit for execution of actions
```

## Commit norm

The commits are normed thanks to a program made by [Adrien Ricou](https://github.com/Gradrien/Git-Shortcuts).

| Commit type       | Description        |
| --------- | --------------|
| [ADD] :rocket: | Deploying new code |
| [MODIFY] :sparkles: | Modifying code |
| [COD.STY] :zap: | Improving performance |
| [FIX] :bug: | Fixing a bug |
| [HANDLE] :sparkles: | Handling new features |
| [INCLUDE] :wrench: | Modifying user defined headers|
| [LIB] :wrench: | Modifying libraries files |
| [REMOVE] :fire: | Removing code or files |
| [UNIT.TESTS] :white_check_mark: | Added tests |
| [MERGE] :twisted_rightwards_arrows: | Merging branches |
| [DOCS] :memo: | Added documentation |
| [CI/CD] :green_heart: | CI/CD related push |
| [FIRST.PUSH] :tada: | First push hoorah |
| [HOTFIX] :ambulance: | Big problem, quick fix |
| [CODE.STRUCT] :art: | Code structure related push |
| [RESSOURCES] :truck: | New ressources added |
| [COMMENTS] :bulb: | Added commentaries |

**Emoji are available thanks to the Gitmoji tool

## Authors

* **Hippolyte David** - [HippolyteDavid](https://github.com/HippolyteDavid)
* **Elouan Savy-Camaret** - [ElouanSavy](https://github.com/ElouanSavy)
* **Kevin Demy** - [Sakutaroo](https://github.com/Sakutaroo)
* **Nolann Bougrainville** - [NolannB14](https://github.com/NolannB14)
* **Nils Martin** - [nilsmartin33](https://github.com/nilsmartin33)
* **Adrien Ricou** - [Gradrien](https://github.com/Gradrien)
