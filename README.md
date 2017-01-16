# maze-generator-solver
Python projects for
* (i) [Maze generator](#maze-generator) algorithm based on Depth-First Search and Recursive Backtracker ([examples](#maze-generator-examples))
* (ii) [Maze solver](#maze-solver) algorithm based on A\* Search ([examples](#maze-solver-examples))

---

<a name="maze-generator"></a>
## Maze Generator (maze-generator-depth-first-search.py)
> Based on Depth-First Search and Recursive Backtracker

Usage:
```python
python maze-generator-depth-first-search.py [-h] [-p PATH] [-c COUNT] [-s SIZE] -mx WIDTH -my HEIGHT [-g GOLD] [-ng NUMBEROFGOLD] [-d DIAMOND] [-nd NUMBEROFDIAMOND]
```

The arguments shoud be:

```-p PATH, --path PATH``` *(optional)*
* path of the directory that contains the mazes to be generated

```-c COUNT, --count COUNT``` *(optional)*
* amount of mazes to be generated
    
```-s SIZE, --size SIZE``` *(optional but default value is 10)*
* size of the maze blocks

```-mx WIDTH, --width WIDTH``` *(required)*
* width of the maze

```-my HEIGHT, --height HEIGHT``` *(required)*
* height of the maze

```-g GOLD, --gold GOLD``` *(optional)*
* has gold blocks through maze

```-ng NUMBEROFGOLD, --numberOfGold NUMBEROFGOLD``` *(optional but default value is 5)*
* number of blocks of gold through maze

```-d DIAMOND, --diamond DIAMOND``` *(optional)*
* has diamond blocks through maze

```-nd NUMBEROFDIAMOND, --numberOfDiamond NUMBEROFDIAMOND``` *(optional but default value is 1)*
* number of blocks of diamond through maze

<a name="maze-solver"></a>
## Maze Solver (maze-solver-a-star.py)
> Based on A* Search

Usage:
```python
python maze-solver-a-star.py [-h] [-p PATH] [-c COUNT] [-s SIZE]
```

The arguments shoud be:

```-p PATH, --path PATH``` *(optional)*
* path of the directory that contains the mazes to be solved

```-c COUNT, --count COUNT``` *(optional)*
* amount of mazes to be generated

```-s SIZE, --size SIZE``` *(optional but default value is 10)*
* size of the maze blocks

<a name="all-examples"></a>
## Examples

<a name="maze-generator-examples"></a>
### Examples for generating mazes

```python maze-generator-depth-first-search.py -mx 32 -my 32```

**Another examples:**

    ```python maze-generator-depth-first-search.py -mx 32 -my 64``` (32 columns and 64 rows)

    ```python maze-generator-depth-first-search.py -mx 64 -my 32``` (64 columns and 32 rows)

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -c 3```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -g=True -d=True```

```python maze-generator-depth-first-search.py -mx 32 -my 32 -s 5 -ng=15 -nd=5```

**Another examples:**

    ```python maze-generator-depth-first-search.py -mx 32 -my 64 -ng=15 -nd=5``` (32 columns and 64 rows)

    ```python maze-generator-depth-first-search.py -mx 64 -my 32 -ng=15 -nd=5``` (64 columns and 32 rows)

**Generating maze(s) in the "C:/mazes" directory**

```python maze-generator-depth-first-search.py -mx 32 -my 32 -p C:/mazes```

<a name="maze-solver-examples"></a>
### > Examples for solving mazes

```python maze-solver-a-star.py```

```python maze-solver-a-star.py -s 5```

```python maze-solver-a-star.py -s 5 -c 3```

```python maze-solver-a-star.py -s 5``` (same of example #2)

```python maze-solver-a-star.py -s 5``` (same of example #2)

**Solving maze(s) from the "C:/mazes" directory**

```python maze-solver-a-star.py -p C:/mazes```
