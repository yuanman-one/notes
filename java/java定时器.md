# 定时器(Timer)

[TOC]

## 开始

1. 可以安排自动的计划任务的类，每个任务都是一个线程
2. 步骤
   1. 创建 Timer 实例
   2. 常用方法
      - a. `schedule(TimerTask task, Date time)` 在指定的时间安排指定的任务执行。
        注意：TimerTask 是一个抽象类，其中此类提供了执行定时器任务的 run（）方法
      - b、schedule(TimerTask task, Date firstTime, long period)
        从指定 的时间开始 ，对指定的任务执行重复的 固定延迟执行 。
      - c、schedule(TimerTask task, long delay)
        在指定的延迟之后安排指定的任务执行。
      - d、schedule(TimerTask task, long delay, long period)
        在指定 的延迟之后开始 ，重新执行 固定延迟执行的指定任务
      - e、cancel() 取消此计时器任务。
  ![202213233828.jpg](/202213233828.jpg "原神")
