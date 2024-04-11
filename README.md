
<a name="readme-top"></a>

<!-- PROJECT SUMMARY -->
<div align="center">
    <img src="https://upload.wikimedia.org/wikipedia/commons/7/7b/An_illustration_of_the_dining_philosophers_problem.png" alt="Dining Philosophers Problem" width="" height="80">

<h3 align="center">Philosophers</h3>

  <p align="center">
    Summary:
This project make us learn about threads, processes and the use of mutexes
    <br>
  </p>
</div>

<!-- TABLE OF CONTENTS -->

- [About The Project](#about-the-project)
- [Usage](#usage)
- [Sources](#sources)

<!-- ABOUT THE PROJECT -->
## About The Project

Each philosophers is represented with a thread, during the program some threads will need to access some variables (memory) and modify it.
The use of mutexes is thus necessary to protect those variables to being modified at the same time by multiple threads.
Those problems are called data races and to check for those we can use the flag `-fsanitize=thread` at the compilation.

This is all coded in C.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE -->
## Usage

The program takes 4 parameters and an optional one: <br>
  - the number of philosophers (hence the number of forks)
  - the time to die (in milliseconds)
  - the time to eat (in milliseconds)
  - the time to sleep (in millseconds)
  - (optional) the number of meal each philosophers must eat to stop the simulation

Once the simulation is started, at each action the corresponding message is on the prompt

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- SOURCES -->
## Sources

* About the dining philosophers problem
  * https://en.wikipedia.org/wiki/Dining_philosophers_problem
  * https://medium.com/@jinghua.shih/operating-system-the-dining-philosophers-problem-6f35f210a4e2

* For the threads / processes / mutexes
  * https://softpixel.com/~cwright/programming/threads/threads.c.php
  * https://en.wikipedia.org/wiki/Lock_(computer_science)
  * https://www.geeksforgeeks.org/difference-between-process-and-thread/
  * https://en.wikipedia.org/wiki/Race_condition#Data_race

<p align="right">(<a href="#readme-top">back to top</a>)</p>