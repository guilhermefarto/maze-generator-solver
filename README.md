# maze-generator-solver
Python projects for
* (i) [Maze generator](#maze-generator) algorithm based on Depth-First Search and Recursive Backtracker
* (ii) [Maze solver](#maze-solver) algorithm based on A* Search

---

<a name="maze-generator"></a>
## Maze Generator (maze-generator-depth-first-search.py)
> Based on Depth-First Search and Recursive Backtracker

Usage:
```python
python maze-generator-depth-first-search.py [-h] [-p PATH] [-c COUNT] [-s SIZE] -mx WIDTH -my HEIGHT [-g GOLD] [-ng NUMBEROFGOLD] [-d DIAMOND] [-nd NUMBEROFDIAMOND]
```

The arguments shoud be:

```-p PATH, --path PATH```
* path of the directory that contains the mazes to be generated

```-c COUNT, --count COUNT```
* amount of mazes to be generated
    
```-s SIZE, --size SIZE```
* size of the maze blocks

```-mx WIDTH, --width WIDTH```
* width of the maze

```-my HEIGHT, --height HEIGHT```
* height of the maze

```-g GOLD, --gold GOLD```
* has gold blocks through maze

```-ng NUMBEROFGOLD, --numberOfGold NUMBEROFGOLD```
* number of blocks of gold through maze

```-d DIAMOND, --diamond DIAMOND```
* has diamond blocks through maze

```-nd NUMBEROFDIAMOND, --numberOfDiamond NUMBEROFDIAMOND```
* number of blocks of diamond through maze

> ### Examples

```python maze-generator-depth-first-search.py -mx 32 -my 32```

**Another examples:**

> ```python maze-generator-depth-first-search.py -mx 32 -my 64``` (32 columns and 64 rows)

> ```python maze-generator-depth-first-search.py -mx 64 -my 32``` (64 columns and 32 rows)

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -c 3```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -g=True -d=True```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -ng=15 -nd=5```

**Another examples:**

> ```python maze-generator-depth-first-search.py -mx 32 -my 64 -ng=15 -nd=5``` (32 columns and 64 rows)

> ```python maze-generator-depth-first-search.py -mx 64 -my 32 -ng=15 -nd=5``` (64 columns and 32 rows)

Generating maze to "C:/mazes" directory

```python maze-generator-depth-first-search.py -mx 32 -my 32 -p C:/mazes```

<a name="maze-solver"></a>
## Maze Solver (maze-solver-a-star.py)
> Based on A* Search

Usage:
```python
python maze-solver-a-star.py [-h] [-p PATH] [-c COUNT] [-s SIZE]
```

The arguments shoud be:

```-p PATH, --path PATH```
* path of the directory that contains the mazes to be solved

```-c COUNT, --count COUNT```
* amount of mazes to be generated

```-s SIZE, --size SIZE```
* size of the maze blocks

> ### Examples

```python maze-solver-a-star.py```

```python maze-solver-a-star.py -s 5```

```python maze-solver-a-star.py -s 5 -c 3```

```python maze-solver-a-star.py -s 5``` (same of example #2)

```python maze-solver-a-star.py -s 5``` (same of example #2)

Solving maze from "C:/mazes" directory

```python maze-solver-a-star.py -p C:/mazes```
