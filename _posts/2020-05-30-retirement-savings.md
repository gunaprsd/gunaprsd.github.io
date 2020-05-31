---
layout: post
title:  "Retirement Savings 101"
date:   2020-05-30 00:00:00 -0800
author: Guna Prasaad
categories:
---

*Disclaimer: This is a personal note written by the author to clarify the trade-offs within various retirement savings options to self. It is shared only in the public interest that it could be useful to others. It is not intended to serve as an official recommendation either by the author or any associated entities. The author is not a financial advisor in any capacity and provides no guarantee about the factual correctness of any of the following information. However, please reach out if you would like something modified for correctness.*

I recently joined Facebook as a Software Engineer. One of the many things that are thrown at you as you begin settling at your full time job is **Retirement Savings**. As I started reading more, I discovered several retirement savings options - for e.g. traditional 401(k), IRA and their Roth alternatives. While they all share the common purpose of saving for retirement, each one of them is different from the other in a rather subtle way. You can, of course, find several websites and blogposts talking about their similarities and differences such as [this](https://money.usnews.com/money/retirement/articles/retirement-accounts-you-should-consider), [this](https://www.investopedia.com/ask/answers/12/401k.asp) and [this](https://www.schwab.com/ira). Be that as it may, I often found myself unable to answer some key questions about their advantages. I hope to *quantify* the costs and benefits of using these retirement savings accounts.

I will focus only on 4 types of retirement accounts here: traditional and Roth 401(k); traditional and Roth IRA. 

## When you stick to the plan
Fundamentally, there are two kinds of retirement plans based on who sponsors it. 
A 401(k) is a company sponsored retirement plan, while an Individual Retirement Account (IRA) is sponsored by yourself. 
Each company you work at will typically create a 401(k) for you. You can manage an IRA across companies and where you work at has nothing to do with your IRA. 

The unifying constraint in all these types of accounts is that you reap the full benefits when you withdraw money when you retire i.e. after you are $59\frac{1}{2}$ years. Let's look at how simlarities and differences between these different types of accounts when you stick to this plan. 

| Detail                                  | Traditional 401(k)  | Roth 401(k) | Traditional IRA | Roth IRA  |
|-----------------------------------------|---------------------|-------------|-----------------|-----------|
| Employer Contribution Allowed           | Yes                 | Yes         | No              | No        |
| AGI Limit                               | No                  | No          | No              | Yes       |
| Contribution Limit                      | Yes                 | Yes         | Yes             | Yes       |
| Taxed during Contribution               | No                  | Yes         | No              | Yes       |
| Taxed during Withdrawal - Contributions | Yes                 | No          | Yes             | No        |
| Taxed during Withdrawal - Earnings      | Yes                 | No          | Yes             | No        |

Since these are tax advantaged accounts, the IRS has created some checks and balances to prevent abusing them. The first kind is an Adjusted Gross Income (AGI) limit, which applies only to Roth IRA. You are eligible to contribute to a Roth IRA account only if your income is below certain threshold. The second kind of limit is on the amount you can contribute to every financial year. For example, your personal contributions to traditional and Roth 401(k) combined is capped at USD $19,500$; and traditional and Roth IRA combined is capped at USD $6000$ for 2020. You can find up-to-date details elsewhere.

The next major difference is in terms of if and when you pay taxes on contributions and earnings. Contributions to traditional 401(k) or IRA are usually tax deffered and taxed during withdrawal. On the other hand, contributions to Roth 401(k) and IRA are taxed during contribution and is not taxed during withdrawal. Earnings,however, are handled slightly differently. Earnings on contributions in a traditional 401(k) or IRA are taxed during withdrawal, while in case of a Roth 401(k) or IRA, they can be withdrawn tax-free.

### Benefit of a Tax-Advantaged Growth
What exactly is the benefit of a tax-advantaged growth? It helps to quantify this. To do this we are going to make some assumptions: Let the current and future tax rates be $t_1$ and $t_2$ and the contribution amount is $y$ USD. The net growth rate of principal when you invest in one of these accounts be $g$ i.e. if you invest USD $P$, it grows to $(1+g)P$ during withdrawal however many years later. 

We are interested in the *take home value* $\tau$ of this investment in two scenarios: (1) when you invest it in one of these retirement savings accounts and (2) when you invest it elsewhere. To simplify our analysis, we make a key assumption, "that the principal grows at a similar net growth rate even when you invest it elsewhere". While these retirement savings accounts typically have a restricted set of investment options compared to a brokerage account, we should ideally invest in assets with a similar risk profile and hence similar growth assumption is not wild. 

**Case 1: Invest elsewhere**. 
USD $y$ of pre-tax income amounts to $(1-t_1) * y$ investment that would grow to $(1+g) * (1-t_1) * y$. Since only the capital gain is taxed, the final take home value would be

$$\tau_1 = (1 + (1 - t_2) * g) * (1 - t_1) * y $$. 

**Case 2: Invest in a Traditional 401(k) or IRA**. 
The entire amount, USD $y$, is invested into the account, and that grows to $(1+g) * y$. The entire amount is taxed and the final take home value would be

$$\tau_2 = (1 - t_2) * (1 + g) * y$$. 

**Case 3: Invest in a Roth 401(k) or IRA**. 
USD $y$ of pre-tax income amounts to $(1-t_1) * y$ investment that would grow to $(1+g) * (1-t_1) * y$ and can be withdrawn tax-free.

$$\tau_3 = (1 - t_1) * (1 + g) * y$$. 

For instance, let's say the investment grew to $5\times$ over $30$years (That's not huge! It is approximately a $5.5\%$ YoY compound growth which is quite conservative). So $g=4$. Let's say you pay $35\%$ tax right now and expect to pay $15\%$ when you retire. If you invest USD $1000$ today, then 
* If you save elsewhere, it would grow to a take home of $(0.65 + 4 * 0.85) * 1000 = 4050$
* If you save in a traditional 401(k) or IRA account, you would get $0.85 * 5 * 1000 = 4250$
* If you save in a Roth 401(k) or IRA account, you would get $5 * 0.65 * 1000 = 3250$

On the other hand, if you expect to be in a higher tax bracket later, say current is $20\%$ and future is $35\%$ then,
* Saving elsewhere will yield a take home of $(0.8 + 4 * 0.65) * 1000 = 3400$
* Saving in a traditional 401(k) or IRA would yield $0.65 * 5 * 1000 = 3250$
* Saving in a Roth account would yield $0.8 * 5 * 1000 = 4000$. 

Clearly, if you expect to find yourself at a lower tax bracket later, then the take home value of Traditional > Elsewhere > Roth. If you expect a higher tax rate in the future, then Roth > Elsewhere > Traditional. 

## When You Cannot Stick to the Plan
Barring a few exceptional cases, the Government wants you to stick to your plan and withdraw money only after you retire at $59\frac{1}{2}$. These are not your run-of-the-mill savings account. So, they disincentivize you to treat it like one by imposing penalties. There is usually a 10% penalty on top of whatever income tax you owe if you withdraw money from these accounts before you are $59\frac{1}{2}$ years old. To me $59\frac{1}{2}$ is a good 30 years away and I frankly don't like to look so much ahead. I might want to cash out earlier. Given this uncertainty, how much is the advantage worth the liquidity I am giving away? Does that mean these investments are totally unattractive? 

Turns out, not exactly! And that is why it helps to quantify the tax and employer benefits that come with these accounts against its limitation. Let us start with a simple question.

### Should you match your employer contribution limit?
Most employers match your contributions to your 401(k) upto a certain limit. You can think of this as extra money that you do not get from your employer if you do not contribute. Consider this an incentive by your employer for you to save for your retirement. Should you match this amount, consider this locks in your money for a while? 

Let's say your employer matches $100\%$ upto USD $5000$. Your post tax earnings at a $30\%$ tax rate would be USD $3500$. But with the employer match, your contribution becomes USD $10000$, and even if you withdraw immediately incurring a penalty of $10\%$, it becomes ~ $(1 - 0.3 - 0.1) * 2 * 5000$ = USD $6000$. It totally makes sense to match your employer contribution here.

Precisely, if your employer match ratio is $x$ upto limit USD $y$ and tax ratio $t$, your take home portion corresponding to USD $y$ would be $(1-t)y$ if you do not contribute. If you do and withdraw immediately, it would be $(0.9-t)(1+x)y$. So, it makes sense to contribute when $ (0.9-t)(1+x)y > (1-t)y$
which yields 

$$x > \frac{1}{(9-10t)}$$ 

So, Even for a tax rate as high as $40\%$, you should contribute upto the limit if your employer match is greater than $20\%$.

### Should you contribute more than employer matching limit?
Now, we are done with all the extra money from your employer. The primary advantage of contributing to your retirement accounts now is the tax benefits. 

Let's model the scenarios we are interested in. The take home value at withdrawal for various scenarios in these retirement accounts with the same current and future tax rate (i.e. $t_1 = t_2$) are summarized below. *'Compared to Regular'* denotes the relationship of the take home value with that of a regular investment account. *'Adjusted Growth Rate'*, $\hat{g}$, denotes the effective growth rate for the corresponding type of the retirement account after taking into the account the taxes/penalty due to an early withdrawal. For instance, $\tau$ of Traditional/Roth account for a certain type of withdrawal with AGR $\hat{g}$ is $(1-t) * (1+\hat{g}) * \mathbf{y}$.

**Traditional 401(k) or IRA**
  
| Age                   | Qualified*  | Take Home Value                       | Compared to Regular           | Adjusted Growth Rate  |
|-----------------------|-------------|---------------------------------------|----------------------------------|-----------------------|
| $\geq 59\frac{1}{2}$  | -           | $(1-t) * (1+g) * \mathbf{y}$        | Always Greater                   | $g$                   |
| $< 59\frac{1}{2}$     | Yes         | $(1-t) * (1+g) * \mathbf{y}$        | Always Greater                   | $g$                   |
| $< 59\frac{1}{2}$     | No          | $0.9 * (1-t) * (1+g) * \mathbf{y}$  | Equal when $g = \frac{1}{10t-1}$ | $\frac{9g - 1}{10}$   |


**Roth 401(k) or IRA**
To understand the various withdrawal scenarios for Roth accounts, I recommend the reader to take a look at this [post](https://www.investopedia.com/roth-ira-withdrawal-rules-4769951).  
| Age                   | 5Y Rule Met? | Qualified  | Take Home Value                                   | Compared to Regular  | Adjusted Growth Rate |
|-----------------------|--------------|------------|---------------------------------------------------|-----------------------------|----------------------|
| $\geq 59\frac{1}{2}$  | Yes          | -          | $(1 + g) * \mathbf{(1-t) * y}$                  | Always Greater              | $g$                  |
| $\geq 59\frac{1}{2}$  | No           | -          | $(1 + (1 - t) * g) * \mathbf{(1-t) * y}$      | Always Equal                | $(1-t) * g$          |
| $< 59\frac{1}{2}$     | Yes          | Yes        | $(1 + g) * \mathbf{(1-t) * y}$                  | Always Greater              | $g$                  | 
| $< 59\frac{1}{2}$     | No           | Yes        | $(1 + (1 - t) * g) * \mathbf{(1-t) * y}$      | Always Equal                | $(1-t) * g$          |              
| $< 59\frac{1}{2}$     | Yes/No       | No         | $(1 + 0.9 * (1-t) * g) * \mathbf{(1-t) * y}$  | Always $10\%$ Lesser        | $ 0.9(1 - t) * g$    |


Obviously, it is beneficial to maintain the retirement accounts until maturity. However, let us analyze the case when you want to do an early withdrawal. We want to make sure we do not lose money in that scenario compared to having invested it elsewhere. We essentialy need to find the break-even point for using vs. not using these retirement accounts.

In case of a traditional 401(k) or IRA account, in order to break even we want $ 0.9 * (1-t) * (1+g) * y \geq (1 + (1-t) * g) * (1-t) * y$. So, the investment should have grown at least $$ g \geq \frac{1}{10t - 1} $$. In other words, you will not be hurt more than "not saving for retirement using these accounts" if you withdraw your money prematurely after it has grown to $\frac{10t}{10t-1}$ (i.e. $1 + g$) in your traditional 401(k) or IRA account. The adjusted growth rate in case of a Traditional account is $\frac{9g - 1}{10}$. Interestingly, the higher the growth lower the impact of an unqualified withdrawal. For a $g=4$, $\hat{g} \approx 0.7 * g$ and $g=5$ yeilds $\hat{g} 0.88 * g$. 

For a Roth 401(k) or IRA, there is no break-even if you make an unqualified withdrawal. In fact, you would lose  $$ 0.1 * (1-t) * g * (1-t) * y $$. This is a $10\%$ loss in growth compared to investing the money elsewhere. The adjusted growth rate is $\hat{g} = 0.9 * (1-t) * g$ and for a tax rate of $30\%$, $\hat{g} = 0.63 * g$. Here, the impact of an unqualified withdrawal depends both on the tax bracket at which you do and the growth. 

In addition, Roth also expands the scope of qualified withdrawals and you should use them when it makes sense. Does it ever make sense to withdraw without meeting the 5Y rule i.e. You start contributing to a Roth IRA account and withdraw the money in less than 5 years. Yes! In fact, you would exactly break-even with growing your money elsewhere. However, it is sub-optimal -- incurring a loss in terms of the tax you pay.
