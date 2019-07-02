# BDD Overview

Behaviour-Driven Development (BDD) is a set of practices that aim to reduce some common wasteful activities in software development:

行为驱动开发（BDD）是一个旨在减少软件开发中一些常见冗余活动的一系列实践方法：

- Rework caused by misunderstood or vague requirements

  由于需求模糊、理解偏差而造成的返工

- Technical debt caused by reluctance to refactor code

  不愿重构而造成的技术债务

- Slow feedback cycles caused by silos and hand-overs

  孤岛及交接造成的缓慢反馈

BDD aims to narrow the communication gaps between team members, foster better understanding of the customer and promote continuous communication with real world *examples*.

BDD旨在缩小团队成员间的沟通成本，促进更好地了解客户，并促进与现实世界的实例持续沟通。

Examples describe how the software is *intended to behave*, often illustrating a particular business rule or requirement.

示例描述了软件如何去表现，通常用于说明特定的业务规则或要求。

A simple example

> Liz should be asked to guess again when she guesses “joke”

This example is from a word guessing game. It’s illustrating a rule stipulating that a guess must be 5 letters.

BDD can be split in two parts - *Deliberate Discovery* and *Test-Driven Development*.

这个例子来自猜词游戏。 它说明了一条规则，规定猜测必须是5个字母。

BDD可以分为两部分 -  Deliberate Discovery 刻意发现 和  Test-Driven Development 测试驱动开发。

# Deliberate Discovery[ 🔗︎](https://cucumber.io/docs/bdd/overview/#deliberate-discovery)

There are many reasons why software projects go wrong. A very common reason is that different people in the organisation or on the team have very different understandings of how the software should behave, and what problems it’s trying to solve.

软件项目出错的原因有很多，一个非常常见的原因是组织中或团队中的不同人对软件的行为方式有不同的理解，以及它试图解决什么问题。

> Ignorance is the single greatest impediment to throughput. - [Dan North](https://dannorth.net/2010/08/30/introducing-deliberate-discovery/)
>
> 无知是生产力最大的阻碍。 - Dan North

Teams that *deliberately* seek to discover what they are ignorant about *before* development starts are more productive, because there is less rework.

在开发开始之前，刻意寻求发现未知盲点的团队更有成效，因为返工更少。

The most effective way to do this is through conversation and collaboration between key stakeholders, such as:

最有效的方法是通过关键利益相关者之间的对话和协作，例如：

- Product owners 产品负责人
- Business analysts 业务分析师
- Domain experts 领域专家
- Users 用户
- Programmers 程序员
- UX designers UX设计师
- Testers 测试
- Ops engineers 运维工程师
- And probably some others 其他人员

The Cucumber way to do this is [Example Mapping](https://cucumber.io/blog/2015/12/08/example-mapping-introduction), a simple technique for coming up with examples together.

Cucumber是通过一个简单

When people in different roles have conversations about concrete examples they will often discover a lot about the problem domain.

当不同角色的人们就具体的例子进行讨论时，他们经常会发现问题域的很多问题。

The examples they produce together can then become automated tests and living documentation of how the system behaves.

它们共同产生的示例可以成为系统行为的自动化测试和实时文档。

# Test-Driven Development[ 🔗︎](https://cucumber.io/docs/bdd/overview/#test-driven-development)

Test-Driven Development (TDD) is a software development technique where automated tests are written *before* the code. Developers use those tests to *drive* the development.

测试驱动开发（TDD）是一种编码前进行自动化测试的软件开发技术。开发者慎用那些测试来驱动开发。

![Red-Green-Refactor diagram](https://cucumber.io/img/TDD-cycle.png)

TDD can be practiced at different levels of granularity, from acceptance tests to unit tests. The BDD flavour of TDD uses natural language to describe tests. They can be understood by non-programmers and are often based on examples created collaboratively using Example Mapping.

TDD可以从验收测试到单元测试在不同的颗粒度上实践。 TDD的BDD风格使用自然语言来描述测试。 非程序员可以理解它们，并且通常基于使用Example Mapping协作创建的示例。

[Gherkin](https://cucumber.io/docs/gherkin) is a simple syntax for such natural language tests, and Cucumber is the tool that can execute them.

Gkerkin是一种简单语法，用自然语言描述测试，而Cucumber是执行测试的工具。

Test after is not BDD

测试之后不是BDD

Many people write tests after the code is written, even with Cucumber. This is not BDD or TDD, because the tests do not *drive* the implementation when they are written afterwards.

大多数人在编码后写测试脚本，甚至在用Cucumber时也是如此。由于并没有驱动实现，因此这既不是BDD，也不是TDD，

TDD/BDD is not about testing

TDD/BDD

A common misunderstanding of TDD and BDD is that they are testing techniques. They’re not. As the name suggests, TDD and BDD are about software *development*.

一个关于TDD和BDD的普遍误解是它们都是测试技术，然而并不是。正如名字所暗示的那样，TDD和BDD关系软件开发。

It is the process of approaching your design and forcing you to think about the desired outcome and API before you code.

这是在您编码之前接近您的设计并迫使您考虑所需结果和API的过程。

Automated tests are a by-product of TDD and BDD.

自动化测试只是TDD和BDD的副产品。
