# Vocab-Scheduler 0.2

[中文版](README.zh-cn.md)

## Getting Started

In Scheduler 0.2, I redesigned and rewrote the whole program from scratch by writing much less code and adding extra functionalities. The scheduler 0.2 reads the command arguments as input (detail below) and creates your schedule (based on Ebbinghaus forgetting curve) in a `.csv` file (open with Microsoft Excel).

Note: The schedule will make you go through all vocabularies for 6 passes, but also remember to review a particular list (unit of task) twice on the first day. So when you finally accomplished everything on the scheduler, you did it 8 passes.  

[This](date_view_31lists(s)_3_27_2020.csv) is an example of a 31-list-vocabulary test starting March 27, 2020.

## Prerequisite

```
pip3 install pandas
```

## Usage

```
❯ python3 scheduler2.py 6 2020 3 26 Unit
```

Arguments: `python3 scheduler2.py units_of_vocabularies start_year start_month start_day customized_task_name`