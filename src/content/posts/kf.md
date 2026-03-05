---
title: kf
published: 2026-03-05
description: ''
image: ''
tags: []
category: ''
draft: false 
lang: ''
---

### REF

[Kalman-and-Bayesian-Filters-in-Python](https://github.com/rlabbe/Kalman-and-Bayesian-Filters-in-Python)

Question:

07-Kalman-Filter-Math

- Continuous White Noise Model
$$\mathbf Q = \int_0^{\Delta t} \mathbf F(t)\mathbf{Q_c}\mathbf F^\mathsf{T}(t) dt$$

$\mathbf F(t)\mathbf{Q_c}\mathbf F^\mathsf{T}(t)$就是在算：
这个 “加速度抖动”，经过时间 t 的传播后，在位置、速度、加速度上分别产生了多大的不确定性，以及它们之间的相关性。


:::tip
如果随机向量 $\mathbf{z}$ 的协方差矩阵是 $\mathbf{Q}_c$，并且我们对它进行线性变换 $\mathbf{y}=\mathbf{F}\mathbf{z}$，那么变换后新向量 $\mathbf{y}$ 的协方差矩阵就是：

$$
\mathbf{Q}_y = \mathbf{F}\mathbf{Q}_c\mathbf{F}^\top
$$
:::
