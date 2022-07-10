<h1 align="center">Move a lawnmower automatically</h1> 

<p align="center"> 
<a href="https://github.com/lprtk/scala-lawnmower/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues/lprtk/scala-lawnmower"></a> 
<a href="https://github.com/lprtk/scala-lawnmower/network"><img alt="GitHub forks" src="https://img.shields.io/github/forks/lprtk/scala-lawnmower"></a> 
<a href="https://github.com/lprtk/scala-lawnmower/stargazers"><img alt="Github Stars" src="https://img.shields.io/github/stars/lprtk/scala-lawnmower"></a> 
<a href="https://github.com/lprtk/scala-lawnmower/"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a> 
</p>


## Table of contents
* [Content :mag_right:](#Content)
* [File details :open_file_folder:](#File-details)
* [Features :computer:](#Features) 

<a id="section01"></a> 
## Content 

<p align="justify">As part of a scala course, this project aims to program a lawnmower to traverse the entirety of a rectangular area. The position of the mower is represented by a combination of coordinates (x, y) and a letter indicating the orientation according to cardinal notation (N, E, W, S). The lawn is divided into a grid to simplify movement.<br>
For example, the mower's position might be (0,0, N), which means it's in the lower left corner of the lawn, facing north. To control and move the mower, just send it a simple sequence of letters: D, G or A. The letters D and G rotate the mower 90° to the right or left, but do not move it. The letter A means that the mower moves one square in the direction it is facing, without changing its orientation.<br>
If the position, after movement, is outside the lawn, the mower does not move, retains its orientation and processes the next command.<p>

<p align="justify">To program the mower, it is given an input file constructed as follows:<p>
<ul>
    <li><p align="justify">The first line is the coordinates of the upper right corner of the lawn, those of the lower left corner are assumed to be (0,0).</p></li>
    <li><p align="justify">The rest of the file allows you to control all the mowers that have been deployed.</p></li>
</ul>
    
<p align="justify">Each mower has two lines about it:<p>
<ul>
    <li><p align="justify">The first line gives the initial position of the mower, as well as its orientation. The position and orientation are given as 2 numbers and a letter, separated by a space.</p></li>
    <li><p align="justify">The second line is a series of instructions telling the mower to explore the lawn. The instructions are a series of characters without spaces.</p></li>
</ul>

<p align="justify">Each mower moves sequentially, which means that the second mower does not move until the first mower has completed its instruction series. When a mower completes a series of instructions, it communicates its position and orientation.<p>

<a id="section02"></a>
## File details
In the src folder, there are three scala files
* **ParserFile**
  * This is a .scala file which contains a class to retrieve the size of the garden, the instructions of each mower 'commands' and the position of each mower 'location'.
* **LawnMower**
  * This is a .scala file which contains a class that allows the mower to move in the garden. It contains several functions that allow to turn, to move forward, to execute all the commands and to indicate the position of the mower.
* **Run**
  * This is a .scala file which contains an object that allows to check that the instruction file is well filled in and to launch the mowers according to the instructions provided.

</br>

Here is the project pattern: 
```
- project
    > scala-lawnmower
        > data 
            > main
                > ressources
                    - consignes.txt
                > scala
                    > project
                        - ParserFile.scala
                        - LawnMower.scala
                        - Run.scala
```

<a id="section03"></a> 
## Features 
<p align="center"><a href="https://github.com/lprtk/lprtk">My profil</a> • 
<a href="https://github.com/lprtk/lprtk">My GitHub</a>
</p>
