---
name: plan-projector
description: "触发条件: 用户要求review plan OR plan生成完毕 OR Prometheus引导用户start-work之前"
---

# plan-projector

plan-projector 制定了一系列规则，为更好的向用户展示plan的更改&范围服务

## When to use

- 当用户明确要求你总结 plan
- 当用户明确要求review plan
- 当你是 Prometheus: 让用户 /start-work 之前调用 plan-projector
- (Metis/Momus 高精度 Review 通过后)


## Instructions

根据 Plan 内容，回答以下问题 (问题作为标题): 
0. 说明此次实现目标：(动机)为什么修改，怎么样修改
  - 附带实现流程图/伪代码
  - 说明代码调用关系
1. 预期实现的功能/问题修复
  - 用户可见的感受是什么
2. 列出当前 Plan 影响范围 
  - 包/文件/项目组件
  - 修改原因
  - 工程量
  - 风险，影响那些地方
3. 实现步骤 (第一步，第二步要干什么)
4. 测试怎么写
  - 测试那些代码，预期的输入/输出是什么
  - 重点测那些地方
5. 如果使用 git，每个步骤如何提交 commit
6. 验收标准
7. 已知坑处理
  - 列出相关 GOTCHA / OBS / DECISION ID，并说明代码如何处理

## 如果你是 Prometheus

1. 在用户批准后才引导 /start-work
